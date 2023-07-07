# Comparing `tmp/xugrid-0.6.0.tar.gz` & `tmp/xugrid-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xugrid-0.6.0.tar", last modified: Wed Jul  5 14:38:00 2023, max compression
+gzip compressed data, was "xugrid-0.6.1.tar", last modified: Fri Jul  7 15:08:05 2023, max compression
```

## Comparing `xugrid-0.6.0.tar` & `xugrid-0.6.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 14:38:00.009214 xugrid-0.6.0/
--rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.6.0/LICENSE
--rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3298 2023-07-05 14:38:00.010215 xugrid-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.6.0/README.rst
--rw-rw-rw-   0        0        0     2199 2023-07-05 14:19:40.000000 xugrid-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      178 2023-07-05 14:38:00.012230 xugrid-0.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.706218 xugrid-0.6.0/tests/
--rw-rw-rw-   0        0        0    17755 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_connectivity.py
--rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_conventions.py
--rw-rw-rw-   0        0        0     9008 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_conversion.py
--rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_data.py
--rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_interpolate.py
--rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_meshkernel_utils.py
--rw-rw-rw-   0        0        0     8494 2023-06-26 11:20:36.000000 xugrid-0.6.0/tests/test_partitioning.py
--rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_plot.py
--rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.6.0/tests/test_snap.py
--rw-rw-rw-   0        0        0    11263 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_ugrid1d.py
--rw-rw-rw-   0        0        0    32742 2023-06-26 11:20:36.000000 xugrid-0.6.0/tests/test_ugrid2d.py
--rw-rw-rw-   0        0        0    28063 2023-07-05 13:51:43.000000 xugrid-0.6.0/tests/test_ugrid_dataset.py
--rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.6.0/tests/test_voronoi.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.733220 xugrid-0.6.0/xugrid/
--rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/constants.py
--rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/conversion.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.821272 xugrid-0.6.0/xugrid/core/
--rw-rw-rw-   0        0        0     4322 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/core/accessorbase.py
--rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/core/common.py
--rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/core/dataarray_accessor.py
--rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/core/dataset_accessor.py
--rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/core/wrap.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.853211 xugrid-0.6.0/xugrid/data/
--rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/data/__init__.py
--rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/data/registry.txt
--rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/data/sample_data.py
--rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/data/synthetic.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/meshkernel_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.867212 xugrid-0.6.0/xugrid/plot/
--rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/plot/__init__.py
--rw-rw-rw-   0        0        0    24101 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.918213 xugrid-0.6.0/xugrid/regrid/
--rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/regrid/overlap_1d.py
--rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.6.0/xugrid/regrid/reduce.py
--rw-rw-rw-   0        0        0    18493 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/regrid/regridder.py
--rw-rw-rw-   0        0        0    23864 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/regrid/structured.py
--rw-rw-rw-   0        0        0     4883 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/regrid/unstructured.py
--rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.6.0/xugrid/regrid/utils.py
--rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/regrid/weight_matrix.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:38:00.002219 xugrid-0.6.0/xugrid/ugrid/
--rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/ugrid/__init__.py
--rw-rw-rw-   0        0        0    24707 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/connectivity.py
--rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/ugrid/conventions.py
--rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.6.0/xugrid/ugrid/interpolate.py
--rw-rw-rw-   0        0        0    11044 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/ugrid/partitioning.py
--rw-rw-rw-   0        0        0    15005 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/snapping.py
--rw-rw-rw-   0        0        0    19654 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/ugrid1d.py
--rw-rw-rw-   0        0        0    56124 2023-06-26 11:20:36.000000 xugrid-0.6.0/xugrid/ugrid/ugrid2d.py
--rw-rw-rw-   0        0        0    22664 2023-07-05 13:51:43.000000 xugrid-0.6.0/xugrid/ugrid/ugridbase.py
--rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.6.0/xugrid/ugrid/voronoi.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:37:59.765220 xugrid-0.6.0/xugrid.egg-info/
--rw-rw-rw-   0        0        0     3298 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 14:37:59.000000 xugrid-0.6.0/xugrid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.837699 xugrid-0.6.1/
+-rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3298 2023-07-07 15:08:05.837699 xugrid-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.6.1/README.rst
+-rw-rw-rw-   0        0        0     2199 2023-07-07 15:03:53.000000 xugrid-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0      178 2023-07-07 15:08:05.840699 xugrid-0.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.595715 xugrid-0.6.1/tests/
+-rw-rw-rw-   0        0        0    17755 2023-07-05 13:51:43.000000 xugrid-0.6.1/tests/test_connectivity.py
+-rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_conventions.py
+-rw-rw-rw-   0        0        0     9008 2023-07-05 13:51:43.000000 xugrid-0.6.1/tests/test_conversion.py
+-rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_data.py
+-rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_interpolate.py
+-rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_meshkernel_utils.py
+-rw-rw-rw-   0        0        0     8494 2023-06-26 11:20:36.000000 xugrid-0.6.1/tests/test_partitioning.py
+-rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_plot.py
+-rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_snap.py
+-rw-rw-rw-   0        0        0    11263 2023-07-05 13:51:43.000000 xugrid-0.6.1/tests/test_ugrid1d.py
+-rw-rw-rw-   0        0        0    32742 2023-06-26 11:20:36.000000 xugrid-0.6.1/tests/test_ugrid2d.py
+-rw-rw-rw-   0        0        0    34035 2023-07-07 15:02:46.000000 xugrid-0.6.1/tests/test_ugrid_dataset.py
+-rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.6.1/tests/test_voronoi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.619697 xugrid-0.6.1/xugrid/
+-rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/constants.py
+-rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/conversion.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.667696 xugrid-0.6.1/xugrid/core/
+-rw-rw-rw-   0        0        0     4322 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/core/accessorbase.py
+-rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/core/common.py
+-rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/core/dataarray_accessor.py
+-rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/core/dataset_accessor.py
+-rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/core/wrap.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.687699 xugrid-0.6.1/xugrid/data/
+-rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/data/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/data/registry.txt
+-rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/data/sample_data.py
+-rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/data/synthetic.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/meshkernel_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.700696 xugrid-0.6.1/xugrid/plot/
+-rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/plot/__init__.py
+-rw-rw-rw-   0        0        0    24101 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.739698 xugrid-0.6.1/xugrid/regrid/
+-rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/regrid/overlap_1d.py
+-rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.6.1/xugrid/regrid/reduce.py
+-rw-rw-rw-   0        0        0    18493 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/regrid/regridder.py
+-rw-rw-rw-   0        0        0    23864 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/regrid/structured.py
+-rw-rw-rw-   0        0        0     4883 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/regrid/unstructured.py
+-rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.6.1/xugrid/regrid/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/regrid/weight_matrix.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.835699 xugrid-0.6.1/xugrid/ugrid/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/ugrid/__init__.py
+-rw-rw-rw-   0        0        0    24707 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/ugrid/connectivity.py
+-rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/ugrid/conventions.py
+-rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/ugrid/interpolate.py
+-rw-rw-rw-   0        0        0    11044 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/ugrid/partitioning.py
+-rw-rw-rw-   0        0        0    15005 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/ugrid/snapping.py
+-rw-rw-rw-   0        0        0    19654 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/ugrid/ugrid1d.py
+-rw-rw-rw-   0        0        0    56167 2023-07-07 15:02:46.000000 xugrid-0.6.1/xugrid/ugrid/ugrid2d.py
+-rw-rw-rw-   0        0        0    22700 2023-07-07 15:02:46.000000 xugrid-0.6.1/xugrid/ugrid/ugridbase.py
+-rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/ugrid/voronoi.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.634697 xugrid-0.6.1/xugrid.egg-info/
+-rw-rw-rw-   0        0        0     3298 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/top_level.txt
```

### Comparing `xugrid-0.6.0/LICENSE` & `xugrid-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/PKG-INFO` & `xugrid-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.6.0
+Version: 0.6.1
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.6.0/README.rst` & `xugrid-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/pyproject.toml` & `xugrid-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xugrid"
 description = "Xarray extension for unstructured grids"
 readme = { file = "README.rst", content-type = "text/x-rst" }
-version = "0.6.0"
+version = "0.6.1"
 maintainers = [{ name = "Huite Bootsma", email = "huite.bootsma@deltares.nl" }]
 requires-python = ">=3.7"
 dependencies = [
     'pandas',
     'numba',
     'numba_celltree',
     'numpy',
```

### Comparing `xugrid-0.6.0/tests/test_connectivity.py` & `xugrid-0.6.1/tests/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_conventions.py` & `xugrid-0.6.1/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_conversion.py` & `xugrid-0.6.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_data.py` & `xugrid-0.6.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_interpolate.py` & `xugrid-0.6.1/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_meshkernel_utils.py` & `xugrid-0.6.1/tests/test_meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_partitioning.py` & `xugrid-0.6.1/tests/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_plot.py` & `xugrid-0.6.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_snap.py` & `xugrid-0.6.1/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_ugrid1d.py` & `xugrid-0.6.1/tests/test_ugrid1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_ugrid2d.py` & `xugrid-0.6.1/tests/test_ugrid2d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/tests/test_ugrid_dataset.py` & `xugrid-0.6.1/tests/test_ugrid_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -783,7 +783,200 @@
 
 def test_merge():
     uds2d = xugrid.UgridDataset(UGRID_DS())
     uds1d = ugrid1d_ds()
     merged = xugrid.merge([uds2d, uds1d])
     assert isinstance(merged, xugrid.UgridDataset)
     assert len(merged.grids) == 2
+
+
+def get_ugrid_fillvaluem999_startindex1():
+    """
+    this is a very minimal but comparable dataset to Grevelingen_0002_map.nc (FM output)
+    It contains triangles and squares
+    the fillvalue of the connectivity arrays is -999
+    the start_index of the connectivity arrays is 1
+
+    """
+
+    ds2 = xr.Dataset()
+
+    mesh2d_attrs = {
+        "cf_role": "mesh_topology",
+        "topology_dimension": 2,
+        "node_dimension": "nmesh2d_node",
+        "edge_dimension": "nmesh2d_edge",
+        "face_dimension": "nmesh2d_face",
+        "max_face_nodes_dimension": "max_nmesh2d_face_nodes",
+        "face_node_connectivity": "mesh2d_face_nodes",
+        "edge_node_connectivity": "mesh2d_edge_nodes",
+        "node_coordinates": "mesh2d_node_x mesh2d_node_y",
+        "name": "mesh2d",
+    }
+    ds2["mesh2d"] = xr.DataArray(np.array(0, dtype=int), attrs=mesh2d_attrs)
+
+    node_x = np.array(
+        [
+            48231.65428822,
+            48264.81400401,
+            48350.0,
+            48450.0,
+            48235.96727817,
+            48287.80875187,
+            48306.85396605,
+            48400.0,
+            48500.0,
+            48273.38390534,
+            48450.0,
+            48350.77800678,
+            48342.73889736,
+        ]
+    )
+    node_x_attrs = {
+        "units": "m",
+        "standard_name": "projection_x_coordinate",
+        "long_name": "x-coordinate of mesh nodes",
+        "mesh": "mesh2d",
+        "location": "node",
+    }
+    ds2["mesh2d_node_x"] = xr.DataArray(
+        node_x, dims=(mesh2d_attrs["node_dimension"]), attrs=node_x_attrs
+    )
+
+    node_y = np.array(
+        [
+            419541.94243367,
+            419605.7455447,
+            419605.94894,
+            419605.94894,
+            419454.05602638,
+            419488.96173469,
+            419552.39342675,
+            419519.3464,
+            419519.3464,
+            419418.34074563,
+            419432.74386,
+            419447.63359856,
+            419378.75075546,
+        ]
+    )
+    node_y_attrs = {
+        "units": "m",
+        "standard_name": "projection_y_coordinate",
+        "long_name": "y-coordinate of mesh nodes",
+        "mesh": "mesh2d",
+        "location": "node",
+    }
+    ds2["mesh2d_node_y"] = xr.DataArray(
+        node_y, dims=(mesh2d_attrs["node_dimension"]), attrs=node_y_attrs
+    )
+
+    fnc = np.array(
+        [
+            [1, 7, 2, -999],
+            [3, 2, 7, -999],
+            [8, 4, 3, -999],
+            [1, 6, 7, -999],
+            [8, 3, 7, -999],
+            [9, 4, 8, -999],
+            [5, 10, 6, -999],
+            [8, 7, 6, 12],
+            [11, 9, 8, -999],
+            [10, 12, 6, -999],
+            [11, 8, 12, -999],
+            [10, 13, 12, -999],
+            [11, 12, 13, -999],
+        ],
+        dtype=int,
+    )
+    fnc_attrs = {
+        "_FillValue": -999,
+        "cf_role": "face_node_connectivity",
+        "start_index": 1,
+        "coordinates": "mesh2d_face_x mesh2d_face_y",
+    }
+    ds2["mesh2d_face_nodes"] = xr.DataArray(
+        fnc,
+        dims=(mesh2d_attrs["face_dimension"], mesh2d_attrs["max_face_nodes_dimension"]),
+        attrs=fnc_attrs,
+    )
+
+    enc = np.array(
+        [
+            [1, 2],
+            [1, 6],
+            [1, 7],
+            [2, 3],
+            [2, 7],
+            [3, 4],
+            [3, 7],
+            [3, 8],
+            [4, 8],
+            [4, 9],
+            [5, 6],
+            [5, 10],
+            [6, 7],
+            [6, 10],
+            [6, 12],
+            [7, 8],
+            [8, 9],
+            [8, 11],
+            [8, 12],
+            [9, 11],
+            [10, 12],
+            [10, 13],
+            [11, 12],
+            [11, 13],
+            [12, 13],
+        ],
+        dtype=int,
+    )
+    enc_attrs = {
+        "cf_role": "edge_node_connectivity",
+        "mesh": "mesh2d",
+        "location": "edge",
+        "long_name": "Mapping from every edge to the two nodes that it connects",
+        "start_index": 1,
+        "_FillValue": -999,
+    }
+    ds2["mesh2d_edge_nodes"] = xr.DataArray(
+        enc, dims=(mesh2d_attrs["edge_dimension"], "two"), attrs=enc_attrs
+    )
+
+    # add dummy face variable in order to have a face dimension in the uds
+    facevar = np.ones(shape=(ds2.dims[mesh2d_attrs["face_dimension"]]))
+    ds2["mesh2d_facevar"] = xr.DataArray(facevar, dims=(mesh2d_attrs["face_dimension"]))
+
+    # add dummy nodevar to plot and trigger triangulation procedure
+    nodevar = np.ones(shape=(ds2.dims[mesh2d_attrs["node_dimension"]]))
+    ds2["mesh2d_nodevar"] = xr.DataArray(nodevar, dims=(mesh2d_attrs["node_dimension"]))
+
+    # upon loading a dataset from a file, xarray decodes it, so we also do it here
+    ds2_enc = xr.decode_cf(ds2)
+
+    uds = xugrid.UgridDataset(ds2_enc)
+
+    return uds
+
+
+def test_fm_fillvalue_startindex_isel():
+    """
+    FM data has 1-based starting index and _FillValue -999, this raises several issues. Since it is not possible to generate a Ugrid2d with these attributes, we are testing with raw data
+    """
+
+    # xugrid 0.5.0 warns "RuntimeWarning: invalid value encountered in cast: cast = data.astype(dtype, copy=True)"
+    uds = get_ugrid_fillvaluem999_startindex1()
+
+    # xugrid 0.6.0 raises "ValueError: Invalid edge_node_connectivity"
+    uds.isel({uds.grid.face_dimension: [1]})
+
+
+def test_fm_facenodeconnectivity_fillvalue():
+    """
+    FM data has 1-based starting index and _FillValue -999, this raises several issues. Since it is not possible to generate a Ugrid2d with these attributes, we are testing with raw data
+    """
+
+    # xugrid 0.5.0 warns "RuntimeWarning: invalid value encountered in cast: cast = data.astype(dtype, copy=True)"
+    uds = get_ugrid_fillvaluem999_startindex1()
+
+    # xugrid 0.6.0 has -2 values in the array
+    assert (uds.grid.face_node_connectivity != -2).all()
```

### Comparing `xugrid-0.6.0/tests/test_voronoi.py` & `xugrid-0.6.1/tests/test_voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/__init__.py` & `xugrid-0.6.1/xugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/constants.py` & `xugrid-0.6.1/xugrid/constants.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/conversion.py` & `xugrid-0.6.1/xugrid/conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/core/accessorbase.py` & `xugrid-0.6.1/xugrid/core/accessorbase.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/core/common.py` & `xugrid-0.6.1/xugrid/core/common.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/core/dataarray_accessor.py` & `xugrid-0.6.1/xugrid/core/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/core/dataset_accessor.py` & `xugrid-0.6.1/xugrid/core/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/core/wrap.py` & `xugrid-0.6.1/xugrid/core/wrap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/data/sample_data.py` & `xugrid-0.6.1/xugrid/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/data/synthetic.py` & `xugrid-0.6.1/xugrid/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/meshkernel_utils.py` & `xugrid-0.6.1/xugrid/meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/plot/plot.py` & `xugrid-0.6.1/xugrid/plot/plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/overlap_1d.py` & `xugrid-0.6.1/xugrid/regrid/overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/reduce.py` & `xugrid-0.6.1/xugrid/regrid/reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/regridder.py` & `xugrid-0.6.1/xugrid/regrid/regridder.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/structured.py` & `xugrid-0.6.1/xugrid/regrid/structured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/unstructured.py` & `xugrid-0.6.1/xugrid/regrid/unstructured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/utils.py` & `xugrid-0.6.1/xugrid/regrid/utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/regrid/weight_matrix.py` & `xugrid-0.6.1/xugrid/regrid/weight_matrix.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/connectivity.py` & `xugrid-0.6.1/xugrid/ugrid/connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/conventions.py` & `xugrid-0.6.1/xugrid/ugrid/conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/interpolate.py` & `xugrid-0.6.1/xugrid/ugrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/partitioning.py` & `xugrid-0.6.1/xugrid/ugrid/partitioning.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/snapping.py` & `xugrid-0.6.1/xugrid/ugrid/snapping.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/ugrid1d.py` & `xugrid-0.6.1/xugrid/ugrid/ugrid1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid/ugrid/ugrid2d.py` & `xugrid-0.6.1/xugrid/ugrid/ugrid2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,22 +255,22 @@
         connectivity = ds.ugrid_roles.connectivity[topology]
         coordinates = ds.ugrid_roles.coordinates[topology]
         ugrid_vars = (
             [topology]
             + list(connectivity.values())
             + list(chain.from_iterable(chain.from_iterable(coordinates.values())))
         )
-        fill_value = -1
 
         x_index = coordinates["node_coordinates"][0][0]
         y_index = coordinates["node_coordinates"][1][0]
         node_x_coordinates = ds[x_index].astype(FloatDType).values
         node_y_coordinates = ds[y_index].astype(FloatDType).values
 
         face_nodes = connectivity["face_node_connectivity"]
+        fill_value = ds[face_nodes].encoding.get("_FillValue", -1)
         face_node_connectivity = cls._prepare_connectivity(
             ds[face_nodes], fill_value, dtype=IntDType
         ).values
 
         edge_nodes = connectivity.get("edge_node_connectivity")
         if edge_nodes:
             edge_node_connectivity = cls._prepare_connectivity(
```

### Comparing `xugrid-0.6.0/xugrid/ugrid/ugridbase.py` & `xugrid-0.6.1/xugrid/ugrid/ugridbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,14 +377,15 @@
         else:
             is_fill = np.isnan(data)
         data[is_fill] = fill_value
 
         cast = data.astype(dtype, copy=True)
         if start_index:
             cast -= start_index
+        cast[is_fill] = fill_value
         if (cast[~is_fill] < 0).any():
             raise ValueError("connectivity contains negative values")
         return da.copy(data=cast)
 
     def _precheck(self, multi_index):
         dim, index = multi_index.popitem()
         for check_dim, check_index in multi_index.items():
```

### Comparing `xugrid-0.6.0/xugrid/ugrid/voronoi.py` & `xugrid-0.6.1/xugrid/ugrid/voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.0/xugrid.egg-info/PKG-INFO` & `xugrid-0.6.1/xugrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.6.0
+Version: 0.6.1
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.6.0/xugrid.egg-info/SOURCES.txt` & `xugrid-0.6.1/xugrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*


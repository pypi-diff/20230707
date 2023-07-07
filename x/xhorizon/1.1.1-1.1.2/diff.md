# Comparing `tmp/xhorizon-1.1.1.tar.gz` & `tmp/xhorizon-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhorizon-1.1.1.tar", last modified: Fri Jul  7 06:13:28 2023, max compression
+gzip compressed data, was "xhorizon-1.1.2.tar", last modified: Fri Jul  7 06:36:57 2023, max compression
```

## Comparing `xhorizon-1.1.1.tar` & `xhorizon-1.1.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.217649 xhorizon-1.1.1/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1102 2023-07-04 09:21:53.000000 xhorizon-1.1.1/LICENSE
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1567 2023-07-07 06:13:28.217649 xhorizon-1.1.1/PKG-INFO
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1078 2023-07-07 00:13:54.000000 xhorizon-1.1.1/README.rst
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      332 2023-07-04 09:21:53.000000 xhorizon-1.1.1/pyproject.toml
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      594 2023-07-07 06:13:28.217649 xhorizon-1.1.1/setup.cfg
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      114 2023-07-04 09:21:53.000000 xhorizon-1.1.1/setup.py
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1275 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/__init__.py
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon/diagram_tools/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      382 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/__init__.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     6376 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/block_fill.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     6737 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/block_masks.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     6273 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/coord_transf.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1088 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/curve_class.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     9309 2023-07-05 07:11:58.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/curvemakers.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     8592 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/diagram_classes.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1432 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/plotstyle.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     8035 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/region_factory.py
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon/evap/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      567 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/__init__.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     3943 2023-07-06 09:06:05.000000 xhorizon-1.1.1/src/xhorizon/evap/demo.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     4283 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/demo_AdS.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     7658 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/demo_dS.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     3867 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/demo_zoom.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    15275 2023-07-06 07:47:56.000000 xhorizon-1.1.1/src/xhorizon/evap/draw.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    15636 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/draw_dS.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    15508 2023-07-05 07:34:55.000000 xhorizon-1.1.1/src/xhorizon/evap/evap.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    10281 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/helpers.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     4668 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/legend.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     7652 2023-07-05 07:31:40.000000 xhorizon-1.1.1/src/xhorizon/evap/massplot.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1499 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/schwarzparams.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    17568 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/tests.py
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.217649 xhorizon-1.1.1/src/xhorizon/shell_junction/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      548 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/__init__.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     5968 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/active_slice_class.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     5733 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/helpers.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     5292 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/interpolators.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     2760 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/passive_slice_class.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     4870 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/reg_corner_masks.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    19931 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/tests.py
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.217649 xhorizon-1.1.1/src/xhorizon/tortoise/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      214 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/__init__.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)      483 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/math_util.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1676 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_class.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    11273 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_factory.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     5827 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_tests.py
--rw-rw-r--   0 jcs       (1000) jcs       (1000)    12641 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/tortoise.py
-drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon.egg-info/
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1567 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/PKG-INFO
--rw-rw-r--   0 jcs       (1000) jcs       (1000)     1509 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/SOURCES.txt
--rw-rw-r--   0 jcs       (1000) jcs       (1000)        1 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/dependency_links.txt
--rw-rw-r--   0 jcs       (1000) jcs       (1000)        9 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/top_level.txt
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1102 2023-07-04 09:21:53.000000 xhorizon-1.1.2/LICENSE
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1567 2023-07-07 06:36:57.730219 xhorizon-1.1.2/PKG-INFO
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1078 2023-07-07 00:13:54.000000 xhorizon-1.1.2/README.rst
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      332 2023-07-04 09:21:53.000000 xhorizon-1.1.2/pyproject.toml
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      667 2023-07-07 06:36:57.730219 xhorizon-1.1.2/setup.cfg
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)       79 2023-07-07 06:32:16.000000 xhorizon-1.1.2/setup.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/xhorizon/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1275 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/__init__.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/xhorizon/diagram_tools/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      382 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     6376 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/block_fill.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     6737 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/block_masks.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     6273 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/coord_transf.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1088 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/curve_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     9309 2023-07-05 07:11:58.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/curvemakers.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     8592 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/diagram_classes.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1432 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/plotstyle.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     8035 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/diagram_tools/region_factory.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/xhorizon/evap/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      567 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     3943 2023-07-06 09:06:05.000000 xhorizon-1.1.2/src/xhorizon/evap/demo.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     4283 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/demo_AdS.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     7658 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/demo_dS.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     3867 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/demo_zoom.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    15275 2023-07-06 07:47:56.000000 xhorizon-1.1.2/src/xhorizon/evap/draw.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    15636 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/draw_dS.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    15508 2023-07-05 07:34:55.000000 xhorizon-1.1.2/src/xhorizon/evap/evap.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    10281 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/helpers.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     4668 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/legend.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     7652 2023-07-05 07:31:40.000000 xhorizon-1.1.2/src/xhorizon/evap/massplot.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1499 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/schwarzparams.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    17568 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/evap/tests.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/xhorizon/shell_junction/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      548 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5968 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/active_slice_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5733 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/helpers.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5292 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/interpolators.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     2760 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/passive_slice_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     4870 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/reg_corner_masks.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    19931 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/shell_junction/tests.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/xhorizon/tortoise/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      214 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/tortoise/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      483 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/tortoise/math_util.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1676 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/tortoise/metfunc_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    11273 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/tortoise/metfunc_factory.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5827 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/tortoise/metfunc_tests.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    12641 2023-07-04 09:21:53.000000 xhorizon-1.1.2/src/xhorizon/tortoise/tortoise.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:36:57.730219 xhorizon-1.1.2/src/xhorizon.egg-info/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1567 2023-07-07 06:36:57.000000 xhorizon-1.1.2/src/xhorizon.egg-info/PKG-INFO
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1544 2023-07-07 06:36:57.000000 xhorizon-1.1.2/src/xhorizon.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)        1 2023-07-07 06:36:57.000000 xhorizon-1.1.2/src/xhorizon.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)       50 2023-07-07 06:36:57.000000 xhorizon-1.1.2/src/xhorizon.egg-info/requires.txt
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)        9 2023-07-07 06:36:57.000000 xhorizon-1.1.2/src/xhorizon.egg-info/top_level.txt
```

### Comparing `xhorizon-1.1.1/LICENSE` & `xhorizon-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/PKG-INFO` & `xhorizon-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhorizon
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for explicitly computing Penrose diagrams in general relativity.
 Home-page: https://github.com/xh-diagrams/xhorizon
 Author: Joseph C Schindler
 Author-email: jcschindler01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xhorizon-1.1.1/README.rst` & `xhorizon-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/setup.cfg` & `xhorizon-1.1.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
+install_requires = 
+	numpy>=1.22.3
+	scipy>=1.8.0
+	matplotlib>=3.5.1,<4.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `xhorizon-1.1.1/src/xhorizon/__init__.py` & `xhorizon-1.1.2/src/xhorizon/__init__.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/block_fill.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/block_fill.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/block_masks.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/block_masks.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/coord_transf.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/coord_transf.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/curve_class.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/curve_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/curvemakers.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/curvemakers.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/diagram_classes.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/diagram_classes.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/plotstyle.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/plotstyle.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/diagram_tools/region_factory.py` & `xhorizon-1.1.2/src/xhorizon/diagram_tools/region_factory.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/__init__.py` & `xhorizon-1.1.2/src/xhorizon/evap/__init__.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/demo.py` & `xhorizon-1.1.2/src/xhorizon/evap/demo.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/demo_AdS.py` & `xhorizon-1.1.2/src/xhorizon/evap/demo_AdS.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/demo_dS.py` & `xhorizon-1.1.2/src/xhorizon/evap/demo_dS.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/demo_zoom.py` & `xhorizon-1.1.2/src/xhorizon/evap/demo_zoom.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/draw.py` & `xhorizon-1.1.2/src/xhorizon/evap/draw.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/draw_dS.py` & `xhorizon-1.1.2/src/xhorizon/evap/draw_dS.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/evap.py` & `xhorizon-1.1.2/src/xhorizon/evap/evap.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/helpers.py` & `xhorizon-1.1.2/src/xhorizon/evap/helpers.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/legend.py` & `xhorizon-1.1.2/src/xhorizon/evap/legend.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/massplot.py` & `xhorizon-1.1.2/src/xhorizon/evap/massplot.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/schwarzparams.py` & `xhorizon-1.1.2/src/xhorizon/evap/schwarzparams.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/evap/tests.py` & `xhorizon-1.1.2/src/xhorizon/evap/tests.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/__init__.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/__init__.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/active_slice_class.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/active_slice_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/helpers.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/helpers.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/interpolators.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/interpolators.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/passive_slice_class.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/passive_slice_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/reg_corner_masks.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/reg_corner_masks.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/shell_junction/tests.py` & `xhorizon-1.1.2/src/xhorizon/shell_junction/tests.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_class.py` & `xhorizon-1.1.2/src/xhorizon/tortoise/metfunc_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_factory.py` & `xhorizon-1.1.2/src/xhorizon/tortoise/metfunc_factory.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_tests.py` & `xhorizon-1.1.2/src/xhorizon/tortoise/metfunc_tests.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon/tortoise/tortoise.py` & `xhorizon-1.1.2/src/xhorizon/tortoise/tortoise.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.1.1/src/xhorizon.egg-info/PKG-INFO` & `xhorizon-1.1.2/src/xhorizon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhorizon
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for explicitly computing Penrose diagrams in general relativity.
 Home-page: https://github.com/xh-diagrams/xhorizon
 Author: Joseph C Schindler
 Author-email: jcschindler01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xhorizon-1.1.1/src/xhorizon.egg-info/SOURCES.txt` & `xhorizon-1.1.2/src/xhorizon.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/xhorizon/__init__.py
 src/xhorizon.egg-info/PKG-INFO
 src/xhorizon.egg-info/SOURCES.txt
 src/xhorizon.egg-info/dependency_links.txt
+src/xhorizon.egg-info/requires.txt
 src/xhorizon.egg-info/top_level.txt
 src/xhorizon/diagram_tools/__init__.py
 src/xhorizon/diagram_tools/block_fill.py
 src/xhorizon/diagram_tools/block_masks.py
 src/xhorizon/diagram_tools/coord_transf.py
 src/xhorizon/diagram_tools/curve_class.py
 src/xhorizon/diagram_tools/curvemakers.py
```


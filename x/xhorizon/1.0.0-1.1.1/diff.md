# Comparing `tmp/xhorizon-1.0.0.tar.gz` & `tmp/xhorizon-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhorizon-1.0.0.tar", last modified: Mon Apr 11 22:29:05 2022, max compression
+gzip compressed data, was "xhorizon-1.1.1.tar", last modified: Fri Jul  7 06:13:28 2023, max compression
```

## Comparing `xhorizon-1.0.0.tar` & `xhorizon-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:05.482000 xhorizon-1.0.0/
--rw-rw-rw-   0        0        0     1102 2022-04-11 18:54:31.000000 xhorizon-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1125 2022-04-11 22:29:05.462000 xhorizon-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      555 2022-04-11 22:26:43.000000 xhorizon-1.0.0/README.rst
--rw-rw-rw-   0        0        0      332 2022-03-29 04:43:43.000000 xhorizon-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      697 2022-04-11 22:29:05.479000 xhorizon-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      114 2022-03-29 04:43:43.000000 xhorizon-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:03.906000 xhorizon-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:04.087000 xhorizon-1.0.0/src/xhorizon/
--rw-rw-rw-   0        0        0     1275 2022-04-11 18:48:35.000000 xhorizon-1.0.0/src/xhorizon/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:04.499000 xhorizon-1.0.0/src/xhorizon/diagram_tools/
--rw-rw-rw-   0        0        0      382 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/__init__.py
--rw-rw-rw-   0        0        0     6376 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/block_fill.py
--rw-rw-rw-   0        0        0     6737 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/block_masks.py
--rw-rw-rw-   0        0        0     6273 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/coord_transf.py
--rw-rw-rw-   0        0        0     1088 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/curve_class.py
--rw-rw-rw-   0        0        0     9309 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/curvemakers.py
--rw-rw-rw-   0        0        0     8592 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/diagram_classes.py
--rw-rw-rw-   0        0        0     1432 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/plotstyle.py
--rw-rw-rw-   0        0        0     8035 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/diagram_tools/region_factory.py
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:04.977000 xhorizon-1.0.0/src/xhorizon/evap/
--rw-rw-rw-   0        0        0      567 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/__init__.py
--rw-rw-rw-   0        0        0     3936 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/demo.py
--rw-rw-rw-   0        0        0     4283 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/demo_AdS.py
--rw-rw-rw-   0        0        0     7658 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/demo_dS.py
--rw-rw-rw-   0        0        0     3867 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/demo_zoom.py
--rw-rw-rw-   0        0        0    15280 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/draw.py
--rw-rw-rw-   0        0        0    15636 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/draw_dS.py
--rw-rw-rw-   0        0        0    15504 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/evap.py
--rw-rw-rw-   0        0        0    10281 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/helpers.py
--rw-rw-rw-   0        0        0     4668 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/legend.py
--rw-rw-rw-   0        0        0     7650 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/massplot.py
--rw-rw-rw-   0        0        0     1499 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/schwarzparams.py
--rw-rw-rw-   0        0        0    17568 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/evap/tests.py
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:05.209000 xhorizon-1.0.0/src/xhorizon/shell_junction/
--rw-rw-rw-   0        0        0      548 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/__init__.py
--rw-rw-rw-   0        0        0     5968 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/active_slice_class.py
--rw-rw-rw-   0        0        0     5733 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/helpers.py
--rw-rw-rw-   0        0        0     5292 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/interpolators.py
--rw-rw-rw-   0        0        0     2760 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/passive_slice_class.py
--rw-rw-rw-   0        0        0     4870 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/reg_corner_masks.py
--rw-rw-rw-   0        0        0    19931 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/shell_junction/tests.py
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:05.439000 xhorizon-1.0.0/src/xhorizon/tortoise/
--rw-rw-rw-   0        0        0      214 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/tortoise/__init__.py
--rw-rw-rw-   0        0        0      483 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/tortoise/math_util.py
--rw-rw-rw-   0        0        0     1676 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/tortoise/metfunc_class.py
--rw-rw-rw-   0        0        0    11273 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/tortoise/metfunc_factory.py
--rw-rw-rw-   0        0        0     5827 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/tortoise/metfunc_tests.py
--rw-rw-rw-   0        0        0    12641 2022-03-11 20:25:02.000000 xhorizon-1.0.0/src/xhorizon/tortoise/tortoise.py
-drwxrwxrwx   0        0        0        0 2022-04-11 22:29:04.228000 xhorizon-1.0.0/src/xhorizon.egg-info/
--rw-rw-rw-   0        0        0     1125 2022-04-11 22:29:02.000000 xhorizon-1.0.0/src/xhorizon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1544 2022-04-11 22:29:03.000000 xhorizon-1.0.0/src/xhorizon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-11 22:29:03.000000 xhorizon-1.0.0/src/xhorizon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-04-11 22:29:03.000000 xhorizon-1.0.0/src/xhorizon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-04-11 22:29:03.000000 xhorizon-1.0.0/src/xhorizon.egg-info/top_level.txt
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.217649 xhorizon-1.1.1/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1102 2023-07-04 09:21:53.000000 xhorizon-1.1.1/LICENSE
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1567 2023-07-07 06:13:28.217649 xhorizon-1.1.1/PKG-INFO
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1078 2023-07-07 00:13:54.000000 xhorizon-1.1.1/README.rst
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      332 2023-07-04 09:21:53.000000 xhorizon-1.1.1/pyproject.toml
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      594 2023-07-07 06:13:28.217649 xhorizon-1.1.1/setup.cfg
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      114 2023-07-04 09:21:53.000000 xhorizon-1.1.1/setup.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1275 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/__init__.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon/diagram_tools/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      382 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     6376 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/block_fill.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     6737 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/block_masks.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     6273 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/coord_transf.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1088 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/curve_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     9309 2023-07-05 07:11:58.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/curvemakers.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     8592 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/diagram_classes.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1432 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/plotstyle.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     8035 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/diagram_tools/region_factory.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon/evap/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      567 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     3943 2023-07-06 09:06:05.000000 xhorizon-1.1.1/src/xhorizon/evap/demo.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     4283 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/demo_AdS.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     7658 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/demo_dS.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     3867 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/demo_zoom.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    15275 2023-07-06 07:47:56.000000 xhorizon-1.1.1/src/xhorizon/evap/draw.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    15636 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/draw_dS.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    15508 2023-07-05 07:34:55.000000 xhorizon-1.1.1/src/xhorizon/evap/evap.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    10281 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/helpers.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     4668 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/legend.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     7652 2023-07-05 07:31:40.000000 xhorizon-1.1.1/src/xhorizon/evap/massplot.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1499 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/schwarzparams.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    17568 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/evap/tests.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.217649 xhorizon-1.1.1/src/xhorizon/shell_junction/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      548 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5968 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/active_slice_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5733 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/helpers.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5292 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/interpolators.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     2760 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/passive_slice_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     4870 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/reg_corner_masks.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    19931 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/shell_junction/tests.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.217649 xhorizon-1.1.1/src/xhorizon/tortoise/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      214 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/__init__.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)      483 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/math_util.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1676 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_class.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    11273 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_factory.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     5827 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_tests.py
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)    12641 2023-07-04 09:21:53.000000 xhorizon-1.1.1/src/xhorizon/tortoise/tortoise.py
+drwxrwxr-x   0 jcs       (1000) jcs       (1000)        0 2023-07-07 06:13:28.213649 xhorizon-1.1.1/src/xhorizon.egg-info/
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1567 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/PKG-INFO
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)     1509 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)        1 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcs       (1000) jcs       (1000)        9 2023-07-07 06:13:28.000000 xhorizon-1.1.1/src/xhorizon.egg-info/top_level.txt
```

### Comparing `xhorizon-1.0.0/LICENSE` & `xhorizon-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/PKG-INFO` & `xhorizon-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-Metadata-Version: 2.1
-Name: xhorizon
-Version: 1.0.0
-Summary: A Python package for explicitly computing Penrose diagrams in general relativity.
-Home-page: https://github.com/xh-diagrams/xhorizon
-Author: Joseph C Schindler
-Author-email: jcschindler01@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-
-xhorizon
-================================
-
-xhorizon: Explicitly computed Penrose diagrams in general relativity.
-
-A Python package.
-
-| **I finally gave the package a makeover and updated to Python 3!**
-
-| **The new documentation is still under construction...**
-| **Check back soon for examples and a tutorial!**
-
-
-Links
------
-   - `GitHub <https://github.com/xh-diagrams/xhorizon>`_.
-   - `Documetation <https://xhorizon.readthedocs.io/>`_.
-   - `PyPi <https://pypi.org/project/xhorizon/>`_.
-
-
-Getting Started
----------------
-::
-
-  pip install xhorizon
-
-
+Metadata-Version: 2.1
+Name: xhorizon
+Version: 1.1.1
+Summary: A Python package for explicitly computing Penrose diagrams in general relativity.
+Home-page: https://github.com/xh-diagrams/xhorizon
+Author: Joseph C Schindler
+Author-email: jcschindler01@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+
+xhorizon
+================================
+
+
+*xhorizon*: Explicitly computing Penrose diagrams in general relativity.
+
+A Python package.
+
+
+| **I finally gave the package a makeover and updated to Python 3!**
+
+| **The new documentation is still under construction...**
+| **but there is now an ever expanding tutorial!**
+
+
+
+Links
+-----
+   - `GitHub <https://github.com/xh-diagrams/xhorizon>`_.
+   - `Documentation <https://xhorizon.readthedocs.io/>`_.
+   - `PyPi <https://pypi.org/project/xhorizon/>`_.
+
+
+Background Theory
+-----------------
+JC Schindler, A Aguirre. 
+*Algorithms for the explicit computation of Penrose diagrams.*
+`Class Quantum Grav 35 105019 <https://doi.org/10.1088/1361-6382/aabce2>`_.
+(2018).
+`arxiv:1802.02263 <https://arxiv.org/abs/1802.02263>`_.
+
+
+Getting Started
+---------------
+To install::
+
+   pip install xhorizon
+
+To start using the tools, begin with the `tutorial <https://xhorizon.readthedocs.io/en/stable/TUTORIAL/00-overview.html>`_ and keep an eye out for `example scripts <https://github.com/xh-diagrams/xhorizon/tree/main/scripts/examples>`_.
+
```

### Comparing `xhorizon-1.0.0/src/xhorizon/__init__.py` & `xhorizon-1.1.1/src/xhorizon/__init__.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/block_fill.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/block_fill.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/block_masks.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/block_masks.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/coord_transf.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/coord_transf.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/curve_class.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/curve_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/curvemakers.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/curvemakers.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/diagram_classes.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/diagram_classes.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/plotstyle.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/plotstyle.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/diagram_tools/region_factory.py` & `xhorizon-1.1.1/src/xhorizon/diagram_tools/region_factory.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/__init__.py` & `xhorizon-1.1.1/src/xhorizon/evap/__init__.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/demo.py` & `xhorizon-1.1.1/src/xhorizon/evap/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,41 +47,41 @@
 		plt.ylim(-0.5*aspect*sq,0.5*aspect*sq)
 	################################
 	
 
 	## save
 	path = "temp-figs/demo"
 	sfp = dict(dpi=800)
-	temp_only = False
+	temp_only = True
 
 	## draw
 	draw = True
 
 	## label
 	label = '$(a)$'
 
 	# func type
-	ftype = 2
+	ftype = 0
 
 	## input
 	l  = 1e-4
 	le = 1e-4
 
 	## input
 	R  = 2e-3
 
 	## if background
 	L = 10.
 
 	## evap
-	Nevap = 12
+	Nevap = 3
 	Tevap = 10.
 
 	## accrete
-	Nacc = 5
+	Nacc = 1
 	Tacc = .5
 
 	## seed
 	seed = 0
 
 	## vv
 	voff = -Tacc - 0.
@@ -138,30 +138,30 @@
 		print("plot")
 		pp = dict(l=1.*l, R=1.*R)
 		xh.evap.drawreg(reglist, chainparams, fparams=pp)
 
 
 	## label
 	if True:
-		plt.annotate(s=label, xy=(.95,.97), xycoords='axes fraction', ha='right', va='top', size=8)
+		plt.annotate(text=label, xy=(.95,.97), xycoords='axes fraction', ha='right', va='top', size=8)
 
 
 	## auto param label
 	if False:
 		plabel = [r"$l_{ev}=%3s$"%(le), r"", r"$l=%3s$"%(l), r"$2M=%3s$"%(R)]
 		plabel += [r"", r"$\tau_{acc}=%3s$"%(Tacc), r"$\tau_{ev}=%3s$"%(Tevap)]
 		plabel = "\n".join(plabel)
-		plt.annotate(s=plabel, xy=(.95,.03), xycoords='axes fraction', ha='right', va='bottom', size=8)
+		plt.annotate(text=plabel, xy=(.95,.03), xycoords='axes fraction', ha='right', va='bottom', size=8)
 
 	## manual param label
 	if False:
 		plabel = [r"$\tau_{ev}=%s$"%(Tevap), r"$\tau_{acc}=%s$"%(Tacc)]
 		plabel += [r"", r"$M=10^{-3}$", r"$l_{ev}=l=10^{-4}$"]
 		plabel = "\n".join(plabel)
-		plt.annotate(s=plabel, xy=(.95,.03), xycoords='axes fraction', ha='right', va='bottom', size=8)
+		plt.annotate(text=plabel, xy=(.95,.03), xycoords='axes fraction', ha='right', va='bottom', size=8)
 
 	## mass plot
 	mpgo = True
 	if mpgo:
 		massplot(chainparams, params)
 
 	## save
```

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/demo_AdS.py` & `xhorizon-1.1.1/src/xhorizon/evap/demo_AdS.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/demo_dS.py` & `xhorizon-1.1.1/src/xhorizon/evap/demo_dS.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/demo_zoom.py` & `xhorizon-1.1.1/src/xhorizon/evap/demo_zoom.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/draw.py` & `xhorizon-1.1.1/src/xhorizon/evap/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 				## style
 				style = dict(lw=0.9, c='0.5', zorder=11000)
 				style.update(sty)
 				## singularity style
 				if b.sgnf<0.:
 					style.update(sty2)
 				## curve
-				cv = xh.cm.rstarlines_special_2([0.], b.uvbounds, c=0., sty=style, inf=1.*inf, npoints=1.*npoints, eps=1e-12)
+				cv = xh.cm.rstarlines_special_2([0.], b.uvbounds, c=0., sty=style, inf=1.*inf, npoints=1*npoints, eps=1e-12)
 				b.add_curves_uv(cv)
 
 
 
 def rline_inf_col(reglist, npoints=5001, inf=1000., sty={}, M=.5):
 	"""
 	Add boundary lines to regions in reglist.
@@ -318,26 +318,26 @@
 	## general
 	style = dict(ls='-', zorder=10, lw=.4, alpha=.2)
 	style.update(sty)
 	## l scale
 	x = np.arange(0.,.5*R/l,.5)
 	scale = l
 	style.update(dict(c='c'))
-	rlines(reglist, scale*x, sty=style, inf=10., npoints=2001.)
+	rlines(reglist, scale*x, sty=style, inf=10., npoints=2001)
 	## R scale
 	x = np.arange(0.,25.01,.5)
 	scale = R
 	style.update(dict(c='m'))
-	rlines(reglist, scale*x, sty=style, inf=25., npoints=1001.)
+	rlines(reglist, scale*x, sty=style, inf=25., npoints=1001)
 	## Tevap scale
 	if Tevap is not None:
 		x = np.arange(0.,25.01,.5)
 		scale = Tevap
 		style.update(dict(c='#0000f0'))
-		rlines(reglist, scale*x, sty=style, inf=25., npoints=1001.)
+		rlines(reglist, scale*x, sty=style, inf=25., npoints=1001)
 
 
 def vticks(reglist, dv=1., inf1=100., inf2=50.+irr, sty={}):
 	"""
 	Remainder lets dv carry across regions.
 	"""
 	## init
@@ -494,15 +494,15 @@
 	for reg in reglist:
 		for b in reg.blocks:
 			for i in range(len(rvals)):
 				if (b.rj[0]<rvals[i]) and (rvals[i]<b.rj[1]):
 					style = dict(c='c', ls='-', lw=.5, zorder=1500)
 					style.update(sty)
 					rstarvals = 1.*b.master.metfunc.F(rvals[i:i+1])
-					b.add_curves_uv(xh.cm.rstarlines_special_2(rstarvals, b.uvbounds, c=b.master.rparams['c'], sty=style, inf=1.*inf, npoints=1.*npoints))
+					b.add_curves_uv(xh.cm.rstarlines_special_2(rstarvals, b.uvbounds, c=b.master.rparams['c'], sty=style, inf=1.*inf, npoints=1*npoints))
 	return reglist
 
 
 def colorlines(reglist, rmin=1.1, rmax=25., dr=.5, sty={}, cm=plt.cm.hsv_r, npoints=2001, inf=25.):
 	"""
 	Add colorscaled lines of constant radius to region.
 	Useful to check for matching.
```

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/draw_dS.py` & `xhorizon-1.1.1/src/xhorizon/evap/draw_dS.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/evap.py` & `xhorizon-1.1.1/src/xhorizon/evap/evap.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 		ps_matchmode = list of strings, each either 'ru' or 'rv', to determine how future slice is sliced when fslice is active
 	"""
 	print("du funclist_chain")
 	print(repr(du))
 	print("dv funclist_chain")
 	print(repr(dv))
 	## init default values
-	if u0==None:
+	if u0 is None:
 		u0 = np.zeros(len(funclist))
-	if v0==None:
+	if v0 is None:
 		v0 = np.zeros(len(funclist))
 	if ps_matchmode==None:
 		ps_matchmode = ['rv' for func in funclist]
 	if fs_matchmode==None:
 		fs_matchmode = ['rv' for func in funclist]
 	## set irrelevant first and last du and dv values to zero
 	du[0], du[-1] = 0., 0.
```

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/helpers.py` & `xhorizon-1.1.1/src/xhorizon/evap/helpers.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/legend.py` & `xhorizon-1.1.1/src/xhorizon/evap/legend.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/massplot.py` & `xhorizon-1.1.1/src/xhorizon/evap/massplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from pprint import pprint
 import matplotlib.patches
 
 def massplotrc():
 	## tex
-	plt.rcParams['text.usetex'] = True
+	#plt.rcParams['text.usetex'] = True
 	plt.rcParams['font.family'] = 'serif'
 	plt.rcParams['font.serif'] = []
-	plt.rcParams['text.latex.preamble'] = []
+	#plt.rcParams['text.latex.preamble'] = []
 	## rc
 	plt.rcParams['font.size'] = 7
 	plt.rcParams['axes.linewidth'] = .4
 	plt.rcParams['xtick.major.size'] = 2
 	plt.rcParams['ytick.major.size'] = 2
```

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/schwarzparams.py` & `xhorizon-1.1.1/src/xhorizon/evap/schwarzparams.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/evap/tests.py` & `xhorizon-1.1.1/src/xhorizon/evap/tests.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/__init__.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/__init__.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/active_slice_class.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/active_slice_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/helpers.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/helpers.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/interpolators.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/interpolators.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/passive_slice_class.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/passive_slice_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/reg_corner_masks.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/reg_corner_masks.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/shell_junction/tests.py` & `xhorizon-1.1.1/src/xhorizon/shell_junction/tests.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/tortoise/metfunc_class.py` & `xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_class.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/tortoise/metfunc_factory.py` & `xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_factory.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/tortoise/metfunc_tests.py` & `xhorizon-1.1.1/src/xhorizon/tortoise/metfunc_tests.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon/tortoise/tortoise.py` & `xhorizon-1.1.1/src/xhorizon/tortoise/tortoise.py`

 * *Files identical despite different names*

### Comparing `xhorizon-1.0.0/src/xhorizon.egg-info/PKG-INFO` & `xhorizon-1.1.1/src/xhorizon.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-Metadata-Version: 2.1
-Name: xhorizon
-Version: 1.0.0
-Summary: A Python package for explicitly computing Penrose diagrams in general relativity.
-Home-page: https://github.com/xh-diagrams/xhorizon
-Author: Joseph C Schindler
-Author-email: jcschindler01@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-
-xhorizon
-================================
-
-xhorizon: Explicitly computed Penrose diagrams in general relativity.
-
-A Python package.
-
-| **I finally gave the package a makeover and updated to Python 3!**
-
-| **The new documentation is still under construction...**
-| **Check back soon for examples and a tutorial!**
-
-
-Links
------
-   - `GitHub <https://github.com/xh-diagrams/xhorizon>`_.
-   - `Documetation <https://xhorizon.readthedocs.io/>`_.
-   - `PyPi <https://pypi.org/project/xhorizon/>`_.
-
-
-Getting Started
----------------
-::
-
-  pip install xhorizon
-
-
+Metadata-Version: 2.1
+Name: xhorizon
+Version: 1.1.1
+Summary: A Python package for explicitly computing Penrose diagrams in general relativity.
+Home-page: https://github.com/xh-diagrams/xhorizon
+Author: Joseph C Schindler
+Author-email: jcschindler01@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+
+xhorizon
+================================
+
+
+*xhorizon*: Explicitly computing Penrose diagrams in general relativity.
+
+A Python package.
+
+
+| **I finally gave the package a makeover and updated to Python 3!**
+
+| **The new documentation is still under construction...**
+| **but there is now an ever expanding tutorial!**
+
+
+
+Links
+-----
+   - `GitHub <https://github.com/xh-diagrams/xhorizon>`_.
+   - `Documentation <https://xhorizon.readthedocs.io/>`_.
+   - `PyPi <https://pypi.org/project/xhorizon/>`_.
+
+
+Background Theory
+-----------------
+JC Schindler, A Aguirre. 
+*Algorithms for the explicit computation of Penrose diagrams.*
+`Class Quantum Grav 35 105019 <https://doi.org/10.1088/1361-6382/aabce2>`_.
+(2018).
+`arxiv:1802.02263 <https://arxiv.org/abs/1802.02263>`_.
+
+
+Getting Started
+---------------
+To install::
+
+   pip install xhorizon
+
+To start using the tools, begin with the `tutorial <https://xhorizon.readthedocs.io/en/stable/TUTORIAL/00-overview.html>`_ and keep an eye out for `example scripts <https://github.com/xh-diagrams/xhorizon/tree/main/scripts/examples>`_.
+
```

### Comparing `xhorizon-1.0.0/src/xhorizon.egg-info/SOURCES.txt` & `xhorizon-1.1.1/src/xhorizon.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/xhorizon/__init__.py
 src/xhorizon.egg-info/PKG-INFO
 src/xhorizon.egg-info/SOURCES.txt
 src/xhorizon.egg-info/dependency_links.txt
-src/xhorizon.egg-info/requires.txt
 src/xhorizon.egg-info/top_level.txt
 src/xhorizon/diagram_tools/__init__.py
 src/xhorizon/diagram_tools/block_fill.py
 src/xhorizon/diagram_tools/block_masks.py
 src/xhorizon/diagram_tools/coord_transf.py
 src/xhorizon/diagram_tools/curve_class.py
 src/xhorizon/diagram_tools/curvemakers.py
```


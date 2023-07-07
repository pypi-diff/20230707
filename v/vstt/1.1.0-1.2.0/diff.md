# Comparing `tmp/vstt-1.1.0.tar.gz` & `tmp/vstt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-1.1.0.tar", last modified: Tue Jun 27 08:43:02 2023, max compression
+gzip compressed data, was "vstt-1.2.0.tar", last modified: Fri Jul  7 10:12:35 2023, max compression
```

## Comparing `vstt-1.1.0.tar` & `vstt-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:43:02.725079 vstt-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-27 08:42:45.000000 vstt-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-27 08:43:02.725079 vstt-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-27 08:42:45.000000 vstt-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-27 08:42:45.000000 vstt-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:43:02.725079 vstt-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:43:02.721079 vstt-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:43:02.721079 vstt-1.1.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-27 08:42:45.000000 vstt-1.1.0/src/vstt/vtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:43:02.725079 vstt-1.1.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-27 08:43:02.000000 vstt-1.1.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-27 08:43:02.000000 vstt-1.1.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 08:43:02.000000 vstt-1.1.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 08:43:02.000000 vstt-1.1.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 08:43:02.000000 vstt-1.1.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 08:43:02.000000 vstt-1.1.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 08:43:02.725079 vstt-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-27 08:42:45.000000 vstt-1.1.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:12:35.145755 vstt-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-07 10:12:23.000000 vstt-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-07 10:12:35.145755 vstt-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 10:12:23.000000 vstt-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-07 10:12:23.000000 vstt-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:12:35.145755 vstt-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:12:35.137755 vstt-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:12:35.141755 vstt-1.2.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16593 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-07 10:12:23.000000 vstt-1.2.0/src/vstt/vtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:12:35.141755 vstt-1.2.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-07 10:12:35.000000 vstt-1.2.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-07 10:12:35.000000 vstt-1.2.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:12:35.000000 vstt-1.2.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 10:12:35.000000 vstt-1.2.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-07 10:12:35.000000 vstt-1.2.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 10:12:35.000000 vstt-1.2.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:12:35.145755 vstt-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-07 10:12:23.000000 vstt-1.2.0/tests/test_vstt.py
```

### Comparing `vstt-1.1.0/LICENSE` & `vstt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/PKG-INFO` & `vstt-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -32,12 +32,15 @@
 [![Docs](https://readthedocs.org/projects/vstt/badge/?version=main)](https://vstt.readthedocs.io)
 [![CI](https://github.com/ssciwr/vstt/actions/workflows/ci.yml/badge.svg)](https://github.com/ssciwr/vstt/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/ssciwr/vstt/branch/main/graph/badge.svg?token=sjsAdTyLH1)](https://codecov.io/gh/ssciwr/vstt)
 [![Sonar](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_vstt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_vstt)
 
 Visuomotor Serial Targeting Task (VSTT)
 
-Documentation: [vstt.readthedocs.io](https://vstt.readthedocs.io/)
+VSTT is an open source Python GUI tool for designing,
+running and analyzing motor skill acquisition experiments.
+
+See [vstt.readthedocs.io](https://vstt.readthedocs.io/) for more information.
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/gui.png)
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/results.png)
```

### Comparing `vstt-1.1.0/README.md` & `vstt-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,12 +4,15 @@
 [![Docs](https://readthedocs.org/projects/vstt/badge/?version=main)](https://vstt.readthedocs.io)
 [![CI](https://github.com/ssciwr/vstt/actions/workflows/ci.yml/badge.svg)](https://github.com/ssciwr/vstt/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/ssciwr/vstt/branch/main/graph/badge.svg?token=sjsAdTyLH1)](https://codecov.io/gh/ssciwr/vstt)
 [![Sonar](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_vstt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_vstt)
 
 Visuomotor Serial Targeting Task (VSTT)
 
-Documentation: [vstt.readthedocs.io](https://vstt.readthedocs.io/)
+VSTT is an open source Python GUI tool for designing,
+running and analyzing motor skill acquisition experiments.
+
+See [vstt.readthedocs.io](https://vstt.readthedocs.io/) for more information.
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/gui.png)
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/results.png)
```

### Comparing `vstt-1.1.0/pyproject.toml` & `vstt-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
   "pyautogui",
   "ascii-magic",
   "keyboard",
 ]
 docs = [
   "ipykernel",
   "matplotlib",
+  "myst_parser",
   "nbsphinx",
   "pandoc",
   "sphinx>=4.5.0",
   "sphinx_rtd_theme>=1.0.0",
   "shapely",
 ]
```

### Comparing `vstt-1.1.0/src/vstt/__main__.py` & `vstt-1.2.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/common.py` & `vstt-1.2.0/src/vstt/common.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/display.py` & `vstt-1.2.0/src/vstt/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         "to_center_movement_time": False,
         "to_target_time": True,
         "to_center_time": False,
         "to_target_distance": True,
         "to_center_distance": False,
         "to_target_rmse": True,
         "to_center_rmse": False,
+        "to_target_success": False,
+        "to_center_success": False,
         "averages": True,
     }
 
 
 def display_options_labels() -> Dict[str, str]:
     return {
         "to_target_paths": "Display cursor paths to target",
@@ -37,14 +39,16 @@
         "to_center_movement_time": "Statistic: movement time to center",
         "to_target_time": "Statistic: total time to target",
         "to_center_time": "Statistic: total time to center",
         "to_target_distance": "Statistic: movement distance to target",
         "to_center_distance": "Statistic: movement distance to center",
         "to_target_rmse": "Statistic: RMSE movement to target",
         "to_center_rmse": "Statistic: RMSE movement to center",
+        "to_target_success": "Statistic: successful movement to target",
+        "to_center_success": "Statistic: successful movement to center",
         "averages": "Also show statistics averaged over all targets",
     }
 
 
 def import_display_options(display_options_dict: dict) -> vstt.vtypes.DisplayOptions:
     return vstt.common.import_typed_dict(
         display_options_dict, default_display_options()
```

### Comparing `vstt-1.1.0/src/vstt/display_widget.py` & `vstt-1.2.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/experiment.py` & `vstt-1.2.0/src/vstt/experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/geom.py` & `vstt-1.2.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/gui.py` & `vstt-1.2.0/src/vstt/gui.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/joystick_wrapper.py` & `vstt-1.2.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/meta.py` & `vstt-1.2.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/meta_widget.py` & `vstt-1.2.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/results_widget.py` & `vstt-1.2.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/stats.py` & `vstt-1.2.0/src/vstt/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         stats = []
         for base_stat, label, unit in [
             ("reaction_time", "Reaction", "s"),
             ("movement_time", "Movement", "s"),
             ("time", "Time", "s"),
             ("distance", "Distance", ""),
             ("rmse", "RMSE", ""),
+            ("success", "Success", ""),
         ]:
             stats.append((f"to_{destination}_{base_stat}", label, unit))
         list_dest_stats.append((destination, stats))
     return list_dest_stats
 
 
 def _get_trial_data_columns() -> List[str]:
```

### Comparing `vstt-1.1.0/src/vstt/task.py` & `vstt-1.2.0/src/vstt/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         self._cursor_path = ShapeStim(
             win, vertices=[(0.0, 0.0)], lineColor="white", closeShape=False
         )
         self._cursor_path_vertices: List[Tuple[float, float]] = []
         self.clock = Clock()
         if trial["show_cursor_path"]:
             self.drawables.append(self._cursor_path)
+        self.first_target_of_condition_shown = False
 
     def cursor_path_add_vertex(
         self, vertex: Tuple[float, float], clear_existing: bool = False
     ) -> None:
         if clear_existing:
             self._cursor_path_vertices = []
         self._cursor_path_vertices.append(vertex)
@@ -203,14 +204,16 @@
                     trial["enter_to_skip_delay"],
                     trial["show_delay_countdown"],
                     self.trial_handler if trial["post_block_display_results"] else None,
                     self.experiment.display_options,
                     current_condition_first_trial_index,
                     True,
                     self.win,
+                    self.mouse,
+                    current_cursor_pos,
                 )
         if self.win.nDroppedFrames > 0:
             logging.warning(f"Dropped {self.win.nDroppedFrames} frames")
 
     def _do_splash_screen(self) -> None:
         vis.splash_screen(
             display_time_seconds=self.experiment.metadata["display_duration"],
@@ -261,14 +264,16 @@
                 trial["enter_to_skip_delay"],
                 trial["show_delay_countdown"],
                 self.trial_handler if trial["post_trial_display_results"] else None,
                 self.experiment.display_options,
                 self.trial_handler.thisTrialN,
                 False,
                 self.win,
+                self.mouse,
+                trial_manager.cursor.pos,
             )
         return trial_manager.cursor.pos
 
     def _do_target(
         self, trial: Dict[str, Any], index: int, tm: TrialManager, trial_data: TrialData
     ) -> None:
         minimum_window_for_flip = 1.0 / 60.0
@@ -292,14 +297,20 @@
                     tm.cursor.setPos(mouse_pos)
                 tm.cursor_path_add_vertex(mouse_pos, clear_existing=True)
             if not trial["fixed_target_intervals"]:
                 if is_central_target:
                     pre_target_delay = trial["pre_central_target_delay"]
                 else:
                     pre_target_delay = trial["pre_target_delay"]
+                    if (
+                        not tm.first_target_of_condition_shown
+                        and trial["pre_first_target_extra_delay"] > 0
+                    ):
+                        pre_target_delay += trial["pre_first_target_extra_delay"]
+                        tm.first_target_of_condition_shown = True
                 stop_waiting_time = t0 + pre_target_delay
             if stop_waiting_time > t0:
                 if trial["hide_target_when_reached"]:
                     vis.update_target_colors(
                         tm.targets, trial["show_inactive_targets"], None
                     )
                     if trial["show_target_labels"] and tm.target_labels is not None:
```

### Comparing `vstt-1.1.0/src/vstt/trial.py` & `vstt-1.2.0/src/vstt/trial.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         "show_target_labels": False,
         "target_labels": "0 1 2 3 4 5 6 7",
         "fixed_target_intervals": False,
         "target_duration": 5.0,
         "central_target_duration": 5.0,
         "pre_target_delay": 0.0,
         "pre_central_target_delay": 0.0,
+        "pre_first_target_extra_delay": 0.0,
         "target_distance": 0.4,
         "target_size": 0.04,
         "central_target_size": 0.02,
         "show_inactive_targets": True,
         "ignore_incorrect_targets": True,
         "play_sound": True,
         "use_joystick": False,
@@ -77,14 +78,15 @@
         "show_target_labels": "Display target labels",
         "target_labels": "Target labels",
         "fixed_target_intervals": "Fixed target display intervals",
         "target_duration": "Target display duration (secs)",
         "central_target_duration": "Central target display duration (secs)",
         "pre_target_delay": "Delay before outer target display (secs)",
         "pre_central_target_delay": "Delay before central target display (secs)",
+        "pre_first_target_extra_delay": "Extra delay before first outer target of condition (secs)",
         "target_distance": "Distance to targets (screen height fraction)",
         "target_size": "Target size (screen height fraction)",
         "central_target_size": "Central target size (screen height fraction)",
         "show_inactive_targets": "Show inactive targets",
         "ignore_incorrect_targets": "Ignore cursor hitting incorrect target",
         "play_sound": "Play a sound on target display",
         "use_joystick": "Control the cursor using a joystick",
@@ -129,14 +131,15 @@
     # make any negative time durations zero
     for duration in [
         "condition_timeout",
         "target_duration",
         "central_target_duration",
         "pre_target_delay",
         "pre_central_target_delay",
+        "pre_first_target_extra_delay",
         "post_trial_delay",
         "post_block_delay",
     ]:
         if trial[duration] < 0.0:  # type: ignore
             trial[duration] = 0.0  # type: ignore
     # convert string of target indices to a numpy array of ints
     target_indices = np.fromstring(trial["target_indices"], dtype="int", sep=" ")
```

### Comparing `vstt-1.1.0/src/vstt/trials_widget.py` & `vstt-1.2.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/update.py` & `vstt-1.2.0/src/vstt/update.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/src/vstt/vis.py` & `vstt-1.2.0/src/vstt/vis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 from typing import List
 from typing import Optional
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
 from PIL.Image import Image
 from psychopy.clock import Clock
 from psychopy.colors import colorNames
 from psychopy.data import TrialHandlerExt
+from psychopy.event import Mouse
 from psychopy.hardware.keyboard import Keyboard
 from psychopy.visual.basevisual import BaseVisualStim
 from psychopy.visual.circle import Circle
 from psychopy.visual.elementarray import ElementArrayStim
 from psychopy.visual.shape import ShapeStim
 from psychopy.visual.textbox2 import TextBox2
 from psychopy.visual.window import Window
@@ -144,15 +146,36 @@
 
 
 def _make_stats_txt(display_options: DisplayOptions, stats: pd.Series) -> str:
     txt_stats = ""
     for destination, stat_label_units in list_dest_stat_label_units():
         for stat, label, unit in stat_label_units:
             if display_options.get(stat, False):  # type: ignore
-                txt_stats += f"{label} (to {destination}): {stats[stat]: .3f}{unit}\n"
+                stat_str = f"{stats[stat]: .3f}{unit}"
+                if stat == "to_target_success" or stat == "to_center_success":
+                    if "to_target_success_trial" in stats:
+                        stat_str = f"{stats[stat]:.0%}"
+                    else:
+                        stat_str = f"{stats[stat] == 1}"
+                txt_stats += f"{label} (to {destination}): {stat_str}\n"
+    return txt_stats
+
+
+def _make_average_stats_txt(display_options: DisplayOptions, stats: pd.Series) -> str:
+    txt_stats = ""
+    for destination, stat_label_units in list_dest_stat_label_units():
+        for stat, label, unit in stat_label_units:
+            if display_options.get(stat, False):  # type: ignore
+                stat_str = f"{stats[stat]: .3f}{unit}"
+                if stat == "to_target_success" or stat == "to_center_success":
+                    if "to_target_success_trial" in stats:
+                        stat_str = f"{stats[stat + '_trial']:.0%}"
+                    else:
+                        stat_str = f"{stats[stat]: .0%}"
+                txt_stats += f"{label} (to {destination}): {stat_str}\n"
     return txt_stats
 
 
 def _make_stats_drawables(
     trial_handler: TrialHandlerExt,
     display_options: DisplayOptions,
     stats_df: pd.DataFrame,
@@ -178,14 +201,18 @@
     )
     # stats
     letter_height = 0.014
     # split target_pos pair into two scalars so they survive the groupby.mean()
     stats_df[["target_pos_x", "target_pos_y"]] = pd.DataFrame(
         stats_df.target_pos.tolist(), index=stats_df.index
     )
+    # convert to_target_success and to_center_success into scalars 0/1
+    stats_df.to_target_success = stats_df.to_target_success.astype(int)
+    stats_df.to_center_success = stats_df.to_center_success.astype(int)
+
     for _, row in (
         stats_df.groupby("target_index", as_index=False)
         .mean(numeric_only=True)
         .iterrows()
     ):
         color = colors[int(np.rint(row.target_index))]
         txt_stats = _make_stats_txt(display_options, row)
@@ -205,17 +232,35 @@
                     txt_stats,
                     pos=text_pos,
                     color=color,
                     alignment="center",
                     letterHeight=letter_height,
                 )
             )
+
+    # update the values of to_target_success and to_center_success to the success fraction
+    filtered_df = (
+        stats_df[
+            (stats_df.condition_index == i_condition)
+            & (stats_df.i_trial == trial_indices[0])
+        ]
+        if not len(trial_indices) > 1
+        else stats_df
+    )
+    to_target_success_fraction = sum(filtered_df.to_target_success) / len(
+        filtered_df.to_target_success
+    )
+    to_center_success_fraction = sum(filtered_df.to_center_success) / len(
+        filtered_df.to_center_success
+    )
+    stats_df["to_target_success"] = to_target_success_fraction
+    stats_df["to_center_success"] = to_center_success_fraction
     # average stats
     if display_options["averages"]:
-        txt_stats = "Averages:\n" + _make_stats_txt(
+        txt_stats = "Averages:\n" + _make_average_stats_txt(
             display_options, stats_df.mean(numeric_only=True)
         )
         drawables.append(
             TextBox2(
                 win,
                 txt_stats,
                 anchor="top_left",
@@ -285,14 +330,16 @@
     enter_to_skip_delay: bool,
     show_delay_countdown: bool,
     trial_handler: Optional[TrialHandlerExt],
     display_options: DisplayOptions,
     i_trial: int,
     all_trials_for_this_condition: bool,
     win: Optional[Window] = None,
+    mouse: Optional[Mouse] = None,
+    mouse_pos: Optional[Tuple[float, float]] = None,
     return_screenshot: bool = False,
 ) -> Optional[Image]:
     close_window_when_done = False
     if win is None:
         win = _make_window()
         close_window_when_done = True
     drawables = []
@@ -302,28 +349,45 @@
             condition_index = next(
                 iter(
                     stats_df.loc[stats_df.i_trial == i_trial].condition_index.to_numpy()
                 ),
                 -1,
             )
             stats_df = stats_df.loc[stats_df.condition_index == condition_index]
+            for dest in ["target", "center"]:
+                stats_df[f"to_{dest}_success_trial"] = get_successful_trial_fraction(
+                    stats_df, dest
+                )
         else:
             stats_df = stats_df.loc[stats_df.i_trial == i_trial]
         drawables = _make_stats_drawables(trial_handler, display_options, stats_df, win)
     return display_drawables(
         display_time_seconds,
         enter_to_skip_delay,
         show_delay_countdown,
         drawables,
         win,
         close_window_when_done,
+        mouse,
+        mouse_pos,
         return_screenshot,
     )
 
 
+def get_successful_trial_fraction(stats_df: pd.DataFrame, dest: str) -> float:
+    to_dest_success_trial = 0
+    trial_indices = stats_df["i_trial"].unique()
+    for trial_index in trial_indices:
+        data = stats_df.loc[stats_df.i_trial == trial_index]
+        to_dest_failed_number = (~data[f"to_{dest}_success"]).values.sum()
+        to_dest_success_trial += 1 if not to_dest_failed_number else 0
+    to_dest_success_trial_fraction = to_dest_success_trial / len(trial_indices)
+    return to_dest_success_trial_fraction
+
+
 def _make_textbox_press_enter(win: Window) -> TextBox2:
     return TextBox2(
         win,
         "Please press Enter when you are ready to continue...",
         pos=(0, -0.47),
         color="navy",
         alignment="center",
@@ -375,14 +439,16 @@
 def display_drawables(
     display_time_seconds: float,
     enter_to_skip_delay: bool,
     show_delay_countdown: bool,
     drawables: List[BaseVisualStim],
     win: Window,
     close_window_when_done: bool,
+    mouse: Optional[Mouse] = None,
+    mouse_pos: Optional[Tuple[float, float]] = None,
     return_screenshot: bool = False,
 ) -> Optional[Image]:
     screenshot = None
     if drawables is None:
         drawables = []
     if return_screenshot:
         # do one flip, take screenshot, return image
@@ -409,14 +475,16 @@
                 new_remaining_display_time = int(
                     np.ceil(display_time_seconds - clock.getTime())
                 )
                 if new_remaining_display_time < remaining_display_time:
                     remaining_display_time = new_remaining_display_time
                     countdown_textbox.text = f"{remaining_display_time}"
             try:
+                if mouse is not None and mouse_pos is not None:
+                    mouse.setPos(mouse_pos)
                 draw_and_flip(win, drawables, kb, "return")
             except MotorTaskCancelledByUser:
                 if close_window_when_done:
                     win.close()
                 return None
     if close_window_when_done:
         win.close()
```

### Comparing `vstt-1.1.0/src/vstt/vtypes.py` & `vstt-1.2.0/src/vstt/vtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     show_target_labels: bool
     target_labels: str
     fixed_target_intervals: bool
     target_duration: float
     central_target_duration: float
     pre_target_delay: float
     pre_central_target_delay: float
+    pre_first_target_extra_delay: float
     target_distance: float
     target_size: float
     central_target_size: float
     show_inactive_targets: bool
     ignore_incorrect_targets: bool
     play_sound: bool
     use_joystick: bool
@@ -58,14 +59,16 @@
     to_center_movement_time: bool
     to_target_time: bool
     to_center_time: bool
     to_target_distance: bool
     to_center_distance: bool
     to_target_rmse: bool
     to_center_rmse: bool
+    to_target_success: bool
+    to_center_success: bool
     averages: bool
 
 
 class Metadata(TypedDict):
     name: str
     subject: str
     date: str
```

### Comparing `vstt-1.1.0/src/vstt.egg-info/PKG-INFO` & `vstt-1.2.0/src/vstt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 1.1.0
+Version: 1.2.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -32,12 +32,15 @@
 [![Docs](https://readthedocs.org/projects/vstt/badge/?version=main)](https://vstt.readthedocs.io)
 [![CI](https://github.com/ssciwr/vstt/actions/workflows/ci.yml/badge.svg)](https://github.com/ssciwr/vstt/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/ssciwr/vstt/branch/main/graph/badge.svg?token=sjsAdTyLH1)](https://codecov.io/gh/ssciwr/vstt)
 [![Sonar](https://sonarcloud.io/api/project_badges/measure?project=ssciwr_vstt&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ssciwr_vstt)
 
 Visuomotor Serial Targeting Task (VSTT)
 
-Documentation: [vstt.readthedocs.io](https://vstt.readthedocs.io/)
+VSTT is an open source Python GUI tool for designing,
+running and analyzing motor skill acquisition experiments.
+
+See [vstt.readthedocs.io](https://vstt.readthedocs.io/) for more information.
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/gui.png)
 
 ![screenshot](https://raw.githubusercontent.com/ssciwr/vstt/main/docs/quickstart/images/results.png)
```

### Comparing `vstt-1.1.0/src/vstt.egg-info/SOURCES.txt` & `vstt-1.2.0/src/vstt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_display.py` & `vstt-1.2.0/tests/test_display.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,19 @@
         "to_target_distance": False,
         "to_center_distance": False,
         "to_target_rmse": False,
         "to_center_rmse": False,
         "averages": True,
         "unknown_key1": "ignore me",
         "unknown_key2": False,
+        "to_target_success": False,
+        "to_center_success": False,
     }
+    for key in default_display_options:
+        assert key in display_options_dict
     # if any keys are missing or have invalid values, default values are used instead
     missing_keys = [
         "to_center_reaction_time",
         "to_target_rmse",
         "to_center_rmse",
     ]
     for key in missing_keys:
```

### Comparing `vstt-1.1.0/tests/test_display_widget.py` & `vstt-1.2.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_experiment.py` & `vstt-1.2.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_geom.py` & `vstt-1.2.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_gui.py` & `vstt-1.2.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_joystick_wrapper.py` & `vstt-1.2.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_meta.py` & `vstt-1.2.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_meta_widget.py` & `vstt-1.2.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_results_widget.py` & `vstt-1.2.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_stats.py` & `vstt-1.2.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_task.py` & `vstt-1.2.0/tests/test_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,25 +215,27 @@
         assert (
             abs(to_target_timestamps[-1] - (count + 3) * target_duration)
             < allowed_error_on_timestamp
         )
 
 
 def test_task_condition_timeout_no_user_input(window: Window) -> None:
-    # 4 seconds condition timeout where each trial has 1 target which is displayed for up to 1.35 seconds
-    # should get 2 trials in ~2.70secs, 3rd trial should time out
+    # 4 seconds condition timeout where each trial has 1 target which is displayed for up to 1.3 seconds
+    # first target of condition has additional 0.20 seconds delay
+    # should get 2 trials in ~2.80secs, 3rd trial should time out
     experiment = Experiment()
     experiment.metadata["display_duration"] = 0.0
     trial1 = vstt.trial.default_trial()
     trial1["weight"] = 100
     trial1["condition_timeout"] = 4.0
     trial1["num_targets"] = 1
-    trial1["target_duration"] = 1.35
+    trial1["target_duration"] = 1.30
     trial1["pre_target_delay"] = 0.0
     trial1["pre_central_target_delay"] = 0.0
+    trial1["pre_first_target_extra_delay"] = 0.20
     trial1["add_central_target"] = False
     trial1["automove_cursor_to_center"] = False
     trial1["freeze_cursor_between_targets"] = False
     trial1["post_block_delay"] = 0.0
     trial1["play_sound"] = False
     # 6 seconds timeout: 3 targets, each for 1.05 seconds -> single completed trial
     trial2 = deepcopy(trial1)
@@ -244,13 +246,14 @@
     assert experiment.trial_handler_with_results is None
     task = vstt.task.MotorTask(experiment, window)
     # run task without moving mouse, which will stay in center for entire experiment
     assert task.run() is True
     # task ran successfully, updated experiment with results
     assert experiment.has_unsaved_changes is True
     assert experiment.trial_handler_with_results is not None
+    experiment.stats.to_pickle("./df.pkl")
     # we should get exactly 3 trials
     assert len(experiment.stats.i_trial.unique()) == 3
     # first two trials have 1 target, last trial has 3 targets -> 5 targets total
     assert len(experiment.stats.to_target_success) == 5
     # all targets should have been missed
     assert np.all(~experiment.stats.to_target_success)
```

### Comparing `vstt-1.1.0/tests/test_trial.py` & `vstt-1.2.0/tests/test_trial.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         "hide_target_when_reached": True,
         "target_labels": "0 1 2 3 4 5",
         "fixed_target_intervals": False,
         "target_duration": 3,
         "central_target_duration": 3,
         "pre_target_delay": 0,
         "pre_central_target_delay": 0,
+        "pre_first_target_extra_delay": 0,
         "target_distance": 0.3,
         "target_size": 0.03,
         "central_target_size": 0.01,
         "show_inactive_targets": False,
         "ignore_incorrect_targets": True,
         "play_sound": True,
         "use_joystick": True,
@@ -111,35 +112,39 @@
 def test_validate_trial_durations() -> None:
     trial = vstt.trial.default_trial()
     # positive durations are not modified
     trial["target_duration"] = 1
     trial["central_target_duration"] = 1
     trial["pre_target_delay"] = 0.1
     trial["pre_central_target_delay"] = 0.087
+    trial["pre_first_target_extra_delay"] = 0.08123
     trial["post_trial_delay"] = 0.2
     trial["post_block_delay"] = 0.7
     vtrial = vstt.trial.import_and_validate_trial(trial)
     assert vtrial["target_duration"] == 1
     assert vtrial["central_target_duration"] == 1
     assert vtrial["pre_target_delay"] == 0.1
     assert vtrial["pre_central_target_delay"] == 0.087
+    assert vtrial["pre_first_target_extra_delay"] == 0.08123
     assert vtrial["post_trial_delay"] == 0.2
     assert vtrial["post_block_delay"] == 0.7
     # negative durations are cast to zero
     trial["target_duration"] = -1
     trial["central_target_duration"] = -0.8
     trial["pre_target_delay"] = -0.1
     trial["pre_central_target_delay"] = -0.087
+    trial["pre_first_target_extra_delay"] = -0.08123
     trial["post_trial_delay"] = -0.2
     trial["post_block_delay"] = -0.7
     vtrial = vstt.trial.import_and_validate_trial(trial)
     assert vtrial["target_duration"] == 0
     assert vtrial["central_target_duration"] == 0
     assert vtrial["pre_target_delay"] == 0
     assert vtrial["pre_central_target_delay"] == 0
+    assert vtrial["pre_first_target_extra_delay"] == 0
     assert vtrial["post_trial_delay"] == 0
     assert vtrial["post_block_delay"] == 0
 
 
 def test_validate_trial_target_order() -> None:
     trial = vstt.trial.default_trial()
     assert isinstance(trial["target_indices"], str)
```

### Comparing `vstt-1.1.0/tests/test_trials_widget.py` & `vstt-1.2.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_update.py` & `vstt-1.2.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `vstt-1.1.0/tests/test_vis.py` & `vstt-1.2.0/tests/test_vis.py`

 * *Files 8% similar despite different names*

```diff
@@ -223,14 +223,16 @@
         "to_target_time": False,
         "to_center_time": False,
         "to_target_distance": False,
         "to_center_distance": False,
         "to_target_rmse": False,
         "to_center_rmse": False,
         "averages": False,
+        "to_target_success": False,
+        "to_center_success": False,
     }
     for all_trials_for_this_condition in [False, True]:
         # trial 0: 0,1,2 are trials without auto-move to center
         screenshot = gtu.call_target_and_get_screenshot(
             vstt.vis.display_results,
             (
                 60,
@@ -284,14 +286,16 @@
         "to_target_time": True,
         "to_center_time": True,
         "to_target_distance": True,
         "to_center_distance": True,
         "to_target_rmse": True,
         "to_center_rmse": True,
         "averages": True,
+        "to_target_success": True,
+        "to_center_success": True,
     }
     for all_trials_for_this_condition in [False, True]:
         # trial 0: 0,1,2 are trials without auto-move to center
         screenshot = gtu.call_target_and_get_screenshot(
             vstt.vis.display_results,
             (
                 60,
```


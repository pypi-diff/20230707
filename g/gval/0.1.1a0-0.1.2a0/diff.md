# Comparing `tmp/gval-0.1.1a0.tar.gz` & `tmp/gval-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gval-0.1.1a0.tar", last modified: Fri Jul  7 06:42:30 2023, max compression
+gzip compressed data, was "gval-0.1.2a0.tar", last modified: Fri Jul  7 06:49:49 2023, max compression
```

## Comparing `gval-0.1.1a0.tar` & `gval-0.1.2a0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/
--rw-rw-r--   0 sven      (1000) sven      (1000)      528 2023-05-08 19:00:19.000000 gval-0.1.1a0/LICENSE.MD
--rw-rw-r--   0 sven      (1000) sven      (1000)     3048 2023-07-07 06:42:30.113097 gval-0.1.1a0/PKG-INFO
--rw-rw-r--   0 sven      (1000) sven      (1000)     2857 2023-07-07 05:28:04.000000 gval-0.1.1a0/README.MD
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/docs/
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/docs/sphinx/
--rw-rw-r--   0 sven      (1000) sven      (1000)     2754 2023-07-07 05:28:04.000000 gval-0.1.1a0/docs/sphinx/PYPI_README.MD
--rw-rw-r--   0 sven      (1000) sven      (1000)     2770 2023-07-07 05:28:04.000000 gval-0.1.1a0/docs/sphinx/SPHINX_README.MD
--rw-rw-r--   0 sven      (1000) sven      (1000)     1338 2023-07-07 06:42:24.000000 gval-0.1.1a0/pyproject.toml
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/requirements/
--rw-rw-r--   0 sven      (1000) sven      (1000)      478 2023-07-07 05:28:04.000000 gval-0.1.1a0/requirements/base.txt
--rw-rw-r--   0 sven      (1000) sven      (1000)      234 2023-07-07 06:42:30.113097 gval-0.1.1a0/setup.cfg
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval/
--rw-rw-r--   0 sven      (1000) sven      (1000)      388 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/__init__.py
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval/accessors/
--rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-04-05 20:48:55.000000 gval-0.1.1a0/src/gval/accessors/__init__.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      441 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/accessors/gval_array.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     4015 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/accessors/gval_dataframe.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      435 2023-04-05 20:48:55.000000 gval-0.1.1a0/src/gval/accessors/gval_dataset.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    26071 2023-07-07 05:28:04.000000 gval-0.1.1a0/src/gval/accessors/gval_xarray.py
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval/comparison/
--rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-04-14 21:42:31.000000 gval-0.1.1a0/src/gval/comparison/__init__.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    10792 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/comparison/agreement.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    13533 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/comparison/compute_categorical_metrics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     7368 2023-06-30 17:06:41.000000 gval-0.1.1a0/src/gval/comparison/compute_comparison.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     2605 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/comparison/compute_continuous_metrics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    11460 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/comparison/pairing_functions.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    13348 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/comparison/tabulation.py
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval/homogenize/
--rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-03-21 17:27:31.000000 gval-0.1.1a0/src/gval/homogenize/__init__.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     4278 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/homogenize/numeric_alignment.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     3316 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/homogenize/rasterize.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    10875 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/homogenize/spatial_alignment.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     2630 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/homogenize/vectorize.py
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval/statistics/
--rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-03-21 17:27:31.000000 gval-0.1.1a0/src/gval/statistics/__init__.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     1278 2023-03-21 17:27:31.000000 gval-0.1.1a0/src/gval/statistics/base_statistics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     9951 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/statistics/categorical_stat_funcs.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     9145 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/statistics/categorical_statistics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     9339 2023-06-28 16:23:50.000000 gval-0.1.1a0/src/gval/statistics/continuous_stat_funcs.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     2744 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/statistics/continuous_stat_utils.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     9147 2023-06-30 17:06:41.000000 gval-0.1.1a0/src/gval/statistics/continuous_statistics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      892 2023-03-22 00:55:59.000000 gval-0.1.1a0/src/gval/statistics/test.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      920 2023-03-22 00:55:59.000000 gval-0.1.1a0/src/gval/statistics/test2.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      462 2023-06-14 17:49:51.000000 gval-0.1.1a0/src/gval/statistics/test3.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      156 2023-06-14 17:48:41.000000 gval-0.1.1a0/src/gval/statistics/test4.py
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval/utils/
--rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-03-21 17:27:31.000000 gval-0.1.1a0/src/gval/utils/__init__.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      555 2023-03-21 17:27:31.000000 gval-0.1.1a0/src/gval/utils/exceptions.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     8522 2023-06-16 15:18:58.000000 gval-0.1.1a0/src/gval/utils/loading_datasets.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     2902 2023-06-30 17:06:41.000000 gval-0.1.1a0/src/gval/utils/schemas.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     6613 2023-07-07 05:28:04.000000 gval-0.1.1a0/src/gval/utils/visualize.py
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/src/gval.egg-info/
--rw-rw-r--   0 sven      (1000) sven      (1000)     3048 2023-07-07 06:42:30.000000 gval-0.1.1a0/src/gval.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1000) sven      (1000)     1752 2023-07-07 06:42:30.000000 gval-0.1.1a0/src/gval.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1000) sven      (1000)        1 2023-07-07 06:42:30.000000 gval-0.1.1a0/src/gval.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1000) sven      (1000)      568 2023-07-07 06:42:30.000000 gval-0.1.1a0/src/gval.egg-info/requires.txt
--rw-rw-r--   0 sven      (1000) sven      (1000)        5 2023-07-07 06:42:30.000000 gval-0.1.1a0/src/gval.egg-info/top_level.txt
-drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:42:30.113097 gval-0.1.1a0/tests/
--rw-rw-r--   0 sven      (1000) sven      (1000)      719 2023-06-12 23:04:35.000000 gval-0.1.1a0/tests/test.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     9237 2023-07-07 05:28:04.000000 gval-0.1.1a0/tests/test_accessors.py
--rw-rw-r--   0 sven      (1000) sven      (1000)    12225 2023-06-30 17:06:41.000000 gval-0.1.1a0/tests/test_compare.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     3134 2023-05-01 17:01:35.000000 gval-0.1.1a0/tests/test_compute_categorical_metrics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     3715 2023-06-28 16:23:50.000000 gval-0.1.1a0/tests/test_compute_continuous_metrics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     4964 2023-06-28 16:23:50.000000 gval-0.1.1a0/tests/test_continuous_metrics.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     8676 2023-05-23 19:40:17.000000 gval-0.1.1a0/tests/test_homogenize.py
--rw-rw-r--   0 sven      (1000) sven      (1000)      645 2023-03-20 17:43:07.000000 gval-0.1.1a0/tests/test_load_xarray.py
--rw-rw-r--   0 sven      (1000) sven      (1000)     3522 2023-04-07 01:46:26.000000 gval-0.1.1a0/tests/test_statistics.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/
+-rw-rw-r--   0 sven      (1000) sven      (1000)      528 2023-05-08 19:00:19.000000 gval-0.1.2a0/LICENSE.MD
+-rw-rw-r--   0 sven      (1000) sven      (1000)     3283 2023-07-07 06:49:49.175830 gval-0.1.2a0/PKG-INFO
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2857 2023-07-07 05:28:04.000000 gval-0.1.2a0/README.MD
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/docs/
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/docs/sphinx/
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2754 2023-07-07 05:28:04.000000 gval-0.1.2a0/docs/sphinx/PYPI_README.MD
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2770 2023-07-07 05:28:04.000000 gval-0.1.2a0/docs/sphinx/SPHINX_README.MD
+-rw-rw-r--   0 sven      (1000) sven      (1000)     1340 2023-07-07 06:49:45.000000 gval-0.1.2a0/pyproject.toml
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/requirements/
+-rw-rw-r--   0 sven      (1000) sven      (1000)      478 2023-07-07 05:28:04.000000 gval-0.1.2a0/requirements/base.txt
+-rw-rw-r--   0 sven      (1000) sven      (1000)      234 2023-07-07 06:49:49.175830 gval-0.1.2a0/setup.cfg
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval/
+-rw-rw-r--   0 sven      (1000) sven      (1000)      388 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/__init__.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval/accessors/
+-rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-04-05 20:48:55.000000 gval-0.1.2a0/src/gval/accessors/__init__.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      441 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/accessors/gval_array.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     4015 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/accessors/gval_dataframe.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      435 2023-04-05 20:48:55.000000 gval-0.1.2a0/src/gval/accessors/gval_dataset.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    26071 2023-07-07 05:28:04.000000 gval-0.1.2a0/src/gval/accessors/gval_xarray.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval/comparison/
+-rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-04-14 21:42:31.000000 gval-0.1.2a0/src/gval/comparison/__init__.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    10792 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/comparison/agreement.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    13533 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/comparison/compute_categorical_metrics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     7368 2023-06-30 17:06:41.000000 gval-0.1.2a0/src/gval/comparison/compute_comparison.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2605 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/comparison/compute_continuous_metrics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    11460 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/comparison/pairing_functions.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    13348 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/comparison/tabulation.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval/homogenize/
+-rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-03-21 17:27:31.000000 gval-0.1.2a0/src/gval/homogenize/__init__.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     4278 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/homogenize/numeric_alignment.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     3316 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/homogenize/rasterize.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    10875 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/homogenize/spatial_alignment.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2630 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/homogenize/vectorize.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval/statistics/
+-rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-03-21 17:27:31.000000 gval-0.1.2a0/src/gval/statistics/__init__.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     1278 2023-03-21 17:27:31.000000 gval-0.1.2a0/src/gval/statistics/base_statistics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     9951 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/statistics/categorical_stat_funcs.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     9145 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/statistics/categorical_statistics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     9339 2023-06-28 16:23:50.000000 gval-0.1.2a0/src/gval/statistics/continuous_stat_funcs.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2744 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/statistics/continuous_stat_utils.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     9147 2023-06-30 17:06:41.000000 gval-0.1.2a0/src/gval/statistics/continuous_statistics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      892 2023-03-22 00:55:59.000000 gval-0.1.2a0/src/gval/statistics/test.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      920 2023-03-22 00:55:59.000000 gval-0.1.2a0/src/gval/statistics/test2.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      462 2023-06-14 17:49:51.000000 gval-0.1.2a0/src/gval/statistics/test3.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      156 2023-06-14 17:48:41.000000 gval-0.1.2a0/src/gval/statistics/test4.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval/utils/
+-rw-rw-r--   0 sven      (1000) sven      (1000)        0 2023-03-21 17:27:31.000000 gval-0.1.2a0/src/gval/utils/__init__.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      555 2023-03-21 17:27:31.000000 gval-0.1.2a0/src/gval/utils/exceptions.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     8522 2023-06-16 15:18:58.000000 gval-0.1.2a0/src/gval/utils/loading_datasets.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     2902 2023-06-30 17:06:41.000000 gval-0.1.2a0/src/gval/utils/schemas.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     6613 2023-07-07 05:28:04.000000 gval-0.1.2a0/src/gval/utils/visualize.py
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/src/gval.egg-info/
+-rw-rw-r--   0 sven      (1000) sven      (1000)     3283 2023-07-07 06:49:49.000000 gval-0.1.2a0/src/gval.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1000) sven      (1000)     1752 2023-07-07 06:49:49.000000 gval-0.1.2a0/src/gval.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1000) sven      (1000)        1 2023-07-07 06:49:49.000000 gval-0.1.2a0/src/gval.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1000) sven      (1000)      568 2023-07-07 06:49:49.000000 gval-0.1.2a0/src/gval.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1000) sven      (1000)        5 2023-07-07 06:49:49.000000 gval-0.1.2a0/src/gval.egg-info/top_level.txt
+drwxrwxr-x   0 sven      (1000) sven      (1000)        0 2023-07-07 06:49:49.175830 gval-0.1.2a0/tests/
+-rw-rw-r--   0 sven      (1000) sven      (1000)      719 2023-06-12 23:04:35.000000 gval-0.1.2a0/tests/test.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     9237 2023-07-07 05:28:04.000000 gval-0.1.2a0/tests/test_accessors.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)    12225 2023-06-30 17:06:41.000000 gval-0.1.2a0/tests/test_compare.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     3134 2023-05-01 17:01:35.000000 gval-0.1.2a0/tests/test_compute_categorical_metrics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     3715 2023-06-28 16:23:50.000000 gval-0.1.2a0/tests/test_compute_continuous_metrics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     4964 2023-06-28 16:23:50.000000 gval-0.1.2a0/tests/test_continuous_metrics.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     8676 2023-05-23 19:40:17.000000 gval-0.1.2a0/tests/test_homogenize.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)      645 2023-03-20 17:43:07.000000 gval-0.1.2a0/tests/test_load_xarray.py
+-rw-rw-r--   0 sven      (1000) sven      (1000)     3522 2023-04-07 01:46:26.000000 gval-0.1.2a0/tests/test_statistics.py
```

### Comparing `gval-0.1.1a0/LICENSE.MD` & `gval-0.1.2a0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/PKG-INFO` & `gval-0.1.2a0/README.MD`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-Metadata-Version: 2.1
-Name: gval
-Version: 0.1.1a0
-Summary: Flexible, portable, and efficient geospatial evaluations for a variety of data.
-License: MIT
-Keywords: geospatial,evaluations
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.MD
-
- ![alt
+![alt text](https://github.com/NOAA-OWP/gval/raw/main/docs/images/gval_dark_mode.png#gh-dark-mode-only) ![alt
 text](https://github.com/NOAA-OWP/gval/raw/main/docs/images/gval_light_mode.png#gh-light-mode-only)
 
 ![Build and
 Test](https://github.com/NOAA-OWP/gval/actions/workflows/python-app.yml/badge.svg)![Coverage](https://github.com/NOAA-OWP/gval/raw/testing/docs/images/coverage.svg)
 
 GVAL (pronounced "g-val") is a high-level Python framework to evaluate
 the skill of geospatial datasets by comparing candidates to benchmark
```

### Comparing `gval-0.1.1a0/README.MD` & `gval-0.1.2a0/docs/sphinx/PYPI_README.MD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![alt text](https://github.com/NOAA-OWP/gval/raw/main/docs/images/gval_dark_mode.png#gh-dark-mode-only) ![alt
+ ![alt
 text](https://github.com/NOAA-OWP/gval/raw/main/docs/images/gval_light_mode.png#gh-light-mode-only)
 
 ![Build and
 Test](https://github.com/NOAA-OWP/gval/actions/workflows/python-app.yml/badge.svg)![Coverage](https://github.com/NOAA-OWP/gval/raw/testing/docs/images/coverage.svg)
 
 GVAL (pronounced "g-val") is a high-level Python framework to evaluate
 the skill of geospatial datasets by comparing candidates to benchmark
```

### Comparing `gval-0.1.1a0/docs/sphinx/PYPI_README.MD` & `gval-0.1.2a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: gval
+Version: 0.1.2a0
+Summary: Flexible, portable, and efficient geospatial evaluations for a variety of data.
+Author-email: Fernando Aristizabal <fernando.aristizabal@noaa.gov>, Gregory Petrochenkov <gregory.petrochenkov@noaa.gov>
+License: MIT
+Project-URL: repository, https://github.com/NOAA-OWP/gval
+Project-URL: homepage, https://noaa-owp.github.io/gval/
+Keywords: geospatial,evaluations
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.MD
+
  ![alt
 text](https://github.com/NOAA-OWP/gval/raw/main/docs/images/gval_light_mode.png#gh-light-mode-only)
 
 ![Build and
 Test](https://github.com/NOAA-OWP/gval/actions/workflows/python-app.yml/badge.svg)![Coverage](https://github.com/NOAA-OWP/gval/raw/testing/docs/images/coverage.svg)
 
 GVAL (pronounced "g-val") is a high-level Python framework to evaluate
```

### Comparing `gval-0.1.1a0/docs/sphinx/SPHINX_README.MD` & `gval-0.1.2a0/docs/sphinx/SPHINX_README.MD`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/pyproject.toml` & `gval-0.1.2a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'gval'
 description = "Flexible, portable, and efficient geospatial evaluations for a variety of data."
-
-
-
+authors = [
+    {name = "Fernando Aristizabal", email = "fernando.aristizabal@noaa.gov"},
+    {name = "Gregory Petrochenkov", email = "gregory.petrochenkov@noaa.gov"}
+]
 requires-python = ">=3.8"
 keywords = ["geospatial", "evaluations"]
 license = {text = "MIT"}
-version = "0.1.1-alpha"
+version = "0.1.2-alpha"
 dynamic = ["readme", "dependencies"]
 
+
 [project.optional-dependencies]
 dev = ["pytest==7.2.2",
     "pytest-benchmark==4.0.0",
     "pytest-cov==4.1.0",
     "pytest-cases==3.6.14",
     "flake8==6.0.0",
     "flake8-black==0.3.6",
@@ -33,20 +35,16 @@
     "nbsphinx==0.9.2",
     "sqlalchemy==2.0.17",
     "colorama==0.4.6",
     "build==0.10.0",
     "twine==4.0.2"
 ]
 
-[metadata]
-authors = [
-    {name = "Fernando Aristizabal", email = "fernando.aristizabal@noaa.gov"},
-    {name = "Gregory Petrochenkov", email = "gregory.petrochenkov@noaa.gov"}
-]
-
+[project.urls]
 repository = "https://github.com/NOAA-OWP/gval"
 homepage = "https://noaa-owp.github.io/gval/"
 
 
+
 [tool.setuptools.dynamic]
 dependencies = {file = ["./requirements/base.txt"]}
 readme = {file = ["./docs/sphinx/PYPI_README.MD"], content-type = "text/markdown"}
```

### Comparing `gval-0.1.1a0/src/gval/accessors/gval_dataframe.py` & `gval-0.1.2a0/src/gval/accessors/gval_dataframe.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/accessors/gval_xarray.py` & `gval-0.1.2a0/src/gval/accessors/gval_xarray.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/comparison/agreement.py` & `gval-0.1.2a0/src/gval/comparison/agreement.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/comparison/compute_categorical_metrics.py` & `gval-0.1.2a0/src/gval/comparison/compute_categorical_metrics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/comparison/compute_comparison.py` & `gval-0.1.2a0/src/gval/comparison/compute_comparison.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/comparison/compute_continuous_metrics.py` & `gval-0.1.2a0/src/gval/comparison/compute_continuous_metrics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/comparison/pairing_functions.py` & `gval-0.1.2a0/src/gval/comparison/pairing_functions.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/comparison/tabulation.py` & `gval-0.1.2a0/src/gval/comparison/tabulation.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/homogenize/numeric_alignment.py` & `gval-0.1.2a0/src/gval/homogenize/numeric_alignment.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/homogenize/rasterize.py` & `gval-0.1.2a0/src/gval/homogenize/rasterize.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/homogenize/spatial_alignment.py` & `gval-0.1.2a0/src/gval/homogenize/spatial_alignment.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/homogenize/vectorize.py` & `gval-0.1.2a0/src/gval/homogenize/vectorize.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/base_statistics.py` & `gval-0.1.2a0/src/gval/statistics/base_statistics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/categorical_stat_funcs.py` & `gval-0.1.2a0/src/gval/statistics/categorical_stat_funcs.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/categorical_statistics.py` & `gval-0.1.2a0/src/gval/statistics/categorical_statistics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/continuous_stat_funcs.py` & `gval-0.1.2a0/src/gval/statistics/continuous_stat_funcs.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/continuous_stat_utils.py` & `gval-0.1.2a0/src/gval/statistics/continuous_stat_utils.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/continuous_statistics.py` & `gval-0.1.2a0/src/gval/statistics/continuous_statistics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/test.py` & `gval-0.1.2a0/src/gval/statistics/test.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/statistics/test2.py` & `gval-0.1.2a0/src/gval/statistics/test2.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/utils/exceptions.py` & `gval-0.1.2a0/src/gval/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/utils/loading_datasets.py` & `gval-0.1.2a0/src/gval/utils/loading_datasets.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/utils/schemas.py` & `gval-0.1.2a0/src/gval/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval/utils/visualize.py` & `gval-0.1.2a0/src/gval/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval.egg-info/PKG-INFO` & `gval-0.1.2a0/src/gval.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: gval
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: Flexible, portable, and efficient geospatial evaluations for a variety of data.
+Author-email: Fernando Aristizabal <fernando.aristizabal@noaa.gov>, Gregory Petrochenkov <gregory.petrochenkov@noaa.gov>
 License: MIT
+Project-URL: repository, https://github.com/NOAA-OWP/gval
+Project-URL: homepage, https://noaa-owp.github.io/gval/
 Keywords: geospatial,evaluations
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.MD
 
  ![alt
```

### Comparing `gval-0.1.1a0/src/gval.egg-info/SOURCES.txt` & `gval-0.1.2a0/src/gval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/src/gval.egg-info/requires.txt` & `gval-0.1.2a0/src/gval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test.py` & `gval-0.1.2a0/tests/test.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_accessors.py` & `gval-0.1.2a0/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_compare.py` & `gval-0.1.2a0/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_compute_categorical_metrics.py` & `gval-0.1.2a0/tests/test_compute_categorical_metrics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_compute_continuous_metrics.py` & `gval-0.1.2a0/tests/test_compute_continuous_metrics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_continuous_metrics.py` & `gval-0.1.2a0/tests/test_continuous_metrics.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_homogenize.py` & `gval-0.1.2a0/tests/test_homogenize.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_load_xarray.py` & `gval-0.1.2a0/tests/test_load_xarray.py`

 * *Files identical despite different names*

### Comparing `gval-0.1.1a0/tests/test_statistics.py` & `gval-0.1.2a0/tests/test_statistics.py`

 * *Files identical despite different names*


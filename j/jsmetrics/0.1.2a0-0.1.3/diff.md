# Comparing `tmp/jsmetrics-0.1.2a0.tar.gz` & `tmp/jsmetrics-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsmetrics-0.1.2a0.tar", last modified: Sat May 27 11:23:57 2023, max compression
+gzip compressed data, was "jsmetrics-0.1.3.tar", last modified: Fri Jul  7 08:35:47 2023, max compression
```

## Comparing `jsmetrics-0.1.2a0.tar` & `jsmetrics-0.1.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.112666 jsmetrics-0.1.2a0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
--rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
--rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
--rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/_static/images/jet_shift_violin.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/statement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.116666 jsmetrics-0.1.2a0/jsmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/core/check_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/details_for_all_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26250 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    22302 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    42201 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/jsmetrics/utils/windspeed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/jsmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:23:57.000000 jsmetrics-0.1.2a0/jsmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.120666 jsmetrics-0.1.2a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/metric_verification/
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/metric_verification/metric_verification.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:23:57.124666 jsmetrics-0.1.2a0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_jet_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-27 11:23:54.000000 jsmetrics-0.1.2a0/tests/unit/test_windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20782 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.353314 jsmetrics-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.349313 jsmetrics-0.1.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+-rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+-rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/jet_shift_violin.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/statement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/core/check_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/details_for_all_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26464 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22927 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.361315 jsmetrics-0.1.3/jsmetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20782 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.361315 jsmetrics-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.361315 jsmetrics-0.1.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/tests/metric_verification/
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/metric_verification/metric_verification.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_jet_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_windspeed_utils.py
```

### Comparing `jsmetrics-0.1.2a0/CONTRIBUTING.rst` & `jsmetrics-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/HISTORY.rst` & `jsmetrics-0.1.3/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 =======
 History
 =======
 
+0.1.3 (2023-07-07)
+-------------------------
+* Add "method='nearest'" to jet statistics and core algorithms for cases when coords cannot be represented within float precision range.
+
+0.1.2 (2023-06-06)
+-------------------------
+* Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data 
+* Add check for NoLeapDatetime
+
 
 0.1.2-alpha (2023-05-27)
 -------------------------
 * Add check for NoLeapDatetime
 
 
 0.1.1 (2023-05-26)
 -------------------------
 * Fix Woollings et al. 2010 and filter windows to use day timeunits for window to stop it removing too much data.
 * Add data util function to add number of days to 360Day Datetime type
 
+
 0.1.1-beta (2023-04-07)
 -------------------------
 * add parameter for Kerr et al. 2020
 * Add Ceppi et al jet speed adaptation from Screen et al. 2022
 * Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
 * Supress warning for quadratic func
```

### Comparing `jsmetrics-0.1.2a0/LICENSE` & `jsmetrics-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/PKG-INFO` & `jsmetrics-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.2a0
+Version: 0.1.3
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -27,14 +27,15 @@
 
 ============================================
 jsmetrics: Jet-stream metrics and algorithms
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
+**preprint now available here: https://egusphere.copernicus.org/preprints/2023/egusphere-2023-661/**   
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
@@ -246,25 +247,35 @@
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+0.1.3 (2023-07-07)
+-------------------------
+* Add "method='nearest'" to jet statistics and core algorithms for cases when coords cannot be represented within float precision range.
+
+0.1.2 (2023-06-06)
+-------------------------
+* Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data 
+* Add check for NoLeapDatetime
+
 
 0.1.2-alpha (2023-05-27)
 -------------------------
 * Add check for NoLeapDatetime
 
 
 0.1.1 (2023-05-26)
 -------------------------
 * Fix Woollings et al. 2010 and filter windows to use day timeunits for window to stop it removing too much data.
 * Add data util function to add number of days to 360Day Datetime type
 
+
 0.1.1-beta (2023-04-07)
 -------------------------
 * add parameter for Kerr et al. 2020
 * Add Ceppi et al jet speed adaptation from Screen et al. 2022
 * Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
 * Supress warning for quadratic func
```

### Comparing `jsmetrics-0.1.2a0/README.rst` & `jsmetrics-0.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ============================================
 jsmetrics: Jet-stream metrics and algorithms
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
+**preprint now available here: https://egusphere.copernicus.org/preprints/2023/egusphere-2023-661/**   
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
```

### Comparing `jsmetrics-0.1.2a0/docs/Makefile` & `jsmetrics-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png` & `jsmetrics-0.1.3/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png` & `jsmetrics-0.1.3/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png` & `jsmetrics-0.1.3/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/_static/images/jet_shift_violin.png` & `jsmetrics-0.1.3/docs/_static/images/jet_shift_violin.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/conf.py` & `jsmetrics-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/index.rst` & `jsmetrics-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/installation.rst` & `jsmetrics-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/make.bat` & `jsmetrics-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/docs/metrics.rst` & `jsmetrics-0.1.3/docs/metrics.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/core/check_data.py` & `jsmetrics-0.1.3/jsmetrics/core/check_data.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/details_for_all_metrics.py` & `jsmetrics-0.1.3/jsmetrics/details_for_all_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms.py` & `jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_core_algorithms_components.py` & `jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,19 @@
         raise TypeError("array of pressure level needs to be list or numpy.array")
 
     sum_weighted_ws = 0
     for plev, (i, plev_hPa) in zip(data["plev"], enumerate(all_plevs_hPa)):
         if i != 0:
             plev_hPa = plev_hPa - all_plevs_hPa[i - 1]
         sum_weighted_ws += (
-            (data.sel(plev=plev)["ua"] ** 2 + data.sel(plev=plev)["va"] ** 2) ** (1 / 2)
+            (
+                data.sel(plev=plev, method="nearest")["ua"] ** 2
+                + data.sel(plev=plev, method="nearest")["va"] ** 2
+            )
+            ** (1 / 2)
         ) * plev_hPa
     return sum_weighted_ws
 
 
 def get_weighted_average_ws(sum_weighted_ws, all_plevs_hPa):
     """
     Calculates weighted average wind-speed:
@@ -136,15 +140,15 @@
     """
     row["jet_maxima"] = (
         ("plev", "lat", "lon"),
         np.zeros((row["plev"].size, row["lat"].size, row["lon"].size)),
     )
     for lon in row["lon"]:
         for plev in row["plev"]:
-            current = row.sel(lon=lon, plev=plev)
+            current = row.sel(lon=lon, plev=plev, method="nearest")
             current = current.where((abs(current["ws"]) >= 30) & (current["ua"] > 0))
             local_maxima_lat_inds = data_utils.get_local_maxima(current["ws"].data)[0]
             if len(local_maxima_lat_inds) > 0:
                 for lat_ind in local_maxima_lat_inds:
                     row["jet_maxima"].loc[
                         dict(
                             lat=current["lat"].data[lat_ind],
@@ -176,15 +180,15 @@
         Data for one time unit containing jet-cores (ID number relates to each unique core)
     """
     row["jet_core_id"] = (
         ("plev", "lat", "lon"),
         np.zeros((row["plev"].size, row["lat"].size, row["lon"].size)),
     )
     for lon in row["lon"]:
-        current = row.sel(lon=lon)
+        current = row.sel(lon=lon, method="nearest")
         core_alg = JetStreamCoreIdentificationAlgorithm(
             current,
             ws_core_threshold=ws_core_threshold,
             ws_boundary_threshold=ws_boundary_threshold,
         )
         core_alg.run()
         row["jet_core_id"].loc[dict(lon=lon)] = core_alg.output_data["core_id"]
@@ -490,15 +494,15 @@
         Data of a single time unit containing 0 or 1 value (local wind maxima) for that time unit
     """
     if "local_wind_maxima" not in row.data_vars:
         raise ValueError("local_wind_maxima needs to be defined.")
 
     row = row.transpose("plev", "lat", ...)
     for lon in row["lon"]:
-        current = row.sel(lon=lon)
+        current = row.sel(lon=lon, method="nearest")
         pot_local_maximas = get_potential_local_wind_maximas_by_ws_threshold(
             current["ws"], 30
         ).data
         ind_local_wind_maximas = data_utils.get_local_maxima(pot_local_maximas, axis=1)
         # Turn into 2-d numpy array
         ind_local_wind_maximas = np.array(
             [
@@ -712,15 +716,17 @@
                 self._lats_for_search.append(lat)
 
     def _calc_jet_centre_points(self):
         """
         Will return a list of the coordinates for all jet-centre points
         """
         for coord in self._all_coords_arr:
-            coord_ws = float(self.output_data.sel(lat=coord[0], lon=coord[1])["ws"])
+            coord_ws = float(
+                self.output_data.sel(lat=coord[0], lon=coord[1], method="nearest")["ws"]
+            )
             lat_grid_vals = np.arange(
                 coord[0] - self._lat_resolution,
                 coord[0] + self._lat_resolution + 0.01,
                 self._lat_resolution,
             )
             lat_grid_vals = lat_grid_vals[
                 (lat_grid_vals >= float(self.output_data["lat"].min()))
@@ -737,17 +743,17 @@
             ).T.reshape(-1, 2)
             add_coord = True
             for val_to_check in matrix_vals_to_check:
                 if val_to_check[-1] not in self.output_data["lon"]:
                     continue
                 if (
                     float(
-                        self.output_data.sel(lat=val_to_check[0], lon=val_to_check[1])[
-                            "ws"
-                        ]
+                        self.output_data.sel(
+                            lat=val_to_check[0], lon=val_to_check[1], method="nearest"
+                        )["ws"]
                     )
                     > coord_ws
                 ):
                     add_coord = False
                     break
             if add_coord:
                 self._jet_centres.append(coord)
```

### Comparing `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics.py` & `jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,16 +210,27 @@
                 scaled_ws,
             ) = jet_statistics_components.get_latitude_and_speed_where_max_ws_at_reduced_resolution(
                 max_lat_and_ws, lat_resolution=0.01
             )
             scaled_max_lats.append(scaled_max_lat)
             scaled_max_ws.append(scaled_ws)
         else:
-            scaled_max_lats.append(np.nan)
-            scaled_max_ws.append(np.nan)
+            if np.isnan(max_lat_and_ws).all():
+                scaled_max_lats.append(np.nan)
+                scaled_max_ws.append(np.nan)
+            else:
+                if np.nanmax(max_lat_and_ws[0]) == data["lat"].max():
+                    scaled_max_lats.append(np.nanmax(max_lat_and_ws[0]))
+                    scaled_max_ws.append(np.nanmax(max_lat_and_ws[1]))
+                elif np.nanmin(max_lat_and_ws[0]) == data["lat"].min():
+                    scaled_max_lats.append(np.nanmin(max_lat_and_ws[0]))
+                    scaled_max_ws.append(np.nanmin(max_lat_and_ws[1]))
+                else:
+                    scaled_max_lats.append(np.nan)
+                    scaled_max_ws.append(np.nan)
 
     #  Step 6. Get jet-widths using scaled windspeed and usual jet-lat
     max_lats = all_max_lats_and_ws[::, 0, 1]
     jet_widths = list(
         map(
             lambda zm, la, wa: jet_statistics_components.calc_jet_width_for_one_day(
                 zm, la, wa
```

### Comparing `jsmetrics-0.1.2a0/jsmetrics/metrics/jet_statistics_components.py` & `jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     assert "lat" in data.coords, "'lat' needs to be in data.coords"
 
     sub_data = data.sel(lat=slice(lat_min, lat_max))
 
     sum_weighted_lat_flux = None
     sum_weighted_ws_by_lat = None
     for lat in sub_data["lat"].data:
-        lat_data = sub_data.sel(lat=lat)
+        lat_data = sub_data.sel(lat=lat, method="nearest")
         lat_sum_weighted_ws = get_mass_weighted_average_wind(lat_data, ws_col)
         if sum_weighted_lat_flux is None:
             sum_weighted_ws_by_lat = lat_sum_weighted_ws
             sum_weighted_lat_flux = lat_sum_weighted_ws * lat
         else:
             sum_weighted_ws_by_lat += lat_sum_weighted_ws
             sum_weighted_lat_flux += lat_sum_weighted_ws * lat
@@ -1193,15 +1193,15 @@
     Parameters
     ----------
     data_row : xarray.DataArray
         Data row to extract variable from using given latitude
     lat_val : float or int
         latitude value to extract from data row
     """
-    return float(data_row.sel(lat=lat_val))
+    return float(data_row.sel(lat=lat_val, method="nearest"))
 
 
 def get_moving_averaged_smoothed_jet_lats_for_one_day(data_row, width_of_pulse=10):
     """
     Get moving average of smoothed_jet_lats for one day. Used in combination with a groupby mapping.
 
     Component of method from Kerr et al. (2020) https://onlinelibrary.wiley.com/doi/10.1029/2020JD032735
```

### Comparing `jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics.py` & `jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/metrics/waviness_metrics_components.py` & `jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/utils/data_utils.py` & `jsmetrics-0.1.3/jsmetrics/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/utils/spatial_utils.py` & `jsmetrics-0.1.3/jsmetrics/utils/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics/utils/windspeed_utils.py` & `jsmetrics-0.1.3/jsmetrics/utils/windspeed_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/jsmetrics.egg-info/PKG-INFO` & `jsmetrics-0.1.3/jsmetrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.2a0
+Version: 0.1.3
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -27,14 +27,15 @@
 
 ============================================
 jsmetrics: Jet-stream metrics and algorithms
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
+**preprint now available here: https://egusphere.copernicus.org/preprints/2023/egusphere-2023-661/**   
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
@@ -246,25 +247,35 @@
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+0.1.3 (2023-07-07)
+-------------------------
+* Add "method='nearest'" to jet statistics and core algorithms for cases when coords cannot be represented within float precision range.
+
+0.1.2 (2023-06-06)
+-------------------------
+* Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data 
+* Add check for NoLeapDatetime
+
 
 0.1.2-alpha (2023-05-27)
 -------------------------
 * Add check for NoLeapDatetime
 
 
 0.1.1 (2023-05-26)
 -------------------------
 * Fix Woollings et al. 2010 and filter windows to use day timeunits for window to stop it removing too much data.
 * Add data util function to add number of days to 360Day Datetime type
 
+
 0.1.1-beta (2023-04-07)
 -------------------------
 * add parameter for Kerr et al. 2020
 * Add Ceppi et al jet speed adaptation from Screen et al. 2022
 * Add fix for sort_xarray_data_coords so it works when only one coord value in coordinate (i.e. so each metric can work when only one longitude)
 * Supress warning for quadratic func
```

### Comparing `jsmetrics-0.1.2a0/jsmetrics.egg-info/SOURCES.txt` & `jsmetrics-0.1.3/jsmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/setup.cfg` & `jsmetrics-0.1.3/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.2-alpha
+current_version = 0.1.3
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `jsmetrics-0.1.2a0/setup.py` & `jsmetrics-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = "jsmetrics"
 DESCRIPTION = "Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray."
 URL = "https://github.com/Thomasjkeel/jsmetrics"
 AUTHOR = "Thomas Keel"
 AUTHOR_EMAIL = "thomas.keel.18@ucl.ac.uk"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.2-alpha"
+VERSION = "0.1.3"
 LICENSE = "MIT License"
 
 KEYWORDS = "jet-stream climate metrics algorithms xarray"
 
 with open("README.rst") as file:
     readme = file.read()
```

### Comparing `jsmetrics-0.1.2a0/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.3/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.3/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.3/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/metric_verification/metric_verification.ipynb` & `jsmetrics-0.1.3/tests/metric_verification/metric_verification.ipynb`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/__init__.py` & `jsmetrics-0.1.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/test_data_utils.py` & `jsmetrics-0.1.3/tests/unit/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/test_jet_algorithms.py` & `jsmetrics-0.1.3/tests/unit/test_jet_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/test_jet_statistics.py` & `jsmetrics-0.1.3/tests/unit/test_jet_statistics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/test_spatial_utils.py` & `jsmetrics-0.1.3/tests/unit/test_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/test_waviness_metrics.py` & `jsmetrics-0.1.3/tests/unit/test_waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.2a0/tests/unit/test_windspeed_utils.py` & `jsmetrics-0.1.3/tests/unit/test_windspeed_utils.py`

 * *Files identical despite different names*


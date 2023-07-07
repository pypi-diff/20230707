# Comparing `tmp/astrohack-0.1.6.tar.gz` & `tmp/astrohack-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.6.tar", last modified: Fri Jun 16 20:11:22 2023, max compression
+gzip compressed data, was "astrohack-0.1.7.tar", last modified: Fri Jul  7 19:34:11 2023, max compression
```

## Comparing `astrohack-0.1.6.tar` & `astrohack-0.1.7.tar`

### file list

```diff
@@ -1,101 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 20:11:06.000000 astrohack-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:11:06.000000 astrohack-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 20:11:22.558641 astrohack-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-16 20:11:06.000000 astrohack-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:06.000000 astrohack-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 20:11:06.000000 astrohack-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:11:22.558641 astrohack-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.546640 astrohack-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.550640 astrohack-0.1.6/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.550640 astrohack-0.1.6/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_graph_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22857 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22945 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_imaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    42607 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_mds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_panel_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_phase_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/_utils/_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/combine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.546640 astrohack-0.1.6/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.554641 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    33129 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-16 20:11:06.000000 astrohack-0.1.6/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.550640 astrohack-0.1.6/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 20:11:22.000000 astrohack-0.1.6/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:22.558641 astrohack-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_class_telescope.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-06-16 20:11:06.000000 astrohack-0.1.6/tests/test_stakeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 19:33:55.000000 astrohack-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:33:55.000000 astrohack-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 19:34:11.470522 astrohack-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-07 19:33:55.000000 astrohack-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:33:55.000000 astrohack-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 19:33:55.000000 astrohack-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:34:11.470522 astrohack-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.462522 astrohack-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.462522 astrohack-0.1.7/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19864 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22554 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_imaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    36145 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_panel_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27855 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_phase_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/_utils/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.462522 astrohack-0.1.7/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33264 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/mds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.470522 astrohack-0.1.7/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-07 19:33:55.000000 astrohack-0.1.7/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:34:11.466522 astrohack-0.1.7/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 19:34:11.000000 astrohack-0.1.7/src/astrohack.egg-info/top_level.txt
```

### Comparing `astrohack-0.1.6/LICENSE` & `astrohack-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/PKG-INFO` & `astrohack-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.6
+Version: 0.1.7
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 ![astrohack](docs/_media/astrohack_logo.png)
 
-[![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.8 3.9 3.10 3.11](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads/release/python-380/)
 ![Linux Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-linux.yml/badge.svg)
 ![macOS Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-macos.yml/badge.svg)
 ![Published](https://github.com/casangi/astrohack/actions/workflows/pythonpublish.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
-
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
 
 # Installing
 It is recommended to use the [conda](https://docs.conda.io/projects/conda/en/latest/) environment manager to create a clean, self-contained runtime where astrohack and all its dependencies can be installed:
 ```sh
-conda create --name astrohack python=3.8 --no-default-packages
+conda create --name astrohack python=3.11 --no-default-packages
 conda activate astrohack
 
 ```
 > 📝 On macOS it is required to pre-install `python-casacore` using `conda install -c conda-forge python-casacore`.
 
 Making astroHACK available for download from conda-forge directly is pending, so until then the current recommendation is to sully that pristine environment by calling pip [from within conda](https://www.anaconda.com/blog/using-pip-in-a-conda-environment), like this:
 ```sh
```

### Comparing `astrohack-0.1.6/README.md` & `astrohack-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ![astrohack](docs/_media/astrohack_logo.png)
 
-[![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.8 3.9 3.10 3.11](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads/release/python-380/)
 ![Linux Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-linux.yml/badge.svg)
 ![macOS Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-macos.yml/badge.svg)
 ![Published](https://github.com/casangi/astrohack/actions/workflows/pythonpublish.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
-
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
 
 # Installing
 It is recommended to use the [conda](https://docs.conda.io/projects/conda/en/latest/) environment manager to create a clean, self-contained runtime where astrohack and all its dependencies can be installed:
 ```sh
-conda create --name astrohack python=3.8 --no-default-packages
+conda create --name astrohack python=3.11 --no-default-packages
 conda activate astrohack
 
 ```
 > 📝 On macOS it is required to pre-install `python-casacore` using `conda install -c conda-forge python-casacore`.
 
 Making astroHACK available for download from conda-forge directly is pending, so until then the current recommendation is to sully that pristine environment by calling pip [from within conda](https://www.anaconda.com/blog/using-pip-in-a-conda-environment), like this:
 ```sh
```

### Comparing `astrohack-0.1.6/pyproject.toml` & `astrohack-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 [project]
 name = "astrohack"
-version = "0.1.6"
+version = "0.1.7"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
-requires-python = ">= 3.8, < 3.11"
+requires-python = ">= 3.8, < 3.12"
 
 dependencies = [
-'astropy==5.2.1',
-'click==8.1.3',
-'dask==2023.3.2',
-'dask_jobqueue==0.8.1',
-'distributed==2023.3.2',
-'gdown==4.7.1',
-'matplotlib==3.7.1',
-'memory_profiler==0.61.0',
-'numba==0.56.3',
-'numpy==1.22.4',
-'param==1.13.0',
-'plotly==5.14.0',
-'prettytable==3.6.0',
-'psutil==5.9.4',
-'pytest==7.2.2',
-'scikit_image==0.19.3',
-'scipy==1.7.3',
-'setuptools==65.6.3',
-'Shapely==2.0.1',
-'xarray==2022.12.0',
-'zarr==2.13.3',
-'bokeh==2.4.3',
+'astropy',
+'dask',
+'distributed',
+'gdown',
+'matplotlib',
+'memory_profiler',
+'numba>=0.57.0',
+'numpy',
+'prettytable',
+'pytest',
+'scikit_image',
+'scipy',
+'xarray',
+'zarr',
+'bokeh',
 'jupyterlab',
-'python_casacore==3.5.2; sys_platform != "darwin" '
+'python_casacore>=3.5.2; sys_platform != "darwin" '
 ]
 
 
 [project.optional-dependencies]
 docs = [
     'ipykernel',
     'ipympl',
```

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.7/src/astrohack/_utils/_algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     n_time, n_chan, n_pol = data_avg_shape
 
     n_avg_chan = avg_freq.shape[0]
     
     # Update new chan dim.
     data_avg_shape[1] = n_avg_chan  
 
-    data_avg = np.zeros(data_avg_shape, dtype=np.complex)
-    weight_sum = np.zeros(data_avg_shape, dtype=np.float)
+    data_avg = np.zeros(data_avg_shape, dtype=np.complex128)
+    weight_sum = np.zeros(data_avg_shape, dtype=np.float64)
 
     index = 0
 
     for avg_index in avg_chan_index:
 
         while (index < n_chan) and (avg_map[index] == avg_index):
 
@@ -209,24 +209,34 @@
     return results, variances
     
     
 def _get_grid_parms(vis_map_dict,pnt_map_dict, ant_names):
     
     grid_parms = {}
     for ant_index in vis_map_dict.keys():
-        diff = np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'],axis=0)
-        r_diff = np.sqrt(np.abs(diff[:,0]**2 + diff[:,1]**2))
-
-        max_dis = np.max(r_diff)/100
-        n_pix = np.sum([r_diff > max_dis]) + 1
-        cell_size = np.mean(r_diff[r_diff > max_dis])
+        abs_diff = np.abs(np.diff(pnt_map_dict['ant_'+ant_names[ant_index]]['POINTING_OFFSET'],axis=0))
+        
+        max_dis_x = np.max(abs_diff[:,0])/100
+        max_dis_y = np.max(abs_diff[:,1])/100
+        
+        n_pix_x = np.sum([abs_diff[:,0] > max_dis_x]) + 1
+        n_pix_y = np.sum([abs_diff[:,1] > max_dis_y]) + 1
+        
+        cell_size_x = np.mean(abs_diff[abs_diff[:,0] > max_dis_x,0])
+        cell_size_y = np.mean(abs_diff[abs_diff[:,1] > max_dis_y,1])
+        
+        if n_pix_x < n_pix_y:
+            n_pix = n_pix_x**2
+            cell_size = cell_size_x
+        else:
+            n_pix = n_pix_y**2
+            cell_size = cell_size_y
         
         grid_parms['ant_'+ant_names[ant_index]] = {'n_pix':n_pix,'cell_size':cell_size}
 
-
     return grid_parms
 
 def _significant_digits(x, digits):
     if np.isscalar(x):
         return _significant_digits_scalar(x,digits)
     else:
         return list(map(_significant_digits,x,[digits]*len(x)))
```

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_combine.py` & `astrohack-0.1.7/src/astrohack/_utils/_combine.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_constants.py` & `astrohack-0.1.7/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.7/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_dask_graph_tools.py` & `astrohack-0.1.7/src/astrohack/_utils/_dask_graph_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_diagnostics.py` & `astrohack-0.1.7/src/astrohack/_utils/_diagnostics.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_dio.py` & `astrohack-0.1.7/src/astrohack/_utils/_dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.7/src/astrohack/_utils/_extract_holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,20 +360,14 @@
             xds.attrs["m_max"] = np.max(xds["DIRECTIONAL_COSINES"][:,1].values)
             xds.attrs["m_min"] = np.min(xds["DIRECTIONAL_COSINES"][:,1].values)
             
             xds.attrs["grid_parms"] = grid_parms[map_ant_tag]
             
             holog_file = holog_name
 
-            if overwrite is False:
-                if os.path.exists(holog_file):
-                    logger.error(
-                        "Holog file {file} exists. To overwite set the overwrite=True option in extract_holog or remove current file.".format(file=holog_file))
-                    raise
-
             logger.info(
                 "Writing holog file to {file}".format(file=holog_file)
             )
             xds.to_zarr(
                 os.path.join(
                     holog_file, 'ddi_' + str(ddi) + "/" + str(holog_map_key) + "/" + "ant_" + str(ant_names[map_ant_index])
                 ),
```

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.7/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_gaussfitter.py` & `astrohack-0.1.7/src/astrohack/_utils/_gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_holog.py` & `astrohack-0.1.7/src/astrohack/_utils/_holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,18 +68,18 @@
     
     if holog_chunk_params["chan_average"]:
         reference_scaling_frequency = np.mean(freq_chan)
 
         avg_chan_map, avg_freq = _create_average_chan_map(freq_chan, holog_chunk_params["chan_tolerance_factor"])
         
         # Only a single channel left after averaging.
-        beam_grid = np.zeros((n_holog_map,) + (1, n_pol) + grid_l.shape, dtype=np.complex)
+        beam_grid = np.zeros((n_holog_map,) + (1, n_pol) + grid_l.shape, dtype=np.complex128)
 
     else:
-        beam_grid = np.zeros((n_holog_map,) + (n_chan, n_pol) + grid_l.shape, dtype=np.complex)
+        beam_grid = np.zeros((n_holog_map,) + (n_chan, n_pol) + grid_l.shape, dtype=np.complex128)
 
     time_centroid = []
 
     for holog_map_index, holog_map in enumerate(ant_data_dict[ddi].keys()):
         ant_xds = ant_data_dict[ddi][holog_map]
         
         ###To Do: Add flagging code
```

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.7/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.7/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_mds.py` & `astrohack-0.1.7/src/astrohack/mds.py`

 * *Files 0% similar despite different names*

```diff
@@ -871,8 +871,7 @@
     def summary(self):
         """ Prints summary of the AstrohackPointFile object, with available data, attributes and available methods
         """
         _print_summary_header(self.file)
         _print_attributes(self._meta_data)
         _print_data_contents(self, ["Antenna"])
         _print_method_list([self.summary])
-
```

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_panel.py` & `astrohack-0.1.7/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/antenna_surface.py` & `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/base_panel.py` & `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/polygon_panel.py` & `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/ring_panel.py` & `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_panel_classes/telescope.py` & `astrohack-0.1.7/src/astrohack/_utils/_panel_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.7/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_phase_fitting.py` & `astrohack-0.1.7/src/astrohack/_utils/_phase_fitting.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/_utils/_tools.py` & `astrohack-0.1.7/src/astrohack/_utils/_tools.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/astrohack_client.py` & `astrohack-0.1.7/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/combine.py` & `astrohack-0.1.7/src/astrohack/combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import numpy as np
 
 from astrohack._utils._combine import _combine_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._dio import check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
-from astrohack._utils._mds import AstrohackImageFile
+from astrohack.mds import AstrohackImageFile
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 
 
-def combine(image_name, combine_name=None, ant_id=None, ddi=None, weighted=False, parallel=False,
-            overwrite=False):
+def combine(image_name, combine_name=None, ant_id=None, ddi=None, weighted=False, parallel=False, overwrite=False):
     """Combine DDIs in a Holography image to increase SNR
 
     :param image_name: Input holography data file name. Accepted data format is the output from ``astrohack.holog.holog``
     :type image_name: str
     :param combine_name: Name of output file; File name will be appended with suffix *.combine.zarr*. Defaults to *basename* of input file plus holography panel file suffix.
     :type combine_name: str, optional
     :param ant_id: List of Antennae to be processed. None will use all antennae. Defaults to None, ex. ea25.
@@ -46,16 +45,15 @@
             },
             ⋮
             ant_n: …
         }
     """
     logger = _get_astrohack_logger()
     fname = 'combine'
-    combine_params = _check_combine_parms(fname, image_name, combine_name, ant_id, ddi, weighted, parallel,
-                                          overwrite)
+    combine_params = _check_combine_parms(fname, image_name, combine_name, ant_id, ddi, weighted, parallel, overwrite)
     input_params = combine_params.copy()
 
     check_if_file_exists(fname, combine_params['image_file'])
     check_if_file_will_be_overwritten(fname, combine_params['combine_file'], combine_params['overwrite'])
 
     image_mds = AstrohackImageFile(combine_params['image_file'])
     image_mds._open()
```

### Comparing `astrohack-0.1.6/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json` & `astrohack-0.1.7/src/astrohack/data/.file_meta_data/J1924-2914.ms.calibrated.split.SPW3.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json` & `astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json` & `astrohack-0.1.7/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed_split.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/dio.py` & `astrohack-0.1.7/src/astrohack/dio.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import json
 import numpy as np
 
 from casacore import tables
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
-from astrohack._utils._mds import AstrohackImageFile
-from astrohack._utils._mds import AstrohackHologFile
-from astrohack._utils._mds import AstrohackPanelFile
-from astrohack._utils._mds import AstrohackPointFile
+from astrohack.mds import AstrohackImageFile
+from astrohack.mds import AstrohackHologFile
+from astrohack.mds import AstrohackPanelFile
+from astrohack.mds import AstrohackPointFile
 
 from astrohack._utils._dio import _reshape
 from astrohack._utils._dio import _print_array
 
 
 def open_holog(file):
     """ Open holog file and return instance of the holog data object. Object includes summary function to list available dictionary keys.
```

### Comparing `astrohack-0.1.6/src/astrohack/extract_holog.py` & `astrohack-0.1.7/src/astrohack/extract_holog.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from astrohack._utils._dio import  check_if_file_will_be_overwritten, check_if_file_exists
 from astrohack._utils._dio import _load_holog_file
 from astrohack._utils._extract_holog import _extract_holog_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._tools import _jsonify
-from astrohack._utils._mds import AstrohackHologFile
 
+from astrohack.mds import AstrohackHologFile
 
 def extract_holog(
     ms_name,
     holog_obs_dict=None,
     ddi=None,
     baseline_average_distance=None,
     baseline_average_nearest=None,
@@ -143,28 +143,32 @@
                                                      parallel,
                                                      reuse_point_zarr,
                                                      overwrite)
     input_params = extract_holog_parms.copy()
     
     check_if_file_exists(fname, extract_holog_parms['ms_name'])
     check_if_file_will_be_overwritten(fname, extract_holog_parms['holog_name'], extract_holog_parms['overwrite'])
-    check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], extract_holog_parms['overwrite'])
+    
         
-    ############# Exstract pointing infromation and save to point.zarr #############
+    ############# Extract pointing infromation and save to point.zarr #############
     if extract_holog_parms["reuse_point_zarr"]:
         try:
             pnt_dict = _load_point_file(extract_holog_parms['point_name'])
         except:
-            logger.warning(f'[{fname}]: Could not find {extract_holog_parms["point_name"]}, creating point new '
-                           f'point.zarr.')
-            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
-                                         parallel=extract_holog_parms['parallel'])
+            logger.warning(f'[{fname}]: Could not find {extract_holog_parms["point_name"]}, creating point new 'f'point.zarr.')
+
+            # If you tried to reuse .pointing and there was a failure, delete old file and recreate
+            check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], True)
+            pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
     else:
-        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'],
-                                     parallel=extract_holog_parms['parallel'])
+
+        # If you don't want to reuse .point delete and recreate
+        check_if_file_will_be_overwritten(fname, extract_holog_parms['point_name'], True)
+        pnt_dict = _extract_pointing(extract_holog_parms['ms_name'], extract_holog_parms['point_name'], parallel=extract_holog_parms['parallel'])
+        
 
     ######## Get Spectral Windows ########
     ctb = ctables.table(
         os.path.join(extract_holog_parms['ms_name'], "DATA_DESCRIPTION"),
         readonly=True,
         lockoptions={"option": "usernoread"},
         ack=False,
```

### Comparing `astrohack-0.1.6/src/astrohack/holog.py` & `astrohack-0.1.7/src/astrohack/holog.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numbers
 
 from astrohack._utils._holog import _holog_chunk, _create_image_meta_data
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._dio import check_if_file_will_be_overwritten, check_if_file_exists, _read_meta_data
-from astrohack._utils._mds import AstrohackImageFile
+from astrohack.mds import AstrohackImageFile
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 
 
 def holog(holog_name, grid_size=None, cell_size=None, image_name=None, padding_factor=50,
           grid_interpolation_mode="linear", chan_average=True, chan_tolerance_factor=0.005, scan_average=True,
           ant_id=None, ddi=None, to_stokes=True, apply_mask=True, phase_fit=True, overwrite=False, parallel=False):
     """ Process holography data and derive aperture illumination pattern.
```

### Comparing `astrohack-0.1.6/src/astrohack/panel.py` & `astrohack-0.1.7/src/astrohack/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from astrohack._utils._dio import _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists, _write_meta_data
 from astrohack._utils._panel import _panel_chunk
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms, _parm_check_passed
 from astrohack._utils._tools import _remove_suffix
 from astrohack._utils._dask_graph_tools import _dask_general_compute
 
-from astrohack._utils._mds import AstrohackPanelFile, AstrohackImageFile
+from astrohack.mds import AstrohackPanelFile, AstrohackImageFile
 
 
 def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, ant_id=None, ddi=None,
           parallel=False, overwrite=False):
     """Analyze holography images to derive panel adjustments
 
     :param image_name: Input holography data file name. Accepted data formats are the output from ``astrohack.holog.holog`` and AIPS holography data prepackaged using ``astrohack.panel.aips_holog_to_astrohack``.
```

### Comparing `astrohack-0.1.6/src/astrohack/profiling.py` & `astrohack-0.1.7/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack/visualization/viewer.py` & `astrohack-0.1.7/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.6/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.7/src/astrohack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.6
+Version: 0.1.7
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 ![astrohack](docs/_media/astrohack_logo.png)
 
-[![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.8 3.9 3.10 3.11](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads/release/python-380/)
 ![Linux Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-linux.yml/badge.svg)
 ![macOS Tests](https://github.com/casangi/astrohack/actions/workflows/python-testing-macos.yml/badge.svg)
 ![Published](https://github.com/casangi/astrohack/actions/workflows/pythonpublish.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
 
-
 astroHack (Holography Antenna Commissioning Kit) is a Python package that produces antenna aperture images and panel adjustment corrections from calibrated holography measurement sets. Initially, it will support holography data from the VLA and ALMA, with the future goal of supporting the ngVLA. Much of the core functionality from the following AIPS tasks has been ported: UVHOL, HOLOG, and PANEL. astroHack enables parallel execution by using Dask and efficient single-threaded performance by making use of Numba.
 
 > 📝 astroHACK is under active development! Breaking API changes are still happening on a regular basis, so proceed with caution.
 
 # Installing
 It is recommended to use the [conda](https://docs.conda.io/projects/conda/en/latest/) environment manager to create a clean, self-contained runtime where astrohack and all its dependencies can be installed:
 ```sh
-conda create --name astrohack python=3.8 --no-default-packages
+conda create --name astrohack python=3.11 --no-default-packages
 conda activate astrohack
 
 ```
 > 📝 On macOS it is required to pre-install `python-casacore` using `conda install -c conda-forge python-casacore`.
 
 Making astroHACK available for download from conda-forge directly is pending, so until then the current recommendation is to sully that pristine environment by calling pip [from within conda](https://www.anaconda.com/blog/using-pip-in-a-conda-environment), like this:
 ```sh
```

### Comparing `astrohack-0.1.6/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.7/src/astrohack.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/astrohack/astrohack_client.py
 src/astrohack/combine.py
 src/astrohack/dio.py
 src/astrohack/extract_holog.py
 src/astrohack/gdown_utils.py
 src/astrohack/holog.py
 src/astrohack/locit.py
+src/astrohack/mds.py
 src/astrohack/panel.py
 src/astrohack/profiling.py
 src/astrohack.egg-info/PKG-INFO
 src/astrohack.egg-info/SOURCES.txt
 src/astrohack.egg-info/dependency_links.txt
 src/astrohack.egg-info/requires.txt
 src/astrohack.egg-info/top_level.txt
@@ -27,15 +28,14 @@
 src/astrohack/_utils/_diagnostics.py
 src/astrohack/_utils/_dio.py
 src/astrohack/_utils/_extract_holog.py
 src/astrohack/_utils/_extract_point.py
 src/astrohack/_utils/_gaussfitter.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
-src/astrohack/_utils/_mds.py
 src/astrohack/_utils/_panel.py
 src/astrohack/_utils/_phase_fitting.py
 src/astrohack/_utils/_tools.py
 src/astrohack/_utils/_dask_plugins/__init__.py
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
@@ -67,13 +67,8 @@
 src/astrohack/data/telescopes/vla.zarr/.zattrs
 src/astrohack/data/telescopes/vla.zarr/.zgroup
 src/astrohack/data/telescopes/vla.zarr/.zmetadata
 src/astrohack/data/telescopes/vlba.zarr/.zattrs
 src/astrohack/data/telescopes/vlba.zarr/.zgroup
 src/astrohack/data/telescopes/vlba.zarr/.zmetadata
 src/astrohack/visualization/__init__.py
-src/astrohack/visualization/viewer.py
-tests/test_class_antenna_surface.py
-tests/test_class_base_panel.py
-tests/test_class_ring_panel.py
-tests/test_class_telescope.py
-tests/test_stakeholder.py
+src/astrohack/visualization/viewer.py
```


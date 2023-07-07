# Comparing `tmp/wrainfo-0.9.3.tar.gz` & `tmp/wrainfo-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrainfo-0.9.3.tar", last modified: Tue Jan 10 15:38:03 2023, max compression
+gzip compressed data, was "wrainfo-0.9.5.tar", last modified: Fri Jul  7 07:25:16 2023, max compression
```

## Comparing `wrainfo-0.9.3.tar` & `wrainfo-0.9.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.170637 wrainfo-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)      436 2022-12-06 14:53:03.000000 wrainfo-0.9.3/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     4527 2022-08-05 12:37:14.000000 wrainfo-0.9.3/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)     5817 2023-01-10 10:26:31.000000 wrainfo-0.9.3/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)    11332 2022-09-28 17:04:24.000000 wrainfo-0.9.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-08-05 12:37:14.000000 wrainfo-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9137 2023-01-10 15:38:03.170637 wrainfo-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7857 2023-01-10 11:04:18.000000 wrainfo-0.9.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.158637 wrainfo-0.9.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      608 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.158637 wrainfo-0.9.3/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.158637 wrainfo-0.9.3/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.158637 wrainfo-0.9.3/docs/_build/html/_images/
--rw-r--r--   0 root         (0) root         (0)    21687 2022-09-28 17:04:24.000000 wrainfo-0.9.3/docs/_build/html/_images/fernlab_logo.png
--rw-r--r--   0 root         (0) root         (0)   118413 2023-01-10 15:36:05.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_12_0.png
--rw-r--r--   0 root         (0) root         (0)    93973 2023-01-10 15:36:05.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_18_0.png
--rw-r--r--   0 root         (0) root         (0)    46981 2023-01-10 15:36:06.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_18_0.png
--rw-r--r--   0 root         (0) root         (0)   176535 2023-01-10 15:36:06.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_24_0.png
--rw-r--r--   0 root         (0) root         (0)    55590 2023-01-10 15:36:06.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_27_0.png
--rw-r--r--   0 root         (0) root         (0)    29055 2023-01-10 15:36:06.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_6_1.png
--rw-r--r--   0 root         (0) root         (0)   124737 2023-01-10 15:36:07.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_geometry_module_13_1.png
--rw-r--r--   0 root         (0) root         (0)    47775 2023-01-10 15:36:08.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_precipitation_estimation_7_1.png
--rw-r--r--   0 root         (0) root         (0)    70372 2023-01-10 15:36:09.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_31_1.png
--rw-r--r--   0 root         (0) root         (0)    50260 2023-01-10 15:36:09.000000 wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_34_1.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.162637 wrainfo-0.9.3/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)      286 2023-01-10 15:35:36.000000 wrainfo-0.9.3/docs/_build/html/_static/file.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-10 15:35:36.000000 wrainfo-0.9.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-01-10 15:35:36.000000 wrainfo-0.9.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)    52116 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/_build/html/_static/wrainfo_logo.png
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/authors.rst
--rwxrwxrwx   0 root         (0) root         (0)     9956 2022-08-15 14:13:55.000000 wrainfo-0.9.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.166637 wrainfo-0.9.3/docs/images/
--rwxrwxrwx   0 root         (0) root         (0)    21687 2022-09-28 17:04:24.000000 wrainfo-0.9.3/docs/images/fernlab_logo.png
--rwxrwxrwx   0 root         (0) root         (0)  1508369 2023-01-10 11:04:18.000000 wrainfo-0.9.3/docs/images/wr_furuno_comparison_of_raw_reflectivity_and_clutter_corrected_reflectivity.png
--rwxrwxrwx   0 root         (0) root         (0)  1316808 2023-01-10 11:04:18.000000 wrainfo-0.9.3/docs/images/wr_furuno_georeferenced_and_gridded_precipitation_data_with_WRaINfo.png
--rwxrwxrwx   0 root         (0) root         (0)  1645974 2023-01-10 11:04:19.000000 wrainfo-0.9.3/docs/images/wr_furuno_reflectivity_attenaution_corrected_and_estimated_precipitation.png
--rwxrwxrwx   0 root         (0) root         (0)  1408283 2023-01-10 11:04:19.000000 wrainfo-0.9.3/docs/images/wr_furuno_reflectivity_before_and_after_attenaution_correction.png
--rwxrwxrwx   0 root         (0) root         (0)    52116 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/images/wrainfo_logo.png
--rw-rw-rw-   0 root         (0) root         (0)     5390 2023-01-10 10:26:31.000000 wrainfo-0.9.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3225 2022-10-10 13:35:01.000000 wrainfo-0.9.3/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-08-05 12:37:14.000000 wrainfo-0.9.3/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.166637 wrainfo-0.9.3/docs/process_chains/
--rwxrwxrwx   0 root         (0) root         (0)      108 2022-09-19 15:57:23.000000 wrainfo-0.9.3/docs/process_chains/clutter_chain.rst
--rwxrwxrwx   0 root         (0) root         (0)      846 2022-09-20 15:14:17.000000 wrainfo-0.9.3/docs/process_chains/introduction.rst
--rwxrwxrwx   0 root         (0) root         (0)      116 2022-09-19 15:57:23.000000 wrainfo-0.9.3/docs/process_chains/static_cmap.rst
--rwxrwxrwx   0 root         (0) root         (0)      145 2022-09-19 15:57:23.000000 wrainfo-0.9.3/docs/process_chains/wr_routine_furuno_level2a.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.166637 wrainfo-0.9.3/docs/tutorials_and_examples/
--rwxrwxrwx   0 root         (0) root         (0)      149 2022-08-28 12:01:46.000000 wrainfo-0.9.3/docs/tutorials_and_examples/attenuation_correction_module.rst
--rwxrwxrwx   0 root         (0) root         (0)      263 2022-08-21 18:21:41.000000 wrainfo-0.9.3/docs/tutorials_and_examples/clutter_detection_module.rst
--rwxrwxrwx   0 root         (0) root         (0)      223 2022-08-21 18:21:41.000000 wrainfo-0.9.3/docs/tutorials_and_examples/data_input.rst
--rwxrwxrwx   0 root         (0) root         (0)     2070 2022-09-29 11:22:04.000000 wrainfo-0.9.3/docs/tutorials_and_examples/features_overview.rst
--rwxrwxrwx   0 root         (0) root         (0)      120 2022-09-16 15:52:46.000000 wrainfo-0.9.3/docs/tutorials_and_examples/further_features.rst
--rwxrwxrwx   0 root         (0) root         (0)      117 2022-09-16 14:12:18.000000 wrainfo-0.9.3/docs/tutorials_and_examples/geometry_module.rst
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-08-17 10:33:30.000000 wrainfo-0.9.3/docs/tutorials_and_examples/getting_started_with_wrainfo.rst
--rwxrwxrwx   0 root         (0) root         (0)      155 2022-08-28 08:01:37.000000 wrainfo-0.9.3/docs/tutorials_and_examples/precipitation_estimation_module.rst
--rwxrwxrwx   0 root         (0) root         (0)      111 2022-08-21 18:10:28.000000 wrainfo-0.9.3/docs/tutorials_and_examples/reader_module.rst
--rwxrwxrwx   0 root         (0) root         (0)      117 2022-08-21 17:59:15.000000 wrainfo-0.9.3/docs/tutorials_and_examples/tutorials_and_examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-01-10 15:38:03.170637 wrainfo-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3542 2023-01-10 10:26:31.000000 wrainfo-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.166637 wrainfo-0.9.3/wrainfo/
--rw-rw-rw-   0 root         (0) root         (0)     1551 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9815 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/attenuation_corr.py
--rwxrwxrwx   0 root         (0) root         (0)     6366 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/clutter.py
--rwxrwxrwx   0 root         (0) root         (0)     4269 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/compression.py
--rwxrwxrwx   0 root         (0) root         (0)     3149 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/error_flist.py
--rwxrwxrwx   0 root         (0) root         (0)     7331 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/geometry.py
--rwxrwxrwx   0 root         (0) root         (0)     2670 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/precipitation.py
--rwxrwxrwx   0 root         (0) root         (0)    13877 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/process_chains.py
--rwxrwxrwx   0 root         (0) root         (0)    11034 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1018 2023-01-10 10:26:31.000000 wrainfo-0.9.3/wrainfo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 15:38:03.170637 wrainfo-0.9.3/wrainfo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9137 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2659 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      510 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-10 15:38:03.000000 wrainfo-0.9.3/wrainfo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.151470 wrainfo-0.9.5/
+-rw-rw-rw-   0 root         (0) root         (0)      436 2022-12-06 14:53:03.000000 wrainfo-0.9.5/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2022-08-05 12:37:14.000000 wrainfo-0.9.5/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5982 2023-07-06 14:15:29.000000 wrainfo-0.9.5/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11332 2022-09-28 17:04:24.000000 wrainfo-0.9.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      262 2022-08-05 12:37:14.000000 wrainfo-0.9.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9137 2023-07-07 07:25:16.151470 wrainfo-0.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7857 2023-01-10 11:04:18.000000 wrainfo-0.9.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.143470 wrainfo-0.9.5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.139470 wrainfo-0.9.5/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.139470 wrainfo-0.9.5/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.143470 wrainfo-0.9.5/docs/_build/html/_images/
+-rw-r--r--   0 root         (0) root         (0)    21687 2022-09-28 17:04:24.000000 wrainfo-0.9.5/docs/_build/html/_images/fernlab_logo.png
+-rw-r--r--   0 root         (0) root         (0)   118413 2023-07-07 07:23:56.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_12_0.png
+-rw-r--r--   0 root         (0) root         (0)    93973 2023-07-07 07:23:56.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_18_0.png
+-rw-r--r--   0 root         (0) root         (0)    46981 2023-07-07 07:23:57.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_18_0.png
+-rw-r--r--   0 root         (0) root         (0)   176535 2023-07-07 07:23:57.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_24_0.png
+-rw-r--r--   0 root         (0) root         (0)    55590 2023-07-07 07:23:57.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_27_0.png
+-rw-r--r--   0 root         (0) root         (0)    29055 2023-07-07 07:23:57.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_6_1.png
+-rw-r--r--   0 root         (0) root         (0)   124737 2023-07-07 07:23:58.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_geometry_module_13_1.png
+-rw-r--r--   0 root         (0) root         (0)    47775 2023-07-07 07:23:59.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_precipitation_estimation_7_1.png
+-rw-r--r--   0 root         (0) root         (0)    70372 2023-07-07 07:24:00.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_31_1.png
+-rw-r--r--   0 root         (0) root         (0)    50260 2023-07-07 07:24:00.000000 wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_34_1.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.143470 wrainfo-0.9.5/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-25 11:20:36.000000 wrainfo-0.9.5/docs/_build/html/_static/file.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-25 11:20:36.000000 wrainfo-0.9.5/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-25 11:20:36.000000 wrainfo-0.9.5/docs/_build/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)    52116 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/_build/html/_static/wrainfo_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/authors.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9956 2022-08-15 14:13:55.000000 wrainfo-0.9.5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.151470 wrainfo-0.9.5/docs/images/
+-rwxrwxrwx   0 root         (0) root         (0)    21687 2022-09-28 17:04:24.000000 wrainfo-0.9.5/docs/images/fernlab_logo.png
+-rwxrwxrwx   0 root         (0) root         (0)  1508369 2023-01-10 11:04:18.000000 wrainfo-0.9.5/docs/images/wr_furuno_comparison_of_raw_reflectivity_and_clutter_corrected_reflectivity.png
+-rwxrwxrwx   0 root         (0) root         (0)  1316808 2023-01-10 11:04:18.000000 wrainfo-0.9.5/docs/images/wr_furuno_georeferenced_and_gridded_precipitation_data_with_WRaINfo.png
+-rwxrwxrwx   0 root         (0) root         (0)  1645974 2023-01-10 11:04:19.000000 wrainfo-0.9.5/docs/images/wr_furuno_reflectivity_attenaution_corrected_and_estimated_precipitation.png
+-rwxrwxrwx   0 root         (0) root         (0)  1408283 2023-01-10 11:04:19.000000 wrainfo-0.9.5/docs/images/wr_furuno_reflectivity_before_and_after_attenaution_correction.png
+-rwxrwxrwx   0 root         (0) root         (0)    52116 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/images/wrainfo_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     5390 2023-01-10 10:26:31.000000 wrainfo-0.9.5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2022-10-10 13:35:01.000000 wrainfo-0.9.5/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      805 2022-08-05 12:37:14.000000 wrainfo-0.9.5/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.151470 wrainfo-0.9.5/docs/process_chains/
+-rwxrwxrwx   0 root         (0) root         (0)      108 2022-09-19 15:57:23.000000 wrainfo-0.9.5/docs/process_chains/clutter_chain.rst
+-rwxrwxrwx   0 root         (0) root         (0)      846 2022-09-20 15:14:17.000000 wrainfo-0.9.5/docs/process_chains/introduction.rst
+-rwxrwxrwx   0 root         (0) root         (0)      116 2022-09-19 15:57:23.000000 wrainfo-0.9.5/docs/process_chains/static_cmap.rst
+-rwxrwxrwx   0 root         (0) root         (0)      145 2022-09-19 15:57:23.000000 wrainfo-0.9.5/docs/process_chains/wr_routine_furuno_level2a.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.151470 wrainfo-0.9.5/docs/tutorials_and_examples/
+-rwxrwxrwx   0 root         (0) root         (0)      149 2022-08-28 12:01:46.000000 wrainfo-0.9.5/docs/tutorials_and_examples/attenuation_correction_module.rst
+-rwxrwxrwx   0 root         (0) root         (0)      263 2022-08-21 18:21:41.000000 wrainfo-0.9.5/docs/tutorials_and_examples/clutter_detection_module.rst
+-rwxrwxrwx   0 root         (0) root         (0)      223 2022-08-21 18:21:41.000000 wrainfo-0.9.5/docs/tutorials_and_examples/data_input.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2070 2022-09-29 11:22:04.000000 wrainfo-0.9.5/docs/tutorials_and_examples/features_overview.rst
+-rwxrwxrwx   0 root         (0) root         (0)      120 2022-09-16 15:52:46.000000 wrainfo-0.9.5/docs/tutorials_and_examples/further_features.rst
+-rwxrwxrwx   0 root         (0) root         (0)      117 2022-09-16 14:12:18.000000 wrainfo-0.9.5/docs/tutorials_and_examples/geometry_module.rst
+-rw-rw-rw-   0 root         (0) root         (0)      505 2022-08-17 10:33:30.000000 wrainfo-0.9.5/docs/tutorials_and_examples/getting_started_with_wrainfo.rst
+-rwxrwxrwx   0 root         (0) root         (0)      155 2022-08-28 08:01:37.000000 wrainfo-0.9.5/docs/tutorials_and_examples/precipitation_estimation_module.rst
+-rwxrwxrwx   0 root         (0) root         (0)      111 2022-08-21 18:10:28.000000 wrainfo-0.9.5/docs/tutorials_and_examples/reader_module.rst
+-rwxrwxrwx   0 root         (0) root         (0)      117 2022-08-21 17:59:15.000000 wrainfo-0.9.5/docs/tutorials_and_examples/tutorials_and_examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-07-07 07:25:16.155470 wrainfo-0.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3564 2023-07-06 15:49:18.000000 wrainfo-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.151470 wrainfo-0.9.5/wrainfo/
+-rw-rw-rw-   0 root         (0) root         (0)     1551 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9815 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/attenuation_corr.py
+-rwxrwxrwx   0 root         (0) root         (0)     6321 2023-06-15 05:56:44.000000 wrainfo-0.9.5/wrainfo/clutter.py
+-rwxrwxrwx   0 root         (0) root         (0)     4269 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/compression.py
+-rwxrwxrwx   0 root         (0) root         (0)     3149 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/error_flist.py
+-rwxrwxrwx   0 root         (0) root         (0)     7331 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/geometry.py
+-rwxrwxrwx   0 root         (0) root         (0)     2670 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/precipitation.py
+-rwxrwxrwx   0 root         (0) root         (0)    13877 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/process_chains.py
+-rwxrwxrwx   0 root         (0) root         (0)    11034 2023-01-10 10:26:31.000000 wrainfo-0.9.5/wrainfo/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-07-07 07:16:03.000000 wrainfo-0.9.5/wrainfo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 07:25:16.151470 wrainfo-0.9.5/wrainfo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9137 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      522 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-07 07:25:16.000000 wrainfo-0.9.5/wrainfo.egg-info/top_level.txt
```

### Comparing `wrainfo-0.9.3/CONTRIBUTING.rst` & `wrainfo-0.9.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/HISTORY.rst` & `wrainfo-0.9.5/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 =======
 History
 =======
 
+0.9.4 (2023-07-04)
+------------------
+
+General settings:
+
+* update numpy version
+* install dep from conda package manager
+
+Bugs:
+
+* fixed bug in wrainfo.clutter.py
+
 0.9.3 (2023-01-10)
 ------------------
 
 General settings:
 
 * update parameters in the configuration file
```

### Comparing `wrainfo-0.9.3/LICENSE` & `wrainfo-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/PKG-INFO` & `wrainfo-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrainfo
-Version: 0.9.3
+Version: 0.9.5
 Summary: Is a software to process FURUNO weather radar data.
 Home-page: https://git.gfz-potsdam.de/fernlab/products/furuno/wrainfo
 Author: FernLab
 Author-email: fernlab@gfz-potsdam.de
 License: Apache Software License 2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/fernlab/products/furuno/wrainfo
 Project-URL: Documentation, https://fernlab.git-pages.gfz-potsdam.de/products/furuno/wrainfo/doc/
```

### Comparing `wrainfo-0.9.3/README.rst` & `wrainfo-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/Makefile` & `wrainfo-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/fernlab_logo.png` & `wrainfo-0.9.5/docs/_build/html/_images/fernlab_logo.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_12_0.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_12_0.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_18_0.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_attenuation_correction_18_0.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_18_0.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_18_0.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_24_0.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_24_0.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_27_0.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_27_0.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_clutter_detection_6_1.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_clutter_detection_6_1.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_geometry_module_13_1.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_geometry_module_13_1.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_precipitation_estimation_7_1.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_precipitation_estimation_7_1.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_31_1.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_31_1.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_34_1.png` & `wrainfo-0.9.5/docs/_build/html/_images/jupyter_notebooks_read_furuno_data_34_1.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/_build/html/_static/wrainfo_logo.png` & `wrainfo-0.9.5/docs/_build/html/_static/wrainfo_logo.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/conf.py` & `wrainfo-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/images/fernlab_logo.png` & `wrainfo-0.9.5/docs/images/fernlab_logo.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/images/wr_furuno_comparison_of_raw_reflectivity_and_clutter_corrected_reflectivity.png` & `wrainfo-0.9.5/docs/images/wr_furuno_comparison_of_raw_reflectivity_and_clutter_corrected_reflectivity.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/images/wr_furuno_georeferenced_and_gridded_precipitation_data_with_WRaINfo.png` & `wrainfo-0.9.5/docs/images/wr_furuno_georeferenced_and_gridded_precipitation_data_with_WRaINfo.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/images/wr_furuno_reflectivity_attenaution_corrected_and_estimated_precipitation.png` & `wrainfo-0.9.5/docs/images/wr_furuno_reflectivity_attenaution_corrected_and_estimated_precipitation.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/images/wr_furuno_reflectivity_before_and_after_attenaution_correction.png` & `wrainfo-0.9.5/docs/images/wr_furuno_reflectivity_before_and_after_attenaution_correction.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/images/wrainfo_logo.png` & `wrainfo-0.9.5/docs/images/wrainfo_logo.png`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/index.rst` & `wrainfo-0.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/installation.rst` & `wrainfo-0.9.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/make.bat` & `wrainfo-0.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/process_chains/introduction.rst` & `wrainfo-0.9.5/docs/process_chains/introduction.rst`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/docs/tutorials_and_examples/features_overview.rst` & `wrainfo-0.9.5/docs/tutorials_and_examples/features_overview.rst`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/setup.py` & `wrainfo-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,21 @@
     history = history_file.read()
 
 version = {}
 
 with open("wrainfo/version.py") as version_file:
     exec(version_file.read(), version)
 
-req = ['numpy==1.20.3',
+req = ['numpy>=1.22.1',
        'pytest>=6.2.5',
        'scipy>=1.7.0',
        'wradlib>=1.15.0',
        'xarray[complete]==0.20.2',
-       'rioxarray==0.12.0']
+       'rioxarray==0.12.0',
+       'GDAL==3.6.*']
 
 req_setup = ['pytest-runner']
 
 req_test = ['pytest>=3', 'pytest-cov', 'pytest-reporter-html1', 'urlchecker==0.0.32']
 
 req_doc = [
     'sphinx>=4.1.1',
```

### Comparing `wrainfo-0.9.3/wrainfo/__init__.py` & `wrainfo-0.9.5/wrainfo/__init__.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/attenuation_corr.py` & `wrainfo-0.9.5/wrainfo/attenuation_corr.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/clutter.py` & `wrainfo-0.9.5/wrainfo/clutter.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,20 +155,19 @@
             logger.warning("Could not load file:' " + file + "'.")
             continue
 
         # create a data array of reflectivity values
         if sum_dbzh_values is None:
             sum_dbzh_values = np.zeros_like(data.DBZH[0, :, :].values)
 
-        else:
-            values = data.DBZH[0, :, :].values
+        values = data.DBZH[0, :, :].values
 
-            # extract only correct values without NaN values
-            good = ~np.isnan(values)
-            sum_dbzh_values[good] += np.zeros_like(data.DBZH[0, :, :].values[good])
+        # extract only correct values without NaN values
+        good = ~np.isnan(values)
+        sum_dbzh_values[good] += data.DBZH[0, :, :].values[good]
 
         file_count += 1
 
         new = round(20 * file_count / len(files), 0)
 
         if status:
             if new > elapsed:
```

### Comparing `wrainfo-0.9.3/wrainfo/compression.py` & `wrainfo-0.9.5/wrainfo/compression.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/error_flist.py` & `wrainfo-0.9.5/wrainfo/error_flist.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/geometry.py` & `wrainfo-0.9.5/wrainfo/geometry.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/precipitation.py` & `wrainfo-0.9.5/wrainfo/precipitation.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/process_chains.py` & `wrainfo-0.9.5/wrainfo/process_chains.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/reader.py` & `wrainfo-0.9.5/wrainfo/reader.py`

 * *Files identical despite different names*

### Comparing `wrainfo-0.9.3/wrainfo/version.py` & `wrainfo-0.9.5/wrainfo/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '0.9.3'
-__versionalias__ = '2023-01-10_09'
+__version__ = '0.9.5'
+__versionalias__ = '2023-07-07_09'
```

### Comparing `wrainfo-0.9.3/wrainfo.egg-info/PKG-INFO` & `wrainfo-0.9.5/wrainfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrainfo
-Version: 0.9.3
+Version: 0.9.5
 Summary: Is a software to process FURUNO weather radar data.
 Home-page: https://git.gfz-potsdam.de/fernlab/products/furuno/wrainfo
 Author: FernLab
 Author-email: fernlab@gfz-potsdam.de
 License: Apache Software License 2.0
 Project-URL: Source code, https://git.gfz-potsdam.de/fernlab/products/furuno/wrainfo
 Project-URL: Documentation, https://fernlab.git-pages.gfz-potsdam.de/products/furuno/wrainfo/doc/
```

### Comparing `wrainfo-0.9.3/wrainfo.egg-info/SOURCES.txt` & `wrainfo-0.9.5/wrainfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


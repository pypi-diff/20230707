# Comparing `tmp/pyxel_sim-1.9.tar.gz` & `tmp/pyxel_sim-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel_sim-1.9.tar", last modified: Thu Jun  1 10:40:29 2023, max compression
+gzip compressed data, was "pyxel_sim-1.9.1.tar", last modified: Fri Jul  7 10:08:53 2023, max compression
```

## Comparing `pyxel_sim-1.9.tar` & `pyxel_sim-1.9.1.tar`

### file list

```diff
@@ -1,343 +1,543 @@
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.105435 pyxel_sim-1.9/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      552 2023-03-29 16:35:58.000000 pyxel_sim-1.9/AUTHORS.rst
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1085 2022-08-02 12:27:04.000000 pyxel_sim-1.9/LICENSE.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      244 2023-03-29 16:35:58.000000 pyxel_sim-1.9/MANIFEST.in
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6924 2023-06-01 10:40:29.103587 pyxel_sim-1.9/PKG-INFO
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5492 2023-05-15 05:35:04.000000 pyxel_sim-1.9/README.md
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.675500 pyxel_sim-1.9/continuous_integration/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.066278 pyxel_sim-1.9/continuous_integration/scripts/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   130300 2023-05-24 09:13:19.000000 pyxel_sim-1.9/continuous_integration/scripts/auto_generated.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   128772 2023-05-08 19:38:26.000000 pyxel_sim-1.9/continuous_integration/scripts/before_auto_generated.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    29848 2023-05-24 04:59:59.000000 pyxel_sim-1.9/continuous_integration/scripts/create_json_schema.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2421 2023-03-29 16:35:58.000000 pyxel_sim-1.9/continuous_integration/scripts/download_last_environment_artifact.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      249 2023-04-18 08:58:54.000000 pyxel_sim-1.9/continuous_integration/scripts/dummy.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.687646 pyxel_sim-1.9/docs/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.684401 pyxel_sim-1.9/docs/html/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.070375 pyxel_sim-1.9/docs/html/_static/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:04.000000 pyxel_sim-1.9/docs/html/_static/dummy.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.073493 pyxel_sim-1.9/docs/source/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.077008 pyxel_sim-1.9/docs/source/_static/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:04.000000 pyxel_sim-1.9/docs/source/_static/dummy.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10728 2023-05-24 04:59:59.000000 pyxel_sim-1.9/docs/source/conf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5669 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyproject.toml
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.107892 pyxel_sim-1.9/pyxel/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1013 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      653 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/__main__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      495 2023-06-01 10:40:29.108292 pyxel_sim-1.9/pyxel/_version.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.320146 pyxel_sim-1.9/pyxel/backends/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      478 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/backends/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2840 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/backends/asdf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6324 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/backends/hdf5.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.634432 pyxel_sim-1.9/pyxel/calibration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1087 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/calibration/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14707 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/calibration/algorithm.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20616 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/calibration/archipelago.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17840 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/archipelago_datatree.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18051 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2065 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/fitness.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16917 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/calibration/fitting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17657 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/fitting_datatree.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2056 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/calibration/protocols.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5992 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/calibration/user_defined.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13610 2023-05-25 05:43:54.000000 pyxel_sim-1.9/pyxel/calibration/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.691558 pyxel_sim-1.9/pyxel/configuration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      511 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/configuration/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15239 2023-05-24 09:17:19.000000 pyxel_sim-1.9/pyxel/configuration/configuration.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.888254 pyxel_sim-1.9/pyxel/data_structure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      707 2023-04-15 09:29:03.000000 pyxel_sim-1.9/pyxel/data_structure/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4914 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/data_structure/array.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16476 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/data_structure/charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1154 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4902 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/data_structure/persistence.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      952 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/phase.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1940 2023-05-17 07:08:29.000000 pyxel_sim-1.9/pyxel/data_structure/photon.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1132 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/pixel.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2101 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/data_structure/processed_data.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4439 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/data_structure/scene.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1049 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/signal.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1340 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/data_structure/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.063362 pyxel_sim-1.9/pyxel/detectors/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      867 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.118015 pyxel_sim-1.9/pyxel/detectors/apd/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      516 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/apd/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5666 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/apd/apd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15856 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/apd/apd_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      875 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/apd/apd_geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.173248 pyxel_sim-1.9/pyxel/detectors/ccd/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      464 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/ccd/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5496 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/ccd/ccd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      869 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/ccd/ccd_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9216 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/characteristics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.199785 pyxel_sim-1.9/pyxel/detectors/cmos/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      468 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/cmos/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5358 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/cmos/cmos.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      877 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/cmos/cmos_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    22369 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/detectors/detector.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2412 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8273 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.247063 pyxel_sim-1.9/pyxel/detectors/mkid/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      468 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/mkid/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7083 2023-05-24 08:34:39.000000 pyxel_sim-1.9/pyxel/detectors/mkid/mkid.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      877 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/mkid/mkid_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      472 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/optics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2824 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/detectors/readout_properties.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4085 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/evaluator.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.300724 pyxel_sim-1.9/pyxel/exposure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      532 2023-05-17 07:08:29.000000 pyxel_sim-1.9/pyxel/exposure/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10011 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/exposure/exposure.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4710 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/exposure/readout.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.327623 pyxel_sim-1.9/pyxel/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      479 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/inputs/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9604 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/inputs/loader.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.390809 pyxel_sim-1.9/pyxel/models/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      450 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.535819 pyxel_sim-1.9/pyxel/models/charge_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      643 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_collection/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      696 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_collection/collection.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9200 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_collection/diffusion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4890 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_collection/fixed_pattern_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1488 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_collection/full_well.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3229 2023-05-17 07:08:29.000000 pyxel_sim-1.9/pyxel/models/charge_collection/inter_pixel_capacitance.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15959 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_collection/persistence.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.678669 pyxel_sim-1.9/pyxel/models/charge_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      859 2023-05-30 12:18:54.000000 pyxel_sim-1.9/pyxel/models/charge_generation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1165 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/charge_generation/apd_gain.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16775 2023-05-24 04:59:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/charge_deposition.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2539 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/charge_injection.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.835229 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16084 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/cosmix.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.740004 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.976460 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13498 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/particle.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23212 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/plotting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20041 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/simulation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3672 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/util.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12524 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/dark_current.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6059 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/dark_current_rule07.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.069638 pyxel_sim-1.9/pyxel/models/charge_generation/data/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1875 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/mct-stopping-power.csv
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    51083 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    50826 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2524 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1941 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/load_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4979 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/photoelectrons.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.264847 pyxel_sim-1.9/pyxel/models/charge_measurement/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      853 2023-05-25 08:34:10.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16977 2023-05-25 08:34:10.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/linearity.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1636 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/measurement.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.350327 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13399 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    33333 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8678 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/non_linearity_calculation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3063 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/offset.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5626 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/readout_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2490 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/reset_noise.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.462156 pyxel_sim-1.9/pyxel/models/charge_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2677 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/EMCCD_poisson.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      496 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.517357 pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8702 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18727 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/cdm.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.637538 pyxel_sim-1.9/pyxel/models/data_processing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      647 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/models/data_processing/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6055 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/models/data_processing/linear_regression.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5397 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/models/data_processing/mean_variance.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4798 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/data_processing/source_extractor.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3882 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/models/data_processing/statistics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.671692 pyxel_sim-1.9/pyxel/models/optics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      662 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/optics/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2009 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/optics/point_spread_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12726 2023-05-22 12:43:55.000000 pyxel_sim-1.9/pyxel/models/optics/poppy.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.730350 pyxel_sim-1.9/pyxel/models/phasing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      450 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/phasing/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2126 2023-05-24 08:34:39.000000 pyxel_sim-1.9/pyxel/models/phasing/pulse_processing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.884241 pyxel_sim-1.9/pyxel/models/photon_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      630 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/photon_collection/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7918 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2951 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1794 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/point_spread_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12512 2023-05-22 12:43:55.000000 pyxel_sim-1.9/pyxel/models/photon_collection/poppy.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2611 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3657 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/photon_collection/stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.988669 pyxel_sim-1.9/pyxel/models/photon_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      750 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/photon_generation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8144 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_generation/illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3150 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_generation/load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2811 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_generation/shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3887 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/photon_generation/stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.210492 pyxel_sim-1.9/pyxel/models/readout_electronics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      716 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1413 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/amplification.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9454 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/amplifier_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3552 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/dead_time.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      916 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/phase_conversion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2348 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7109 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc_with_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2267 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/simple_adc.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.232095 pyxel_sim-1.9/pyxel/models/scene_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/scene_generation/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.259567 pyxel_sim-1.9/pyxel/models/signal_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      403 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/signal_transfer/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1272 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.346727 pyxel_sim-1.9/pyxel/notebook/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      784 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/notebook/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16292 2023-05-31 14:39:03.000000 pyxel_sim-1.9/pyxel/notebook/calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5202 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/notebook/html_representation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10431 2023-05-24 08:34:39.000000 pyxel_sim-1.9/pyxel/notebook/jupyxel.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.422174 pyxel_sim-1.9/pyxel/observation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      532 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/observation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    43007 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/observation/observation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5340 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/observation/parameter_values.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3903 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/options.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.565094 pyxel_sim-1.9/pyxel/outputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      621 2023-04-19 20:35:04.000000 pyxel_sim-1.9/pyxel/outputs/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4847 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/calibration_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3146 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/exposure_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4488 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/observation_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16300 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/outputs.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.696763 pyxel_sim-1.9/pyxel/pipelines/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      681 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/pipelines/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6107 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/pipelines/model_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3089 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/pipelines/model_group.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8201 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/pipelines/pipeline.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9320 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/pipelines/processor.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20958 2023-05-31 14:38:11.000000 pyxel_sim-1.9/pyxel/run.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4567 2023-05-30 05:42:20.000000 pyxel_sim-1.9/pyxel/show_versions.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6124 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/state.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.748908 pyxel_sim-1.9/pyxel/templates/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4039 2023-05-24 04:59:59.000000 pyxel_sim-1.9/pyxel/templates/_TEMPLATE.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.938172 pyxel_sim-1.9/pyxel/util/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3015 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3867 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/util/add_model.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1973 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/util/examples.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6171 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7475 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/util/materials.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2308 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/util/memory.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      999 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/random.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2202 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/timing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.960083 pyxel_sim-1.9/pyxel_sim.egg-info/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6924 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/PKG-INFO
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10638 2023-06-01 10:40:22.000000 pyxel_sim-1.9/pyxel_sim.egg-info/SOURCES.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        1 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/dependency_links.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       41 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/entry_points.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      425 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/requires.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      101 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/top_level.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       38 2023-06-01 10:40:29.105879 pyxel_sim-1.9/setup.cfg
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      266 2023-03-29 16:35:59.000000 pyxel_sim-1.9/setup.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.052468 pyxel_sim-1.9/tests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      375 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.112009 pyxel_sim-1.9/tests/calibration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7424 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/calibration/test_check_ranges.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2932 2023-05-31 10:39:47.000000 pyxel_sim-1.9/tests/calibration/test_fitness.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2171 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/calibration/test_slice_to_range.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.166710 pyxel_sim-1.9/tests/configuration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15979 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/configuration/test_load.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1589 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/configuration/test_schema.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1485 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/conftest.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.174528 pyxel_sim-1.9/tests/data_structure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12924 2023-05-24 08:35:07.000000 pyxel_sim-1.9/tests/data_structure/test_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3890 2023-04-15 09:29:03.000000 pyxel_sim-1.9/tests/data_structure/test_processed_data.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.419458 pyxel_sim-1.9/tests/detectors/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15278 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_ccd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4861 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_ccd_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4295 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_ccd_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11767 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_cmos.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4590 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_cmos_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4359 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_cmos_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7061 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/detectors/test_detectors.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2367 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6977 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12053 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_mkid.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4583 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_mkid_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4308 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_mkid_geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.465334 pyxel_sim-1.9/tests/exposure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1827 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/exposure/test_readout.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.536674 pyxel_sim-1.9/tests/functional_tests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:05.000000 pyxel_sim-1.9/tests/functional_tests/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3369 2023-05-17 07:08:30.000000 pyxel_sim-1.9/tests/functional_tests/test_basic_exposure.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4076 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/functional_tests/test_parametric.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5386 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/functional_tests/test_yaml.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.583129 pyxel_sim-1.9/tests/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21926 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/inputs/test_image.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.792841 pyxel_sim-1.9/tests/model_tests/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.611553 pyxel_sim-1.9/tests/model_tests/amplifier_crosstalk/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1060 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/model_tests/amplifier_crosstalk/test_crosstalk.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.649427 pyxel_sim-1.9/tests/models/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.774176 pyxel_sim-1.9/tests/models/charge_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3046 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_collection/test_fixed_pattern_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5572 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/models/charge_collection/test_persistence.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1946 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_collection/test_simple_full_well.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9628 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_collection/test_simple_ipc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3609 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_collection/test_simple_persistence.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.932761 pyxel_sim-1.9/tests/models/charge_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2551 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_apd_gain.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2867 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_charge_deposition_in_MCT.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3528 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_charge_injection.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5033 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_dark_current.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1843 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_dark_current_rule07.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4309 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_load_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3366 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_generation/test_photoelectrons.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.244769 pyxel_sim-1.9/tests/models/charge_measurement/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2659 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_nghxrg.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5951 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_non_linearity.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3793 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_offset.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4752 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_readout_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2723 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_reset_noise.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.299909 pyxel_sim-1.9/tests/models/charge_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2265 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_transfer/arctic_remove.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1680 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_transfer/test_arctic_add.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8639 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_transfer/test_cdm.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      718 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_transfer/test_emccd_poisson.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.317423 pyxel_sim-1.9/tests/models/data_processing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1916 2023-05-17 07:08:30.000000 pyxel_sim-1.9/tests/models/data_processing/test_statistics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.336552 pyxel_sim-1.9/tests/models/phasing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3187 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/phasing/test_pulse_processing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.532086 pyxel_sim-1.9/tests/models/photon_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2914 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/photon_collection/test_illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3899 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/photon_collection/test_load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2042 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/photon_collection/test_load_psf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5010 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/models/photon_collection/test_optical_psf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5640 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/photon_collection/test_shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2081 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/photon_collection/test_stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.708821 pyxel_sim-1.9/tests/models/readout_electronics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3384 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_ac_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3384 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_dc_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2924 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_dead_time_filter.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      720 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_get_matrix.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1069 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_phase_conversion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1071 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3229 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc_with_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2161 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_simple_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2029 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/test_save_load_detector.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.716014 pyxel_sim-1.9/tests/pipelines/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.741396 pyxel_sim-1.9/tests/pipelines/observation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2360 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/pipelines/observation/test_validate_steps.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1925 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/pipelines/test_pipelines.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.772580 pyxel_sim-1.9/tests/running_mode/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21242 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/running_mode/test_observation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1772 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/test_evaluator.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1914 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/test_options.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      486 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/test_show_versions.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.983777 pyxel_sim-1.9/tests/unittests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      375 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1654 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_arguments.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4832 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3908 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_detector.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6789 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15920 2023-05-31 10:39:47.000000 pyxel_sim-1.9/tests/unittests/test_fitting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2463 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_model_function.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.081576 pyxel_sim-1.9/tests/util/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10118 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/util/test_fit_into_array.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1375 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/util/test_memory.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2362 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/util/test_random.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.820615 pyxel_sim-1.9/venv/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.100325 pyxel_sim-1.9/venv/bin/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1176 2023-01-04 09:36:07.000000 pyxel_sim-1.9/venv/bin/activate_this.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.671072 pyxel_sim-1.9.1/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       65 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.dockerignore
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      180 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/.flake8
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       31 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.gitattributes
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      758 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/.gitignore
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:51.943036 pyxel_sim-1.9.1/.gitlab/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.115502 pyxel_sim-1.9.1/.gitlab/issue_templates/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      916 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.gitlab/issue_templates/bug_report.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      766 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.gitlab/issue_templates/documentation_improvement.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      683 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.gitlab/issue_templates/feature_request.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      579 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.gitlab/issue_templates/submit_question.md
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.118329 pyxel_sim-1.9.1/.gitlab/merge_request_templates/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1945 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/.gitlab/merge_request_templates/merge_request_template.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8113 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/.gitlab-ci.yml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/.gitmodules
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      815 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      552 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/AUTHORS.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    55097 2023-07-07 09:25:08.000000 pyxel_sim-1.9.1/CHANGELOG.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3400 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2257 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/Dockerfile
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5755 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/HOW_TO_RELEASE.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1085 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/LICENSE.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      244 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/MANIFEST.in
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6926 2023-07-07 10:08:53.669925 pyxel_sim-1.9.1/PKG-INFO
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5492 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/README.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2733 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/badges.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.124385 pyxel_sim-1.9.1/continuous_integration/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      526 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/continuous_integration/pyxel-1.4-environment.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      678 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/continuous_integration/pyxel-1.5-environment.yaml
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.134897 pyxel_sim-1.9.1/continuous_integration/scripts/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   131624 2023-05-25 14:28:38.000000 pyxel_sim-1.9.1/continuous_integration/scripts/auto_generated.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    29191 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/continuous_integration/scripts/create_json_schema.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2421 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/continuous_integration/scripts/download_last_environment_artifact.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       47 2023-02-02 10:30:03.000000 pyxel_sim-1.9.1/continuous_integration/scripts/requirements.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2240 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/development.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      171 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docker-compose.yml
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.154384 pyxel_sim-1.9.1/docs/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      606 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/Makefile
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      334 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/README.rst
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.158435 pyxel_sim-1.9.1/docs/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      197 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/_static/redirect.html
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1456 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/docker-howto.md
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:51.946809 pyxel_sim-1.9.1/docs/html/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.161082 pyxel_sim-1.9.1/docs/html/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/html/_static/dummy.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      777 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/make.bat
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      286 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/requirements-docs.txt
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.167683 pyxel_sim-1.9.1/docs/source/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.241613 pyxel_sim-1.9.1/docs/source/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   428380 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/H4RG.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/dummy.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)  1975157 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/_static/jupyterlab_json_schema.mp4
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.316589 pyxel_sim-1.9.1/docs/source/_static/old/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   136896 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_pipeline.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    71577 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_pipeline_spie-paper.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    50225 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_pipeline_spie-paper_NEW.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    86839 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_poster_spie-paper.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    81266 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_poster_spie-paper_NEW.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    69624 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_toplevel.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    74202 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_toplevel_time_dependent.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    48536 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_architecture_webserver_GUI.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    60953 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/old/pyxel_detector_spie-paper.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   873681 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/_static/pycharm_json_schema.mp4
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   334914 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/_static/pycharm_json_schema_associate.mp4
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   977790 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/_static/pyxel-logo.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    48535 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/pyxel_ccd_pipeline.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    53745 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/pyxel_cmos_pipeline.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    50117 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/pyxel_detector.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    50225 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/docs/source/_static/pyxel_pipeline.graphml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   968399 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/_static/vscode_json_schema.mp4
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.343337 pyxel_sim-1.9.1/docs/source/about/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.350827 pyxel_sim-1.9.1/docs/source/about/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    66594 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/about/_static/ESA_logo_2020_Deep.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   112599 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/about/_static/eso_colour.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      309 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/about/acknowledgements.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      983 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/about/acronyms.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       74 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/about/bibliography.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3221 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/about/brief_history.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4989 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/about/citation.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       48 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/about/contributors.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       81 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/about/license.rst
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.371839 pyxel_sim-1.9.1/docs/source/background/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.487456 pyxel_sim-1.9.1/docs/source/background/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   179653 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/background/_static/architecture.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    86387 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/calibration.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    89527 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/background/_static/detector.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    28804 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/exposure.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    84975 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/_static/model-table.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    61149 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/observation.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    86554 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/_static/pipeline.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   262135 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/pyxel_ccd_pipeline.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   161009 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/pyxel_detector.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   204388 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/running_modes.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    96339 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/_static/yaml_new.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1235 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/architecture.rst
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.571757 pyxel_sim-1.9.1/docs/source/background/detectors/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1266 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/detectors/apd.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1407 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/detectors/ccd.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1571 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/detectors/cmos.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3038 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/detectors/mkid.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3102 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/background/detectors.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      633 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/background/overview.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6776 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/pipeline.rst
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.581805 pyxel_sim-1.9.1/docs/source/background/running_modes/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4789 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/docs/source/background/running_modes/calibration_mode.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2382 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/docs/source/background/running_modes/exposure_mode.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5816 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/docs/source/background/running_modes/observation_mode.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1393 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/background/running_modes.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4614 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/background/yaml.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    10728 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/conf.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.612755 pyxel_sim-1.9.1/docs/source/howto/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.646167 pyxel_sim-1.9.1/docs/source/howto/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   114015 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/pycharm_associated_1.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    92881 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/pycharm_example_annotation.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    80264 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/pycharm_example_validation.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   116306 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/pycharm_mappings.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    46393 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/vscode_example_annotation.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    43350 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/vscode_example_validation.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    28336 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/vscode_yaml_extension.jpg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    52744 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/_static/vscode_yaml_extension.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6954 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/detector_import_export.ipynb
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3642 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/howto/exposure.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4565 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/howto/json_schema.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6045 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/howto/new_model.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      752 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/howto/overview.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    51139 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/howto/proton_L2_solarMax_11mm_Shielding.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3736 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/index.rst
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.706055 pyxel_sim-1.9.1/docs/source/references/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.740630 pyxel_sim-1.9.1/docs/source/references/api/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      786 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/calibration.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      226 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/configuration.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1124 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/datastructures.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1416 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/detectorproperties.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      912 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/detectors.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      252 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/exposure.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      124 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/inputs.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      463 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/notebook.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      399 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/observation.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      487 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/outputs.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      617 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/pipelines.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      240 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/docs/source/references/api/run.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      390 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/api/util.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      366 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/references/apireference.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       40 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/changelog.md
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    29205 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/references/contributing.rst
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.755116 pyxel_sim-1.9.1/docs/source/references/model_groups/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.770550 pyxel_sim-1.9.1/docs/source/references/model_groups/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   264229 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/_static/cdm.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   248472 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/_static/cosmix.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   109368 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/_static/nghxrg.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    97998 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/_static/poppy.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    11742 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/_static/sar_architecture.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9880 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/charge_collection_models.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15412 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/charge_generation_models.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    14013 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/charge_measurement_models.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5335 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/charge_transfer_models.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1879 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/phasing_models.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6597 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/references/model_groups/readout_electronics.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1939 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/references/models.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      250 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/references/overview.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    18017 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/docs/source/refs.bib
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.788264 pyxel_sim-1.9.1/docs/source/tutorials/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.796123 pyxel_sim-1.9.1/docs/source/tutorials/_static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   406993 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/tutorials/_static/Pyxel-example-transparent.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    35277 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/docs/source/tutorials/_static/pyxel-logo.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6198 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/tutorials/environments.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2344 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/docs/source/tutorials/examples.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      910 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/docs/source/tutorials/get_help.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    14966 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/docs/source/tutorials/install.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4564 2023-07-07 09:29:23.000000 pyxel_sim-1.9.1/docs/source/tutorials/overview.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4241 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/docs/source/tutorials/running.rst
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1440 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/kubernetes.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    23121 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/logo.png
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5810 2023-07-07 09:23:56.000000 pyxel_sim-1.9.1/pyproject.toml
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.673574 pyxel_sim-1.9.1/pyxel/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1013 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/pyxel/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      653 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/__main__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      497 2023-07-07 10:08:53.673774 pyxel_sim-1.9.1/pyxel/_version.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.823190 pyxel_sim-1.9.1/pyxel/backends/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      478 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/backends/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2840 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/backends/asdf.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6324 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/backends/hdf5.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.870464 pyxel_sim-1.9.1/pyxel/calibration/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1087 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    14707 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/calibration/algorithm.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    20620 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/archipelago.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    17844 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/archipelago_datatree.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    18051 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/calibration.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2065 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/fitness.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16893 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/fitting.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    17633 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/calibration/fitting_datatree.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2056 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/calibration/protocols.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5992 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/calibration/user_defined.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    13610 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/calibration/util.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.874412 pyxel_sim-1.9.1/pyxel/configuration/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      511 2023-05-10 07:49:39.000000 pyxel_sim-1.9.1/pyxel/configuration/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15335 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/configuration/configuration.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.906568 pyxel_sim-1.9.1/pyxel/data_structure/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      707 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/data_structure/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4914 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/data_structure/array.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16476 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/data_structure/charge.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1154 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/data_structure/image.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4902 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/data_structure/persistence.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      952 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/data_structure/phase.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1940 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/data_structure/photon.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1132 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/data_structure/pixel.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2101 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/data_structure/processed_data.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4436 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/data_structure/scene.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1049 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/data_structure/signal.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1340 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/data_structure/util.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.926423 pyxel_sim-1.9.1/pyxel/detectors/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      867 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/__init__.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.934951 pyxel_sim-1.9.1/pyxel/detectors/apd/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      516 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/detectors/apd/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5666 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/apd/apd.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15851 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/detectors/apd/apd_characteristics.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      875 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/apd/apd_geometry.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.941962 pyxel_sim-1.9.1/pyxel/detectors/ccd/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      464 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/ccd/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5496 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/ccd/ccd.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      869 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/ccd/ccd_geometry.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9216 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/characteristics.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.948136 pyxel_sim-1.9.1/pyxel/detectors/cmos/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      468 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/cmos/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5358 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/cmos/cmos.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      877 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/cmos/cmos_geometry.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    22357 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/detectors/detector.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2412 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/environment.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8273 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/geometry.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.959612 pyxel_sim-1.9.1/pyxel/detectors/mkid/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      468 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/mkid/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7083 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/mkid/mkid.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      877 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/detectors/mkid/mkid_geometry.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      472 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/detectors/optics.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2824 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/detectors/readout_properties.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4085 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/evaluator.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.971097 pyxel_sim-1.9.1/pyxel/exposure/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      532 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/exposure/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    10015 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/exposure/exposure.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4710 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/exposure/readout.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.977067 pyxel_sim-1.9.1/pyxel/inputs/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      479 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/inputs/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9604 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/inputs/loader.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.981111 pyxel_sim-1.9.1/pyxel/models/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      450 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/__init__.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:52.995931 pyxel_sim-1.9.1/pyxel/models/charge_collection/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      643 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      696 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/collection.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9200 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/diffusion.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4890 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/fixed_pattern_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1488 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/full_well.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3229 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/inter_pixel_capacitance.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15959 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_collection/persistence.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.032859 pyxel_sim-1.9.1/pyxel/models/charge_generation/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      859 2023-06-02 11:05:25.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1165 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/apd_gain.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16775 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/charge_deposition.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2539 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/charge_injection.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.047918 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      387 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16084 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/cosmix.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:51.970059 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.081606 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    13498 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/particle.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    23212 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/plotting.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    20041 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/simulation.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3672 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/util.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    12524 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/dark_current.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6059 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/dark_current_rule07.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.095656 pyxel_sim-1.9.1/pyxel/models/charge_generation/data/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1875 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/data/mct-stopping-power.csv
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    51083 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    50826 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2524 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1978 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/load_charge.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4979 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_generation/photoelectrons.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.110299 pyxel_sim-1.9.1/pyxel/models/charge_measurement/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      853 2023-05-31 08:33:42.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16977 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/linearity.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1636 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/measurement.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.124982 pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    26213 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/01_README.ipynb
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      387 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    13399 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/nghxrg.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    33333 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8678 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/non_linearity_calculation.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3063 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/offset.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5626 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/readout_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2490 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_measurement/reset_noise.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.132285 pyxel_sim-1.9.1/pyxel/models/charge_transfer/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2677 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/models/charge_transfer/EMCCD_poisson.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      496 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_transfer/__init__.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.137371 pyxel_sim-1.9.1/pyxel/models/charge_transfer/arctic_cti/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      387 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/charge_transfer/arctic_cti/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8702 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    18727 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/charge_transfer/cdm.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.145770 pyxel_sim-1.9.1/pyxel/models/data_processing/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      647 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/data_processing/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6098 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/models/data_processing/linear_regression.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5435 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/models/data_processing/mean_variance.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4798 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/models/data_processing/source_extractor.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3920 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/models/data_processing/statistics.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.150628 pyxel_sim-1.9.1/pyxel/models/optics/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      662 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/models/optics/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2009 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/models/optics/point_spread_function.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    12726 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/optics/poppy.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.154905 pyxel_sim-1.9.1/pyxel/models/phasing/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      450 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/phasing/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2126 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/phasing/pulse_processing.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.172500 pyxel_sim-1.9.1/pyxel/models/photon_collection/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      630 2023-07-07 09:20:01.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7918 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/illumination.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2951 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/load_image.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1794 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/point_spread_function.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    12512 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/poppy.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2611 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/shot_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3657 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_collection/stripe_pattern.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.182658 pyxel_sim-1.9.1/pyxel/models/photon_generation/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      750 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/models/photon_generation/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8144 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_generation/illumination.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3150 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_generation/load_image.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2811 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_generation/shot_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3887 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/photon_generation/stripe_pattern.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.197327 pyxel_sim-1.9.1/pyxel/models/readout_electronics/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      716 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1413 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/amplification.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9454 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/amplifier_crosstalk.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3552 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/dead_time.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      916 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/phase_conversion.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2348 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/sar_adc.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7109 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/sar_adc_with_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2267 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/models/readout_electronics/simple_adc.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.198781 pyxel_sim-1.9.1/pyxel/models/scene_generation/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      387 2023-07-07 09:20:01.000000 pyxel_sim-1.9.1/pyxel/models/scene_generation/__init__.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.200349 pyxel_sim-1.9.1/pyxel/models/signal_transfer/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      403 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/signal_transfer/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1272 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/pyxel/models/util.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.207671 pyxel_sim-1.9.1/pyxel/notebook/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      784 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/notebook/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16292 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/notebook/calibration.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5202 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/notebook/html_representation.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    10431 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/notebook/jupyxel.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.215915 pyxel_sim-1.9.1/pyxel/observation/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      532 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/observation/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    43007 2023-07-07 09:20:01.000000 pyxel_sim-1.9.1/pyxel/observation/observation.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5340 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/observation/parameter_values.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3903 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/options.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.254516 pyxel_sim-1.9.1/pyxel/outputs/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      621 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/outputs/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4847 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/outputs/calibration_outputs.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3146 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/outputs/exposure_outputs.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4488 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/outputs/observation_outputs.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    16300 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/outputs/outputs.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.277871 pyxel_sim-1.9.1/pyxel/pipelines/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      681 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/pipelines/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6510 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/pipelines/model_function.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2425 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/pipelines/model_group.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7915 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/pipelines/pipeline.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8644 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/pipelines/processor.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      102 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/pyxel/py.typed
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    20912 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/run.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4567 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/show_versions.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6124 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/state.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.282827 pyxel_sim-1.9.1/pyxel/templates/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4039 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/templates/_TEMPLATE.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.299282 pyxel_sim-1.9.1/pyxel/util/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2721 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/util/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3867 2023-07-07 09:20:01.000000 pyxel_sim-1.9.1/pyxel/util/add_model.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1973 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/util/examples.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6171 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/util/image.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7475 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/util/materials.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2308 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/pyxel/util/memory.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      999 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/pyxel/util/randomize.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2202 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/pyxel/util/timing.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    35277 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/pyxel-logo.png
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.310226 pyxel_sim-1.9.1/pyxel_sim.egg-info/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6926 2023-07-07 10:08:50.000000 pyxel_sim-1.9.1/pyxel_sim.egg-info/PKG-INFO
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    17889 2023-07-07 10:08:51.000000 pyxel_sim-1.9.1/pyxel_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        1 2023-07-07 10:08:50.000000 pyxel_sim-1.9.1/pyxel_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       41 2023-07-07 10:08:50.000000 pyxel_sim-1.9.1/pyxel_sim.egg-info/entry_points.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      434 2023-07-07 10:08:50.000000 pyxel_sim-1.9.1/pyxel_sim.egg-info/requires.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      105 2023-07-07 10:08:50.000000 pyxel_sim-1.9.1/pyxel_sim.egg-info/top_level.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       38 2023-07-07 10:08:53.671345 pyxel_sim-1.9.1/setup.cfg
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      266 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/setup.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.311444 pyxel_sim-1.9.1/static/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   177560 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/static/pyxel_schema.json
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.338541 pyxel_sim-1.9.1/tests/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      375 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/__init__.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.345648 pyxel_sim-1.9.1/tests/calibration/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7424 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/calibration/test_check_ranges.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2932 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/tests/calibration/test_fitness.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2171 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/calibration/test_slice_to_range.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.349787 pyxel_sim-1.9.1/tests/configuration/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.374244 pyxel_sim-1.9.1/tests/configuration/data/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3002 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/configuration/data/calibration.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2960 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/configuration/data/exposure1.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3613 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/configuration/data/exposure2.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2542 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/configuration/data/observation_custom.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3736 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/configuration/data/observation_custom_parallel.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3013 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/configuration/data/observation_product.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3436 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/configuration/data/observation_sequential.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15979 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/configuration/test_load.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1589 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/configuration/test_schema.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1485 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/conftest.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.456594 pyxel_sim-1.9.1/tests/data/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       41 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/ascii_input_0.data
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       33 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/ascii_input_1.data
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       41 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/ascii_input_2.data
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       33 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/ascii_input_3.data
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       33 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/ascii_input_4.data
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)       40 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/ascii_input_5.data
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9690 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate-data-weights.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    83520 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate-data.fits
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      160 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate-data.npy
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    25073 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate-data.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1506 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1503 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_custom_fitness.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1499 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_fits.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1505 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_least_squares.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3863 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/data/calibrate_models.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1541 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_nlopt.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1517 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_sade.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1501 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_sga.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1569 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/calibrate_weighting.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3576 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/data/dummy_simple.yaml
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.505747 pyxel_sim-1.9.1/tests/data/inputs/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    51139 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/proton_L2_solarMax_11mm_Shielding.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    50826 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/proton_L2_solarMax_NoShielding.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)   657923 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2784 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/data/inputs/stopping_power_protons.txt
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3724 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/data/parametric.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3137 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/data/yaml.yaml
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.509976 pyxel_sim-1.9.1/tests/data_structure/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    12924 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/data_structure/test_charge.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3890 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/data_structure/test_processed_data.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.543093 pyxel_sim-1.9.1/tests/detectors/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15278 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/detectors/test_ccd.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4861 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/detectors/test_ccd_characteristics.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4295 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/detectors/test_ccd_geometry.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    11767 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/detectors/test_cmos.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4590 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/detectors/test_cmos_characteristics.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4359 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/detectors/test_cmos_geometry.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     7061 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/detectors/test_detectors.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2367 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/detectors/test_environment.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6977 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/detectors/test_geometry.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    12053 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/detectors/test_mkid.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4583 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/detectors/test_mkid_characteristics.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4308 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/detectors/test_mkid_geometry.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.545102 pyxel_sim-1.9.1/tests/exposure/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1827 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/exposure/test_readout.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.551672 pyxel_sim-1.9.1/tests/functional_tests/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2022-10-19 07:19:18.000000 pyxel_sim-1.9.1/tests/functional_tests/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3369 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/functional_tests/test_basic_exposure.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4076 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/functional_tests/test_parametric.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5386 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/functional_tests/test_yaml.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.554225 pyxel_sim-1.9.1/tests/inputs/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    21926 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/inputs/test_image.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:51.992711 pyxel_sim-1.9.1/tests/model_tests/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.556906 pyxel_sim-1.9.1/tests/model_tests/amplifier_crosstalk/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1060 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/model_tests/amplifier_crosstalk/test_crosstalk.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.559213 pyxel_sim-1.9.1/tests/models/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.566580 pyxel_sim-1.9.1/tests/models/charge_collection/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3046 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_collection/test_fixed_pattern_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5572 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/charge_collection/test_persistence.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1946 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_collection/test_simple_full_well.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     9628 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_collection/test_simple_ipc.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3609 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_collection/test_simple_persistence.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.585294 pyxel_sim-1.9.1/tests/models/charge_generation/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2551 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_apd_gain.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2867 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_charge_deposition_in_MCT.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3528 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_charge_injection.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5033 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_dark_current.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1843 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_dark_current_rule07.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4309 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_load_charge.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3366 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_generation/test_photoelectrons.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.595494 pyxel_sim-1.9.1/tests/models/charge_measurement/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2659 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_measurement/test_nghxrg.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5951 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/charge_measurement/test_non_linearity.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3793 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_measurement/test_offset.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4752 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_measurement/test_readout_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2723 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/charge_measurement/test_reset_noise.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.601244 pyxel_sim-1.9.1/tests/models/charge_transfer/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2265 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_transfer/arctic_remove.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1680 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_transfer/test_arctic_add.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     8639 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/charge_transfer/test_cdm.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      718 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/charge_transfer/test_emccd_poisson.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.603097 pyxel_sim-1.9.1/tests/models/data_processing/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1916 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/data_processing/test_statistics.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.605435 pyxel_sim-1.9.1/tests/models/phasing/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3187 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/phasing/test_pulse_processing.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.614802 pyxel_sim-1.9.1/tests/models/photon_collection/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2914 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/photon_collection/test_illumination.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3899 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/photon_collection/test_load_image.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2042 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/photon_collection/test_load_psf.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5010 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/models/photon_collection/test_optical_psf.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     5640 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/photon_collection/test_shot_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2081 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/photon_collection/test_stripe_pattern.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.638762 pyxel_sim-1.9.1/tests/models/readout_electronics/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3384 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_ac_crosstalk.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3384 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_dc_crosstalk.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2924 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_dead_time_filter.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      720 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_get_matrix.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1069 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_phase_conversion.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1071 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_sar_adc.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3229 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_sar_adc_with_noise.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2161 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/readout_electronics/test_simple_adc.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2029 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/models/test_save_load_detector.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.640363 pyxel_sim-1.9.1/tests/pipelines/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.642407 pyxel_sim-1.9.1/tests/pipelines/observation/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2360 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/pipelines/observation/test_validate_steps.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1925 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/pipelines/test_pipelines.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.644055 pyxel_sim-1.9.1/tests/running_mode/
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.651293 pyxel_sim-1.9.1/tests/running_mode/data/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2386 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/running_mode/data/observation_product.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2260 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/running_mode/data/observation_product_simple.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2421 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/running_mode/data/observation_sequential.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2263 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/running_mode/data/observation_sequential_simple.yaml
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    21242 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/running_mode/test_observation.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1772 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/test_evaluator.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1914 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/test_options.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      486 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/test_show_versions.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.663701 pyxel_sim-1.9.1/tests/unittests/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)      375 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/unittests/__init__.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1654 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/unittests/test_arguments.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4832 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/unittests/test_calibration.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     3908 2023-02-09 12:44:30.000000 pyxel_sim-1.9.1/tests/unittests/test_detector.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     6789 2022-12-02 12:57:13.000000 pyxel_sim-1.9.1/tests/unittests/test_environment.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    15920 2023-07-05 11:16:59.000000 pyxel_sim-1.9.1/tests/unittests/test_fitting.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2463 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/unittests/test_model_function.py
+drwxr-xr-x   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)        0 2023-07-07 10:08:53.667636 pyxel_sim-1.9.1/tests/util/
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)    10118 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tests/util/test_fit_into_array.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     1375 2023-05-10 07:49:40.000000 pyxel_sim-1.9.1/tests/util/test_memory.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     2362 2023-01-10 14:26:17.000000 pyxel_sim-1.9.1/tests/util/test_random.py
+-rw-r--r--   0 constanze.seibert (1199361496) ESAAD\Domain Users (1276952531)     4392 2023-06-01 09:58:19.000000 pyxel_sim-1.9.1/tox.ini
```

### Comparing `pyxel_sim-1.9/AUTHORS.rst` & `pyxel_sim-1.9.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/LICENSE.txt` & `pyxel_sim-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/PKG-INFO` & `pyxel_sim-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel_sim
-Version: 1.9
+Version: 1.9.1
 Summary: Pyxel detector simulation framework.
 Author-email: The Pyxel development team <pyxel@esa.int>
 License: MIT
 Project-URL: homepage, https://esa.gitlab.io/pyxel/
 Project-URL: documentation, https://esa.gitlab.io/pyxel/doc/
 Project-URL: repository, https://gitlab.com/esa/pyxel
 Project-URL: changelog, https://gitlab.com/esa/pyxel/-/releases
```

### Comparing `pyxel_sim-1.9/README.md` & `pyxel_sim-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/continuous_integration/scripts/auto_generated.py` & `pyxel_sim-1.9.1/continuous_integration/scripts/auto_generated.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,42 +20,39 @@
 from typing import Any, Iterator, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import click
 from apischema import schema
 from apischema.json_schema import JsonSchemaVersion, deserialization_schema
 
 
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelLoadSaveDetectorArguments(Mapping[str, Any]):
     filename: float = field(
-        metadata=schema(title="filename", description="Filename to load/save.")
-    )
-
+    metadata=schema(title='filename', description='Filename to load/save.')
+)
 
 @dataclass
 class ModelLoadDetector:
     name: str
     arguments: ModelLoadSaveDetectorArguments
-    func: Literal["pyxel.models.load_detector"] = "pyxel.models.load_detector"
+    func: Literal['pyxel.models.load_detector'] = 'pyxel.models.load_detector'
     enabled: bool = True
 
-
 @dataclass
 class ModelSaveDetector:
     name: str
     arguments: ModelLoadSaveDetectorArguments
-    func: Literal["pyxel.models.save_detector"] = "pyxel.models.save_detector"
+    func: Literal['pyxel.models.save_detector'] = 'pyxel.models.save_detector'
     enabled: bool = True
 
-
 @dataclass
 class ModelFunction:
     name: str
-    func: str = field(metadata=schema(pattern="^(?!pyxel\.models\.)"))
+    func: str = field(metadata=schema(pattern='^(?!pyxel\.models\.)'))
     arguments: Optional[Mapping[str, Any]] = None
     enabled: bool = True
 
 
 @dataclass
 class ModelGroup:
     models: Sequence[ModelFunction]
@@ -77,4004 +74,3868 @@
     readout_electronics: Optional[Sequence[ModelFunction]] = None
     data_processing: Optional[Sequence[ModelFunction]] = None
 
 
 #
 # Model: Photon Collection / Illumination
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonCollectionIlluminationArguments(Mapping[str, Any]):
     level: float = field(
-        metadata=schema(title="level", description="Flux of photon per pixel.")
+        metadata=schema(
+            title='level'
+            ,description='Flux of photon per pixel.'
+        )
     )
-    option: Literal["uniform", "rectangular", "elliptic"] = field(
-        default="uniform",
+    option: Literal['uniform', 'rectangular', 'elliptic'] = field(
+        default='uniform',
         metadata=schema(
-            title="option",
-            description=(
-                "A string indicating the type of illumination: - ``uniform`` Uniformly"
-                "fill the entire array with photon. (Default) - ``elliptic`` Mask with"
-                "elliptic object. - ``rectangular`` Mask with rectangular object."
-            ),
-        ),
+            title='option'
+            ,description=(
+                    'A string indicating the type of illumination: - ``uniform`` Uniformly'
+                    'fill the entire array with photon. (Default) - ``elliptic`` Mask with'
+                    'elliptic object. - ``rectangular`` Mask with rectangular object.'
+                )
+        )
     )
     object_size: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title="object_size",
-            description=(
-                "List or tuple of length 2, integers defining the diameters of the"
-                "elliptic or rectangular object in vertical and horizontal directions."
-            ),
-        ),
+            title='object_size'
+            ,description=(
+                    'List or tuple of length 2, integers defining the diameters of the'
+                    'elliptic or rectangular object in vertical and horizontal directions.'
+                )
+        )
     )
     object_center: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title="object_center",
-            description=(
-                "List or tuple of length 2, two integers (row and column number),"
-                "defining the coordinates of the center of the elliptic or rectangular"
-                "object."
-            ),
-        ),
+            title='object_center'
+            ,description=(
+                    'List or tuple of length 2, two integers (row and column number),'
+                    'defining the coordinates of the center of the elliptic or rectangular'
+                    'object.'
+                )
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
-        ),
+            title='time_scale'
+            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("level", "option", "object_size", "object_center", "time_scale"))
-
+        return iter(('level', 'option', 'object_size', 'object_center', 'time_scale'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'illumination'",
-    description=(
-        "Generate photon uniformly over the entire array or over an elliptic or"
-        "rectangular object."
-    ),
+    title="Model 'illumination'"
+    ,description=(
+        'Generate photon uniformly over the entire array or over an elliptic or'
+        'rectangular object.'
+    )
 )
 @dataclass
 class ModelPhotonCollectionIllumination:
     name: str
     arguments: ModelPhotonCollectionIlluminationArguments
-    func: Literal[
-        "pyxel.models.photon_collection.illumination"
-    ] = "pyxel.models.photon_collection.illumination"
+    func: Literal['pyxel.models.photon_collection.illumination'] = 'pyxel.models.photon_collection.illumination'
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Load Image
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonCollectionLoadImageArguments(Mapping[str, Any]):
     image_file: str = field(
-        metadata=schema(title="image_file", description="Path to image file.")
+        metadata=schema(
+            title='image_file'
+            ,description='Path to image file.'
+        )
     )
     position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="position",
-            description=(
-                "Indices of starting row and column, used when fitting image to"
-                "detector."
-            ),
-        ),
+            title='position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting image to'
+                    'detector.'
+                )
+        )
     )
-    align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="align",
-            description=(
-                'Keyword to align the image to detector. Can be any from: ("center",'
-                '"top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='align'
+            ,description=(
+                    'Keyword to align the image to detector. Can be any from: ("center",'
+                    '"top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
     )
     convert_to_photons: bool = field(
         default=False,
         metadata=schema(
-            title="convert_to_photons",
-            description=(
-                "If ``True``, the model converts the values of loaded image array from"
-                "ADU to photon numbers for each pixel using the Photon Transfer"
-                "Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot"
-                "\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot"
-                "\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`."
-            ),
-        ),
+            title='convert_to_photons'
+            ,description=(
+                    'If ``True``, the model converts the values of loaded image array from'
+                    'ADU to photon numbers for each pixel using the Photon Transfer'
+                    'Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot'
+                    '\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot'
+                    '\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`.'
+                )
+        )
     )
     multiplier: float = field(
         default=1.0,
         metadata=schema(
-            title="multiplier",
-            description="Multiply photon array level with a custom number.",
-        ),
+            title='multiplier'
+            ,description='Multiply photon array level with a custom number.'
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
-        ),
+            title='time_scale'
+            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
+        )
     )
     bit_resolution: Optional[int] = field(
         default=None,
         metadata=schema(
-            title="bit_resolution", description="Bit resolution of the loaded image."
-        ),
+            title='bit_resolution'
+            ,description='Bit resolution of the loaded image.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "image_file",
-                "position",
-                "align",
-                "convert_to_photons",
-                "multiplier",
-                "time_scale",
-                "bit_resolution",
-            )
-        )
-
+        return iter(('image_file', 'position', 'align', 'convert_to_photons', 'multiplier', 'time_scale', 'bit_resolution'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 7
 
 
 @schema(
-    title="Model 'load_image'",
-    description=(
-        "Load :term:`FITS` file as a numpy array and add to the detector as"
-        "input image."
-    ),
+    title="Model 'load_image'"
+    ,description=(
+        'Load :term:`FITS` file as a numpy array and add to the detector as'
+        'input image.'
+    )
 )
 @dataclass
 class ModelPhotonCollectionLoadImage:
     name: str
     arguments: ModelPhotonCollectionLoadImageArguments
-    func: Literal[
-        "pyxel.models.photon_collection.load_image"
-    ] = "pyxel.models.photon_collection.load_image"
+    func: Literal['pyxel.models.photon_collection.load_image'] = 'pyxel.models.photon_collection.load_image'
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Load Psf
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonCollectionLoadPsfArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
         metadata=schema(
-            title="filename", description="Input filename of the point spread function."
+            title='filename'
+            ,description='Input filename of the point spread function.'
         )
     )
     normalize_kernel: bool = field(
         default=True,
-        metadata=schema(title="normalize_kernel", description="Normalize kernel."),
+        metadata=schema(
+            title='normalize_kernel'
+            ,description='Normalize kernel.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("filename", "normalize_kernel"))
-
+        return iter(('filename', 'normalize_kernel'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'load_psf'",
-    description=(
-        "Load a point spread function from file and convolve the photon array"
-        "with the PSF."
-    ),
+    title="Model 'load_psf'"
+    ,description=(
+        'Load a point spread function from file and convolve the photon array'
+        'with the PSF.'
+    )
 )
 @dataclass
 class ModelPhotonCollectionLoadPsf:
     name: str
     arguments: ModelPhotonCollectionLoadPsfArguments
-    func: Literal[
-        "pyxel.models.photon_collection.load_psf"
-    ] = "pyxel.models.photon_collection.load_psf"
+    func: Literal['pyxel.models.photon_collection.load_psf'] = 'pyxel.models.photon_collection.load_psf'
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Optical Psf
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonCollectionOpticalPsfArguments(Mapping[str, Any]):
     wavelength: float = field(
         metadata=schema(
-            title="wavelength", description="Wavelength of incoming light in meters."
+            title='wavelength'
+            ,description='Wavelength of incoming light in meters.'
         )
     )
     fov_arcsec: float = field(
         metadata=schema(
-            title="fov_arcsec", description="Field Of View on detector plane in arcsec."
+            title='fov_arcsec'
+            ,description='Field Of View on detector plane in arcsec.'
         )
     )
     pixelscale: float = field(
         metadata=schema(
-            title="pixelscale",
-            description=(
-                "Pixel scale on detector plane (arcsec/pixel). Defines sampling"
-                "resolution of :term:`PSF`."
-            ),
+            title='pixelscale'
+            ,description=(
+                    'Pixel scale on detector plane (arcsec/pixel). Defines sampling'
+                    'resolution of :term:`PSF`.'
+                )
         )
     )
     optical_system: collections.abc.Sequence[collections.abc.Mapping[str, Any]] = field(
         metadata=schema(
-            title="optical_system",
-            description=(
-                "List of optical elements before detector with their specific"
-                "arguments."
-            ),
+            title='optical_system'
+            ,description=(
+                    'List of optical elements before detector with their specific'
+                    'arguments.'
+                )
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("wavelength", "fov_arcsec", "pixelscale", "optical_system"))
-
+        return iter(('wavelength', 'fov_arcsec', 'pixelscale', 'optical_system'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'optical_psf'",
-    description="Model function for poppy optics model: convolve photon array with psf.",
+    title="Model 'optical_psf'"
+    ,description='Model function for poppy optics model: convolve photon array with psf.'
 )
 @dataclass
 class ModelPhotonCollectionOpticalPsf:
     name: str
     arguments: ModelPhotonCollectionOpticalPsfArguments
-    func: Literal[
-        "pyxel.models.photon_collection.optical_psf"
-    ] = "pyxel.models.photon_collection.optical_psf"
+    func: Literal['pyxel.models.photon_collection.optical_psf'] = 'pyxel.models.photon_collection.optical_psf'
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Shot Noise
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonCollectionShotNoiseArguments(Mapping[str, Any]):
-    type: Literal["poisson", "normal"] = field(
-        default="poisson",
+    type: Literal['poisson', 'normal'] = field(
+        default='poisson',
         metadata=schema(
-            title="type",
-            description="Choose either 'poisson' or 'normal'. Default is Poisson noise.",
-        ),
+            title='type'
+            ,description="Choose either 'poisson' or 'normal'. Default is Poisson noise."
+        )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("type", "seed"))
-
+        return iter(('type', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'shot_noise'",
-    description=(
-        "Add shot noise to the flux of photon per pixel. It can be either"
-        "Poisson noise or Gaussian."
-    ),
+    title="Model 'shot_noise'"
+    ,description=(
+        'Add shot noise to the flux of photon per pixel. It can be either'
+        'Poisson noise or Gaussian.'
+    )
 )
 @dataclass
 class ModelPhotonCollectionShotNoise:
     name: str
-    arguments: ModelPhotonCollectionShotNoiseArguments = field(
-        default_factory=ModelPhotonCollectionShotNoiseArguments
-    )
-    func: Literal[
-        "pyxel.models.photon_collection.shot_noise"
-    ] = "pyxel.models.photon_collection.shot_noise"
+    arguments: ModelPhotonCollectionShotNoiseArguments = field(default_factory=ModelPhotonCollectionShotNoiseArguments)
+    func: Literal['pyxel.models.photon_collection.shot_noise'] = 'pyxel.models.photon_collection.shot_noise'
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Stripe Pattern
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonCollectionStripePatternArguments(Mapping[str, Any]):
     period: int = field(
         default=10,
         metadata=schema(
-            title="period", description="Period of the periodic pattern in pixels."
-        ),
+            title='period'
+            ,description='Period of the periodic pattern in pixels.'
+        )
     )
     level: float = field(
         default=1.0,
         metadata=schema(
-            title="level", description="Amplitude of the periodic pattern."
-        ),
+            title='level'
+            ,description='Amplitude of the periodic pattern.'
+        )
     )
     angle: int = field(
         default=0,
-        metadata=schema(title="angle", description="Angle of the pattern in degrees."),
+        metadata=schema(
+            title='angle'
+            ,description='Angle of the pattern in degrees.'
+        )
     )
     startwith: int = field(
         default=0,
         metadata=schema(
-            title="startwith", description="1 to start with high level or 0 for 0."
-        ),
+            title='startwith'
+            ,description='1 to start with high level or 0 for 0.'
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
-        ),
+            title='time_scale'
+            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("period", "level", "angle", "startwith", "time_scale"))
-
+        return iter(('period', 'level', 'angle', 'startwith', 'time_scale'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
-@schema(title="Model 'stripe_pattern'", description="Stripe pattern model.")
+@schema(
+    title="Model 'stripe_pattern'"
+    ,description='Stripe pattern model.'
+)
 @dataclass
 class ModelPhotonCollectionStripePattern:
     name: str
-    arguments: ModelPhotonCollectionStripePatternArguments = field(
-        default_factory=ModelPhotonCollectionStripePatternArguments
+    arguments: ModelPhotonCollectionStripePatternArguments = field(default_factory=ModelPhotonCollectionStripePatternArguments)
+    func: Literal['pyxel.models.photon_collection.stripe_pattern'] = 'pyxel.models.photon_collection.stripe_pattern'
+    enabled: bool = True
+
+
+#
+# Model: Photon Collection / Wavelength Dependence Airs
+#
+@schema(title='Parameters')
+@dataclass
+class ModelPhotonCollectionWavelengthDependenceAirsArguments(Mapping[str, Any]):
+    psf_filename: str = field(
+        metadata=schema(
+            title='psf_filename'
+            ,description='The location and the filename where the PSFs are located.'
+        )
+    )
+    target_filename: str = field(
+        metadata=schema(
+            title='target_filename'
+            ,description=(
+                    'The location and the filename of the target file used in the'
+                    'simulation.'
+                )
+        )
+    )
+    telescope_diameter_m1: float = field(
+        metadata=schema(
+            title='telescope_diameter_m1'
+            ,description='Diameter of the M1 mirror of the TA in m.'
+        )
+    )
+    telescope_diameter_m2: float = field(
+        metadata=schema(
+            title='telescope_diameter_m2'
+            ,description='Diameter of the M2 mirror of the TA in m.'
+        )
+    )
+    expand_factor: int = field(
+        metadata=schema(
+            title='expand_factor'
+            ,description='Expansion factor used.'
+        )
+    )
+    time_scale: float = field(
+        default=1.0,
+        metadata=schema(
+            title='time_scale'
+            ,description='Time scale in seconds.'
+        )
     )
-    func: Literal[
-        "pyxel.models.photon_collection.stripe_pattern"
-    ] = "pyxel.models.photon_collection.stripe_pattern"
+    def __iter__(self) -> Iterator[str]:
+        return iter(('psf_filename', 'target_filename', 'telescope_diameter_m1', 'telescope_diameter_m2', 'expand_factor', 'time_scale'))
+    def __getitem__(self, item: Any) -> Any:
+        if item in tuple(self):
+            return getattr(self, item)
+        else:
+            raise KeyError
+    def __len__(self) -> int:
+        return 6
+
+
+@schema(
+    title="Model 'wavelength_dependence_airs'"
+    ,description=(
+        'Generate the photon over the array according to a specific dispersion'
+        'pattern (ARIEL-AIRS).'
+    )
+)
+@dataclass
+class ModelPhotonCollectionWavelengthDependenceAirs:
+    name: str
+    arguments: ModelPhotonCollectionWavelengthDependenceAirsArguments
+    func: Literal['pyxel.models.photon_collection.wavelength_dependence_airs'] = 'pyxel.models.photon_collection.wavelength_dependence_airs'
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Illumination
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonGenerationIlluminationArguments(Mapping[str, Any]):
     level: float = field(
-        metadata=schema(title="level", description="Flux of photon per pixel.")
+        metadata=schema(
+            title='level'
+            ,description='Flux of photon per pixel.'
+        )
     )
-    option: Literal["uniform", "rectangular", "elliptic"] = field(
-        default="uniform",
+    option: Literal['uniform', 'rectangular', 'elliptic'] = field(
+        default='uniform',
         metadata=schema(
-            title="option",
-            description=(
-                "A string indicating the type of illumination: - ``uniform`` Uniformly"
-                "fill the entire array with photon. (Default) - ``elliptic`` Mask with"
-                "elliptic object. - ``rectangular`` Mask with rectangular object."
-            ),
-        ),
+            title='option'
+            ,description=(
+                    'A string indicating the type of illumination: - ``uniform`` Uniformly'
+                    'fill the entire array with photon. (Default) - ``elliptic`` Mask with'
+                    'elliptic object. - ``rectangular`` Mask with rectangular object.'
+                )
+        )
     )
     object_size: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title="object_size",
-            description=(
-                "List or tuple of length 2, integers defining the diameters of the"
-                "elliptic or rectangular object in vertical and horizontal directions."
-            ),
-        ),
+            title='object_size'
+            ,description=(
+                    'List or tuple of length 2, integers defining the diameters of the'
+                    'elliptic or rectangular object in vertical and horizontal directions.'
+                )
+        )
     )
     object_center: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title="object_center",
-            description=(
-                "List or tuple of length 2, two integers (row and column number),"
-                "defining the coordinates of the center of the elliptic or rectangular"
-                "object."
-            ),
-        ),
+            title='object_center'
+            ,description=(
+                    'List or tuple of length 2, two integers (row and column number),'
+                    'defining the coordinates of the center of the elliptic or rectangular'
+                    'object.'
+                )
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
-        ),
+            title='time_scale'
+            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("level", "option", "object_size", "object_center", "time_scale"))
-
+        return iter(('level', 'option', 'object_size', 'object_center', 'time_scale'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'illumination'",
-    description=(
-        "Generate photon uniformly over the entire array or over an elliptic or"
-        "rectangular object."
-    ),
+    title="Model 'illumination'"
+    ,description=(
+        'Generate photon uniformly over the entire array or over an elliptic or'
+        'rectangular object.'
+    )
 )
 @dataclass
 class ModelPhotonGenerationIllumination:
     name: str
     arguments: ModelPhotonGenerationIlluminationArguments
-    func: Literal[
-        "pyxel.models.photon_generation.illumination"
-    ] = "pyxel.models.photon_generation.illumination"
+    func: Literal['pyxel.models.photon_generation.illumination'] = 'pyxel.models.photon_generation.illumination'
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Load Image
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonGenerationLoadImageArguments(Mapping[str, Any]):
     image_file: str = field(
-        metadata=schema(title="image_file", description="Path to image file.")
+        metadata=schema(
+            title='image_file'
+            ,description='Path to image file.'
+        )
     )
     position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="position",
-            description=(
-                "Indices of starting row and column, used when fitting image to"
-                "detector."
-            ),
-        ),
+            title='position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting image to'
+                    'detector.'
+                )
+        )
     )
-    align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="align",
-            description=(
-                'Keyword to align the image to detector. Can be any from: ("center",'
-                '"top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='align'
+            ,description=(
+                    'Keyword to align the image to detector. Can be any from: ("center",'
+                    '"top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
     )
     convert_to_photons: bool = field(
         default=False,
         metadata=schema(
-            title="convert_to_photons",
-            description=(
-                "If ``True``, the model converts the values of loaded image array from"
-                "ADU to photon numbers for each pixel using the Photon Transfer"
-                "Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot"
-                "\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot"
-                "\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`."
-            ),
-        ),
+            title='convert_to_photons'
+            ,description=(
+                    'If ``True``, the model converts the values of loaded image array from'
+                    'ADU to photon numbers for each pixel using the Photon Transfer'
+                    'Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot'
+                    '\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot'
+                    '\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`.'
+                )
+        )
     )
     multiplier: float = field(
         default=1.0,
         metadata=schema(
-            title="multiplier",
-            description="Multiply photon array level with a custom number.",
-        ),
+            title='multiplier'
+            ,description='Multiply photon array level with a custom number.'
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
-        ),
+            title='time_scale'
+            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
+        )
     )
     bit_resolution: Optional[int] = field(
         default=None,
         metadata=schema(
-            title="bit_resolution", description="Bit resolution of the loaded image."
-        ),
+            title='bit_resolution'
+            ,description='Bit resolution of the loaded image.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "image_file",
-                "position",
-                "align",
-                "convert_to_photons",
-                "multiplier",
-                "time_scale",
-                "bit_resolution",
-            )
-        )
-
+        return iter(('image_file', 'position', 'align', 'convert_to_photons', 'multiplier', 'time_scale', 'bit_resolution'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 7
 
 
 @schema(
-    title="Model 'load_image'",
-    description=(
-        "Load :term:`FITS` file as a numpy array and add to the detector as"
-        "input image."
-    ),
+    title="Model 'load_image'"
+    ,description=(
+        'Load :term:`FITS` file as a numpy array and add to the detector as'
+        'input image.'
+    )
 )
 @dataclass
 class ModelPhotonGenerationLoadImage:
     name: str
     arguments: ModelPhotonGenerationLoadImageArguments
-    func: Literal[
-        "pyxel.models.photon_generation.load_image"
-    ] = "pyxel.models.photon_generation.load_image"
+    func: Literal['pyxel.models.photon_generation.load_image'] = 'pyxel.models.photon_generation.load_image'
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Shot Noise
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonGenerationShotNoiseArguments(Mapping[str, Any]):
-    type: Literal["poisson", "normal"] = field(
-        default="poisson",
+    type: Literal['poisson', 'normal'] = field(
+        default='poisson',
         metadata=schema(
-            title="type",
-            description="Choose either 'poisson' or 'normal'. Default is Poisson noise.",
-        ),
+            title='type'
+            ,description="Choose either 'poisson' or 'normal'. Default is Poisson noise."
+        )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("type", "seed"))
-
+        return iter(('type', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'shot_noise'",
-    description=(
-        "Add shot noise to the flux of photon per pixel. It can be either"
-        "Poisson noise or Gaussian."
-    ),
+    title="Model 'shot_noise'"
+    ,description=(
+        'Add shot noise to the flux of photon per pixel. It can be either'
+        'Poisson noise or Gaussian.'
+    )
 )
 @dataclass
 class ModelPhotonGenerationShotNoise:
     name: str
-    arguments: ModelPhotonGenerationShotNoiseArguments = field(
-        default_factory=ModelPhotonGenerationShotNoiseArguments
-    )
-    func: Literal[
-        "pyxel.models.photon_generation.shot_noise"
-    ] = "pyxel.models.photon_generation.shot_noise"
+    arguments: ModelPhotonGenerationShotNoiseArguments = field(default_factory=ModelPhotonGenerationShotNoiseArguments)
+    func: Literal['pyxel.models.photon_generation.shot_noise'] = 'pyxel.models.photon_generation.shot_noise'
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Stripe Pattern
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhotonGenerationStripePatternArguments(Mapping[str, Any]):
     period: int = field(
         default=10,
         metadata=schema(
-            title="period", description="Period of the periodic pattern in pixels."
-        ),
+            title='period'
+            ,description='Period of the periodic pattern in pixels.'
+        )
     )
     level: float = field(
         default=1.0,
         metadata=schema(
-            title="level", description="Amplitude of the periodic pattern."
-        ),
+            title='level'
+            ,description='Amplitude of the periodic pattern.'
+        )
     )
     angle: int = field(
         default=0,
-        metadata=schema(title="angle", description="Angle of the pattern in degrees."),
+        metadata=schema(
+            title='angle'
+            ,description='Angle of the pattern in degrees.'
+        )
     )
     startwith: int = field(
         default=0,
         metadata=schema(
-            title="startwith", description="1 to start with high level or 0 for 0."
-        ),
+            title='startwith'
+            ,description='1 to start with high level or 0 for 0.'
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
-        ),
+            title='time_scale'
+            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("period", "level", "angle", "startwith", "time_scale"))
-
+        return iter(('period', 'level', 'angle', 'startwith', 'time_scale'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
-@schema(title="Model 'stripe_pattern'", description="Stripe pattern model.")
+@schema(
+    title="Model 'stripe_pattern'"
+    ,description='Stripe pattern model.'
+)
 @dataclass
 class ModelPhotonGenerationStripePattern:
     name: str
-    arguments: ModelPhotonGenerationStripePatternArguments = field(
-        default_factory=ModelPhotonGenerationStripePatternArguments
-    )
-    func: Literal[
-        "pyxel.models.photon_generation.stripe_pattern"
-    ] = "pyxel.models.photon_generation.stripe_pattern"
+    arguments: ModelPhotonGenerationStripePatternArguments = field(default_factory=ModelPhotonGenerationStripePatternArguments)
+    func: Literal['pyxel.models.photon_generation.stripe_pattern'] = 'pyxel.models.photon_generation.stripe_pattern'
     enabled: bool = True
 
 
 #
 # Model: Optics / Load Psf
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelOpticsLoadPsfArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
         metadata=schema(
-            title="filename", description="Input filename of the point spread function."
+            title='filename'
+            ,description='Input filename of the point spread function.'
         )
     )
     normalize_kernel: bool = field(
         default=True,
-        metadata=schema(title="normalize_kernel", description="Normalize kernel."),
+        metadata=schema(
+            title='normalize_kernel'
+            ,description='Normalize kernel.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("filename", "normalize_kernel"))
-
+        return iter(('filename', 'normalize_kernel'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'load_psf'",
-    description=(
-        "Load a point spread function from file and convolve the photon array"
-        "with the PSF."
-    ),
+    title="Model 'load_psf'"
+    ,description=(
+        'Load a point spread function from file and convolve the photon array'
+        'with the PSF.'
+    )
 )
 @dataclass
 class ModelOpticsLoadPsf:
     name: str
     arguments: ModelOpticsLoadPsfArguments
-    func: Literal["pyxel.models.optics.load_psf"] = "pyxel.models.optics.load_psf"
+    func: Literal['pyxel.models.optics.load_psf'] = 'pyxel.models.optics.load_psf'
     enabled: bool = True
 
 
 #
 # Model: Optics / Optical Psf
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelOpticsOpticalPsfArguments(Mapping[str, Any]):
     wavelength: float = field(
         metadata=schema(
-            title="wavelength", description="Wavelength of incoming light in meters."
+            title='wavelength'
+            ,description='Wavelength of incoming light in meters.'
         )
     )
     fov_arcsec: float = field(
         metadata=schema(
-            title="fov_arcsec", description="Field Of View on detector plane in arcsec."
+            title='fov_arcsec'
+            ,description='Field Of View on detector plane in arcsec.'
         )
     )
     pixelscale: float = field(
         metadata=schema(
-            title="pixelscale",
-            description=(
-                "Pixel scale on detector plane (arcsec/pixel). Defines sampling"
-                "resolution of :term:`PSF`."
-            ),
+            title='pixelscale'
+            ,description=(
+                    'Pixel scale on detector plane (arcsec/pixel). Defines sampling'
+                    'resolution of :term:`PSF`.'
+                )
         )
     )
     optical_system: collections.abc.Sequence[collections.abc.Mapping[str, Any]] = field(
         metadata=schema(
-            title="optical_system",
-            description=(
-                "List of optical elements before detector with their specific"
-                "arguments."
-            ),
+            title='optical_system'
+            ,description=(
+                    'List of optical elements before detector with their specific'
+                    'arguments.'
+                )
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("wavelength", "fov_arcsec", "pixelscale", "optical_system"))
-
+        return iter(('wavelength', 'fov_arcsec', 'pixelscale', 'optical_system'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'optical_psf'",
-    description="Model function for poppy optics model: convolve photon array with psf.",
+    title="Model 'optical_psf'"
+    ,description='Model function for poppy optics model: convolve photon array with psf.'
 )
 @dataclass
 class ModelOpticsOpticalPsf:
     name: str
     arguments: ModelOpticsOpticalPsfArguments
-    func: Literal["pyxel.models.optics.optical_psf"] = "pyxel.models.optics.optical_psf"
+    func: Literal['pyxel.models.optics.optical_psf'] = 'pyxel.models.optics.optical_psf'
     enabled: bool = True
 
 
 #
 # Model: Phasing / Pulse Processing
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelPhasingPulseProcessingArguments(Mapping[str, Any]):
     wavelength: float = field(
-        metadata=schema(title="wavelength", description="Wavelength.")
+        metadata=schema(
+            title='wavelength'
+            ,description='Wavelength.'
+        )
     )
     responsivity: float = field(
-        metadata=schema(title="responsivity", description="Responsivity of the pixel.")
+        metadata=schema(
+            title='responsivity'
+            ,description='Responsivity of the pixel.'
+        )
     )
     scaling_factor: float = field(
         default=250.0,
         metadata=schema(
-            title="scaling_factor",
-            description=(
-                "Scaling factor taking into account the missing pieces of"
-                "superconducting physics, as well as the resonator quality factor, the"
-                "bias power, the quasi-particle losses, etc."
-            ),
-        ),
+            title='scaling_factor'
+            ,description=(
+                    'Scaling factor taking into account the missing pieces of'
+                    'superconducting physics, as well as the resonator quality factor, the'
+                    'bias power, the quasi-particle losses, etc.'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("wavelength", "responsivity", "scaling_factor"))
-
+        return iter(('wavelength', 'responsivity', 'scaling_factor'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
-@schema(title="Model 'pulse_processing'", description="TBW.")
+@schema(
+    title="Model 'pulse_processing'"
+    ,description='TBW.'
+)
 @dataclass
 class ModelPhasingPulseProcessing:
     name: str
     arguments: ModelPhasingPulseProcessingArguments
-    func: Literal[
-        "pyxel.models.phasing.pulse_processing"
-    ] = "pyxel.models.phasing.pulse_processing"
+    func: Literal['pyxel.models.phasing.pulse_processing'] = 'pyxel.models.phasing.pulse_processing'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Apd Gain
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationApdGainArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
-
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 0
 
 
-@schema(title="Model 'apd_gain'", description="Apply APD gain.")
+@schema(
+    title="Model 'apd_gain'"
+    ,description='Apply APD gain.'
+)
 @dataclass
 class ModelChargeGenerationApdGain:
     name: str
-    arguments: ModelChargeGenerationApdGainArguments = field(
-        default_factory=ModelChargeGenerationApdGainArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_generation.apd_gain"
-    ] = "pyxel.models.charge_generation.apd_gain"
+    arguments: ModelChargeGenerationApdGainArguments = field(default_factory=ModelChargeGenerationApdGainArguments)
+    func: Literal['pyxel.models.charge_generation.apd_gain'] = 'pyxel.models.charge_generation.apd_gain'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Charge Blocks
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationChargeBlocksArguments(Mapping[str, Any]):
     charge_level: float = field(
-        metadata=schema(title="charge_level", description="Value of charges.")
+        metadata=schema(
+            title='charge_level'
+            ,description='Value of charges.'
+        )
     )
     block_start: int = field(
         default=0,
         metadata=schema(
-            title="block_start", description="Starting row of the injected charge."
-        ),
+            title='block_start'
+            ,description='Starting row of the injected charge.'
+        )
     )
     block_end: Optional[int] = field(
         default=None,
         metadata=schema(
-            title="block_end", description="Ending row for the injected charge."
-        ),
+            title='block_end'
+            ,description='Ending row for the injected charge.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("charge_level", "block_start", "block_end"))
-
+        return iter(('charge_level', 'block_start', 'block_end'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'charge_blocks'",
-    description="Inject a block of charge into the :term:`CCD` detector.",
+    title="Model 'charge_blocks'"
+    ,description='Inject a block of charge into the :term:`CCD` detector.'
 )
 @dataclass
 class ModelChargeGenerationChargeBlocks:
     name: str
     arguments: ModelChargeGenerationChargeBlocksArguments
-    func: Literal[
-        "pyxel.models.charge_generation.charge_blocks"
-    ] = "pyxel.models.charge_generation.charge_blocks"
+    func: Literal['pyxel.models.charge_generation.charge_blocks'] = 'pyxel.models.charge_generation.charge_blocks'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Charge Deposition
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationChargeDepositionArguments(Mapping[str, Any]):
     flux: float = field(
         metadata=schema(
-            title="flux", description="the flux of incoming particles in particle/s"
+            title='flux'
+            ,description='the flux of incoming particles in particle/s'
         )
     )
     step_size: float = field(
         default=1.0,
         metadata=schema(
-            title="step_size",
-            description=(
-                "the size of the considered unitary step in unit length along which"
-                "energy is deposited"
-            ),
-        ),
+            title='step_size'
+            ,description=(
+                    'the size of the considered unitary step in unit length along which'
+                    'energy is deposited'
+                )
+        )
     )
     energy_mean: float = field(
         default=1.0,
         metadata=schema(
-            title="energy_mean",
-            description="the mean energy of the incoming ionizing particles in MeV",
-        ),
+            title='energy_mean'
+            ,description='the mean energy of the incoming ionizing particles in MeV'
+        )
     )
     energy_spread: float = field(
         default=0.1,
         metadata=schema(
-            title="energy_spread",
-            description="the spread in energy of the incoming ionizing particles in MeV",
-        ),
+            title='energy_spread'
+            ,description='the spread in energy of the incoming ionizing particles in MeV'
+        )
     )
     energy_spectrum: Union[str, pathlib.Path, None] = field(
         default=None,
         metadata=schema(
-            title="energy_spectrum",
-            description=(
-                "the location of the file describing the energy spectrum of incident"
-                "particles if no spectrum is provided energies are randomly drawn from"
-                "a normal distribution with mean and spread defined above note that the"
-                "energy spectrum is assumed to be a txt file with two columns [energy,"
-                "flux] with the energy in MeV"
-            ),
-        ),
-    )
-    energy_spectrum_sampling: Literal["linear", "log"] = field(
-        default="log",
-        metadata=schema(
-            title="energy_spectrum_sampling",
-            description=(
-                '"log" or None: the energy spectrum is sampled in log space "linear" :'
-                "the energy spectrum is sampled in linear space"
-            ),
-        ),
+            title='energy_spectrum'
+            ,description=(
+                    'the location of the file describing the energy spectrum of incident'
+                    'particles if no spectrum is provided energies are randomly drawn from'
+                    'a normal distribution with mean and spread defined above note that the'
+                    'energy spectrum is assumed to be a txt file with two columns [energy,'
+                    'flux] with the energy in MeV'
+                )
+        )
+    )
+    energy_spectrum_sampling: Literal['linear', 'log'] = field(
+        default='log',
+        metadata=schema(
+            title='energy_spectrum_sampling'
+            ,description=(
+                    '"log" or None: the energy spectrum is sampled in log space "linear" :'
+                    'the energy spectrum is sampled in linear space'
+                )
+        )
     )
     ehpair_creation: float = field(
         default=3.65,
         metadata=schema(
-            title="ehpair_creation",
-            description=(
-                "the energy required to generate a electron-hole pair in eV by default"
-                "the Si value at room temperature is parsed i.e. 3.65 eV"
-            ),
-        ),
+            title='ehpair_creation'
+            ,description=(
+                    'the energy required to generate a electron-hole pair in eV by default'
+                    'the Si value at room temperature is parsed i.e. 3.65 eV'
+                )
+        )
     )
     material_density: float = field(
         default=2.329,
         metadata=schema(
-            title="material_density",
-            description=(
-                "the material density in g/cm3 by default he Si value at room"
-                "temperature is parsed i.e. 2.3290 g/cm3"
-            ),
-        ),
+            title='material_density'
+            ,description=(
+                    'the material density in g/cm3 by default he Si value at room'
+                    'temperature is parsed i.e. 2.3290 g/cm3'
+                )
+        )
+    )
+    particle_direction: Literal['isotropic', 'orthogonal'] = field(
+        default='isotropic',
+        metadata=schema(
+            title='particle_direction'
+            ,description=(
+                    '"isotropic" : particles are coming from all directions (outside of the'
+                    'sensor) "orthogonal" : particles are coming from the top of the sensor'
+                    '(thickness = 0) and orthogonal to its surface'
+                )
+        )
     )
-    particle_direction: Literal["isotropic", "orthogonal"] = field(
-        default="isotropic",
+    stopping_power_curve: Union[str, pathlib.Path, None] = field(
+        default=None,
         metadata=schema(
-            title="particle_direction",
-            description=(
-                '"isotropic" : particles are coming from all directions (outside of the'
-                'sensor) "orthogonal" : particles are coming from the top of the sensor'
-                "(thickness = 0) and orthogonal to its surface"
-            ),
-        ),
+            title='stopping_power_curve'
+            ,description=(
+                    'the location of the file describing the total massive stopping power'
+                    'energetic loss per mass of material and per unit path length versus'
+                    'particle energy note that the the stopping power curve is assumed to'
+                    'be a csv file with two columns [energy, stopping power] energy in MeV,'
+                    'stopping power in MeV cm2/g'
+                )
+        )
     )
-    stopping_power_curve: Union[str, pathlib.Path, None] = field(
+    seed: Optional[int] = field(
         default=None,
         metadata=schema(
-            title="stopping_power_curve",
-            description=(
-                "the location of the file describing the total massive stopping power"
-                "energetic loss per mass of material and per unit path length versus"
-                "particle energy note that the the stopping power curve is assumed to"
-                "be a csv file with two columns [energy, stopping power] energy in MeV,"
-                "stopping power in MeV cm2/g"
-            ),
-        ),
-    )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "flux",
-                "step_size",
-                "energy_mean",
-                "energy_spread",
-                "energy_spectrum",
-                "energy_spectrum_sampling",
-                "ehpair_creation",
-                "material_density",
-                "particle_direction",
-                "stopping_power_curve",
-                "seed",
-            )
+            title='seed'
         )
-
+    )
+    def __iter__(self) -> Iterator[str]:
+        return iter(('flux', 'step_size', 'energy_mean', 'energy_spread', 'energy_spectrum', 'energy_spectrum_sampling', 'ehpair_creation', 'material_density', 'particle_direction', 'stopping_power_curve', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 11
 
 
 @schema(
-    title="Model 'charge_deposition'",
-    description=(
-        "Simulate charge deposition by ionizing particles using a stopping"
-        "power curve."
-    ),
+    title="Model 'charge_deposition'"
+    ,description=(
+        'Simulate charge deposition by ionizing particles using a stopping'
+        'power curve.'
+    )
 )
 @dataclass
 class ModelChargeGenerationChargeDeposition:
     name: str
     arguments: ModelChargeGenerationChargeDepositionArguments
-    func: Literal[
-        "pyxel.models.charge_generation.charge_deposition"
-    ] = "pyxel.models.charge_generation.charge_deposition"
+    func: Literal['pyxel.models.charge_generation.charge_deposition'] = 'pyxel.models.charge_generation.charge_deposition'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Charge Deposition In Mct
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationChargeDepositionInMctArguments(Mapping[str, Any]):
     flux: float = field(
         metadata=schema(
-            title="flux", description="the flux of incoming particles in particle/s"
+            title='flux'
+            ,description='the flux of incoming particles in particle/s'
         )
     )
     step_size: float = field(
         default=1.0,
         metadata=schema(
-            title="step_size",
-            description=(
-                "the size of the considered unitary step in unit length along which"
-                "energy is deposited"
-            ),
-        ),
+            title='step_size'
+            ,description=(
+                    'the size of the considered unitary step in unit length along which'
+                    'energy is deposited'
+                )
+        )
     )
     energy_mean: float = field(
         default=1.0,
         metadata=schema(
-            title="energy_mean",
-            description="the mean energy of the incoming ionizing particles in MeV",
-        ),
+            title='energy_mean'
+            ,description='the mean energy of the incoming ionizing particles in MeV'
+        )
     )
     energy_spread: float = field(
         default=0.1,
         metadata=schema(
-            title="energy_spread",
-            description="the spread in energy of the incoming ionizing particles in MeV",
-        ),
+            title='energy_spread'
+            ,description='the spread in energy of the incoming ionizing particles in MeV'
+        )
     )
     energy_spectrum: Union[str, pathlib.Path, None] = field(
         default=None,
         metadata=schema(
-            title="energy_spectrum",
-            description=(
-                "the location of the file describing the energy spectrum of incident"
-                "particles if no spectrum is provided energies are randomly drawn from"
-                "a normal distribution with mean and spread defined above note that the"
-                "energy spectrum is assumed to be a txt file with two columns [energy,"
-                "flux] with the energy in MeV"
-            ),
-        ),
-    )
-    energy_spectrum_sampling: Literal["linear", "log"] = field(
-        default="log",
-        metadata=schema(
-            title="energy_spectrum_sampling",
-            description=(
-                '"log" : the energy spectrum is sampled in log space "linear" : the'
-                "energy spectrum is sampled in linear space"
-            ),
-        ),
+            title='energy_spectrum'
+            ,description=(
+                    'the location of the file describing the energy spectrum of incident'
+                    'particles if no spectrum is provided energies are randomly drawn from'
+                    'a normal distribution with mean and spread defined above note that the'
+                    'energy spectrum is assumed to be a txt file with two columns [energy,'
+                    'flux] with the energy in MeV'
+                )
+        )
+    )
+    energy_spectrum_sampling: Literal['linear', 'log'] = field(
+        default='log',
+        metadata=schema(
+            title='energy_spectrum_sampling'
+            ,description=(
+                    '"log" : the energy spectrum is sampled in log space "linear" : the'
+                    'energy spectrum is sampled in linear space'
+                )
+        )
     )
     cutoff_wavelength: float = field(
         default=2.5,
         metadata=schema(
-            title="cutoff_wavelength",
-            description=(
-                "the longest wavelength in micrometer at which the QE reaches 50% of"
-                "its maximum, used to compute the bandgap energy, and the corresponding"
-                "fraction of cadmium"
-            ),
-        ),
+            title='cutoff_wavelength'
+            ,description=(
+                    'the longest wavelength in micrometer at which the QE reaches 50% of'
+                    'its maximum, used to compute the bandgap energy, and the corresponding'
+                    'fraction of cadmium'
+                )
+        )
+    )
+    particle_direction: Literal['isotropic', 'orthogonal'] = field(
+        default='isotropic',
+        metadata=schema(
+            title='particle_direction'
+            ,description=(
+                    '"isotropic" : particles are coming from all directions (outside of the'
+                    'sensor) "orthogonal" : particles are coming from the top of the sensor'
+                    '(thickness = 0) and orthogonal to its surface'
+                )
+        )
     )
-    particle_direction: Literal["isotropic", "orthogonal"] = field(
-        default="isotropic",
+    stopping_power_curve: Union[str, pathlib.Path, None] = field(
+        default=None,
         metadata=schema(
-            title="particle_direction",
-            description=(
-                '"isotropic" : particles are coming from all directions (outside of the'
-                'sensor) "orthogonal" : particles are coming from the top of the sensor'
-                "(thickness = 0) and orthogonal to its surface"
-            ),
-        ),
+            title='stopping_power_curve'
+            ,description=(
+                    'the location of the file describing the total massive stopping power'
+                    'energetic loss per mass of material and per unit path length versus'
+                    'particle energy note that the the stopping power curve is assumed to'
+                    'be a csv file with two columns [energy, stopping power] energy in MeV,'
+                    'stopping power in MeV cm2/g'
+                )
+        )
     )
-    stopping_power_curve: Union[str, pathlib.Path, None] = field(
+    seed: Optional[int] = field(
         default=None,
         metadata=schema(
-            title="stopping_power_curve",
-            description=(
-                "the location of the file describing the total massive stopping power"
-                "energetic loss per mass of material and per unit path length versus"
-                "particle energy note that the the stopping power curve is assumed to"
-                "be a csv file with two columns [energy, stopping power] energy in MeV,"
-                "stopping power in MeV cm2/g"
-            ),
-        ),
-    )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
-
-    def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "flux",
-                "step_size",
-                "energy_mean",
-                "energy_spread",
-                "energy_spectrum",
-                "energy_spectrum_sampling",
-                "cutoff_wavelength",
-                "particle_direction",
-                "stopping_power_curve",
-                "seed",
-            )
+            title='seed'
         )
-
+    )
+    def __iter__(self) -> Iterator[str]:
+        return iter(('flux', 'step_size', 'energy_mean', 'energy_spread', 'energy_spectrum', 'energy_spectrum_sampling', 'cutoff_wavelength', 'particle_direction', 'stopping_power_curve', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 10
 
 
 @schema(
-    title="Model 'charge_deposition_in_mct'",
-    description=(
-        "Simulate charge deposition by ionizing particles using a stopping"
-        "power curve."
-    ),
+    title="Model 'charge_deposition_in_mct'"
+    ,description=(
+        'Simulate charge deposition by ionizing particles using a stopping'
+        'power curve.'
+    )
 )
 @dataclass
 class ModelChargeGenerationChargeDepositionInMct:
     name: str
     arguments: ModelChargeGenerationChargeDepositionInMctArguments
-    func: Literal[
-        "pyxel.models.charge_generation.charge_deposition_in_mct"
-    ] = "pyxel.models.charge_generation.charge_deposition_in_mct"
+    func: Literal['pyxel.models.charge_generation.charge_deposition_in_mct'] = 'pyxel.models.charge_generation.charge_deposition_in_mct'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Conversion With Qe Map
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationConversionWithQeMapArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
-        metadata=schema(title="filename", description="File path.")
+        metadata=schema(
+            title='filename'
+            ,description='File path.'
+        )
     )
     position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="position",
-            description=(
-                "Indices of starting row and column, used when fitting :term:`QE` map"
-                "to detector."
-            ),
-        ),
+            title='position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting :term:`QE` map'
+                    'to detector.'
+                )
+        )
     )
-    align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="align",
-            description=(
-                "Keyword to align the :term:`QE` map to detector. Can be any from:"
-                '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='align'
+            ,description=(
+                    'Keyword to align the :term:`QE` map to detector. Can be any from:'
+                    '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
+    )
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
+        )
     )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     binomial_sampling: bool = field(
         default=True,
         metadata=schema(
-            title="binomial_sampling", description="Binomial sampling. Default is True."
-        ),
+            title='binomial_sampling'
+            ,description='Binomial sampling. Default is True.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("filename", "position", "align", "seed", "binomial_sampling"))
-
+        return iter(('filename', 'position', 'align', 'seed', 'binomial_sampling'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'conversion_with_qe_map'",
-    description=(
-        "Generate charge from incident photon via photoelectric effect, simple"
-        "model with custom :term:`QE` map."
-    ),
+    title="Model 'conversion_with_qe_map'"
+    ,description=(
+        'Generate charge from incident photon via photoelectric effect, simple'
+        'model with custom :term:`QE` map.'
+    )
 )
 @dataclass
 class ModelChargeGenerationConversionWithQeMap:
     name: str
     arguments: ModelChargeGenerationConversionWithQeMapArguments
-    func: Literal[
-        "pyxel.models.charge_generation.conversion_with_qe_map"
-    ] = "pyxel.models.charge_generation.conversion_with_qe_map"
+    func: Literal['pyxel.models.charge_generation.conversion_with_qe_map'] = 'pyxel.models.charge_generation.conversion_with_qe_map'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Cosmix
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationCosmixArguments(Mapping[str, Any]):
-    simulation_mode: Optional[
-        Literal["cosmic_ray", "cosmics", "radioactive_decay", "snowflakes"]
-    ] = field(
+    simulation_mode: Optional[Literal['cosmic_ray', 'cosmics', 'radioactive_decay', 'snowflakes']] = field(
         default=None,
         metadata=schema(
-            title="simulation_mode",
-            description="Simulation mode: ``cosmic_rays``, ``radioactive_decay``.",
-        ),
+            title='simulation_mode'
+            ,description='Simulation mode: ``cosmic_rays``, ``radioactive_decay``.'
+        )
     )
-    running_mode: Optional[
-        Literal["stopping", "stepsize", "geant4", "plotting"]
-    ] = field(
+    running_mode: Optional[Literal['stopping', 'stepsize', 'geant4', 'plotting']] = field(
         default=None,
         metadata=schema(
-            title="running_mode",
-            description="Mode: ``stopping``, ``stepsize``, ``geant4``, ``plotting``.",
-        ),
+            title='running_mode'
+            ,description='Mode: ``stopping``, ``stepsize``, ``geant4``, ``plotting``.'
+        )
     )
-    particle_type: Optional[Literal["proton", "alpha", "ion"]] = field(
+    particle_type: Optional[Literal['proton', 'alpha', 'ion']] = field(
         default=None,
         metadata=schema(
-            title="particle_type",
-            description="Type of particle: ``proton``, ``alpha``, ``ion``.",
-        ),
+            title='particle_type'
+            ,description='Type of particle: ``proton``, ``alpha``, ``ion``.'
+        )
     )
-    initial_energy: Union[int, float, Literal["random"], None] = field(
+    initial_energy: Union[int, float, Literal['random'], None] = field(
         default=None,
         metadata=schema(
-            title="initial_energy",
-            description="Kinetic energy of particle, set `random` for random.",
-        ),
+            title='initial_energy'
+            ,description='Kinetic energy of particle, set `random` for random.'
+        )
     )
     particles_per_second: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="particles_per_second", description="Number of particles per second."
-        ),
+            title='particles_per_second'
+            ,description='Number of particles per second.'
+        )
     )
     incident_angles: Optional[tuple[str, str]] = field(
         default=None,
         metadata=schema(
-            title="incident_angles", description="Incident angles: ``(α, β)``."
-        ),
+            title='incident_angles'
+            ,description='Incident angles: ``(α, β)``.'
+        )
     )
     starting_position: Optional[tuple[str, str, str]] = field(
         default=None,
         metadata=schema(
-            title="starting_position", description="Starting position: ``(x, y, z)``."
-        ),
+            title='starting_position'
+            ,description='Starting position: ``(x, y, z)``.'
+        )
     )
     spectrum_file: Optional[str] = field(
         default=None,
-        metadata=schema(title="spectrum_file", description="Path to input spectrum"),
+        metadata=schema(
+            title='spectrum_file'
+            ,description='Path to input spectrum'
+        )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
     ionization_energy: float = field(
         default=3.6,
         metadata=schema(
-            title="ionization_energy",
-            description="Mean ionization energy of the semiconductor lattice.",
-        ),
+            title='ionization_energy'
+            ,description='Mean ionization energy of the semiconductor lattice.'
+        )
     )
     progressbar: bool = field(
-        default=True, metadata=schema(title="progressbar", description="Progressbar.")
+        default=True,
+        metadata=schema(
+            title='progressbar'
+            ,description='Progressbar.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "simulation_mode",
-                "running_mode",
-                "particle_type",
-                "initial_energy",
-                "particles_per_second",
-                "incident_angles",
-                "starting_position",
-                "spectrum_file",
-                "seed",
-                "ionization_energy",
-                "progressbar",
-            )
-        )
-
+        return iter(('simulation_mode', 'running_mode', 'particle_type', 'initial_energy', 'particles_per_second', 'incident_angles', 'starting_position', 'spectrum_file', 'seed', 'ionization_energy', 'progressbar'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 11
 
 
-@schema(title="Model 'cosmix'", description="Apply CosmiX model.")
+@schema(
+    title="Model 'cosmix'"
+    ,description='Apply CosmiX model.'
+)
 @dataclass
 class ModelChargeGenerationCosmix:
     name: str
-    arguments: ModelChargeGenerationCosmixArguments = field(
-        default_factory=ModelChargeGenerationCosmixArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_generation.cosmix"
-    ] = "pyxel.models.charge_generation.cosmix"
+    arguments: ModelChargeGenerationCosmixArguments = field(default_factory=ModelChargeGenerationCosmixArguments)
+    func: Literal['pyxel.models.charge_generation.cosmix'] = 'pyxel.models.charge_generation.cosmix'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Dark Current
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationDarkCurrentArguments(Mapping[str, Any]):
     figure_of_merit: float = field(
         metadata=schema(
-            title="figure_of_merit",
-            description="Dark current figure of merit. Unit: nA/cm^2",
+            title='figure_of_merit'
+            ,description='Dark current figure of merit. Unit: nA/cm^2'
         )
     )
     spatial_noise_factor: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="spatial_noise_factor",
-            description="Dark current fixed pattern noise factor.",
-        ),
+            title='spatial_noise_factor'
+            ,description='Dark current fixed pattern noise factor.'
+        )
     )
     band_gap: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="band_gap",
-            description="Semiconductor band_gap. If none, the one for silicon is used. Unit: eV",
-        ),
+            title='band_gap'
+            ,description='Semiconductor band_gap. If none, the one for silicon is used. Unit: eV'
+        )
     )
     band_gap_room_temperature: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="band_gap_room_temperature",
-            description=(
-                "Semiconductor band gap at 300K. If none, the one for silicon is used."
-                "Unit: eV"
-            ),
-        ),
+            title='band_gap_room_temperature'
+            ,description=(
+                    'Semiconductor band gap at 300K. If none, the one for silicon is used.'
+                    'Unit: eV'
+                )
+        )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
     temporal_noise: bool = field(
-        default=True, metadata=schema(title="temporal_noise", description="Shot noise.")
+        default=True,
+        metadata=schema(
+            title='temporal_noise'
+            ,description='Shot noise.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "figure_of_merit",
-                "spatial_noise_factor",
-                "band_gap",
-                "band_gap_room_temperature",
-                "seed",
-                "temporal_noise",
-            )
-        )
-
+        return iter(('figure_of_merit', 'spatial_noise_factor', 'band_gap', 'band_gap_room_temperature', 'seed', 'temporal_noise'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 6
 
 
 @schema(
-    title="Model 'dark_current'", description="Add dark current to the detector charge."
+    title="Model 'dark_current'"
+    ,description='Add dark current to the detector charge.'
 )
 @dataclass
 class ModelChargeGenerationDarkCurrent:
     name: str
     arguments: ModelChargeGenerationDarkCurrentArguments
-    func: Literal[
-        "pyxel.models.charge_generation.dark_current"
-    ] = "pyxel.models.charge_generation.dark_current"
+    func: Literal['pyxel.models.charge_generation.dark_current'] = 'pyxel.models.charge_generation.dark_current'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Dark Current Rule07
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationDarkCurrentRule07Arguments(Mapping[str, Any]):
     cutoff_wavelength: float = field(
         default=2.5,
         metadata=schema(
-            title="cutoff_wavelength", description="Cutoff wavelength. Unit: um"
-        ),
+            title='cutoff_wavelength'
+            ,description='Cutoff wavelength. Unit: um'
+        )
     )
     spatial_noise_factor: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="spatial_noise_factor",
-            description="Dark current fixed pattern noise factor.",
-        ),
+            title='spatial_noise_factor'
+            ,description='Dark current fixed pattern noise factor.'
+        )
+    )
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
+        )
     )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     temporal_noise: bool = field(
-        default=True, metadata=schema(title="temporal_noise", description="Shot noise.")
+        default=True,
+        metadata=schema(
+            title='temporal_noise'
+            ,description='Shot noise.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            ("cutoff_wavelength", "spatial_noise_factor", "seed", "temporal_noise")
-        )
-
+        return iter(('cutoff_wavelength', 'spatial_noise_factor', 'seed', 'temporal_noise'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'dark_current_rule07'",
-    description="Generate charge from dark current process.",
+    title="Model 'dark_current_rule07'"
+    ,description='Generate charge from dark current process.'
 )
 @dataclass
 class ModelChargeGenerationDarkCurrentRule07:
     name: str
-    arguments: ModelChargeGenerationDarkCurrentRule07Arguments = field(
-        default_factory=ModelChargeGenerationDarkCurrentRule07Arguments
-    )
-    func: Literal[
-        "pyxel.models.charge_generation.dark_current_rule07"
-    ] = "pyxel.models.charge_generation.dark_current_rule07"
+    arguments: ModelChargeGenerationDarkCurrentRule07Arguments = field(default_factory=ModelChargeGenerationDarkCurrentRule07Arguments)
+    func: Literal['pyxel.models.charge_generation.dark_current_rule07'] = 'pyxel.models.charge_generation.dark_current_rule07'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Dark Current Saphira
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationDarkCurrentSaphiraArguments(Mapping[str, Any]):
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
-
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
+        )
+    )
     def __iter__(self) -> Iterator[str]:
-        return iter(("seed",))
-
+        return iter(('seed',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'dark_current_saphira'",
-    description="Simulate dark current in a Saphira APD detector.",
+    title="Model 'dark_current_saphira'"
+    ,description='Simulate dark current in a Saphira APD detector.'
 )
 @dataclass
 class ModelChargeGenerationDarkCurrentSaphira:
     name: str
-    arguments: ModelChargeGenerationDarkCurrentSaphiraArguments = field(
-        default_factory=ModelChargeGenerationDarkCurrentSaphiraArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_generation.dark_current_saphira"
-    ] = "pyxel.models.charge_generation.dark_current_saphira"
+    arguments: ModelChargeGenerationDarkCurrentSaphiraArguments = field(default_factory=ModelChargeGenerationDarkCurrentSaphiraArguments)
+    func: Literal['pyxel.models.charge_generation.dark_current_saphira'] = 'pyxel.models.charge_generation.dark_current_saphira'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Load Charge
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationLoadChargeArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
-        metadata=schema(title="filename", description="File path.")
+        metadata=schema(
+            title='filename'
+            ,description='File path.'
+        )
     )
     position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="position",
-            description=(
-                "Indices of starting row and column, used when fitting charge to"
-                "detector."
-            ),
-        ),
+            title='position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting charge to'
+                    'detector.'
+                )
+        )
     )
-    align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="align",
-            description=(
-                'Keyword to align the charge to detector. Can be any from: ("center",'
-                '"top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='align'
+            ,description=(
+                    'Keyword to align the charge to detector. Can be any from: ("center",'
+                    '"top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title="time_scale",
-            description=(
-                "Time scale of the input charge, default is 1 second. 0.001 would be"
-                "ms."
-            ),
-        ),
+            title='time_scale'
+            ,description=(
+                    'Time scale of the input charge, default is 1 second. 0.001 would be'
+                    'ms.'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("filename", "position", "align", "time_scale"))
-
+        return iter(('filename', 'position', 'align', 'time_scale'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'load_charge'",
-    description=(
-        "Load charge from txt file for detector, mostly for but not limited to"
-        ":term:`CCDs<CCD>`."
-    ),
+    title="Model 'load_charge'"
+    ,description=(
+        'Load charge from txt file for detector, mostly for but not limited to'
+        ':term:`CCDs<CCD>`.'
+    )
 )
 @dataclass
 class ModelChargeGenerationLoadCharge:
     name: str
     arguments: ModelChargeGenerationLoadChargeArguments
-    func: Literal[
-        "pyxel.models.charge_generation.load_charge"
-    ] = "pyxel.models.charge_generation.load_charge"
+    func: Literal['pyxel.models.charge_generation.load_charge'] = 'pyxel.models.charge_generation.load_charge'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Simple Conversion
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationSimpleConversionArguments(Mapping[str, Any]):
     quantum_efficiency: Optional[float] = field(
         default=None,
-        metadata=schema(title="quantum_efficiency", description="Quantum efficiency."),
+        metadata=schema(
+            title='quantum_efficiency'
+            ,description='Quantum efficiency.'
+        )
+    )
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
+        )
     )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     binomial_sampling: bool = field(
         default=True,
         metadata=schema(
-            title="binomial_sampling", description="Binomial sampling. Default is True."
-        ),
+            title='binomial_sampling'
+            ,description='Binomial sampling. Default is True.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("quantum_efficiency", "seed", "binomial_sampling"))
-
+        return iter(('quantum_efficiency', 'seed', 'binomial_sampling'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'simple_conversion'",
-    description=(
-        "Generate charge from incident photon via photoelectric effect, simple" "model."
-    ),
+    title="Model 'simple_conversion'"
+    ,description=(
+        'Generate charge from incident photon via photoelectric effect, simple'
+        'model.'
+    )
 )
 @dataclass
 class ModelChargeGenerationSimpleConversion:
     name: str
-    arguments: ModelChargeGenerationSimpleConversionArguments = field(
-        default_factory=ModelChargeGenerationSimpleConversionArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_generation.simple_conversion"
-    ] = "pyxel.models.charge_generation.simple_conversion"
+    arguments: ModelChargeGenerationSimpleConversionArguments = field(default_factory=ModelChargeGenerationSimpleConversionArguments)
+    func: Literal['pyxel.models.charge_generation.simple_conversion'] = 'pyxel.models.charge_generation.simple_conversion'
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Simple Dark Current
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeGenerationSimpleDarkCurrentArguments(Mapping[str, Any]):
     dark_rate: float = field(
         metadata=schema(
-            title="dark_rate",
-            description=(
-                "Dark current, in electrons/pixel/second, which is the way"
-                "manufacturers typically report it."
-            ),
+            title='dark_rate'
+            ,description=(
+                    'Dark current, in electrons/pixel/second, which is the way'
+                    'manufacturers typically report it.'
+                )
+        )
+    )
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
         )
     )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("dark_rate", "seed"))
-
+        return iter(('dark_rate', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'simple_dark_current'",
-    description="Simulate dark current in a detector.",
+    title="Model 'simple_dark_current'"
+    ,description='Simulate dark current in a detector.'
 )
 @dataclass
 class ModelChargeGenerationSimpleDarkCurrent:
     name: str
     arguments: ModelChargeGenerationSimpleDarkCurrentArguments
-    func: Literal[
-        "pyxel.models.charge_generation.simple_dark_current"
-    ] = "pyxel.models.charge_generation.simple_dark_current"
+    func: Literal['pyxel.models.charge_generation.simple_dark_current'] = 'pyxel.models.charge_generation.simple_dark_current'
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Fixed Pattern Noise
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeCollectionFixedPatternNoiseArguments(Mapping[str, Any]):
     filename: Union[pathlib.Path, str, None] = field(
         default=None,
         metadata=schema(
-            title="filename", description="Path to a file with an array or an image."
-        ),
+            title='filename'
+            ,description='Path to a file with an array or an image.'
+        )
     )
     position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="position",
-            description=(
-                "Indices of starting row and column, used when fitting noise to"
-                "detector."
-            ),
-        ),
+            title='position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting noise to'
+                    'detector.'
+                )
+        )
     )
-    align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="align",
-            description=(
-                'Keyword to align the noise to detector. Can be any from: ("center",'
-                '"top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='align'
+            ,description=(
+                    'Keyword to align the noise to detector. Can be any from: ("center",'
+                    '"top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
     )
     fixed_pattern_noise_factor: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="fixed_pattern_noise_factor",
-            description="Fixed pattern noise factor.",
-        ),
+            title='fixed_pattern_noise_factor'
+            ,description='Fixed pattern noise factor.'
+        )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            ("filename", "position", "align", "fixed_pattern_noise_factor", "seed")
-        )
-
+        return iter(('filename', 'position', 'align', 'fixed_pattern_noise_factor', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'fixed_pattern_noise'",
-    description=(
-        "Add fixed pattern noise caused by pixel non-uniformity during charge"
-        "collection."
-    ),
+    title="Model 'fixed_pattern_noise'"
+    ,description=(
+        'Add fixed pattern noise caused by pixel non-uniformity during charge'
+        'collection.'
+    )
 )
 @dataclass
 class ModelChargeCollectionFixedPatternNoise:
     name: str
-    arguments: ModelChargeCollectionFixedPatternNoiseArguments = field(
-        default_factory=ModelChargeCollectionFixedPatternNoiseArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_collection.fixed_pattern_noise"
-    ] = "pyxel.models.charge_collection.fixed_pattern_noise"
+    arguments: ModelChargeCollectionFixedPatternNoiseArguments = field(default_factory=ModelChargeCollectionFixedPatternNoiseArguments)
+    func: Literal['pyxel.models.charge_collection.fixed_pattern_noise'] = 'pyxel.models.charge_collection.fixed_pattern_noise'
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Persistence
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeCollectionPersistenceArguments(Mapping[str, Any]):
     trap_time_constants: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_time_constants", description="A list of trap time constants."
+            title='trap_time_constants'
+            ,description='A list of trap time constants.'
         )
     )
     trap_proportions: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_proportions", description="A list of trap proportions."
+            title='trap_proportions'
+            ,description='A list of trap proportions.'
         )
     )
     trap_densities_filename: Union[pathlib.Path, str] = field(
         metadata=schema(
-            title="trap_densities_filename", description="Path to densities file."
+            title='trap_densities_filename'
+            ,description='Path to densities file.'
         )
     )
     trap_capacities_filename: Union[pathlib.Path, str, None] = field(
         default=None,
         metadata=schema(
-            title="trap_capacities_filename", description="Path to capacities file."
-        ),
+            title='trap_capacities_filename'
+            ,description='Path to capacities file.'
+        )
     )
     trap_densities_position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="trap_densities_position",
-            description=(
-                "Indices of starting row and column, used when fitting densities to"
-                "detector."
-            ),
-        ),
+            title='trap_densities_position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting densities to'
+                    'detector.'
+                )
+        )
     )
-    trap_densities_align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    trap_densities_align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="trap_densities_align",
-            description=(
-                "Keyword to align the densities to detector. Can be any from:"
-                '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='trap_densities_align'
+            ,description=(
+                    'Keyword to align the densities to detector. Can be any from:'
+                    '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
     )
     trap_capacities_position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title="trap_capacities_position",
-            description=(
-                "Indices of starting row and column, used when fitting capacities to"
-                "detector."
-            ),
-        ),
+            title='trap_capacities_position'
+            ,description=(
+                    'Indices of starting row and column, used when fitting capacities to'
+                    'detector.'
+                )
+        )
     )
-    trap_capacities_align: Optional[
-        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
-    ] = field(
+    trap_capacities_align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
         default=None,
         metadata=schema(
-            title="trap_capacities_align",
-            description=(
-                "Keyword to align the capacities to detector. Can be any from:"
-                '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
-            ),
-        ),
+            title='trap_capacities_align'
+            ,description=(
+                    'Keyword to align the capacities to detector. Can be any from:'
+                    '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "trap_time_constants",
-                "trap_proportions",
-                "trap_densities_filename",
-                "trap_capacities_filename",
-                "trap_densities_position",
-                "trap_densities_align",
-                "trap_capacities_position",
-                "trap_capacities_align",
-            )
-        )
-
+        return iter(('trap_time_constants', 'trap_proportions', 'trap_densities_filename', 'trap_capacities_filename', 'trap_densities_position', 'trap_densities_align', 'trap_capacities_position', 'trap_capacities_align'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 8
 
 
-@schema(title="Model 'persistence'", description="Apply persistence model.")
+@schema(
+    title="Model 'persistence'"
+    ,description='Apply persistence model.'
+)
 @dataclass
 class ModelChargeCollectionPersistence:
     name: str
     arguments: ModelChargeCollectionPersistenceArguments
-    func: Literal[
-        "pyxel.models.charge_collection.persistence"
-    ] = "pyxel.models.charge_collection.persistence"
+    func: Literal['pyxel.models.charge_collection.persistence'] = 'pyxel.models.charge_collection.persistence'
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Collection
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeCollectionSimpleCollectionArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
-
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 0
 
 
 @schema(
-    title="Model 'simple_collection'",
-    description="Associate charge with the closest pixel.",
+    title="Model 'simple_collection'"
+    ,description='Associate charge with the closest pixel.'
 )
 @dataclass
 class ModelChargeCollectionSimpleCollection:
     name: str
-    arguments: ModelChargeCollectionSimpleCollectionArguments = field(
-        default_factory=ModelChargeCollectionSimpleCollectionArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_collection.simple_collection"
-    ] = "pyxel.models.charge_collection.simple_collection"
+    arguments: ModelChargeCollectionSimpleCollectionArguments = field(default_factory=ModelChargeCollectionSimpleCollectionArguments)
+    func: Literal['pyxel.models.charge_collection.simple_collection'] = 'pyxel.models.charge_collection.simple_collection'
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Full Well
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeCollectionSimpleFullWellArguments(Mapping[str, Any]):
-    fwc: Optional[int] = field(default=None, metadata=schema(title="fwc"))
-
+    fwc: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='fwc'
+        )
+    )
     def __iter__(self) -> Iterator[str]:
-        return iter(("fwc",))
-
+        return iter(('fwc',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_full_well'",
-    description="Limit the amount of charge in pixel due to full well capacity.",
+    title="Model 'simple_full_well'"
+    ,description='Limit the amount of charge in pixel due to full well capacity.'
 )
 @dataclass
 class ModelChargeCollectionSimpleFullWell:
     name: str
-    arguments: ModelChargeCollectionSimpleFullWellArguments = field(
-        default_factory=ModelChargeCollectionSimpleFullWellArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_collection.simple_full_well"
-    ] = "pyxel.models.charge_collection.simple_full_well"
+    arguments: ModelChargeCollectionSimpleFullWellArguments = field(default_factory=ModelChargeCollectionSimpleFullWellArguments)
+    func: Literal['pyxel.models.charge_collection.simple_full_well'] = 'pyxel.models.charge_collection.simple_full_well'
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Ipc
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeCollectionSimpleIpcArguments(Mapping[str, Any]):
-    coupling: float = field(metadata=schema(title="coupling"))
+    coupling: float = field(
+        metadata=schema(
+            title='coupling'
+        )
+    )
     diagonal_coupling: float = field(
-        default=0.0, metadata=schema(title="diagonal_coupling")
+        default=0.0,
+        metadata=schema(
+            title='diagonal_coupling'
+        )
     )
     anisotropic_coupling: float = field(
-        default=0.0, metadata=schema(title="anisotropic_coupling")
+        default=0.0,
+        metadata=schema(
+            title='anisotropic_coupling'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("coupling", "diagonal_coupling", "anisotropic_coupling"))
-
+        return iter(('coupling', 'diagonal_coupling', 'anisotropic_coupling'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'simple_ipc'", description="Convolve pixel array with the IPC kernel."
+    title="Model 'simple_ipc'"
+    ,description='Convolve pixel array with the IPC kernel.'
 )
 @dataclass
 class ModelChargeCollectionSimpleIpc:
     name: str
     arguments: ModelChargeCollectionSimpleIpcArguments
-    func: Literal[
-        "pyxel.models.charge_collection.simple_ipc"
-    ] = "pyxel.models.charge_collection.simple_ipc"
+    func: Literal['pyxel.models.charge_collection.simple_ipc'] = 'pyxel.models.charge_collection.simple_ipc'
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Persistence
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeCollectionSimplePersistenceArguments(Mapping[str, Any]):
     trap_time_constants: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_time_constants", description="List of trap time constants."
+            title='trap_time_constants'
+            ,description='List of trap time constants.'
         )
     )
     trap_densities: collections.abc.Sequence[float] = field(
-        metadata=schema(title="trap_densities", description="List of trap densities.")
+        metadata=schema(
+            title='trap_densities'
+            ,description='List of trap densities.'
+        )
     )
     trap_capacities: Optional[collections.abc.Sequence[float]] = field(
         default=None,
         metadata=schema(
-            title="trap_capacities", description="List of trap capacities."
-        ),
+            title='trap_capacities'
+            ,description='List of trap capacities.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("trap_time_constants", "trap_densities", "trap_capacities"))
-
+        return iter(('trap_time_constants', 'trap_densities', 'trap_capacities'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'simple_persistence'", description="Apply simple persistence model."
+    title="Model 'simple_persistence'"
+    ,description='Apply simple persistence model.'
 )
 @dataclass
 class ModelChargeCollectionSimplePersistence:
     name: str
     arguments: ModelChargeCollectionSimplePersistenceArguments
-    func: Literal[
-        "pyxel.models.charge_collection.simple_persistence"
-    ] = "pyxel.models.charge_collection.simple_persistence"
+    func: Literal['pyxel.models.charge_collection.simple_persistence'] = 'pyxel.models.charge_collection.simple_persistence'
     enabled: bool = True
 
 
 #
 # Model: Charge Transfer / Arctic Add
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeTransferArcticAddArguments(Mapping[str, Any]):
-    well_fill_power: float = field(metadata=schema(title="well_fill_power"))
+    well_fill_power: float = field(
+        metadata=schema(
+            title='well_fill_power'
+        )
+    )
     trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_densities",
-            description="A 1D arrays of all trap species densities for serial clocking.",
+            title='trap_densities'
+            ,description='A 1D arrays of all trap species densities for serial clocking.'
         )
     )
     trap_release_timescales: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_release_timescales",
-            description="A 1D arrays of all trap release timescales for serial clocking.",
+            title='trap_release_timescales'
+            ,description='A 1D arrays of all trap release timescales for serial clocking.'
         )
     )
     express: int = field(
         default=0,
         metadata=schema(
-            title="express",
-            description=(
-                "As described in more detail in :cite:p:`2014:massey` section 2.1.5,"
-                "the effects of each individual pixel-to-pixel transfer can be very"
-                "similar, so multiple transfers can be computed at once for efficiency."
-                "The ``express`` input sets the number of times the transfers are"
-                "calculated.      * ``express = 1`` is the fastest and least accurate."
-                "* ``express = 2`` means the transfers are re-computed half-way through"
-                "readout.     * ``express = N`` where ``N`` is the total number of"
-                "pixels.  Default ``express = 0`` is a convenient input for automatic"
-                "``express = N``."
-            ),
-        ),
+            title='express'
+            ,description=(
+                    'As described in more detail in :cite:p:`2014:massey` section 2.1.5,'
+                    'the effects of each individual pixel-to-pixel transfer can be very'
+                    'similar, so multiple transfers can be computed at once for efficiency.'
+                    'The ``express`` input sets the number of times the transfers are'
+                    'calculated.      * ``express = 1`` is the fastest and least accurate.'
+                    '* ``express = 2`` means the transfers are re-computed half-way through'
+                    'readout.     * ``express = N`` where ``N`` is the total number of'
+                    'pixels.  Default ``express = 0`` is a convenient input for automatic'
+                    '``express = N``.'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            ("well_fill_power", "trap_densities", "trap_release_timescales", "express")
-        )
-
+        return iter(('well_fill_power', 'trap_densities', 'trap_release_timescales', 'express'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'arctic_add'",
-    description=(
-        "Add :term:`CTI` trails to an image by trapping, releasing and moving"
-        "electrons."
-    ),
+    title="Model 'arctic_add'"
+    ,description=(
+        'Add :term:`CTI` trails to an image by trapping, releasing and moving'
+        'electrons.'
+    )
 )
 @dataclass
 class ModelChargeTransferArcticAdd:
     name: str
     arguments: ModelChargeTransferArcticAddArguments
-    func: Literal[
-        "pyxel.models.charge_transfer.arctic_add"
-    ] = "pyxel.models.charge_transfer.arctic_add"
+    func: Literal['pyxel.models.charge_transfer.arctic_add'] = 'pyxel.models.charge_transfer.arctic_add'
     enabled: bool = True
 
 
 #
 # Model: Charge Transfer / Arctic Remove
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeTransferArcticRemoveArguments(Mapping[str, Any]):
-    well_fill_power: float = field(metadata=schema(title="well_fill_power"))
+    well_fill_power: float = field(
+        metadata=schema(
+            title='well_fill_power'
+        )
+    )
     trap_densities: collections.abc.Sequence[float] = field(
-        metadata=schema(title="trap_densities")
+        metadata=schema(
+            title='trap_densities'
+        )
     )
     trap_release_timescales: collections.abc.Sequence[float] = field(
-        metadata=schema(title="trap_release_timescales")
+        metadata=schema(
+            title='trap_release_timescales'
+        )
     )
     num_iterations: int = field(
         metadata=schema(
-            title="num_iterations",
-            description=(
-                "Number of iterations for the forward modelling. More iterations"
-                "provide higher accuracy at the cost of longer runtime. In practice,"
-                "just 1 to 3 iterations are usually sufficient."
-            ),
+            title='num_iterations'
+            ,description=(
+                    'Number of iterations for the forward modelling. More iterations'
+                    'provide higher accuracy at the cost of longer runtime. In practice,'
+                    'just 1 to 3 iterations are usually sufficient.'
+                )
         )
     )
     express: int = field(
         default=0,
         metadata=schema(
-            title="express",
-            description=(
-                "As described in more detail in :cite:p:`2014:massey` section 2.1.5,"
-                "the effects of each individual pixel-to-pixel transfer can be very"
-                "similar, so multiple transfers can be computed at once for efficiency."
-                "The ``express`` input sets the number of times the transfers are"
-                "calculated.      * ``express = 1`` is the fastest and least accurate."
-                "* ``express = 2`` means the transfers are re-computed half-way through"
-                "readout.     * ``express = N`` where ``N`` is the total number of"
-                "pixels.  Default ``express = 0`` is a convenient input for automatic"
-                "``express = N``."
-            ),
-        ),
+            title='express'
+            ,description=(
+                    'As described in more detail in :cite:p:`2014:massey` section 2.1.5,'
+                    'the effects of each individual pixel-to-pixel transfer can be very'
+                    'similar, so multiple transfers can be computed at once for efficiency.'
+                    'The ``express`` input sets the number of times the transfers are'
+                    'calculated.      * ``express = 1`` is the fastest and least accurate.'
+                    '* ``express = 2`` means the transfers are re-computed half-way through'
+                    'readout.     * ``express = N`` where ``N`` is the total number of'
+                    'pixels.  Default ``express = 0`` is a convenient input for automatic'
+                    '``express = N``.'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "well_fill_power",
-                "trap_densities",
-                "trap_release_timescales",
-                "num_iterations",
-                "express",
-            )
-        )
-
+        return iter(('well_fill_power', 'trap_densities', 'trap_release_timescales', 'num_iterations', 'express'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'arctic_remove'",
-    description=(
-        "Remove :term:`CTI` trails from an image by first modelling the"
-        "addition of :term:`CTI`."
-    ),
+    title="Model 'arctic_remove'"
+    ,description=(
+        'Remove :term:`CTI` trails from an image by first modelling the'
+        'addition of :term:`CTI`.'
+    )
 )
 @dataclass
 class ModelChargeTransferArcticRemove:
     name: str
     arguments: ModelChargeTransferArcticRemoveArguments
-    func: Literal[
-        "pyxel.models.charge_transfer.arctic_remove"
-    ] = "pyxel.models.charge_transfer.arctic_remove"
+    func: Literal['pyxel.models.charge_transfer.arctic_remove'] = 'pyxel.models.charge_transfer.arctic_remove'
     enabled: bool = True
 
 
 #
 # Model: Charge Transfer / Cdm
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeTransferCdmArguments(Mapping[str, Any]):
-    direction: Literal["parallel", "serial"] = field(
+    direction: Literal['parallel', 'serial'] = field(
         metadata=schema(
-            title="direction",
-            description=(
-                'Set ``"parallel"`` for :term:`CTI` in parallel direction or'
-                '``"serial"`` for :term:`CTI` in serial register.'
-            ),
+            title='direction'
+            ,description=(
+                    'Set ``"parallel"`` for :term:`CTI` in parallel direction or'
+                    '``"serial"`` for :term:`CTI` in serial register.'
+                )
         )
     )
     beta: float = field(
         metadata=schema(
-            title="beta",
-            description="Electron cloud expansion coefficient :math:`\\beta`.",
+            title='beta'
+            ,description='Electron cloud expansion coefficient :math:`\\beta`.'
         )
     )
     trap_release_times: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_release_times",
-            description="Trap release time constants :math:`\\tau_r`. Unit: :math:`s`.",
+            title='trap_release_times'
+            ,description='Trap release time constants :math:`\\tau_r`. Unit: :math:`s`.'
         )
     )
     trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="trap_densities",
-            description="Absolute trap densities :math:`n_t`. Unit: :math:`cm^{-3}`.",
+            title='trap_densities'
+            ,description='Absolute trap densities :math:`n_t`. Unit: :math:`cm^{-3}`.'
         )
     )
     sigma: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="sigma",
-            description="Trap capture cross section :math:`\\sigma`. Unit: :math:`cm^2`.",
+            title='sigma'
+            ,description='Trap capture cross section :math:`\\sigma`. Unit: :math:`cm^2`.'
         )
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="full_well_capacity",
-            description="Full well capacity :math:`FWC`. Unit: :math:`e^-`.",
-        ),
+            title='full_well_capacity'
+            ,description='Full well capacity :math:`FWC`. Unit: :math:`e^-`.'
+        )
     )
     max_electron_volume: float = field(
         default=0.0,
         metadata=schema(
-            title="max_electron_volume",
-            description=(
-                "Maximum geometrical volume :math:`V_g` that electrons can occupy"
-                "within a pixel. Unit: :math:`cm^3`."
-            ),
-        ),
+            title='max_electron_volume'
+            ,description=(
+                    'Maximum geometrical volume :math:`V_g` that electrons can occupy'
+                    'within a pixel. Unit: :math:`cm^3`.'
+                )
+        )
     )
     transfer_period: float = field(
         default=0.0,
         metadata=schema(
-            title="transfer_period",
-            description="Transfer period :math:`t` (TDI period). Unit: :math:`s`.",
-        ),
+            title='transfer_period'
+            ,description='Transfer period :math:`t` (TDI period). Unit: :math:`s`.'
+        )
     )
     charge_injection: bool = field(
         default=False,
         metadata=schema(
-            title="charge_injection",
-            description='Enable charge injection (only used in ``"parallel"`` mode).',
-        ),
+            title='charge_injection'
+            ,description='Enable charge injection (only used in ``"parallel"`` mode).'
+        )
     )
     electron_effective_mass: float = field(
         default=0.5,
         metadata=schema(
-            title="electron_effective_mass",
-            description=(
-                "Electron effective mass in the semiconductor lattice. Unit: 1 electron"
-                "mass"
-            ),
-        ),
+            title='electron_effective_mass'
+            ,description=(
+                    'Electron effective mass in the semiconductor lattice. Unit: 1 electron'
+                    'mass'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "direction",
-                "beta",
-                "trap_release_times",
-                "trap_densities",
-                "sigma",
-                "full_well_capacity",
-                "max_electron_volume",
-                "transfer_period",
-                "charge_injection",
-                "electron_effective_mass",
-            )
-        )
-
+        return iter(('direction', 'beta', 'trap_release_times', 'trap_densities', 'sigma', 'full_well_capacity', 'max_electron_volume', 'transfer_period', 'charge_injection', 'electron_effective_mass'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 10
 
 
-@schema(title="Model 'cdm'", description="Charge Distortion Model (CDM) model wrapper.")
+@schema(
+    title="Model 'cdm'"
+    ,description='Charge Distortion Model (CDM) model wrapper.'
+)
 @dataclass
 class ModelChargeTransferCdm:
     name: str
     arguments: ModelChargeTransferCdmArguments
-    func: Literal[
-        "pyxel.models.charge_transfer.cdm"
-    ] = "pyxel.models.charge_transfer.cdm"
+    func: Literal['pyxel.models.charge_transfer.cdm'] = 'pyxel.models.charge_transfer.cdm'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Dc Offset
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementDcOffsetArguments(Mapping[str, Any]):
     offset: float = field(
-        metadata=schema(title="offset", description="DC offset voltage. Unit: V")
+        metadata=schema(
+            title='offset'
+            ,description='DC offset voltage. Unit: V'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("offset",))
-
+        return iter(('offset',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
-@schema(title="Model 'dc_offset'", description="Apply DC voltage to the detector.")
+@schema(
+    title="Model 'dc_offset'"
+    ,description='Apply DC voltage to the detector.'
+)
 @dataclass
 class ModelChargeMeasurementDcOffset:
     name: str
     arguments: ModelChargeMeasurementDcOffsetArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.dc_offset"
-    ] = "pyxel.models.charge_measurement.dc_offset"
+    func: Literal['pyxel.models.charge_measurement.dc_offset'] = 'pyxel.models.charge_measurement.dc_offset'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Ktc Noise
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementKtcNoiseArguments(Mapping[str, Any]):
     node_capacitance: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="node_capacitance", description="Node capacitance. Unit: F"
-        ),
+            title='node_capacitance'
+            ,description='Node capacitance. Unit: F'
+        )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("node_capacitance", "seed"))
-
+        return iter(('node_capacitance', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'ktc_noise'",
-    description="Apply KTC reset noise to detector signal array.",
+    title="Model 'ktc_noise'"
+    ,description='Apply KTC reset noise to detector signal array.'
 )
 @dataclass
 class ModelChargeMeasurementKtcNoise:
     name: str
-    arguments: ModelChargeMeasurementKtcNoiseArguments = field(
-        default_factory=ModelChargeMeasurementKtcNoiseArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_measurement.ktc_noise"
-    ] = "pyxel.models.charge_measurement.ktc_noise"
+    arguments: ModelChargeMeasurementKtcNoiseArguments = field(default_factory=ModelChargeMeasurementKtcNoiseArguments)
+    func: Literal['pyxel.models.charge_measurement.ktc_noise'] = 'pyxel.models.charge_measurement.ktc_noise'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Nghxrg
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementNghxrgArguments(Mapping[str, Any]):
-    noise: collections.abc.Sequence[
-        collections.abc.Mapping[
-            Literal[
-                "ktc_bias_noise",
-                "white_read_noise",
-                "corr_pink_noise",
-                "uncorr_pink_noise",
-                "acn_noise",
-                "pca_zero_noise",
-            ],
-            collections.abc.Mapping[str, float],
-        ]
-    ] = field(metadata=schema(title="noise"))
+    noise: collections.abc.Sequence[collections.abc.Mapping[Literal['ktc_bias_noise', 'white_read_noise', 'corr_pink_noise', 'uncorr_pink_noise', 'acn_noise', 'pca_zero_noise'], collections.abc.Mapping[str, float]]] = field(
+        metadata=schema(
+            title='noise'
+        )
+    )
     window_position: Optional[tuple[int, int]] = field(
         default=None,
         metadata=schema(
-            title="window_position", description="[x0 (columns), y0 (rows)]."
-        ),
+            title='window_position'
+            ,description='[x0 (columns), y0 (rows)].'
+        )
     )
     window_size: Optional[tuple[int, int]] = field(
         default=None,
-        metadata=schema(title="window_size", description="[x (columns), y (rows)]."),
+        metadata=schema(
+            title='window_size'
+            ,description='[x (columns), y (rows)].'
+        )
+    )
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
+        )
     )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     n_output: int = field(
         default=1,
-        metadata=schema(title="n_output", description="Number of detector outputs."),
+        metadata=schema(
+            title='n_output'
+            ,description='Number of detector outputs.'
+        )
     )
     n_row_overhead: int = field(
         default=0,
         metadata=schema(
-            title="n_row_overhead",
-            description=(
-                "New row overhead in pixel. This allows for a short wait at the end of"
-                "a row before starting the next row."
-            ),
-        ),
+            title='n_row_overhead'
+            ,description=(
+                    'New row overhead in pixel. This allows for a short wait at the end of'
+                    'a row before starting the next row.'
+                )
+        )
     )
     n_frame_overhead: int = field(
         default=0,
         metadata=schema(
-            title="n_frame_overhead",
-            description=(
-                "New frame overhead in rows. This allows for a short wait at the end of"
-                "a frame before starting the next frame."
-            ),
-        ),
+            title='n_frame_overhead'
+            ,description=(
+                    'New frame overhead in rows. This allows for a short wait at the end of'
+                    'a frame before starting the next frame.'
+                )
+        )
     )
     reverse_scan_direction: bool = field(
         default=False,
         metadata=schema(
-            title="reverse_scan_direction",
-            description=(
-                "Set this True to reverse the fast scanner readout directions. This"
-                "capability was added to support Teledyne’s programmable fast scan"
-                "readout directions. The default setting (False) corresponds to what"
-                "HxRG detectors default to upon power up."
-            ),
-        ),
+            title='reverse_scan_direction'
+            ,description=(
+                    'Set this True to reverse the fast scanner readout directions. This'
+                    'capability was added to support Teledyne’s programmable fast scan'
+                    'readout directions. The default setting (False) corresponds to what'
+                    'HxRG detectors default to upon power up.'
+                )
+        )
     )
     reference_pixel_border_width: int = field(
         default=4,
         metadata=schema(
-            title="reference_pixel_border_width",
-            description="Width of reference pixel border around image area.",
-        ),
+            title='reference_pixel_border_width'
+            ,description='Width of reference pixel border around image area.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "noise",
-                "window_position",
-                "window_size",
-                "seed",
-                "n_output",
-                "n_row_overhead",
-                "n_frame_overhead",
-                "reverse_scan_direction",
-                "reference_pixel_border_width",
-            )
-        )
-
+        return iter(('noise', 'window_position', 'window_size', 'seed', 'n_output', 'n_row_overhead', 'n_frame_overhead', 'reverse_scan_direction', 'reference_pixel_border_width'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 9
 
 
 @schema(
-    title="Model 'nghxrg'",
-    description="Generate fourier noise power spectrum on HXRG detector.",
+    title="Model 'nghxrg'"
+    ,description='Generate fourier noise power spectrum on HXRG detector.'
 )
 @dataclass
 class ModelChargeMeasurementNghxrg:
     name: str
     arguments: ModelChargeMeasurementNghxrgArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.nghxrg"
-    ] = "pyxel.models.charge_measurement.nghxrg"
+    func: Literal['pyxel.models.charge_measurement.nghxrg'] = 'pyxel.models.charge_measurement.nghxrg'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Node Linearity Poly
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementOutputNodeLinearityPolyArguments(Mapping[str, Any]):
     coefficients: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title="coefficients", description="Coefficient of the polynomial function."
+            title='coefficients'
+            ,description='Coefficient of the polynomial function.'
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("coefficients",))
-
+        return iter(('coefficients',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'output_node_linearity_poly'",
-    description=(
-        "Add non-linearity to signal array to simulate the non-linearity of the"
-        "output node circuit."
-    ),
+    title="Model 'output_node_linearity_poly'"
+    ,description=(
+        'Add non-linearity to signal array to simulate the non-linearity of the'
+        'output node circuit.'
+    )
 )
 @dataclass
 class ModelChargeMeasurementOutputNodeLinearityPoly:
     name: str
     arguments: ModelChargeMeasurementOutputNodeLinearityPolyArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.output_node_linearity_poly"
-    ] = "pyxel.models.charge_measurement.output_node_linearity_poly"
+    func: Literal['pyxel.models.charge_measurement.output_node_linearity_poly'] = 'pyxel.models.charge_measurement.output_node_linearity_poly'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Node Noise
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementOutputNodeNoiseArguments(Mapping[str, Any]):
     std_deviation: float = field(
         metadata=schema(
-            title="std_deviation", description="Standard deviation. Unit: V"
+            title='std_deviation'
+            ,description='Standard deviation. Unit: V'
         )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("std_deviation", "seed"))
-
+        return iter(('std_deviation', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'output_node_noise'",
-    description=(
-        "Add noise to signal array of detector output node using normal random"
-        "distribution."
-    ),
+    title="Model 'output_node_noise'"
+    ,description=(
+        'Add noise to signal array of detector output node using normal random'
+        'distribution.'
+    )
 )
 @dataclass
 class ModelChargeMeasurementOutputNodeNoise:
     name: str
     arguments: ModelChargeMeasurementOutputNodeNoiseArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.output_node_noise"
-    ] = "pyxel.models.charge_measurement.output_node_noise"
+    func: Literal['pyxel.models.charge_measurement.output_node_noise'] = 'pyxel.models.charge_measurement.output_node_noise'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Node Noise Cmos
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementOutputNodeNoiseCmosArguments(Mapping[str, Any]):
     readout_noise: float = field(
         metadata=schema(
-            title="readout_noise",
-            description="Mean readout noise for the array in units of electrons. Unit: electron",
+            title='readout_noise'
+            ,description='Mean readout noise for the array in units of electrons. Unit: electron'
         )
     )
     readout_noise_std: float = field(
         metadata=schema(
-            title="readout_noise_std",
-            description="Readout noise standard deviation in units of electrons. Unit: electron",
+            title='readout_noise_std'
+            ,description='Readout noise standard deviation in units of electrons. Unit: electron'
         )
     )
     seed: Optional[int] = field(
-        default=None, metadata=schema(title="seed", description="Random seed.")
+        default=None,
+        metadata=schema(
+            title='seed'
+            ,description='Random seed.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("readout_noise", "readout_noise_std", "seed"))
-
+        return iter(('readout_noise', 'readout_noise_std', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'output_node_noise_cmos'",
-    description=(
-        "Output node noise model for :term:`CMOS` detectors where readout is"
-        "statistically independent for each pixel."
-    ),
+    title="Model 'output_node_noise_cmos'"
+    ,description=(
+        'Output node noise model for :term:`CMOS` detectors where readout is'
+        'statistically independent for each pixel.'
+    )
 )
 @dataclass
 class ModelChargeMeasurementOutputNodeNoiseCmos:
     name: str
     arguments: ModelChargeMeasurementOutputNodeNoiseCmosArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.output_node_noise_cmos"
-    ] = "pyxel.models.charge_measurement.output_node_noise_cmos"
+    func: Literal['pyxel.models.charge_measurement.output_node_noise_cmos'] = 'pyxel.models.charge_measurement.output_node_noise_cmos'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Pixel Reset Voltage Apd
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementOutputPixelResetVoltageApdArguments(Mapping[str, Any]):
     roic_drop: float = field(
         metadata=schema(
-            title="roic_drop", description="Readout circuit drop voltage. Unit: V"
+            title='roic_drop'
+            ,description='Readout circuit drop voltage. Unit: V'
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("roic_drop",))
-
+        return iter(('roic_drop',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'output_pixel_reset_voltage_apd'",
-    description="Apply output pixel reset voltage to APD detector.",
+    title="Model 'output_pixel_reset_voltage_apd'"
+    ,description='Apply output pixel reset voltage to APD detector.'
 )
 @dataclass
 class ModelChargeMeasurementOutputPixelResetVoltageApd:
     name: str
     arguments: ModelChargeMeasurementOutputPixelResetVoltageApdArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.output_pixel_reset_voltage_apd"
-    ] = "pyxel.models.charge_measurement.output_pixel_reset_voltage_apd"
+    func: Literal['pyxel.models.charge_measurement.output_pixel_reset_voltage_apd'] = 'pyxel.models.charge_measurement.output_pixel_reset_voltage_apd'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Physical Non Linearity
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementPhysicalNonLinearityArguments(Mapping[str, Any]):
     cutoff: float = field(
-        metadata=schema(title="cutoff", description="Cutoff wavelength. unit: um")
+        metadata=schema(
+            title='cutoff'
+            ,description='Cutoff wavelength. unit: um'
+        )
     )
     n_donor: float = field(
-        metadata=schema(title="n_donor", description="Donor density. Unit: atoms/cm^3")
+        metadata=schema(
+            title='n_donor'
+            ,description='Donor density. Unit: atoms/cm^3'
+        )
     )
     n_acceptor: float = field(
         metadata=schema(
-            title="n_acceptor", description="Acceptor density. Unit: atoms/cm^3"
+            title='n_acceptor'
+            ,description='Acceptor density. Unit: atoms/cm^3'
         )
     )
     diode_diameter: float = field(
-        metadata=schema(title="diode_diameter", description="Diode diameter. Unit: um")
+        metadata=schema(
+            title='diode_diameter'
+            ,description='Diode diameter. Unit: um'
+        )
     )
     v_bias: float = field(
-        metadata=schema(title="v_bias", description="Initial bias voltage. Unit: V.")
+        metadata=schema(
+            title='v_bias'
+            ,description='Initial bias voltage. Unit: V.'
+        )
     )
     fixed_capacitance: float = field(
         metadata=schema(
-            title="fixed_capacitance",
-            description="Additional fixed capacitance. Unit: F",
+            title='fixed_capacitance'
+            ,description='Additional fixed capacitance. Unit: F'
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "cutoff",
-                "n_donor",
-                "n_acceptor",
-                "diode_diameter",
-                "v_bias",
-                "fixed_capacitance",
-            )
-        )
-
+        return iter(('cutoff', 'n_donor', 'n_acceptor', 'diode_diameter', 'v_bias', 'fixed_capacitance'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 6
 
 
 @schema(
-    title="Model 'physical_non_linearity'", description="Apply physical non-linearity."
+    title="Model 'physical_non_linearity'"
+    ,description='Apply physical non-linearity.'
 )
 @dataclass
 class ModelChargeMeasurementPhysicalNonLinearity:
     name: str
     arguments: ModelChargeMeasurementPhysicalNonLinearityArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.physical_non_linearity"
-    ] = "pyxel.models.charge_measurement.physical_non_linearity"
+    func: Literal['pyxel.models.charge_measurement.physical_non_linearity'] = 'pyxel.models.charge_measurement.physical_non_linearity'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Physical Non Linearity With Saturation
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
-class ModelChargeMeasurementPhysicalNonLinearityWithSaturationArguments(
-    Mapping[str, Any]
-):
+class ModelChargeMeasurementPhysicalNonLinearityWithSaturationArguments(Mapping[str, Any]):
     cutoff: float = field(
-        metadata=schema(title="cutoff", description="Cutoff wavelength. unit: um")
+        metadata=schema(
+            title='cutoff'
+            ,description='Cutoff wavelength. unit: um'
+        )
     )
     n_donor: float = field(
-        metadata=schema(title="n_donor", description="Donor density. Unit: atoms/cm^3")
+        metadata=schema(
+            title='n_donor'
+            ,description='Donor density. Unit: atoms/cm^3'
+        )
     )
     n_acceptor: float = field(
         metadata=schema(
-            title="n_acceptor", description="Acceptor density. Unit: atoms/cm^3"
+            title='n_acceptor'
+            ,description='Acceptor density. Unit: atoms/cm^3'
         )
     )
     phi_implant: float = field(
         metadata=schema(
-            title="phi_implant", description="Diameter of the implantation. Unit: um"
+            title='phi_implant'
+            ,description='Diameter of the implantation. Unit: um'
         )
     )
     d_implant: float = field(
         metadata=schema(
-            title="d_implant", description="Depth of the implamantation. Unit: um"
+            title='d_implant'
+            ,description='Depth of the implamantation. Unit: um'
         )
     )
     saturation_current: float = field(
         metadata=schema(
-            title="saturation_current", description="Saturation current: e-/s/pix."
+            title='saturation_current'
+            ,description='Saturation current: e-/s/pix.'
         )
     )
     ideality_factor: float = field(
-        metadata=schema(title="ideality_factor", description="Ideality factor.")
+        metadata=schema(
+            title='ideality_factor'
+            ,description='Ideality factor.'
+        )
     )
     v_reset: float = field(
-        metadata=schema(title="v_reset", description="VRESET. Unit: V.")
+        metadata=schema(
+            title='v_reset'
+            ,description='VRESET. Unit: V.'
+        )
+    )
+    d_sub: float = field(
+        metadata=schema(
+            title='d_sub'
+            ,description='DSUB. Unit: V.'
+        )
     )
-    d_sub: float = field(metadata=schema(title="d_sub", description="DSUB. Unit: V."))
     fixed_capacitance: float = field(
         metadata=schema(
-            title="fixed_capacitance",
-            description="Additional fixed capacitance. Unit: F.",
+            title='fixed_capacitance'
+            ,description='Additional fixed capacitance. Unit: F.'
         )
     )
     euler_points: int = field(
         metadata=schema(
-            title="euler_points", description="Number of points in the euler method."
+            title='euler_points'
+            ,description='Number of points in the euler method.'
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            (
-                "cutoff",
-                "n_donor",
-                "n_acceptor",
-                "phi_implant",
-                "d_implant",
-                "saturation_current",
-                "ideality_factor",
-                "v_reset",
-                "d_sub",
-                "fixed_capacitance",
-                "euler_points",
-            )
-        )
-
+        return iter(('cutoff', 'n_donor', 'n_acceptor', 'phi_implant', 'd_implant', 'saturation_current', 'ideality_factor', 'v_reset', 'd_sub', 'fixed_capacitance', 'euler_points'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 11
 
 
 @schema(
-    title="Model 'physical_non_linearity_with_saturation'",
-    description="Apply physical non-linearity with saturation.",
+    title="Model 'physical_non_linearity_with_saturation'"
+    ,description='Apply physical non-linearity with saturation.'
 )
 @dataclass
 class ModelChargeMeasurementPhysicalNonLinearityWithSaturation:
     name: str
     arguments: ModelChargeMeasurementPhysicalNonLinearityWithSaturationArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.physical_non_linearity_with_saturation"
-    ] = "pyxel.models.charge_measurement.physical_non_linearity_with_saturation"
+    func: Literal['pyxel.models.charge_measurement.physical_non_linearity_with_saturation'] = 'pyxel.models.charge_measurement.physical_non_linearity_with_saturation'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Readout Noise Saphira
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementReadoutNoiseSaphiraArguments(Mapping[str, Any]):
     roic_readout_noise: float = field(
         metadata=schema(
-            title="roic_readout_noise",
-            description="Readout integrated circuit noise in volts RMS. Unit: V",
+            title='roic_readout_noise'
+            ,description='Readout integrated circuit noise in volts RMS. Unit: V'
         )
     )
     controller_noise: float = field(
         default=0.0,
         metadata=schema(
-            title="controller_noise",
-            description="Controller noise in volts RMS. Unit: V",
-        ),
+            title='controller_noise'
+            ,description='Controller noise in volts RMS. Unit: V'
+        )
+    )
+    seed: Optional[int] = field(
+        default=None,
+        metadata=schema(
+            title='seed'
+        )
     )
-    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("roic_readout_noise", "controller_noise", "seed"))
-
+        return iter(('roic_readout_noise', 'controller_noise', 'seed'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'readout_noise_saphira'",
-    description="Apply Saphira specific readout noise to the APD detector.",
+    title="Model 'readout_noise_saphira'"
+    ,description='Apply Saphira specific readout noise to the APD detector.'
 )
 @dataclass
 class ModelChargeMeasurementReadoutNoiseSaphira:
     name: str
     arguments: ModelChargeMeasurementReadoutNoiseSaphiraArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.readout_noise_saphira"
-    ] = "pyxel.models.charge_measurement.readout_noise_saphira"
+    func: Literal['pyxel.models.charge_measurement.readout_noise_saphira'] = 'pyxel.models.charge_measurement.readout_noise_saphira'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Simple Measurement
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementSimpleMeasurementArguments(Mapping[str, Any]):
     gain: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="gain",
-            description=(
-                "Gain to apply. By default, this is the sensitivity of charge readout."
-                "Unit: V/e-"
-            ),
-        ),
+            title='gain'
+            ,description=(
+                    'Gain to apply. By default, this is the sensitivity of charge readout.'
+                    'Unit: V/e-'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("gain",))
-
+        return iter(('gain',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_measurement'",
-    description="Convert the pixel array into signal array.",
+    title="Model 'simple_measurement'"
+    ,description='Convert the pixel array into signal array.'
 )
 @dataclass
 class ModelChargeMeasurementSimpleMeasurement:
     name: str
-    arguments: ModelChargeMeasurementSimpleMeasurementArguments = field(
-        default_factory=ModelChargeMeasurementSimpleMeasurementArguments
-    )
-    func: Literal[
-        "pyxel.models.charge_measurement.simple_measurement"
-    ] = "pyxel.models.charge_measurement.simple_measurement"
+    arguments: ModelChargeMeasurementSimpleMeasurementArguments = field(default_factory=ModelChargeMeasurementSimpleMeasurementArguments)
+    func: Literal['pyxel.models.charge_measurement.simple_measurement'] = 'pyxel.models.charge_measurement.simple_measurement'
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Simple Physical Non Linearity
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelChargeMeasurementSimplePhysicalNonLinearityArguments(Mapping[str, Any]):
     cutoff: float = field(
-        metadata=schema(title="cutoff", description="Cutoff wavelength. unit: um")
+        metadata=schema(
+            title='cutoff'
+            ,description='Cutoff wavelength. unit: um'
+        )
     )
     n_donor: float = field(
-        metadata=schema(title="n_donor", description="Donor density. Unit: atoms/cm^3")
+        metadata=schema(
+            title='n_donor'
+            ,description='Donor density. Unit: atoms/cm^3'
+        )
     )
     n_acceptor: float = field(
         metadata=schema(
-            title="n_acceptor", description="Acceptor density. Unit: atoms/cm^3"
+            title='n_acceptor'
+            ,description='Acceptor density. Unit: atoms/cm^3'
         )
     )
     diode_diameter: float = field(
-        metadata=schema(title="diode_diameter", description="Diode diameter. Unit: um")
+        metadata=schema(
+            title='diode_diameter'
+            ,description='Diode diameter. Unit: um'
+        )
     )
     v_bias: float = field(
-        metadata=schema(title="v_bias", description="Initial bias voltage. Unit: V.")
+        metadata=schema(
+            title='v_bias'
+            ,description='Initial bias voltage. Unit: V.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("cutoff", "n_donor", "n_acceptor", "diode_diameter", "v_bias"))
-
+        return iter(('cutoff', 'n_donor', 'n_acceptor', 'diode_diameter', 'v_bias'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'simple_physical_non_linearity'",
-    description="Apply simple physical non-linearity.",
+    title="Model 'simple_physical_non_linearity'"
+    ,description='Apply simple physical non-linearity.'
 )
 @dataclass
 class ModelChargeMeasurementSimplePhysicalNonLinearity:
     name: str
     arguments: ModelChargeMeasurementSimplePhysicalNonLinearityArguments
-    func: Literal[
-        "pyxel.models.charge_measurement.simple_physical_non_linearity"
-    ] = "pyxel.models.charge_measurement.simple_physical_non_linearity"
+    func: Literal['pyxel.models.charge_measurement.simple_physical_non_linearity'] = 'pyxel.models.charge_measurement.simple_physical_non_linearity'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Ac Crosstalk
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsAcCrosstalkArguments(Mapping[str, Any]):
     coupling_matrix: Union[str, pathlib.Path, collections.abc.Sequence] = field(
-        metadata=schema(title="coupling_matrix")
+        metadata=schema(
+            title='coupling_matrix'
+        )
+    )
+    channel_matrix: Sequence = field(
+        metadata=schema(
+            title='channel_matrix'
+        )
+    )
+    readout_directions: Sequence = field(
+        metadata=schema(
+            title='readout_directions'
+        )
     )
-    channel_matrix: Sequence = field(metadata=schema(title="channel_matrix"))
-    readout_directions: Sequence = field(metadata=schema(title="readout_directions"))
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("coupling_matrix", "channel_matrix", "readout_directions"))
-
+        return iter(('coupling_matrix', 'channel_matrix', 'readout_directions'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'ac_crosstalk'",
-    description="Apply AC crosstalk signal to detector signal.",
+    title="Model 'ac_crosstalk'"
+    ,description='Apply AC crosstalk signal to detector signal.'
 )
 @dataclass
 class ModelReadoutElectronicsAcCrosstalk:
     name: str
     arguments: ModelReadoutElectronicsAcCrosstalkArguments
-    func: Literal[
-        "pyxel.models.readout_electronics.ac_crosstalk"
-    ] = "pyxel.models.readout_electronics.ac_crosstalk"
+    func: Literal['pyxel.models.readout_electronics.ac_crosstalk'] = 'pyxel.models.readout_electronics.ac_crosstalk'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Dc Crosstalk
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsDcCrosstalkArguments(Mapping[str, Any]):
     coupling_matrix: Union[str, pathlib.Path, collections.abc.Sequence] = field(
-        metadata=schema(title="coupling_matrix")
+        metadata=schema(
+            title='coupling_matrix'
+        )
+    )
+    channel_matrix: Sequence = field(
+        metadata=schema(
+            title='channel_matrix'
+        )
+    )
+    readout_directions: Sequence = field(
+        metadata=schema(
+            title='readout_directions'
+        )
     )
-    channel_matrix: Sequence = field(metadata=schema(title="channel_matrix"))
-    readout_directions: Sequence = field(metadata=schema(title="readout_directions"))
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("coupling_matrix", "channel_matrix", "readout_directions"))
-
+        return iter(('coupling_matrix', 'channel_matrix', 'readout_directions'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'dc_crosstalk'",
-    description="Apply DC crosstalk signal to detector signal.",
+    title="Model 'dc_crosstalk'"
+    ,description='Apply DC crosstalk signal to detector signal.'
 )
 @dataclass
 class ModelReadoutElectronicsDcCrosstalk:
     name: str
     arguments: ModelReadoutElectronicsDcCrosstalkArguments
-    func: Literal[
-        "pyxel.models.readout_electronics.dc_crosstalk"
-    ] = "pyxel.models.readout_electronics.dc_crosstalk"
+    func: Literal['pyxel.models.readout_electronics.dc_crosstalk'] = 'pyxel.models.readout_electronics.dc_crosstalk'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Dead Time Filter
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsDeadTimeFilterArguments(Mapping[str, Any]):
     tau_0: float = field(
         default=4.4e-07,
         metadata=schema(
-            title="tau_0",
-            description=(
-                "Material dependent characteristic time for the electron-phonon"
-                "coupling. Unit: s"
-            ),
-        ),
+            title='tau_0'
+            ,description=(
+                    'Material dependent characteristic time for the electron-phonon'
+                    'coupling. Unit: s'
+                )
+        )
     )
     n_0: float = field(
         default=17200000000.0,
         metadata=schema(
-            title="n_0",
-            description=(
-                "Material dependent single spin density of states at the Fermi-level."
-                "Unit: um^-3 eV^-1"
-            ),
-        ),
+            title='n_0'
+            ,description=(
+                    'Material dependent single spin density of states at the Fermi-level.'
+                    'Unit: um^-3 eV^-1'
+                )
+        )
     )
     t_c: float = field(
         default=1.26,
         metadata=schema(
-            title="t_c", description="Material dependent critical temperature. Unit: K"
-        ),
+            title='t_c'
+            ,description='Material dependent critical temperature. Unit: K'
+        )
     )
     v: float = field(
         default=30.0,
-        metadata=schema(title="v", description="Superconducting volume. Unit: um^3"),
+        metadata=schema(
+            title='v'
+            ,description='Superconducting volume. Unit: um^3'
+        )
     )
     t_op: float = field(
-        default=0.3, metadata=schema(title="t_op", description="Temperature. Unit: K")
+        default=0.3,
+        metadata=schema(
+            title='t_op'
+            ,description='Temperature. Unit: K'
+        )
     )
     tau_pb: float = field(
         default=2.8e-10,
         metadata=schema(
-            title="tau_pb", description="Phonon pair-breaking time. Unit: s"
-        ),
+            title='tau_pb'
+            ,description='Phonon pair-breaking time. Unit: s'
+        )
     )
     tau_esc: float = field(
         default=1.4e-10,
-        metadata=schema(title="tau_esc", description="Phonon escape time. Unit: s"),
+        metadata=schema(
+            title='tau_esc'
+            ,description='Phonon escape time. Unit: s'
+        )
     )
     tau_sat: float = field(
         default=0.001,
-        metadata=schema(title="tau_sat", description="Saturation time. Unit: s"),
+        metadata=schema(
+            title='tau_sat'
+            ,description='Saturation time. Unit: s'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(
-            ("tau_0", "n_0", "t_c", "v", "t_op", "tau_pb", "tau_esc", "tau_sat")
-        )
-
+        return iter(('tau_0', 'n_0', 't_c', 'v', 't_op', 'tau_pb', 'tau_esc', 'tau_sat'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 8
 
 
-@schema(title="Model 'dead_time_filter'", description="Dead time filter.")
+@schema(
+    title="Model 'dead_time_filter'"
+    ,description='Dead time filter.'
+)
 @dataclass
 class ModelReadoutElectronicsDeadTimeFilter:
     name: str
-    arguments: ModelReadoutElectronicsDeadTimeFilterArguments = field(
-        default_factory=ModelReadoutElectronicsDeadTimeFilterArguments
-    )
-    func: Literal[
-        "pyxel.models.readout_electronics.dead_time_filter"
-    ] = "pyxel.models.readout_electronics.dead_time_filter"
+    arguments: ModelReadoutElectronicsDeadTimeFilterArguments = field(default_factory=ModelReadoutElectronicsDeadTimeFilterArguments)
+    func: Literal['pyxel.models.readout_electronics.dead_time_filter'] = 'pyxel.models.readout_electronics.dead_time_filter'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Sar Adc
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsSarAdcArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
-
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 0
 
 
 @schema(
-    title="Model 'sar_adc'",
-    description=(
-        "Digitize signal array using :term:`SAR` (Successive Approximation"
-        "Register) :term:`ADC` logic."
-    ),
+    title="Model 'sar_adc'"
+    ,description=(
+        'Digitize signal array using :term:`SAR` (Successive Approximation'
+        'Register) :term:`ADC` logic.'
+    )
 )
 @dataclass
 class ModelReadoutElectronicsSarAdc:
     name: str
-    arguments: ModelReadoutElectronicsSarAdcArguments = field(
-        default_factory=ModelReadoutElectronicsSarAdcArguments
-    )
-    func: Literal[
-        "pyxel.models.readout_electronics.sar_adc"
-    ] = "pyxel.models.readout_electronics.sar_adc"
+    arguments: ModelReadoutElectronicsSarAdcArguments = field(default_factory=ModelReadoutElectronicsSarAdcArguments)
+    func: Literal['pyxel.models.readout_electronics.sar_adc'] = 'pyxel.models.readout_electronics.sar_adc'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Sar Adc With Noise
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsSarAdcWithNoiseArguments(Mapping[str, Any]):
     strengths: tuple[float, ...] = field(
         metadata=schema(
-            title="strengths",
-            description=(
-                "Sequence of ``detector.characteristics.adc_bit_resolution`` number(s)."
-                "Unit: V"
-            ),
+            title='strengths'
+            ,description=(
+                    'Sequence of ``detector.characteristics.adc_bit_resolution`` number(s).'
+                    'Unit: V'
+                )
         )
     )
     noises: tuple[float, ...] = field(
         metadata=schema(
-            title="noises",
-            description=(
-                "Sequence of ``detector.characteristics.adc_bit_resolution`` number(s)."
-                "Unit: V"
-            ),
+            title='noises'
+            ,description=(
+                    'Sequence of ``detector.characteristics.adc_bit_resolution`` number(s).'
+                    'Unit: V'
+                )
         )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("strengths", "noises"))
-
+        return iter(('strengths', 'noises'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'sar_adc_with_noise'",
-    description=(
-        "Digitize signal array using :term:`SAR` (Successive Approximation"
-        "Register) :term:`ADC` logic with noise."
-    ),
+    title="Model 'sar_adc_with_noise'"
+    ,description=(
+        'Digitize signal array using :term:`SAR` (Successive Approximation'
+        'Register) :term:`ADC` logic with noise.'
+    )
 )
 @dataclass
 class ModelReadoutElectronicsSarAdcWithNoise:
     name: str
     arguments: ModelReadoutElectronicsSarAdcWithNoiseArguments
-    func: Literal[
-        "pyxel.models.readout_electronics.sar_adc_with_noise"
-    ] = "pyxel.models.readout_electronics.sar_adc_with_noise"
+    func: Literal['pyxel.models.readout_electronics.sar_adc_with_noise'] = 'pyxel.models.readout_electronics.sar_adc_with_noise'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Simple Adc
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsSimpleAdcArguments(Mapping[str, Any]):
-    data_type: Literal["uint16", "uint32", "uint64", "uint"] = field(
-        default="uint32",
+    data_type: Literal['uint16', 'uint32', 'uint64', 'uint'] = field(
+        default='uint32',
         metadata=schema(
-            title="data_type",
-            description=(
-                "The desired data-type for the Image array. The data-type must be an"
-                "unsigned integer. Valid values: 'uint16', 'uint32', 'uint64', 'uint'"
-                "Invalid values: 'int16', 'int32', 'int64', 'int', 'float'..."
-            ),
-        ),
+            title='data_type'
+            ,description=(
+                    'The desired data-type for the Image array. The data-type must be an'
+                    "unsigned integer. Valid values: 'uint16', 'uint32', 'uint64', 'uint'"
+                    "Invalid values: 'int16', 'int32', 'int64', 'int', 'float'..."
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("data_type",))
-
+        return iter(('data_type',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_adc'", description="Apply simple Analog to Digital conversion."
+    title="Model 'simple_adc'"
+    ,description='Apply simple Analog to Digital conversion.'
 )
 @dataclass
 class ModelReadoutElectronicsSimpleAdc:
     name: str
-    arguments: ModelReadoutElectronicsSimpleAdcArguments = field(
-        default_factory=ModelReadoutElectronicsSimpleAdcArguments
-    )
-    func: Literal[
-        "pyxel.models.readout_electronics.simple_adc"
-    ] = "pyxel.models.readout_electronics.simple_adc"
+    arguments: ModelReadoutElectronicsSimpleAdcArguments = field(default_factory=ModelReadoutElectronicsSimpleAdcArguments)
+    func: Literal['pyxel.models.readout_electronics.simple_adc'] = 'pyxel.models.readout_electronics.simple_adc'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Simple Amplifier
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsSimpleAmplifierArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
-
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 0
 
 
 @schema(
-    title="Model 'simple_amplifier'",
-    description=(
-        "Amplify signal using gain from the output amplifier and the signal"
-        "processor."
-    ),
+    title="Model 'simple_amplifier'"
+    ,description=(
+        'Amplify signal using gain from the output amplifier and the signal'
+        'processor.'
+    )
 )
 @dataclass
 class ModelReadoutElectronicsSimpleAmplifier:
     name: str
-    arguments: ModelReadoutElectronicsSimpleAmplifierArguments = field(
-        default_factory=ModelReadoutElectronicsSimpleAmplifierArguments
-    )
-    func: Literal[
-        "pyxel.models.readout_electronics.simple_amplifier"
-    ] = "pyxel.models.readout_electronics.simple_amplifier"
+    arguments: ModelReadoutElectronicsSimpleAmplifierArguments = field(default_factory=ModelReadoutElectronicsSimpleAmplifierArguments)
+    func: Literal['pyxel.models.readout_electronics.simple_amplifier'] = 'pyxel.models.readout_electronics.simple_amplifier'
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Simple Phase Conversion
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelReadoutElectronicsSimplePhaseConversionArguments(Mapping[str, Any]):
     phase_conversion: float = field(
         default=1.0,
         metadata=schema(
-            title="phase_conversion", description="Phase conversion factor"
-        ),
+            title='phase_conversion'
+            ,description='Phase conversion factor'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("phase_conversion",))
-
+        return iter(('phase_conversion',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_phase_conversion'",
-    description="Create an image array from phase array.",
+    title="Model 'simple_phase_conversion'"
+    ,description='Create an image array from phase array.'
 )
 @dataclass
 class ModelReadoutElectronicsSimplePhaseConversion:
     name: str
-    arguments: ModelReadoutElectronicsSimplePhaseConversionArguments = field(
-        default_factory=ModelReadoutElectronicsSimplePhaseConversionArguments
-    )
-    func: Literal[
-        "pyxel.models.readout_electronics.simple_phase_conversion"
-    ] = "pyxel.models.readout_electronics.simple_phase_conversion"
+    arguments: ModelReadoutElectronicsSimplePhaseConversionArguments = field(default_factory=ModelReadoutElectronicsSimplePhaseConversionArguments)
+    func: Literal['pyxel.models.readout_electronics.simple_phase_conversion'] = 'pyxel.models.readout_electronics.simple_phase_conversion'
     enabled: bool = True
 
 
 #
 # Model: Data Processing / Extract Roi To Xarray
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelDataProcessingExtractRoiToXarrayArguments(Mapping[str, Any]):
     thresh: int = field(
         default=50,
         metadata=schema(
-            title="thresh",
-            description="threshold above which information from the image array is extracted",
-        ),
+            title='thresh'
+            ,description='threshold above which information from the image array is extracted'
+        )
     )
     minarea: int = field(
         default=5,
         metadata=schema(
-            title="minarea",
-            description=(
-                "minimum area of elements required that are above the threshold for the"
-                "extractor to extract information"
-            ),
-        ),
+            title='minarea'
+            ,description=(
+                    'minimum area of elements required that are above the threshold for the'
+                    'extractor to extract information'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("thresh", "minarea"))
-
+        return iter(('thresh', 'minarea'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'extract_roi_to_xarray'",
-    description=(
-        "Extract the roi data converts it to xarray dataset and saves the"
-        "information to the final result."
-    ),
+    title="Model 'extract_roi_to_xarray'"
+    ,description=(
+        'Extract the roi data converts it to xarray dataset and saves the'
+        'information to the final result.'
+    )
 )
 @dataclass
 class ModelDataProcessingExtractRoiToXarray:
     name: str
-    arguments: ModelDataProcessingExtractRoiToXarrayArguments = field(
-        default_factory=ModelDataProcessingExtractRoiToXarrayArguments
-    )
-    func: Literal[
-        "pyxel.models.data_processing.extract_roi_to_xarray"
-    ] = "pyxel.models.data_processing.extract_roi_to_xarray"
+    arguments: ModelDataProcessingExtractRoiToXarrayArguments = field(default_factory=ModelDataProcessingExtractRoiToXarrayArguments)
+    func: Literal['pyxel.models.data_processing.extract_roi_to_xarray'] = 'pyxel.models.data_processing.extract_roi_to_xarray'
     enabled: bool = True
 
 
 #
 # Model: Data Processing / Linear Regression
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelDataProcessingLinearRegressionArguments(Mapping[str, Any]):
-    data_structure: Literal["pixel", "photon", "image", "signal"] = field(
-        default="image",
+    data_structure: Literal['pixel', 'photon', 'image', 'signal'] = field(
+        default='image',
         metadata=schema(
-            title="data_structure",
-            description="Data bucket to use for the linear regression.",
-        ),
+            title='data_structure'
+            ,description='Data bucket to use for the linear regression.'
+        )
     )
     name: Optional[str] = field(
         default=None,
-        metadata=schema(title="name", description="Name to use for the result."),
+        metadata=schema(
+            title='name'
+            ,description='Name to use for the result.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("data_structure", "name"))
-
+        return iter(('data_structure', 'name'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'linear_regression'",
-    description=(
+    title="Model 'linear_regression'"
+    ,description=(
         "Compute a linear regression along 'readout_time' and store it in"
         "'.data' bucket."
-    ),
+    )
 )
 @dataclass
 class ModelDataProcessingLinearRegression:
     name: str
-    arguments: ModelDataProcessingLinearRegressionArguments = field(
-        default_factory=ModelDataProcessingLinearRegressionArguments
-    )
-    func: Literal[
-        "pyxel.models.data_processing.linear_regression"
-    ] = "pyxel.models.data_processing.linear_regression"
+    arguments: ModelDataProcessingLinearRegressionArguments = field(default_factory=ModelDataProcessingLinearRegressionArguments)
+    func: Literal['pyxel.models.data_processing.linear_regression'] = 'pyxel.models.data_processing.linear_regression'
     enabled: bool = True
 
 
 #
 # Model: Data Processing / Mean Variance
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelDataProcessingMeanVarianceArguments(Mapping[str, Any]):
-    data_structure: Literal["pixel", "photon", "image", "signal"] = field(
-        default="image",
+    data_structure: Literal['pixel', 'photon', 'image', 'signal'] = field(
+        default='image',
         metadata=schema(
-            title="data_structure",
-            description="Data bucket to use for the linear regression.",
-        ),
+            title='data_structure'
+            ,description='Data bucket to use for the linear regression.'
+        )
     )
     name: Optional[str] = field(
         default=None,
-        metadata=schema(title="name", description="Name to use for the result."),
+        metadata=schema(
+            title='name'
+            ,description='Name to use for the result.'
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("data_structure", "name"))
-
+        return iter(('data_structure', 'name'))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'mean_variance'",
-    description="Compute mean-variance and store it in '.data' bucket.",
+    title="Model 'mean_variance'"
+    ,description="Compute mean-variance and store it in '.data' bucket."
 )
 @dataclass
 class ModelDataProcessingMeanVariance:
     name: str
-    arguments: ModelDataProcessingMeanVarianceArguments = field(
-        default_factory=ModelDataProcessingMeanVarianceArguments
-    )
-    func: Literal[
-        "pyxel.models.data_processing.mean_variance"
-    ] = "pyxel.models.data_processing.mean_variance"
+    arguments: ModelDataProcessingMeanVarianceArguments = field(default_factory=ModelDataProcessingMeanVarianceArguments)
+    func: Literal['pyxel.models.data_processing.mean_variance'] = 'pyxel.models.data_processing.mean_variance'
     enabled: bool = True
 
 
 #
 # Model: Data Processing / Statistics
 #
-@schema(title="Parameters")
+@schema(title='Parameters')
 @dataclass
 class ModelDataProcessingStatisticsArguments(Mapping[str, Any]):
-    data_structure: Literal["pixel", "photon", "signal", "image", "all"] = field(
-        default="all",
+    data_structure: Literal['pixel', 'photon', 'signal', 'image', 'all'] = field(
+        default='all',
         metadata=schema(
-            title="data_structure",
-            description=(
-                'Keyword to choose data structure. Can be any from: ("pixel", "photon",'
-                '"signal", "image", "all"). Default is "all" and computes the'
-                'statistics on "pixel", "photon", "signal" and "image".'
-            ),
-        ),
+            title='data_structure'
+            ,description=(
+                    'Keyword to choose data structure. Can be any from: ("pixel", "photon",'
+                    '"signal", "image", "all"). Default is "all" and computes the'
+                    'statistics on "pixel", "photon", "signal" and "image".'
+                )
+        )
     )
-
     def __iter__(self) -> Iterator[str]:
-        return iter(("data_structure",))
-
+        return iter(('data_structure',))
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
-
     def __len__(self) -> int:
         return 1
 
 
-@schema(title="Model 'statistics'", description="Compute basic statistics.")
+@schema(
+    title="Model 'statistics'"
+    ,description='Compute basic statistics.'
+)
 @dataclass
 class ModelDataProcessingStatistics:
     name: str
-    arguments: ModelDataProcessingStatisticsArguments = field(
-        default_factory=ModelDataProcessingStatisticsArguments
-    )
-    func: Literal[
-        "pyxel.models.data_processing.statistics"
-    ] = "pyxel.models.data_processing.statistics"
+    arguments: ModelDataProcessingStatisticsArguments = field(default_factory=ModelDataProcessingStatisticsArguments)
+    func: Literal['pyxel.models.data_processing.statistics'] = 'pyxel.models.data_processing.statistics'
     enabled: bool = True
 
 
 #
 # Detection pipeline
 #
 @dataclass
 class DetailedDetectionPipeline(DetectionPipeline):
     scene_generation: Optional[
         Sequence[Union[ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title="Scene Generation"))
+    ] = field(default=None, metadata=schema(title='Scene Generation'))
     photon_collection: Optional[
-        Sequence[
-            Union[
-                ModelPhotonCollectionIllumination,
-                ModelPhotonCollectionLoadImage,
-                ModelPhotonCollectionLoadPsf,
-                ModelPhotonCollectionOpticalPsf,
-                ModelPhotonCollectionShotNoise,
-                ModelPhotonCollectionStripePattern,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Photon Collection"))
+        Sequence[Union[ModelPhotonCollectionIllumination, ModelPhotonCollectionLoadImage, ModelPhotonCollectionLoadPsf, ModelPhotonCollectionOpticalPsf, ModelPhotonCollectionShotNoise, ModelPhotonCollectionStripePattern, ModelPhotonCollectionWavelengthDependenceAirs, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Photon Collection'))
     photon_generation: Optional[
-        Sequence[
-            Union[
-                ModelPhotonGenerationIllumination,
-                ModelPhotonGenerationLoadImage,
-                ModelPhotonGenerationShotNoise,
-                ModelPhotonGenerationStripePattern,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Photon Generation"))
+        Sequence[Union[ModelPhotonGenerationIllumination, ModelPhotonGenerationLoadImage, ModelPhotonGenerationShotNoise, ModelPhotonGenerationStripePattern, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Photon Generation'))
     optics: Optional[
-        Sequence[
-            Union[
-                ModelOpticsLoadPsf,
-                ModelOpticsOpticalPsf,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Optics"))
+        Sequence[Union[ModelOpticsLoadPsf, ModelOpticsOpticalPsf, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Optics'))
     phasing: Optional[
-        Sequence[
-            Union[
-                ModelPhasingPulseProcessing,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Phasing"))
+        Sequence[Union[ModelPhasingPulseProcessing, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Phasing'))
     charge_generation: Optional[
-        Sequence[
-            Union[
-                ModelChargeGenerationApdGain,
-                ModelChargeGenerationChargeBlocks,
-                ModelChargeGenerationChargeDeposition,
-                ModelChargeGenerationChargeDepositionInMct,
-                ModelChargeGenerationConversionWithQeMap,
-                ModelChargeGenerationCosmix,
-                ModelChargeGenerationDarkCurrent,
-                ModelChargeGenerationDarkCurrentRule07,
-                ModelChargeGenerationDarkCurrentSaphira,
-                ModelChargeGenerationLoadCharge,
-                ModelChargeGenerationSimpleConversion,
-                ModelChargeGenerationSimpleDarkCurrent,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Charge Generation"))
+        Sequence[Union[ModelChargeGenerationApdGain, ModelChargeGenerationChargeBlocks, ModelChargeGenerationChargeDeposition, ModelChargeGenerationChargeDepositionInMct, ModelChargeGenerationConversionWithQeMap, ModelChargeGenerationCosmix, ModelChargeGenerationDarkCurrent, ModelChargeGenerationDarkCurrentRule07, ModelChargeGenerationDarkCurrentSaphira, ModelChargeGenerationLoadCharge, ModelChargeGenerationSimpleConversion, ModelChargeGenerationSimpleDarkCurrent, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Charge Generation'))
     charge_collection: Optional[
-        Sequence[
-            Union[
-                ModelChargeCollectionFixedPatternNoise,
-                ModelChargeCollectionPersistence,
-                ModelChargeCollectionSimpleCollection,
-                ModelChargeCollectionSimpleFullWell,
-                ModelChargeCollectionSimpleIpc,
-                ModelChargeCollectionSimplePersistence,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Charge Collection"))
+        Sequence[Union[ModelChargeCollectionFixedPatternNoise, ModelChargeCollectionPersistence, ModelChargeCollectionSimpleCollection, ModelChargeCollectionSimpleFullWell, ModelChargeCollectionSimpleIpc, ModelChargeCollectionSimplePersistence, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Charge Collection'))
     charge_transfer: Optional[
-        Sequence[
-            Union[
-                ModelChargeTransferArcticAdd,
-                ModelChargeTransferArcticRemove,
-                ModelChargeTransferCdm,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Charge Transfer"))
+        Sequence[Union[ModelChargeTransferArcticAdd, ModelChargeTransferArcticRemove, ModelChargeTransferCdm, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Charge Transfer'))
     charge_measurement: Optional[
-        Sequence[
-            Union[
-                ModelChargeMeasurementDcOffset,
-                ModelChargeMeasurementKtcNoise,
-                ModelChargeMeasurementNghxrg,
-                ModelChargeMeasurementOutputNodeLinearityPoly,
-                ModelChargeMeasurementOutputNodeNoise,
-                ModelChargeMeasurementOutputNodeNoiseCmos,
-                ModelChargeMeasurementOutputPixelResetVoltageApd,
-                ModelChargeMeasurementPhysicalNonLinearity,
-                ModelChargeMeasurementPhysicalNonLinearityWithSaturation,
-                ModelChargeMeasurementReadoutNoiseSaphira,
-                ModelChargeMeasurementSimpleMeasurement,
-                ModelChargeMeasurementSimplePhysicalNonLinearity,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Charge Measurement"))
+        Sequence[Union[ModelChargeMeasurementDcOffset, ModelChargeMeasurementKtcNoise, ModelChargeMeasurementNghxrg, ModelChargeMeasurementOutputNodeLinearityPoly, ModelChargeMeasurementOutputNodeNoise, ModelChargeMeasurementOutputNodeNoiseCmos, ModelChargeMeasurementOutputPixelResetVoltageApd, ModelChargeMeasurementPhysicalNonLinearity, ModelChargeMeasurementPhysicalNonLinearityWithSaturation, ModelChargeMeasurementReadoutNoiseSaphira, ModelChargeMeasurementSimpleMeasurement, ModelChargeMeasurementSimplePhysicalNonLinearity, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Charge Measurement'))
     signal_transfer: Optional[
         Sequence[Union[ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title="Signal Transfer"))
+    ] = field(default=None, metadata=schema(title='Signal Transfer'))
     readout_electronics: Optional[
-        Sequence[
-            Union[
-                ModelReadoutElectronicsAcCrosstalk,
-                ModelReadoutElectronicsDcCrosstalk,
-                ModelReadoutElectronicsDeadTimeFilter,
-                ModelReadoutElectronicsSarAdc,
-                ModelReadoutElectronicsSarAdcWithNoise,
-                ModelReadoutElectronicsSimpleAdc,
-                ModelReadoutElectronicsSimpleAmplifier,
-                ModelReadoutElectronicsSimplePhaseConversion,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Readout Electronics"))
+        Sequence[Union[ModelReadoutElectronicsAcCrosstalk, ModelReadoutElectronicsDcCrosstalk, ModelReadoutElectronicsDeadTimeFilter, ModelReadoutElectronicsSarAdc, ModelReadoutElectronicsSarAdcWithNoise, ModelReadoutElectronicsSimpleAdc, ModelReadoutElectronicsSimpleAmplifier, ModelReadoutElectronicsSimplePhaseConversion, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Readout Electronics'))
     data_processing: Optional[
-        Sequence[
-            Union[
-                ModelDataProcessingExtractRoiToXarray,
-                ModelDataProcessingLinearRegression,
-                ModelDataProcessingMeanVariance,
-                ModelDataProcessingStatistics,
-                ModelLoadDetector,
-                ModelSaveDetector,
-                ModelFunction,
-            ]
-        ]
-    ] = field(default=None, metadata=schema(title="Data Processing"))
-
-
-@schema(title="Environment", description="Environmental attributes of the detector.")
+        Sequence[Union[ModelDataProcessingExtractRoiToXarray, ModelDataProcessingLinearRegression, ModelDataProcessingMeanVariance, ModelDataProcessingStatistics, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title='Data Processing'))
+@schema(
+    title='Environment',
+    description='Environmental attributes of the detector.'
+)
 @dataclass(kw_only=True)  # Python 3.10+
 class Environment:
     temperature: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="temperature", description="Temperature of the detector. Unit: K"
-        ),
+            title='temperature',
+            description='Temperature of the detector. Unit: K'
+        )
     )
 
 
 @schema(
-    title="Characteristics", description="Characteristic attributes of the detector."
+    title='Characteristics',
+    description='Characteristic attributes of the detector.'
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class Characteristics:
     quantum_efficiency: Optional[float] = field(
         default=None,
-        metadata=schema(title="quantum_efficiency", description="Quantum efficiency."),
+        metadata=schema(
+            title='quantum_efficiency',
+            description='Quantum efficiency.'
+        )
     )
     charge_to_volt_conversion: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="charge_to_volt_conversion",
-            description="Sensitivity of charge readout. Unit: V/e-",
-        ),
+            title='charge_to_volt_conversion',
+            description='Sensitivity of charge readout. Unit: V/e-'
+        )
     )
     pre_amplification: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="pre_amplification", description="Gain of pre-amplifier. Unit: V/V"
-        ),
+            title='pre_amplification',
+            description='Gain of pre-amplifier. Unit: V/V'
+        )
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="full_well_capacity", description="Full well capacity. Unit: e-"
-        ),
+            title='full_well_capacity',
+            description='Full well capacity. Unit: e-'
+        )
     )
     adc_voltage_range: Optional[tuple[float, float]] = field(
         default=None,
         metadata=schema(
-            title="adc_voltage_range", description="ADC voltage range. Unit: V"
-        ),
+            title='adc_voltage_range',
+            description='ADC voltage range. Unit: V'
+        )
     )
     adc_bit_resolution: Optional[int] = field(
         default=None,
-        metadata=schema(title="adc_bit_resolution", description="ADC bit resolution."),
+        metadata=schema(
+            title='adc_bit_resolution',
+            description='ADC bit resolution.'
+        )
     )
 
 
-@schema(title="Geometry", description="Geometrical attributes of the detector.")
+@schema(
+    title='Geometry',
+    description='Geometrical attributes of the detector.'
+)
 @dataclass(kw_only=True)  # Python 3.10+
 class Geometry:
-    row: int = field(metadata=schema(title="row", description="Number of pixel rows."))
+    row: int = field(
+        metadata=schema(
+            title='row',
+            description='Number of pixel rows.'
+        )
+    )
     col: int = field(
-        metadata=schema(title="col", description="Number of pixel columns.")
+        metadata=schema(
+            title='col',
+            description='Number of pixel columns.'
+        )
     )
     total_thickness: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="total_thickness", description="Thickness of detector. Unit: um"
-        ),
+            title='total_thickness',
+            description='Thickness of detector. Unit: um'
+        )
     )
     pixel_vert_size: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="pixel_vert_size", description="Vertical dimension of pixel. Unit: um"
-        ),
+            title='pixel_vert_size',
+            description='Vertical dimension of pixel. Unit: um'
+        )
     )
     pixel_horz_size: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="pixel_horz_size",
-            description="Horizontal dimension of pixel. Unit: um",
-        ),
+            title='pixel_horz_size',
+            description='Horizontal dimension of pixel. Unit: um'
+        )
     )
 
 
 @schema(
-    title="APDCharacteristics",
-    description="Characteristic attributes of the APD detector.",
+    title='APDCharacteristics',
+    description='Characteristic attributes of the APD detector.'
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class APDCharacteristics:
     roic_gain: float = field(
         metadata=schema(
-            title="roic_gain",
-            description="Gain of the read-out integrated circuit. Unit: V/V",
+            title='roic_gain',
+            description='Gain of the read-out integrated circuit. Unit: V/V'
         )
     )
     quantum_efficiency: Optional[float] = field(
         default=None,
-        metadata=schema(title="quantum_efficiency", description="Quantum efficiency."),
+        metadata=schema(
+            title='quantum_efficiency',
+            description='Quantum efficiency.'
+        )
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="full_well_capacity", description="Full well capacity. Unit: e-"
-        ),
+            title='full_well_capacity',
+            description='Full well capacity. Unit: e-'
+        )
     )
     adc_bit_resolution: Optional[int] = field(
         default=None,
-        metadata=schema(title="adc_bit_resolution", description="ADC bit resolution."),
+        metadata=schema(
+            title='adc_bit_resolution',
+            description='ADC bit resolution.'
+        )
     )
     adc_voltage_range: Optional[tuple[float, float]] = field(
         default=None,
         metadata=schema(
-            title="adc_voltage_range", description="ADC voltage range. Unit: V"
-        ),
+            title='adc_voltage_range',
+            description='ADC voltage range. Unit: V'
+        )
     )
     avalanche_gain: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="avalanche_gain", description="APD gain. Unit: electron/electron"
-        ),
+            title='avalanche_gain',
+            description='APD gain. Unit: electron/electron'
+        )
     )
     pixel_reset_voltage: Optional[float] = field(
         default=None,
         metadata=schema(
-            title="pixel_reset_voltage",
+            title='pixel_reset_voltage',
             description=(
-                "DC voltage going into the detector, not the voltage of a reset pixel."
-                "Unit: V"
-            ),
-        ),
+                    'DC voltage going into the detector, not the voltage of a reset pixel.'
+                    'Unit: V'
+                )
+        )
     )
     common_voltage: Optional[float] = field(
         default=None,
-        metadata=schema(title="common_voltage", description="Common voltage. Unit: V"),
+        metadata=schema(
+            title='common_voltage',
+            description='Common voltage. Unit: V'
+        )
     )
 
 
-@schema(title="Detector", description="The detector class.")
+@schema(
+    title='Detector',
+    description='The detector class.'
+)
 @dataclass(kw_only=True)  # Python 3.10+
 class Detector:
     environment: Optional[Environment] = field(
-        default=None, metadata=schema(title="environment")
+        default=None,
+        metadata=schema(
+            title='environment'
+        )
     )
 
 
 @schema(
-    title="CCDGeometry", description="Geometrical attributes of a :term:`CCD` detector."
+    title='CCDGeometry',
+    description='Geometrical attributes of a :term:`CCD` detector.'
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CCDGeometry(Geometry):
     pass
 
 
 @schema(
-    title="CMOSGeometry",
-    description="Geometrical attributes of a :term:`CMOS`-based detector.",
+    title='CMOSGeometry',
+    description='Geometrical attributes of a :term:`CMOS`-based detector.'
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CMOSGeometry(Geometry):
     pass
 
 
 @schema(
-    title="MKIDGeometry",
-    description="Geometrical attributes of a :term:`MKID`-based detector.",
+    title='MKIDGeometry',
+    description='Geometrical attributes of a :term:`MKID`-based detector.'
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class MKIDGeometry(Geometry):
     pass
 
 
 @schema(
-    title="APDGeometry",
-    description="Geometrical attributes of a :term:`APD`-based detector.",
+    title='APDGeometry',
+    description='Geometrical attributes of a :term:`APD`-based detector.'
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class APDGeometry(Geometry):
     pass
 
 
 @schema(
-    title="CCD",
+    title='CCD',
     description=(
-        "Charge-Coupled Device class containing all detector attributes and" "data."
-    ),
+        'Charge-Coupled Device class containing all detector attributes and'
+        'data.'
+        )
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CCD(Detector):
-    geometry: CCDGeometry = field(metadata=schema(title="geometry"))
-    characteristics: Characteristics = field(metadata=schema(title="characteristics"))
+    geometry: CCDGeometry = field(
+        metadata=schema(
+            title='geometry'
+        )
+    )
+    characteristics: Characteristics = field(
+        metadata=schema(
+            title='characteristics'
+        )
+    )
 
 
 @schema(
-    title="CMOS",
+    title='CMOS',
     description=(
-        ":term:`CMOS`-based detector class containing all detector attributes"
-        "and data."
-    ),
+        ':term:`CMOS`-based detector class containing all detector attributes'
+        'and data.'
+        )
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CMOS(Detector):
-    geometry: CMOSGeometry = field(metadata=schema(title="geometry"))
-    characteristics: Characteristics = field(metadata=schema(title="characteristics"))
+    geometry: CMOSGeometry = field(
+        metadata=schema(
+            title='geometry'
+        )
+    )
+    characteristics: Characteristics = field(
+        metadata=schema(
+            title='characteristics'
+        )
+    )
 
 
 @schema(
-    title="MKID",
+    title='MKID',
     description=(
-        ":term:`MKID`-based detector class containing all detector attributes"
-        "and data."
-    ),
+        ':term:`MKID`-based detector class containing all detector attributes'
+        'and data.'
+        )
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class MKID(Detector):
-    geometry: MKIDGeometry = field(metadata=schema(title="geometry"))
-    characteristics: Characteristics = field(metadata=schema(title="characteristics"))
+    geometry: MKIDGeometry = field(
+        metadata=schema(
+            title='geometry'
+        )
+    )
+    characteristics: Characteristics = field(
+        metadata=schema(
+            title='characteristics'
+        )
+    )
 
 
 @schema(
-    title="APD",
+    title='APD',
     description=(
-        ":term:`CMOS`-based detector class containing all detector attributes"
-        "and data."
-    ),
+        ':term:`CMOS`-based detector class containing all detector attributes'
+        'and data.'
+        )
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class APD(Detector):
-    geometry: APDGeometry = field(metadata=schema(title="geometry"))
+    geometry: APDGeometry = field(
+        metadata=schema(
+            title='geometry'
+        )
+    )
     characteristics: APDCharacteristics = field(
-        metadata=schema(title="characteristics")
+        metadata=schema(
+            title='characteristics'
+        )
     )
 
 
+
 #
 # Outputs
 #
 ValidName = Literal[
-    "detector.image.array", "detector.signal.array", "detector.pixel.array"
+    'detector.image.array', 'detector.signal.array', 'detector.pixel.array'
 ]
-ValidFormat = Literal["fits", "hdf", "npy", "txt", "csv", "png", "jpg", "jpeg"]
+ValidFormat = Literal['fits', 'hdf', 'npy', 'txt', 'csv', 'png', 'jpg', 'jpeg']
 
 
 @dataclass
 class Outputs:
     output_folder: pathlib.Path
     save_data_to_file: Optional[
         Sequence[Mapping[ValidName, Sequence[ValidFormat]]]
@@ -4082,196 +3943,177 @@
 
 
 #
 # Exposure
 #
 @dataclass
 class ExposureOutputs(Outputs):
-    save_exposure_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
-
-
+    save_exposure_data: Optional[
+        Sequence[Mapping[str, Sequence[str]]]
+    ] = None
 @dataclass
 class Readout:
     times: Union[Sequence, str, None] = None
     times_from_file: Optional[str] = None
     start_time: float = 0.0
     non_destructive: bool = False
 
 
-@schema(title="Exposure")
+@schema(title='Exposure')
 @dataclass
 class Exposure:
     outputs: ExposureOutputs
     readout: Readout = field(default_factory=Readout)
-    result_type: Literal["image", "signal", "pixel", "all"] = "all"
+    result_type: Literal['image', 'signal', 'pixel', 'all'] = 'all'
     pipeline_seed: Optional[int] = None
 
 
 #
 # Observation
 #
 
 
 @dataclass
 class ObservationOutputs(Outputs):
-    save_observation_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
+    save_observation_data: Optional[
+        Sequence[Mapping[str, Sequence[str]]]
+    ] = None
 
 
 @dataclass
 class ParameterValues:
     key: str
     values: Union[
-        Literal["_"],
-        Sequence[Literal["_"]],
+        Literal['_'],
+        Sequence[Literal['_']],
         Sequence[Union[int, float]],
         Sequence[Sequence[Union[int, float]]],
         Sequence[Sequence[Sequence[Union[int, float]]]],
         Sequence[str],
-        str,  # e.g. 'numpy.unique(...)'
+        str, # e.g. 'numpy.unique(...)'
     ]
     boundaries: Union[Tuple[float, float], Sequence[Tuple[float, float]], None] = None
     enabled: bool = True
     logarithmic: bool = False
 
 
-@schema(title="Observation")
+@schema(title='Observation')
 @dataclass
 class Observation:
     outputs: ObservationOutputs
     parameters: Sequence[ParameterValues]
     readout: Optional[Readout] = None
-    mode: Literal["product", "sequential", "custom"] = "product"
+    mode: Literal['product', 'sequential', 'custom'] = 'product'
     from_file: Optional[str] = None
     column_range: Optional[Tuple[int, int]] = None
     with_dask: bool = False
-    result_type: Literal["image", "signal", "pixel", "all"] = "all"
+    result_type: Literal['image', 'signal', 'pixel', 'all'] = 'all'
     pipeline_seed: Optional[int] = None
 
 
 #
 # Calibration
 #
 @dataclass
 class CalibrationOutputs(Outputs):
-    save_calibration_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
+    save_calibration_data: Optional[
+        Sequence[Mapping[str, Sequence[str]]]
+    ] = None
 
 
 @dataclass
 class Algorithm:
-    type: Literal["sade", "sga", "nlopt"] = "sade"
+    type: Literal['sade', 'sga', 'nlopt'] = 'sade'
     generations: int = 1
     population_size: int = 1
     # SADE #####
     variant: int = 2
     variant_adptv: int = 1
     ftol: float = 1e-6
     xtol: float = 1e-6
     memory: bool = False
     # SGA #####
     cr: float = 0.9
     eta_c: float = 1.0
     m: float = 0.02
     param_m: float = 1.0
     param_s: int = 2
-    crossover: Literal["single", "exponential", "binominal", "sbx"] = "exponential"
-    mutation: Literal["uniform", "gaussian", "polynomial"] = "polynomial"
-    selection: Literal["tournament", "truncated"] = "tournament"
+    crossover: Literal['single', 'exponential', 'binominal', 'sbx'] = 'exponential'
+    mutation: Literal['uniform', 'gaussian', 'polynomial'] = 'polynomial'
+    selection: Literal['tournament', 'truncated'] = 'tournament'
     # NLOPT #####
     nlopt_solver: Literal[
-        "cobyla",
-        "bobyqa",
-        "newuoa",
-        "newuoa_bound",
-        "praxis",
-        "neldermead",
-        "sbplx",
-        "mma",
-        "ccsaq",
-        "slsqp",
-        "lbfgs",
-        "tnewton_precond_restart",
-        "tnewton_precond",
-        "tnewton_restart",
-        "tnewton",
-        "var2",
-        "var1",
-        "auglag",
-        "auglag_eq",
-    ] = "neldermead"
+        'cobyla', 'bobyqa', 'newuoa', 'newuoa_bound', 'praxis', 'neldermead',
+        'sbplx', 'mma', 'ccsaq', 'slsqp', 'lbfgs', 'tnewton_precond_restart',
+        'tnewton_precond', 'tnewton_restart', 'tnewton', 'var2', 'var1', 'auglag',
+        'auglag_eq'
+    ] = 'neldermead'
     maxtime: int = 0
     maxeval: int = 0
     xtol_rel: float = 1.0e-8
     xtol_abs: float = 0.0
     ftol_rel: float = 0.0
     ftol_abs: float = 0.0
     stopval: Optional[float] = None
     # local_optimizer: Optional['pg.nlopt'] = None
-    replacement: Literal["best", "worst", "random"] = "best"
-    nlopt_selection: Literal["best", "worst", "random"] = "best"
+    replacement: Literal['best', 'worst', 'random'] = 'best'
+    nlopt_selection: Literal['best', 'worst', 'random'] = 'best'
 
 
-@schema(title="Fitness function")
+@schema(title='Fitness function')
 @dataclass
 class FitnessFunction:
     func: str
 
 
-@schema(title="Calibration")
+@schema(title='Calibration')
 @dataclass
 class Calibration:
     outputs: CalibrationOutputs
     target_data_path: Sequence[pathlib.Path]
     fitness_function: FitnessFunction
     algorithm: Algorithm
     parameters: Sequence[ParameterValues]
     readout: Optional[Readout] = None
-    mode: Literal["pipeline", "single_model"] = "pipeline"
-    result_type: Literal["image", "signal", "pixel"] = "image"
+    mode: Literal['pipeline', 'single_model'] = 'pipeline'
+    result_type: Literal['image', 'signal', 'pixel'] = 'image'
     result_fit_range: Optional[Sequence[int]] = None
     result_input_arguments: Optional[Sequence[ParameterValues]] = None
     target_fit_range: Optional[Sequence[int]] = None
     pygmo_seed: Optional[int] = None
     pipeline_seed: Optional[int] = None
     num_islands: int = 1
     num_evolutions: int = 1
     num_best_decisions: Optional[int] = None
-    topology: Literal["unconnected", "ring", "fully_connected"] = "unconnected"
+    topology: Literal['unconnected', 'ring', 'fully_connected'] = 'unconnected'
     type_islands: Literal[
-        "multiprocessing", "multithreading", "ipyparallel"
-    ] = "multiprocessing"
+        'multiprocessing', 'multithreading', 'ipyparallel'
+    ] = 'multiprocessing'
     weights_from_file: Optional[Sequence[pathlib.Path]] = None
     weights: Optional[Sequence[float]] = None
 
 
+
 @dataclass
 class Configuration:
     pipeline: DetailedDetectionPipeline
 
     # Running modes
-    exposure: Optional[Exposure] = field(
-        default=None, metadata=schema(title="Exposure")
-    )
-    observation: Optional[Observation] = field(
-        default=None, metadata=schema(title="Observation")
-    )
-    calibration: Optional[Calibration] = field(
-        default=None, metadata=schema(title="Calibration")
-    )
+    exposure: Optional[Exposure] = field(default=None, metadata=schema(title='Exposure'))
+    observation: Optional[Observation] = field(default=None, metadata=schema(title='Observation'))
+    calibration: Optional[Calibration] = field(default=None, metadata=schema(title='Calibration'))
 
     # Detectors
-    ccd_detector: Optional[CCD] = field(default=None, metadata=schema(title="CCD"))
-    cmos_detector: Optional[CMOS] = field(default=None, metadata=schema(title="CMOS"))
-    mkid_detector: Optional[MKID] = field(default=None, metadata=schema(title="MKID"))
-    apd_detector: Optional[APD] = field(default=None, metadata=schema(title="APD"))
-
-
+    ccd_detector: Optional[CCD] = field(default=None, metadata=schema(title='CCD'))
+    cmos_detector: Optional[CMOS] = field(default=None, metadata=schema(title='CMOS'))
+    mkid_detector: Optional[MKID] = field(default=None, metadata=schema(title='MKID'))
+    apd_detector: Optional[APD] = field(default=None, metadata=schema(title='APD'))
 class NotEqualError(Exception):
     ...
 
-
 def compare(first, second) -> None:
     if type(first) != type(second):
         raise NotEqualError
 
     if isinstance(first, dict) and isinstance(second, dict):
         if set(first) != set(second):
             raise NotEqualError
@@ -4292,59 +4134,55 @@
     else:
         if first != second:
             raise NotEqualError
 
 
 @click.command()
 @click.option(
-    "-f",
-    "--filename",
-    default="../../static/pyxel_schema.json",
+    '-f',
+    '--filename',
+    default='../../static/pyxel_schema.json',
     type=click.Path(),
-    help="JSON schema filename",
+    help='JSON schema filename',
     show_default=True,
 )
-@click.option(
-    "--check",
-    is_flag=True,
-    help="Don't write the JSON Schema back, just return the status.",
-)
+@click.option('--check', is_flag=True,
+     help="Don't write the JSON Schema back, just return the status.")
 def create_json_schema(filename: pathlib.Path, check: bool):
     if sys.version_info < (3, 10):
-        raise NotImplementedError("This script must run on Python 3.10+")
+        raise NotImplementedError('This script must run on Python 3.10+')
 
     # Manually define a 'format' for JSON Schema for 'Path'
-    schema(format="uri")(Path)
+    schema(format='uri')(Path)
 
     dct_schema = deserialization_schema(
-        Configuration,
-        version=JsonSchemaVersion.DRAFT_7,
-        all_refs=True,
+        Configuration, version=JsonSchemaVersion.DRAFT_7, all_refs=True,
     )
 
+
     full_filename = pathlib.Path(filename).resolve()
 
     if check:
         with full_filename.open() as fh:
             dct_reference = json.load(fh)
 
         new_dct_schema: Mapping[str, Any] = json.loads(json.dumps(dct_schema))
 
         try:
-            compare(dct_reference, new_dct_schema)
+           compare(dct_reference, new_dct_schema)
         except NotEqualError:
             print(
                 f"Error, JSON Schema file: {full_filename} is not the newest version. "
                 f"Please run 'tox -e json_schema'"
-            )
+             )
             pprint(result)
             sys.exit(1)
         else:
             sys.exit(0)
     else:
         print(json.dumps(dct_schema))
-        with full_filename.open("w") as fh:
+        with full_filename.open('w') as fh:
             json.dump(obj=dct_schema, fp=fh, indent=2, sort_keys=True)
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     create_json_schema()
```

### Comparing `pyxel_sim-1.9/continuous_integration/scripts/create_json_schema.py` & `pyxel_sim-1.9.1/continuous_integration/scripts/create_json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -632,14 +632,15 @@
     yield "    nlopt_selection: Literal['best', 'worst', 'random'] = 'best'"
     yield ""
     yield ""
     yield "@schema(title='Fitness function')"
     yield "@dataclass"
     yield "class FitnessFunction:"
     yield "    func: str"
+    yield "    arguments: Optional[Mapping[str, Any]] = None"
     yield ""
     yield ""
     yield "@schema(title='Calibration')"
     yield "@dataclass"
     yield "class Calibration:"
     yield "    outputs: CalibrationOutputs"
     yield "    target_data_path: Sequence[pathlib.Path]"
@@ -664,53 +665,32 @@
     yield "    weights_from_file: Optional[Sequence[pathlib.Path]] = None"
     yield "    weights: Optional[Sequence[float]] = None"
 
     yield ""
     yield ""
     yield ""
 
-    # Create wrappers for the detectors
-    # detector_classes: Sequence[str] = ("CCD", "CMOS", "MKID", "APD")
-    # for klass_name in detector_classes:
-    #     yield f"#@schema(title='{klass_name}')"
-    #     yield "#@dataclass"
-    #     yield f"#class Wrapper{klass_name}:"
-    #     yield f"#    {klass_name.lower()}: {klass_name}"
-    #     yield ""
-    #     yield ""
-
     # Create wrappers for the modes
     mode_classes: Sequence[str] = ("Exposure", "Observation", "Calibration")
-    # for klass_name in mode_classes:
-    #     yield f"#@schema(title='{klass_name}')"
-    #     yield "#@dataclass"
-    #     yield f"#class Wrapper{klass_name}:"
-    #     yield f"#    {klass_name.lower()}: {klass_name}"
-    #     yield ""
-    #     yield ""
-
-    # wrapper_detector_classes = [f"Wrapper{el}" for el in detector_classes]
-    # wrapper_mode_classes = [f"Wrapper{el}" for el in mode_classes]
 
-    yield "@dataclass"
-    yield "class Configuration:"
-    yield "    pipeline: DetailedDetectionPipeline"
-    # yield f"    # mode: Union[{', '.join(wrapper_mode_classes)}]"
-    # yield f"    # detector: Union[{', '.join(wrapper_detector_classes)}]"
+    all_configurations: list[str] = []
+    for running_mode in mode_classes:
+        for detector_klass in registered_detectors:
+            detector_name: str = detector_klass.__name__
+            klass_name: str = f"Configuration_{running_mode}_{detector_name}"
+
+            yield "@dataclass"
+            yield f"class {klass_name}:"
+            yield "    pipeline: DetailedDetectionPipeline = field(metadata=schema(title='Pipeline'))"
+            yield f"    {running_mode.lower()}: {running_mode} = field(metadata=schema(title={running_mode!r}))"
+            yield f"    {detector_name.lower()}_detector: {detector_name} = field(metadata=schema(title={detector_name!r}))"
 
-    yield ""
-    yield "    # Running modes"
-    for klass_name in mode_classes:
-        yield f"    {klass_name.lower()}: Optional[{klass_name}] = field(default=None, metadata=schema(title={klass_name!r}))"
+            all_configurations.append(klass_name)
 
-    yield ""
-    yield "    # Detectors"
-    for detector_klass in registered_detectors:
-        klass_name: str = detector_klass.__name__
-        yield f"    {klass_name.lower()}_detector: Optional[{klass_name}] = field(default=None, metadata=schema(title={klass_name!r}))"
+    return all_configurations
 
 
 def generate_all_models() -> Iterator[str]:
     lst = get_model_group_info()
     yield "#  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022."
     yield "#"
     yield "#  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which"
@@ -783,15 +763,15 @@
     for model_name in DetectionPipeline.MODEL_GROUPS:
         yield f"    {model_name}: Optional[Sequence[ModelFunction]] = None"
 
     yield ""
     yield ""
 
     yield from generate_group(lst)
-    yield from generate_detectors()
+    all_configurations = yield from generate_detectors()
 
     yield "class NotEqualError(Exception):"
     yield "    ..."
     yield ""
     yield "def compare(first, second) -> None:"
     yield "    if type(first) != type(second):"
     yield "        raise NotEqualError"
@@ -835,15 +815,15 @@
     yield "    if sys.version_info < (3, 10):"
     yield "        raise NotImplementedError('This script must run on Python 3.10+')"
     yield ""
     yield "    # Manually define a 'format' for JSON Schema for 'Path'"
     yield "    schema(format='uri')(Path)"
     yield ""
     yield "    dct_schema = deserialization_schema("
-    yield "        Configuration, version=JsonSchemaVersion.DRAFT_7, all_refs=True,"
+    yield f"        Union[{','.join(all_configurations)}], version=JsonSchemaVersion.DRAFT_7, all_refs=True"
     yield "    )"
     yield ""
     yield ""
     yield "    full_filename = pathlib.Path(filename).resolve()"
     yield ""
     yield "    if check:"
     yield "        with full_filename.open() as fh:"
```

### Comparing `pyxel_sim-1.9/continuous_integration/scripts/download_last_environment_artifact.py` & `pyxel_sim-1.9.1/continuous_integration/scripts/download_last_environment_artifact.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/docs/source/conf.py` & `pyxel_sim-1.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyproject.toml` & `pyxel_sim-1.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,26 @@
     "distributed",
 
     # Jupyter notebook
     "ipywidgets>=7.5",
 
     # Input/Output
     "astropy>=4.3",
-    "fsspec[http]>=2021",
+    "fsspec>=2021",
+    "aiohttp",  # for fsspec
     "h5py",
     "h5netcdf",
     "pyyaml",
     "xlrd",
     "openpyxl",
     "netcdf4",
 
     # Others
     "attrs>=21.3.0",
-    "click",
+    "click!=8.1.4",
     "tqdm",
     "typing-extensions",
     "pympler",
     "pillow",
     "scikit-image",
 ]
 dynamic = ["version"]
@@ -220,14 +221,15 @@
     "E501",     # Omit 'Line too long'
     "D102",     # Missing docstring in public method
     "D103",     # Missing docstring in public function
     "D105",     # Missing docstring in magic method
     "D202",     # No blank lines
     "RUF002",   # Docstring contains ambiguous unicode character
     "RUF003",   # ambiguous unicode character
+    "TCH003",   # Move standard library import in a type-checking block
     "TRY003",   # Avoid specifying long messages outside the exception class
     "TRY301",   # Abstract `raise` to an inner function
 ]
 
 select = [
     "A",        # flake8-builtins
     "B",        # flake8-bugbear
@@ -235,14 +237,15 @@
     "F",        # pyflakes
     "D",        # pydocstyle
     # "SIM",      # flake8-simplify
     "W",        # pycodestyle
     # "PD",       # pandas-vet
     # "S",        # bandit
     "RUF",      # Ruff-specific rules
+    "TCH",      # Flake8 Type Checking
     "TRY",      # Tryceratops
 ]
 
 exclude = ["_TEMPLATE.py", "_version.py"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
```

### Comparing `pyxel_sim-1.9/pyxel/__init__.py` & `pyxel_sim-1.9.1/pyxel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/__main__.py` & `pyxel_sim-1.9.1/pyxel/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/backends/asdf.py` & `pyxel_sim-1.9.1/pyxel/backends/asdf.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/backends/hdf5.py` & `pyxel_sim-1.9.1/pyxel/backends/hdf5.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/__init__.py` & `pyxel_sim-1.9.1/pyxel/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/algorithm.py` & `pyxel_sim-1.9.1/pyxel/calibration/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/archipelago.py` & `pyxel_sim-1.9.1/pyxel/calibration/archipelago.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from timeit import default_timer as timer
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 import xarray as xr
-from dask.delayed import Delayed
 from tqdm.auto import tqdm
 
 from pyxel.calibration import Algorithm, AlgorithmType, IslandProtocol
 from pyxel.calibration.fitting import ModelFitting
 from pyxel.calibration.util import slice_to_range
 
 if TYPE_CHECKING:
     import pygmo as pg
+    from dask.delayed import Delayed
     from numpy.typing import ArrayLike
 
     from pyxel.exposure import Readout
 
 
 # TODO: Deprecate this class ?
 class ArchipelagoLogs:
```

### Comparing `pyxel_sim-1.9/pyxel/calibration/archipelago_datatree.py` & `pyxel_sim-1.9.1/pyxel/calibration/archipelago_datatree.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from timeit import default_timer as timer
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 import xarray as xr
-from dask.delayed import Delayed
 from datatree import DataTree
 from tqdm.auto import tqdm
 
 from pyxel.calibration import Algorithm, IslandProtocol
 from pyxel.calibration.fitting_datatree import ModelFittingDataTree
 from pyxel.calibration.util import slice_to_range
 
 if TYPE_CHECKING:
     import pygmo as pg
+    from dask.delayed import Delayed
     from numpy.typing import ArrayLike
 
     from pyxel.exposure import Readout
 
 
 def extract_data_3d(
     df_results: pd.DataFrame,
```

### Comparing `pyxel_sim-1.9/pyxel/calibration/calibration.py` & `pyxel_sim-1.9.1/pyxel/calibration/calibration.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/fitness.py` & `pyxel_sim-1.9.1/pyxel/calibration/fitness.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/fitting.py` & `pyxel_sim-1.9.1/pyxel/calibration/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from numbers import Number
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 from dask.delayed import delayed
-from numpy.typing import NDArray
 
 from pyxel.calibration import (
     CalibrationMode,
     FittingCallable,
     ProblemSingleObjective,
     check_ranges,
     list_to_3d_slice,
@@ -35,15 +34,15 @@
 )
 from pyxel.exposure import run_exposure_pipeline
 from pyxel.observation import ParameterValues
 from pyxel.pipelines import Processor, ResultId
 
 if TYPE_CHECKING:
     import xarray as xr
-    from numpy.typing import ArrayLike
+    from numpy.typing import ArrayLike, NDArray
 
     from pyxel.exposure import Readout
 
 
 class ModelFitting(ProblemSingleObjective):
     """Pygmo problem class to fit data with any model in Pyxel."""
```

### Comparing `pyxel_sim-1.9/pyxel/calibration/fitting_datatree.py` & `pyxel_sim-1.9.1/pyxel/calibration/fitting_datatree.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from dask.delayed import delayed
-from numpy.typing import NDArray
 
 from pyxel.calibration import (
     FitRange2D,
     FitRange3D,
     FittingCallable,
     ProblemSingleObjective,
     check_fit_ranges,
@@ -36,15 +35,15 @@
 from pyxel.exposure import run_pipeline
 from pyxel.inputs import load_dataarray
 from pyxel.observation import ParameterValues
 from pyxel.pipelines import Processor, ResultId
 
 if TYPE_CHECKING:
     from datatree import DataTree
-    from numpy.typing import ArrayLike
+    from numpy.typing import ArrayLike, NDArray
 
     from pyxel.exposure import Readout
 
 
 def build_processors(
     processor: Processor,
     arguments: Sequence[ParameterValues],
```

### Comparing `pyxel_sim-1.9/pyxel/calibration/protocols.py` & `pyxel_sim-1.9.1/pyxel/calibration/protocols.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/user_defined.py` & `pyxel_sim-1.9.1/pyxel/calibration/user_defined.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/calibration/util.py` & `pyxel_sim-1.9.1/pyxel/calibration/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/configuration/configuration.py` & `pyxel_sim-1.9.1/pyxel/configuration/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 """Configuration loader."""
 
-from collections.abc import Iterator, Sequence
+from collections.abc import Iterator, Mapping, Sequence
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import copy2
 from typing import IO, TYPE_CHECKING, Any, Optional, Union
 
 import yaml
 
@@ -290,16 +290,17 @@
     dct
 
     Returns
     -------
     callable
     """
     func: str = dct["func"]
+    arguments: Optional[Mapping[str, Any]] = dct.get("arguments")
 
-    return FitnessFunction(func=func)
+    return FitnessFunction(func=func, arguments=arguments)
 
 
 def to_calibration(dct: dict) -> "Calibration":
     """Create a Calibration class from a dictionary.
 
     Parameters
     ----------
```

### Comparing `pyxel_sim-1.9/pyxel/data_structure/__init__.py` & `pyxel_sim-1.9.1/pyxel/data_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/array.py` & `pyxel_sim-1.9.1/pyxel/data_structure/array.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/charge.py` & `pyxel_sim-1.9.1/pyxel/data_structure/charge.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/image.py` & `pyxel_sim-1.9.1/pyxel/data_structure/image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/persistence.py` & `pyxel_sim-1.9.1/pyxel/data_structure/persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/phase.py` & `pyxel_sim-1.9.1/pyxel/data_structure/phase.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/photon.py` & `pyxel_sim-1.9.1/pyxel/data_structure/photon.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/pixel.py` & `pyxel_sim-1.9.1/pyxel/data_structure/pixel.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/processed_data.py` & `pyxel_sim-1.9.1/pyxel/data_structure/processed_data.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/scene.py` & `pyxel_sim-1.9.1/pyxel/data_structure/scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel Scene class to track multi-wavelength photon."""
 
 from collections.abc import Mapping, Sequence
 from typing import TYPE_CHECKING
 
+import numpy as np
+
 if TYPE_CHECKING:
-    import numpy as np
     from astropy.io.fits import ImageHDU
     from astropy.table import Table
     from scopesim import Source
 
 
 class Scene:
     """Scene class defining and storing information of all multi-wavelength photon."""
```

### Comparing `pyxel_sim-1.9/pyxel/data_structure/signal.py` & `pyxel_sim-1.9.1/pyxel/data_structure/signal.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/data_structure/util.py` & `pyxel_sim-1.9.1/pyxel/data_structure/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/__init__.py` & `pyxel_sim-1.9.1/pyxel/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/apd/__init__.py` & `pyxel_sim-1.9.1/pyxel/detectors/apd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/apd/apd.py` & `pyxel_sim-1.9.1/pyxel/detectors/apd/apd.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/apd/apd_characteristics.py` & `pyxel_sim-1.9.1/pyxel/detectors/apd/apd_characteristics.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
             "quantum_efficiency": self._quantum_efficiency,
             "full_well_capacity": self._full_well_capacity,
             "adc_voltage_range": self._adc_voltage_range,
             "adc_bit_resolution": self._adc_bit_resolution,
             "roic_gain": self._roic_gain,
         }
 
-        return {**dct, **other_dct}
+        return dct | other_dct
 
     @classmethod
     def from_dict(cls, dct: Mapping):
         """Create a new instance from a `dict`."""
         if "adc_voltage_range" in dct:
             new_dct: Mapping = dicttoolz.dissoc(dct, "adc_voltage_range")
             adc_voltage_range = dct["adc_voltage_range"]
```

### Comparing `pyxel_sim-1.9/pyxel/detectors/apd/apd_geometry.py` & `pyxel_sim-1.9.1/pyxel/detectors/apd/apd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/ccd/ccd.py` & `pyxel_sim-1.9.1/pyxel/detectors/ccd/ccd.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/ccd/ccd_geometry.py` & `pyxel_sim-1.9.1/pyxel/detectors/ccd/ccd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/characteristics.py` & `pyxel_sim-1.9.1/pyxel/detectors/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/cmos/cmos.py` & `pyxel_sim-1.9.1/pyxel/detectors/cmos/cmos.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/cmos/cmos_geometry.py` & `pyxel_sim-1.9.1/pyxel/detectors/cmos/cmos_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/detector.py` & `pyxel_sim-1.9.1/pyxel/detectors/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 """Detector class."""
 import collections
 from collections.abc import Mapping
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional, Union
 
-import numpy as np
-
 from pyxel import __version__, backends
 from pyxel.data_structure import (
     Charge,
     Image,
     Persistence,
     Photon,
     Pixel,
@@ -25,14 +23,15 @@
     Signal,
     SimplePersistence,
 )
 from pyxel.detectors import Environment, ReadoutProperties
 from pyxel.util.memory import get_size, memory_usage_details
 
 if TYPE_CHECKING:
+    import numpy as np
     import xarray as xr
     from datatree import DataTree
 
 
 __all__ = ["Detector"]
 
 
@@ -72,15 +71,15 @@
             and self._scene == other._scene
             and self._charge == other._charge
             and self._pixel == other._pixel
             and self._signal == other._signal
             and self._image == other._image
             and self._processed_data == other._processed_data
             and (
-                (self._data is None and other._data is None)
+                (self._data is other._data is None)
                 or (
                     self._data is not None
                     and other._data is not None
                     and self._data.equals(other._data)
                 )
             )
         )
@@ -489,15 +488,15 @@
         if not full_filename.exists():
             raise FileNotFoundError(f"Filename '{filename}' does not exist !")
 
         extension: str = full_filename.suffix
 
         if extension in (".h5", ".hdf5", ".hdf"):
             return cls.from_hdf5(filename)
-        elif extension in (".asdf",):
+        elif extension == ".asdf":
             return cls.from_asdf(filename)
         else:
             raise ValueError(f"Unknown extension {extension!r}.")
 
     def save(self, filename: Union[str, Path]) -> None:
         """Save a detector object into a filename.
 
@@ -511,15 +510,15 @@
             If the extension of filename is not recognized.
         """
         full_filename = Path(filename).resolve()
         extension: str = full_filename.suffix
 
         if extension in (".h5", ".hdf5", ".hdf"):
             return self.to_hdf5(filename)
-        elif extension in (".asdf",):
+        elif extension == ".asdf":
             return self.to_asdf(filename)
         else:
             raise ValueError(f"Unknown extension {extension!r}.")
 
     # TODO: Move this to another place. See #241
     def to_hdf5(self, filename: Union[str, Path]) -> None:
         """Write the detector content to a :term:`HDF5` file.
```

### Comparing `pyxel_sim-1.9/pyxel/detectors/environment.py` & `pyxel_sim-1.9.1/pyxel/detectors/environment.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/geometry.py` & `pyxel_sim-1.9.1/pyxel/detectors/geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/mkid/mkid.py` & `pyxel_sim-1.9.1/pyxel/detectors/mkid/mkid.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/mkid/mkid_geometry.py` & `pyxel_sim-1.9.1/pyxel/detectors/mkid/mkid_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/detectors/readout_properties.py` & `pyxel_sim-1.9.1/pyxel/detectors/readout_properties.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/evaluator.py` & `pyxel_sim-1.9.1/pyxel/evaluator.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/exposure/__init__.py` & `pyxel_sim-1.9.1/pyxel/exposure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/exposure/exposure.py` & `pyxel_sim-1.9.1/pyxel/exposure/exposure.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 import numpy as np
 import xarray as xr
 from datatree import DataTree
 from tqdm.auto import tqdm
 
 from pyxel import __version__
 from pyxel.data_structure import Charge, Image, Photon, Pixel, Signal
-from pyxel.exposure import Readout
 from pyxel.pipelines import Processor, ResultId, get_result_id, result_keys
 from pyxel.util import set_random_seed
 
 if TYPE_CHECKING:
+    from pyxel.exposure import Readout
     from pyxel.outputs import CalibrationOutputs, ExposureOutputs, ObservationOutputs
 
 
 class Exposure:
     """TBW."""
 
     def __init__(
```

### Comparing `pyxel_sim-1.9/pyxel/exposure/readout.py` & `pyxel_sim-1.9.1/pyxel/exposure/readout.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/inputs/loader.py` & `pyxel_sim-1.9.1/pyxel/inputs/loader.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/collection.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/collection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/diffusion.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/diffusion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/fixed_pattern_noise.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/fixed_pattern_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/full_well.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/full_well.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/inter_pixel_capacitance.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/inter_pixel_capacitance.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_collection/persistence.py` & `pyxel_sim-1.9.1/pyxel/models/charge_collection/persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/apd_gain.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/apd_gain.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/charge_deposition.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/charge_deposition.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/charge_injection.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/charge_injection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/cosmix.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/cosmix.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/particle.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/particle.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/plotting.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/plotting.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/simulation.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/simulation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/util.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/cosmix/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/dark_current.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/dark_current.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/dark_current_rule07.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/dark_current_rule07.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/data/mct-stopping-power.csv` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/data/mct-stopping-power.csv`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/load_charge.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/load_charge.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Simple model to load charge profiles."""
 
 from pathlib import Path
-from typing import Literal, Optional, Union
-
-import numpy as np
+from typing import TYPE_CHECKING, Literal, Optional, Union
 
 from pyxel.detectors import Detector, Geometry
 from pyxel.util import load_cropped_and_aligned_image
 
+if TYPE_CHECKING:
+    import numpy as np
+
 
 def load_charge(
     detector: Detector,
     filename: Union[str, Path],
     position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
```

### Comparing `pyxel_sim-1.9/pyxel/models/charge_generation/photoelectrons.py` & `pyxel_sim-1.9.1/pyxel/models/charge_generation/photoelectrons.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/linearity.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/linearity.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/measurement.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/nghxrg.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/non_linearity_calculation.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/non_linearity_calculation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/offset.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/offset.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/readout_noise.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/readout_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_measurement/reset_noise.py` & `pyxel_sim-1.9.1/pyxel/models/charge_measurement/reset_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_transfer/EMCCD_poisson.py` & `pyxel_sim-1.9.1/pyxel/models/charge_transfer/EMCCD_poisson.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py` & `pyxel_sim-1.9.1/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/charge_transfer/cdm.py` & `pyxel_sim-1.9.1/pyxel/models/charge_transfer/cdm.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/data_processing/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/data_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/data_processing/linear_regression.py` & `pyxel_sim-1.9.1/pyxel/models/data_processing/linear_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Model to compute linear regressions."""
 
-from typing import Literal, Optional, Union
+from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import numpy as np
-import xarray as xr
 
-from pyxel.data_structure import Image, Photon, Pixel, Signal
 from pyxel.detectors import Detector
 
+if TYPE_CHECKING:
+    import xarray as xr
+
+    from pyxel.data_structure import Image, Photon, Pixel, Signal
+
 
 def linear_regression(
     detector: Detector,
     data_structure: Literal["pixel", "photon", "image", "signal"] = "image",
     name: Optional[str] = None,
 ) -> None:
     """Compute a linear regression along 'readout_time' and store it in '.data' bucket.
```

### Comparing `pyxel_sim-1.9/pyxel/models/data_processing/mean_variance.py` & `pyxel_sim-1.9.1/pyxel/models/data_processing/mean_variance.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Model to compute Mean-Variance."""
-from typing import Literal, Optional, Union
+from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import xarray as xr
 from datatree import DataTree
 
-from pyxel.data_structure import Image, Photon, Pixel, Signal
 from pyxel.detectors import Detector
 
+if TYPE_CHECKING:
+    from pyxel.data_structure import Image, Photon, Pixel, Signal
+
 
 def compute_mean_variance(data_array: xr.DataArray) -> xr.DataArray:
     """Compute mean-variance into a DataArray.
 
     Parameters
     ----------
     data_array : DataArray
```

### Comparing `pyxel_sim-1.9/pyxel/models/data_processing/source_extractor.py` & `pyxel_sim-1.9.1/pyxel/models/data_processing/source_extractor.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/data_processing/statistics.py` & `pyxel_sim-1.9.1/pyxel/models/data_processing/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Simple model to compute basic statistics."""
 from collections.abc import Sequence
-from typing import Literal, Union
+from typing import TYPE_CHECKING, Literal, Union
 
 import xarray as xr
 from datatree import DataTree
 
-from pyxel.data_structure import Image, Photon, Pixel, Signal
 from pyxel.detectors import Detector
 
+if TYPE_CHECKING:
+    from pyxel.data_structure import Image, Photon, Pixel, Signal
+
 
 def compute_statistics(
     data_array: xr.DataArray,
     absolute_time: xr.DataArray,
     dimensions: Union[str, Sequence[str]] = ("x", "y"),
 ) -> xr.Dataset:
     """Compute basic statistics and save it into a Dataset.
```

### Comparing `pyxel_sim-1.9/pyxel/models/optics/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/optics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/optics/point_spread_function.py` & `pyxel_sim-1.9.1/pyxel/models/optics/point_spread_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/optics/poppy.py` & `pyxel_sim-1.9.1/pyxel/models/optics/poppy.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/phasing/pulse_processing.py` & `pyxel_sim-1.9.1/pyxel/models/phasing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/illumination.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/illumination.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/load_image.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/load_image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/point_spread_function.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/point_spread_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/poppy.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/poppy.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/shot_noise.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/shot_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_collection/stripe_pattern.py` & `pyxel_sim-1.9.1/pyxel/models/photon_collection/stripe_pattern.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_generation/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/photon_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_generation/illumination.py` & `pyxel_sim-1.9.1/pyxel/models/photon_generation/illumination.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_generation/load_image.py` & `pyxel_sim-1.9.1/pyxel/models/photon_generation/load_image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_generation/shot_noise.py` & `pyxel_sim-1.9.1/pyxel/models/photon_generation/shot_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/photon_generation/stripe_pattern.py` & `pyxel_sim-1.9.1/pyxel/models/photon_generation/stripe_pattern.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/__init__.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/amplification.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/amplification.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/amplifier_crosstalk.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/amplifier_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/dead_time.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/dead_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         * v
         * n_0
         * np.sqrt(2.0 * np.pi * boltzmann_cst * t_op * delta)
         * np.exp(-delta / (boltzmann_cst * t_op))
     )
 
     # Compute recombination constant
-    recombination_cst: float = (
-        tau_0 * n_0 * (boltzmann_cst * t_c) ** 3 / (2.0 * delta**2)
+    recombination_cst: float = (2.0 * delta**2) / (
+        tau_0 * n_0 * (boltzmann_cst * t_c) ** 3
     )
 
     # Compute intrinsic quasiparticle lifetime with respect to recombination
     tau_qp: float = v / (recombination_cst * n_qp)
 
     # Compute apparent quasi-particle lifetime, without saturation lifetime
     # tau_apparent = 1. / (2. / (tau_qp * (1. + (char.tau_esc / char.tau_pb))))
```

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/phase_conversion.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/phase_conversion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/sar_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc_with_noise.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/sar_adc_with_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/readout_electronics/simple_adc.py` & `pyxel_sim-1.9.1/pyxel/models/readout_electronics/simple_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/models/util.py` & `pyxel_sim-1.9.1/pyxel/models/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/notebook/__init__.py` & `pyxel_sim-1.9.1/pyxel/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/notebook/calibration.py` & `pyxel_sim-1.9.1/pyxel/notebook/calibration.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/notebook/html_representation.py` & `pyxel_sim-1.9.1/pyxel/notebook/html_representation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/notebook/jupyxel.py` & `pyxel_sim-1.9.1/pyxel/notebook/jupyxel.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/observation/__init__.py` & `pyxel_sim-1.9.1/pyxel/observation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/observation/observation.py` & `pyxel_sim-1.9.1/pyxel/observation/observation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/observation/parameter_values.py` & `pyxel_sim-1.9.1/pyxel/observation/parameter_values.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/options.py` & `pyxel_sim-1.9.1/pyxel/options.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/outputs/__init__.py` & `pyxel_sim-1.9.1/pyxel/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/outputs/calibration_outputs.py` & `pyxel_sim-1.9.1/pyxel/outputs/calibration_outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/outputs/exposure_outputs.py` & `pyxel_sim-1.9.1/pyxel/outputs/exposure_outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/outputs/observation_outputs.py` & `pyxel_sim-1.9.1/pyxel/outputs/observation_outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/outputs/outputs.py` & `pyxel_sim-1.9.1/pyxel/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/pipelines/__init__.py` & `pyxel_sim-1.9.1/pyxel/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/pipelines/model_function.py` & `pyxel_sim-1.9.1/pyxel/pipelines/model_function.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import inspect
 import warnings
-from collections.abc import MutableMapping
+from collections.abc import Mapping, MutableMapping
 from typing import TYPE_CHECKING, Any, Callable, Optional
 
 from pyxel.evaluator import evaluate_reference
 
 if TYPE_CHECKING:
     import numpy as np
 
@@ -197,21 +197,32 @@
         """TBW."""
         self._func(detector, **self.arguments)
 
 
 class FitnessFunction:
     """Fitness function for model fitting."""
 
-    def __init__(self, func: str):
+    def __init__(self, func: str, arguments: Optional[Mapping[str, Any]] = None):
         self._func: FittingCallable = evaluate_reference(func)
+        self._arguments: Optional[Mapping[str, Any]] = arguments
 
     def __call__(
         self,
         simulated: "np.ndarray",
         target: "np.ndarray",
         weighting: "np.ndarray",
     ) -> float:
         """Compute fitness."""
-        result: float = self._func(
-            simulated=simulated, target=target, weighting=weighting
-        )
+        if self._arguments is None:
+            result: float = self._func(
+                simulated=simulated,
+                target=target,
+                weighting=weighting,
+            )
+        else:
+            result = self._func(
+                simulated=simulated,
+                target=target,
+                weighting=weighting,
+                **self._arguments,
+            )
         return result
```

### Comparing `pyxel_sim-1.9/pyxel/pipelines/model_group.py` & `pyxel_sim-1.9.1/pyxel/pipelines/model_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,20 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import logging
 from collections.abc import Iterator, Mapping, Sequence
 from copy import deepcopy
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
-from pyxel import util
 from pyxel.pipelines import ModelFunction
 
 if TYPE_CHECKING:
     from pyxel.detectors import Detector
-    from pyxel.pipelines import DetectionPipeline
 
 
 # TODO: These methods could also be as a `abc.Sequence` with magical methods:
 #       __getitem__, __iter__, __len__, __contains__, ...
 #       See #181
 class ModelGroup:
     """TBW."""
@@ -59,39 +57,18 @@
                 return model
         else:
             raise AttributeError(f"Cannot find model {item!r}.")
 
     def __dir__(self):
         return dir(type(self)) + [model.name for model in self.models]
 
-    # TODO: Why is this method returning a `bool` ?
-    def run(
-        self,
-        detector: "Detector",
-        pipeline: "DetectionPipeline",
-        abort_model: Optional[str] = None,
-    ) -> bool:
+    def run(self, detector: "Detector"):
         """Execute each enabled model in this group.
 
         Parameters
         ----------
         detector : Detector
-        pipeline : DetectionPipeline
-        abort_model : str, optional
-
-        Returns
-        -------
-        bool
-            TBW.
         """
         model: ModelFunction
-        for model in self.models:
-            if model.name == abort_model:
-                return True
-            if not pipeline.is_running:
-                raise util.PipelineAborted("Pipeline has been aborted.")
-            else:
-                if model.enabled:
-                    self._log.info("Model: %r", model.name)
-                    model(detector)
-
-        return False
+        for model in self:
+            self._log.info("Model: %r", model.name)
+            model(detector)
```

### Comparing `pyxel_sim-1.9/pyxel/pipelines/pipeline.py` & `pyxel_sim-1.9.1/pyxel/pipelines/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         charge_transfer: Optional[Sequence[ModelFunction]] = None,
         charge_measurement: Optional[Sequence[ModelFunction]] = None,
         signal_transfer: Optional[Sequence[ModelFunction]] = None,
         readout_electronics: Optional[Sequence[ModelFunction]] = None,
         data_processing: Optional[Sequence[ModelFunction]] = None,
         doc: Optional[str] = None,
     ):
-        self._is_running = False
         self.doc = doc
 
         self._scene_generation: Optional[ModelGroup] = (
             ModelGroup(scene_generation, name="scene_generation")
             if scene_generation
             else None
         )
@@ -121,15 +120,15 @@
             ModelGroup(data_processing, name="data_processing")
             if data_processing
             else None
         )
 
     def __repr__(self) -> str:
         cls_name: str = self.__class__.__name__
-        return f"{cls_name}<is_running={self._is_running!r}, doc={self.doc!r}>"
+        return f"{cls_name}<doc={self.doc!r}>"
 
     def __iter__(self) -> Iterable[ModelFunction]:
         for model in self.MODEL_GROUPS:
             models_grp: Optional[ModelGroup] = getattr(self, model)
             if models_grp:
                 yield from models_grp
 
@@ -208,23 +207,14 @@
         return self._data_processing
 
     @property
     def model_group_names(self) -> tuple[str, ...]:
         """TBW."""
         return self.MODEL_GROUPS
 
-    @property
-    def is_running(self) -> bool:
-        """Return the running state of this pipeline."""
-        return self._is_running
-
-    def abort(self) -> None:
-        """TBW."""
-        self._is_running = False
-
     # TODO: Is this method used ?
     def get_model(self, name: str) -> ModelFunction:
         """Return a ModelFunction object for the specified model name.
 
         Parameters
         ----------
         name: str
```

### Comparing `pyxel_sim-1.9/pyxel/pipelines/processor.py` & `pyxel_sim-1.9.1/pyxel/pipelines/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,16 @@
             ResultId("photon"),
             ResultId("charge"),
             ResultId("pixel"),
             ResultId("signal"),
             ResultId("image"),
             ResultId("data"),
         ]
-    else:
-        return [ResultId(result_type)]
+
+    return [ResultId(result_type)]
 
 
 # TODO: Is this class needed ?
 class Processor:
     """TBW."""
 
     def __init__(self, detector: "Detector", pipeline: DetectionPipeline):
@@ -183,55 +183,30 @@
 
         if isinstance(obj, dict) and att in obj:
             obj[att] = new_value
         else:
             setattr(obj, att, new_value)
 
     # TODO: Create a method `DetectionPipeline.run`
-    def run_pipeline(self, abort_before: Optional[str] = None) -> "Processor":
+    def run_pipeline(self) -> None:
         """Run a pipeline with all its models in the right order.
 
-        Parameters
-        ----------
-        abort_before : str
-            model name, the pipeline should be aborted before this
-
-        Returns
-        -------
-        Processor
-            TBW.
-
         Notes
         -----
         The ``Processor`` instance with method '.run_pipeline' is modified.
         """
         self._log.info("Start pipeline")
 
-        # TODO: Use with-statement to set/unset ._is_running
-        self.pipeline._is_running = True
-
         for group_name in self.pipeline.model_group_names:
             # Get a group of models
             models_grp: Optional[ModelGroup] = getattr(self.pipeline, group_name)
 
             if models_grp:
                 self._log.info("Processing group: %r", group_name)
-
-                abort_flag = models_grp.run(
-                    detector=self.detector,
-                    pipeline=self.pipeline,
-                    abort_model=abort_before,
-                )
-                if abort_flag:
-                    break
-
-        self.pipeline._is_running = False
-
-        # TODO: Is is necessary to return 'self' ??
-        return self
+                models_grp.run(detector=self.detector)
 
     # TODO: Refactor '.result'. See #524. Deprecate this method ?
     @property
     def result(self) -> dict:
         """Return exposure pipeline final result in a dictionary."""
         if not self._result:
             raise ValueError("No result saved in the processor.")
```

### Comparing `pyxel_sim-1.9/pyxel/run.py` & `pyxel_sim-1.9.1/pyxel/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,14 @@
 
     Examples
     --------
     >>> import pyxel
     >>> pyxel.run("configuration.yaml")
     """
     # Late import to speedup start-up time
-    from pyxel.calibration import Calibration
 
     logging.info("Pyxel version %s", version)
     logging.info("Pipeline started.")
 
     start_time = time.time()
 
     configuration: Configuration = load(Path(input_filename).expanduser().resolve())
```

### Comparing `pyxel_sim-1.9/pyxel/show_versions.py` & `pyxel_sim-1.9.1/pyxel/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/state.py` & `pyxel_sim-1.9.1/pyxel/state.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/templates/_TEMPLATE.py` & `pyxel_sim-1.9.1/pyxel/templates/_TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/__init__.py` & `pyxel_sim-1.9.1/pyxel/util/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,47 +8,34 @@
 """Utility functions."""
 
 import logging
 
 
 import numpy as np
 
-from typing import Optional, Callable
+from typing import Callable
 
 # flake8: noqa
 from .memory import get_size, memory_usage_details
 from .examples import download_examples
 from .timing import time_pipeline
 from .add_model import create_model
-from .random import set_random_seed
+from .randomize import set_random_seed
 from .image import fit_into_array, load_cropped_and_aligned_image
 
 __all__ = [
     "convert_to_int",
     "round_convert_to_int",
-    "PipelineAborted",
     "LogFilter",
     "load_cropped_and_aligned_image",
     "set_random_seed",
     "deprecated",
 ]
 
 
-class PipelineAborted(Exception):
-    """Exception to force the pipeline to stop processing."""
-
-    def __init__(
-        self,
-        message: Optional[str] = None,
-        # errors=None
-    ):
-        super().__init__(message)
-        # self.errors = errors
-
-
 def round_convert_to_int(input_array: np.ndarray) -> np.ndarray:
     """Round list of floats in numpy array and convert to integers.
 
     Use on data before adding into DataFrame.
 
     :param input_array: numpy array object OR numpy array (float, int)
     :return:
```

### Comparing `pyxel_sim-1.9/pyxel/util/add_model.py` & `pyxel_sim-1.9.1/pyxel/util/add_model.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/examples.py` & `pyxel_sim-1.9.1/pyxel/util/examples.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/image.py` & `pyxel_sim-1.9.1/pyxel/util/image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/materials.py` & `pyxel_sim-1.9.1/pyxel/util/materials.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/memory.py` & `pyxel_sim-1.9.1/pyxel/util/memory.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/random.py` & `pyxel_sim-1.9.1/pyxel/util/randomize.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel/util/timing.py` & `pyxel_sim-1.9.1/pyxel/util/timing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/pyxel_sim.egg-info/PKG-INFO` & `pyxel_sim-1.9.1/pyxel_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-sim
-Version: 1.9
+Version: 1.9.1
 Summary: Pyxel detector simulation framework.
 Author-email: The Pyxel development team <pyxel@esa.int>
 License: MIT
 Project-URL: homepage, https://esa.gitlab.io/pyxel/
 Project-URL: documentation, https://esa.gitlab.io/pyxel/doc/
 Project-URL: repository, https://gitlab.com/esa/pyxel
 Project-URL: changelog, https://gitlab.com/esa/pyxel/-/releases
```

### Comparing `pyxel_sim-1.9/tests/calibration/test_check_ranges.py` & `pyxel_sim-1.9.1/tests/calibration/test_check_ranges.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/calibration/test_fitness.py` & `pyxel_sim-1.9.1/tests/calibration/test_fitness.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/calibration/test_slice_to_range.py` & `pyxel_sim-1.9.1/tests/calibration/test_slice_to_range.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/configuration/test_load.py` & `pyxel_sim-1.9.1/tests/configuration/test_load.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/configuration/test_schema.py` & `pyxel_sim-1.9.1/tests/configuration/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/conftest.py` & `pyxel_sim-1.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/data_structure/test_charge.py` & `pyxel_sim-1.9.1/tests/data_structure/test_charge.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/data_structure/test_processed_data.py` & `pyxel_sim-1.9.1/tests/data_structure/test_processed_data.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_ccd.py` & `pyxel_sim-1.9.1/tests/detectors/test_ccd.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_ccd_characteristics.py` & `pyxel_sim-1.9.1/tests/detectors/test_ccd_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_ccd_geometry.py` & `pyxel_sim-1.9.1/tests/detectors/test_ccd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_cmos.py` & `pyxel_sim-1.9.1/tests/detectors/test_cmos.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_cmos_characteristics.py` & `pyxel_sim-1.9.1/tests/detectors/test_cmos_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_cmos_geometry.py` & `pyxel_sim-1.9.1/tests/detectors/test_cmos_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_detectors.py` & `pyxel_sim-1.9.1/tests/detectors/test_detectors.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_environment.py` & `pyxel_sim-1.9.1/tests/detectors/test_environment.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_geometry.py` & `pyxel_sim-1.9.1/tests/detectors/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_mkid.py` & `pyxel_sim-1.9.1/tests/detectors/test_mkid.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_mkid_characteristics.py` & `pyxel_sim-1.9.1/tests/detectors/test_mkid_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/detectors/test_mkid_geometry.py` & `pyxel_sim-1.9.1/tests/detectors/test_mkid_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/exposure/test_readout.py` & `pyxel_sim-1.9.1/tests/exposure/test_readout.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/functional_tests/test_basic_exposure.py` & `pyxel_sim-1.9.1/tests/functional_tests/test_basic_exposure.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/functional_tests/test_parametric.py` & `pyxel_sim-1.9.1/tests/functional_tests/test_parametric.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/functional_tests/test_yaml.py` & `pyxel_sim-1.9.1/tests/functional_tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/inputs/test_image.py` & `pyxel_sim-1.9.1/tests/inputs/test_image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/model_tests/amplifier_crosstalk/test_crosstalk.py` & `pyxel_sim-1.9.1/tests/model_tests/amplifier_crosstalk/test_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_collection/test_fixed_pattern_noise.py` & `pyxel_sim-1.9.1/tests/models/charge_collection/test_fixed_pattern_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_collection/test_persistence.py` & `pyxel_sim-1.9.1/tests/models/charge_collection/test_persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_collection/test_simple_full_well.py` & `pyxel_sim-1.9.1/tests/models/charge_collection/test_simple_full_well.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_collection/test_simple_ipc.py` & `pyxel_sim-1.9.1/tests/models/charge_collection/test_simple_ipc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_collection/test_simple_persistence.py` & `pyxel_sim-1.9.1/tests/models/charge_collection/test_simple_persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_apd_gain.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_apd_gain.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_charge_deposition_in_MCT.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_charge_deposition_in_MCT.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_charge_injection.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_charge_injection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_dark_current.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_dark_current_rule07.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_dark_current_rule07.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_load_charge.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_load_charge.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_generation/test_photoelectrons.py` & `pyxel_sim-1.9.1/tests/models/charge_generation/test_photoelectrons.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_measurement/test_nghxrg.py` & `pyxel_sim-1.9.1/tests/models/charge_measurement/test_nghxrg.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_measurement/test_non_linearity.py` & `pyxel_sim-1.9.1/tests/models/charge_measurement/test_non_linearity.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_measurement/test_offset.py` & `pyxel_sim-1.9.1/tests/models/charge_measurement/test_offset.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_measurement/test_readout_noise.py` & `pyxel_sim-1.9.1/tests/models/charge_measurement/test_readout_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_measurement/test_reset_noise.py` & `pyxel_sim-1.9.1/tests/models/charge_measurement/test_reset_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_transfer/arctic_remove.py` & `pyxel_sim-1.9.1/tests/models/charge_transfer/arctic_remove.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_transfer/test_arctic_add.py` & `pyxel_sim-1.9.1/tests/models/charge_transfer/test_arctic_add.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_transfer/test_cdm.py` & `pyxel_sim-1.9.1/tests/models/charge_transfer/test_cdm.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/charge_transfer/test_emccd_poisson.py` & `pyxel_sim-1.9.1/tests/models/charge_transfer/test_emccd_poisson.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/data_processing/test_statistics.py` & `pyxel_sim-1.9.1/tests/models/data_processing/test_statistics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/phasing/test_pulse_processing.py` & `pyxel_sim-1.9.1/tests/models/phasing/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/photon_collection/test_illumination.py` & `pyxel_sim-1.9.1/tests/models/photon_collection/test_illumination.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/photon_collection/test_load_image.py` & `pyxel_sim-1.9.1/tests/models/photon_collection/test_load_image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/photon_collection/test_load_psf.py` & `pyxel_sim-1.9.1/tests/models/photon_collection/test_load_psf.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/photon_collection/test_optical_psf.py` & `pyxel_sim-1.9.1/tests/models/photon_collection/test_optical_psf.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/photon_collection/test_shot_noise.py` & `pyxel_sim-1.9.1/tests/models/photon_collection/test_shot_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/photon_collection/test_stripe_pattern.py` & `pyxel_sim-1.9.1/tests/models/photon_collection/test_stripe_pattern.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_ac_crosstalk.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_ac_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_dc_crosstalk.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_dc_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_dead_time_filter.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_dead_time_filter.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_get_matrix.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_get_matrix.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_phase_conversion.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_phase_conversion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_sar_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc_with_noise.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_sar_adc_with_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/readout_electronics/test_simple_adc.py` & `pyxel_sim-1.9.1/tests/models/readout_electronics/test_simple_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/models/test_save_load_detector.py` & `pyxel_sim-1.9.1/tests/models/test_save_load_detector.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/pipelines/observation/test_validate_steps.py` & `pyxel_sim-1.9.1/tests/pipelines/observation/test_validate_steps.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/pipelines/test_pipelines.py` & `pyxel_sim-1.9.1/tests/pipelines/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/running_mode/test_observation.py` & `pyxel_sim-1.9.1/tests/running_mode/test_observation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/test_evaluator.py` & `pyxel_sim-1.9.1/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/test_options.py` & `pyxel_sim-1.9.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/unittests/test_arguments.py` & `pyxel_sim-1.9.1/tests/unittests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/unittests/test_calibration.py` & `pyxel_sim-1.9.1/tests/unittests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/unittests/test_detector.py` & `pyxel_sim-1.9.1/tests/unittests/test_detector.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/unittests/test_environment.py` & `pyxel_sim-1.9.1/tests/unittests/test_environment.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/unittests/test_fitting.py` & `pyxel_sim-1.9.1/tests/unittests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/unittests/test_model_function.py` & `pyxel_sim-1.9.1/tests/unittests/test_model_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/util/test_fit_into_array.py` & `pyxel_sim-1.9.1/tests/util/test_fit_into_array.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/util/test_memory.py` & `pyxel_sim-1.9.1/tests/util/test_memory.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.9/tests/util/test_random.py` & `pyxel_sim-1.9.1/tests/util/test_random.py`

 * *Files identical despite different names*


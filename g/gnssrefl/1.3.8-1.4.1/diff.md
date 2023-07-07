# Comparing `tmp/gnssrefl-1.3.8.tar.gz` & `tmp/gnssrefl-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.8.tar", last modified: Thu May  4 13:57:01 2023, max compression
+gzip compressed data, was "gnssrefl-1.4.1.tar", last modified: Fri Jul  7 10:32:58 2023, max compression
```

## Comparing `gnssrefl-1.3.8.tar` & `gnssrefl-1.4.1.tar`

### file list

```diff
@@ -1,90 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.731013 gnssrefl-1.3.8/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/check_rinex_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.731013 gnssrefl-1.3.8/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   174227 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34303 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quicklib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/smoosh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58967 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.731013 gnssrefl-1.3.8/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 13:57:01.000000 gnssrefl-1.3.8/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:57:01.763013 gnssrefl-1.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-04 13:56:44.000000 gnssrefl-1.3.8/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.251297 gnssrefl-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 10:32:43.000000 gnssrefl-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-07 10:32:43.000000 gnssrefl-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 10:32:58.247297 gnssrefl-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-07 10:32:43.000000 gnssrefl-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.227297 gnssrefl-1.4.1/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/check_rinex_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.227297 gnssrefl-1.4.1/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/decipher_argt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16210 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33744 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnssir_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   182915 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28009 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nmea2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nyquist_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/nyquist_libs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34342 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19612 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16994 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickLook_function2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quicklib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50791 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/smoosh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/smoosh_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60208 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60672 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15493 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/vwc_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32905 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/xnmeasnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.227297 gnssrefl-1.4.1/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 10:32:58.000000 gnssrefl-1.4.1/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:32:58.251297 gnssrefl-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:32:58.247297 gnssrefl-1.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-07 10:32:44.000000 gnssrefl-1.4.1/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.8/LICENSE` & `gnssrefl-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/PKG-INFO` & `gnssrefl-1.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.8
+Version: 1.4.1
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.1** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
-Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
-The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
+Our documentation is available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
 
 [Youtube videos for beginners](https://www.youtube.com/channel/UCC1NW5oS7liG7C8NBK148Bg).
 
-New discussion page started about [modern GNSS signals](docs/pages/signal_issues.md).
+If you want to access CDDIS, including orbits, you should make [an account](https://urs.earthdata.nasa.gov/users/new).
+
+If you want to access to any Earthscope data, [an account is required](https://data-idm.unavco.org/user/profile/login).
 
 <HR> 
 
 GNSS-IR was developed with funding from NSF (ATM 0740515, EAR 0948957, AGS 0935725, EAR 1144221, AGS 1449554) and 
 NASA (NNX12AK21G and NNX13AF43G). <code>gnssrefl</code> was initially developed 
 as a fun post-retirement project, followed by support from NASA (80NSSC20K1731).
 
-This documentation was updated on March 24, 2023
+As of August 31, 2023, we will be an independent (unfunded) software package. Please help us maintain/improve this code. 
 
 Kristine M. Larson
 
+July 2, 2023
+
 <HR>
```

### Comparing `gnssrefl-1.3.8/README.md` & `gnssrefl-1.4.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # gnssrefl
 
-**github version: 1.3.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.1** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
-Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
-The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
+Our documentation is available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
 
 [Youtube videos for beginners](https://www.youtube.com/channel/UCC1NW5oS7liG7C8NBK148Bg).
 
-New discussion page started about [modern GNSS signals](docs/pages/signal_issues.md).
+If you want to access CDDIS, including orbits, you should make [an account](https://urs.earthdata.nasa.gov/users/new).
+
+If you want to access to any Earthscope data, [an account is required](https://data-idm.unavco.org/user/profile/login).
 
 <HR> 
 
 GNSS-IR was developed with funding from NSF (ATM 0740515, EAR 0948957, AGS 0935725, EAR 1144221, AGS 1449554) and 
 NASA (NNX12AK21G and NNX13AF43G). <code>gnssrefl</code> was initially developed 
 as a fun post-retirement project, followed by support from NASA (80NSSC20K1731).
 
-This documentation was updated on March 24, 2023
+As of August 31, 2023, we will be an independent (unfunded) software package. Please help us maintain/improve this code. 
 
 Kristine M. Larson
 
+July 2, 2023
+
 <HR>
```

### Comparing `gnssrefl-1.3.8/gnssrefl/EGM96.py` & `gnssrefl-1.4.1/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/check_rinex_file.py` & `gnssrefl-1.4.1/gnssrefl/check_rinex_file.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/computemp1mp2.py` & `gnssrefl-1.4.1/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/daily_avg.py` & `gnssrefl-1.4.1/gnssrefl/daily_avg.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 # start and end year
     minyear = int(min(tv[:,0])) ; maxyear = int(max(tv[:,0]))
     print('begin/end year: ', minyear, maxyear)
 # list of hte frequencies used
 
     flist = np.unique(tvall[:,6])
-    print(flist)
 
     if len(flist) == 0:
         print('There are no results.')
         return
 
     if len(flist) == 1:
         print('There is only one frequency in this file, so there is no point to computing a frequency bias.')
@@ -101,15 +100,15 @@
 
     Parameters
     ----------
     station : str
         station name, 4 ch, lowercase
 
     extension : str
-        folder extension - usually ''
+        folder extension - usually empty string 
 
     year1 : integer
         first year
 
     year2 : integer
         last year 
 
@@ -168,20 +167,22 @@
     fig,ax=plt.subplots()
     year_list = np.arange(year1, year2+1, 1)
     NumFiles = 0
     s1 = time.time()
     for yr in year_list:
         direc = xdir + '/' + str(yr) + '/results/' + station + '/' + extension + '/'
         if os.path.isdir(direc):
+            # i understand why python people like this - but then the results are not sorted ...
             all_files = os.listdir(direc)
+            all_files = np.sort(all_files)
             #print('Number of files in ', yr, len(all_files))
             for f in all_files:
                 fname = direc + f
                 L = len(f)
-        # file names must have 7 characters in them ... 
+        # file names must have 7 characters in them ...  and end in txt for that matter
                 if (L == 7):
                     NumFiles +=  1
         # check that it is a file and not a directory and that it has something/anything in it
                     try:
                         # trying to turn off the annoying empty file warnings
                         with warnings.catch_warnings():
                             warnings.simplefilter("ignore")
@@ -301,16 +302,19 @@
 
     # close the file with all the RH values 
     allrh.close()
 
 
     # plot the number of retrievals vs time
     txtdir =  xdir + '/Files/' + subdir 
-
-    daily_avg_stat_plots(obstimes,meanRH,meanAmp, station,txtdir,tv,ngps,nglo,ngal,nbei,test)
+    nr,nc = tv.shape
+    if nr > 0:
+        daily_avg_stat_plots(obstimes,meanRH,meanAmp, station,txtdir,tv,ngps,nglo,ngal,nbei,test)
+    else:
+        print('No results that met your criteria were found, so no need to make a plot')
 
     return tv, obstimes
 
 def daily_avg_stat_plots(obstimes,meanRH,meanAmp, station,txtdir,tv,ngps,nglo,ngal,nbei,test):
     """
     plots of results for the daily avg code
       
@@ -345,14 +349,15 @@
     nbei : numpy array
         number of beidou satellites each day
 
     test : bool
 
     """
 #   new plot
+
     fs = 12 # fontsize
     fig,ax=plt.subplots()
     ax.plot(obstimes,meanRH,'b.')
     fig.autofmt_xdate()
     plt.ylabel('Reflector Height (m)',fontsize=fs)
     today = str(date.today())
     plt.title(station.upper() + ': Daily Mean Reflector Height, Computed ' + today,fontsize=fs)
@@ -404,15 +409,16 @@
         plt.plot(obstimes, nglo,'r.',label='GLO',markersize=3)
     if (np.sum(ngal) > 0):
         plt.plot(obstimes, ngal,'.',label='GAL',color='orange',markersize=3)
     if (np.sum(nbei) > 0):
         plt.plot(obstimes, nbei,'.',label='BEI',color='green',markersize=3)
 
     #plt.legend(loc="upper left")
-    ax.legend(bbox_to_anchor=(1.02, 1.02))
+    #ax.legend(bbox_to_anchor=(1.02, 1.02))
+    plt.legend(loc="upper right")
     fig.autofmt_xdate()
     plt.title(station.upper() + ': Number of values used in the daily average',fontsize=fs)
     plt.xticks(fontsize=fs)
     plt.yticks(fontsize=fs)
     plt.grid()
     pltname = txtdir + '/' + station + '_nvals.png'
     plt.savefig(pltname)
@@ -433,16 +439,20 @@
     outfile : string
         full name of output file
 
     csvformat : boolean
         true if you want csv format output
 
     """
-    print('Daily average RH file written to: ', outfile)
     # sort the time tags
+    nr,nc = tv.shape
+    # nothing to write 
+    if (nr < 1):
+        return
+    print('Daily average RH file written to: ', outfile)
     ii = np.argsort(obstimes)
     # apply time tags to a new variable
     ntv = tv[ii,:]
     N,M = np.shape(ntv)
     xxx = str(datetime.datetime.now().strftime("%Y-%m-%d %H:%M"))
     fout = open(outfile, 'w+')
     #  header of a sorts
```

### Comparing `gnssrefl-1.3.8/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.4.1/gnssrefl/daily_avg_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def daily_avg(station: str , medfilter: float, ReqTracks: int, txtfile: str = None, plt: bool = True, 
-        extension: str = '', year1: int = 2005, year2: int = 2030, fr: int = 0, csv: bool = False, azim1: int = 0, azim2: int = 360, test: bool = False, subdir: str=None):
+        extension: str = '', year1: int = 2005, year2: int = 2030, fr: int = 0, csv: bool = False, 
+        azim1: int = 0, azim2: int = 360, test: bool = False, subdir: str=None):
     """
     The goal of this code is to consolidate individual RH results into a single file consisting of daily averaged RH without outliers.
 
     There are multiple optional choices as discussed below. The code also creates a file with all the subdaily RH as well.
 
     Examples
     -------- 
@@ -155,30 +156,32 @@
         alldatafile = txtdir + '/' + station + '_allRH.csv' 
     else:
         alldatafile = txtdir + '/' + station + '_allRH.txt' 
 
     tv, obstimes = da.readin_plot_daily(station, extension, year1, year2, fr, alldatafile, csv, medfilter, ReqTracks,azim1,azim2,test,subdir)
 
     # default is to show the plots
-    if plt2screen:
+    nr,nc = tv.shape
+    if plt2screen & (nr > 0):
         matplt.show()
 
     # now write out the result file:
 
     if txtfile is None:
         if csv:
             outfile = txtdir + '/' + station + '_dailyRH.csv' 
         else:
         # use default  filename for the average
             outfile = txtdir + '/' + station + '_dailyRH.txt' 
     else:
         # use filename provided by the user
         outfile = txtdir + '/' + txtfile
 
-    da.write_out_RH_file(obstimes, tv, outfile, csv)
+    if (nr > 0):
+        da.write_out_RH_file(obstimes, tv, outfile, csv)
 
 
 def main():
     args = parse_arguments()
     daily_avg(**args)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.4.1/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/download_ioc.py` & `gnssrefl-1.4.1/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/download_noaa.py` & `gnssrefl-1.4.1/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/download_orbits.py` & `gnssrefl-1.4.1/gnssrefl/download_orbits.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 
             gfr : GFZ rapid, GPS, Galileo and Glonass, since May 17 2021
 
             wum : (disabled) Wuhan, multi-GNSS, not rapid
 
             gnss2 : multi-GNSS, but uses IGN instead of CDDIS
 
+            gnss3 : multi-GNSS, but uses GFZ archive instead of CDDIS
+
             ultra : ultra orbits directly from GFZ
 
             rapid : rapid orbits directly from GFZ
 
     year : integer
         full year
     month : integer
@@ -91,16 +93,16 @@
         optional, allows multiple day download
 
     """
 
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
-    orbit_list = ['igs', 'igr', 'jax', 'grg', 'wum', 'gbm', 'nav', 'gps', 'gps+glo', 'gnss', 'gfr', 'esa', 'gnss2', 'ultra', 'rapid','nav-esa', 'nav-sopac','nav-cddis']
-
+    orbit_list = ['igs', 'igr', 'jax', 'grg', 'wum', 'gbm', 'nav', 'gps', 'gps+glo', 
+            'gnss', 'gfr', 'esa', 'gnss2', 'gnss3','ultra', 'rapid','nav-esa', 'nav-sopac','nav-cddis']
 
 #   assign to normal variables
     pCtr = orbit
 
     if len(str(year)) != 4:
         print('Year must have four characters: ', year)
         sys.exit()
@@ -114,17 +116,20 @@
         print(orbit_list)
         sys.exit()
 
     # if generic names used, we direct people to these orbit types
     if pCtr == 'gps':
         pCtr = 'nav'
 
-    # this is picked up from CDDIS
+    # try to avoid CDDIS. after 2022, just go to rapid. before that, more nuanced ....
     if pCtr == 'gnss':
-        pCtr = 'gbm'
+        if year >= 2022:
+            pCtr = 'gfr'
+        else:
+            pCtr = 'gnss3'
 
     if pCtr == 'gps+glo':
         pCtr = 'jax'
 
     # using gfz multi-gnss for rapid
     if pCtr == 'rapid':
         pCtr = 'gfr'
@@ -160,14 +165,17 @@
                     filename, fdir, foundit = g.getsp3file_flex(year, month, day, pCtr)
                 elif pCtr == 'gfr':
                 # rapid GFZ is available again ...
                     filename, fdir, foundit = g.rapid_gfz_orbits(year, month, day)
                 elif pCtr == 'ultra':
                     hour = 0 # for now only download hour 0 for ultra products
                     filename, fdir, foundit = g.ultra_gfz_orbits(year, month, day, hour)
+                elif pCtr == 'gnss3':
+                # use GFZ archive instead of CDDIS
+                    filename, fdir, foundit = g.gbm_orbits_direct(year, month, day)
                 elif pCtr == 'gnss2':
                 # use IGN instead of CDDIS
                     filename, fdir, foundit = g.avoid_cddis(year, month, day)
                 else:
                     filename, fdir, foundit = g.getsp3file_mgex(year, month, day, pCtr)
             if foundit:
                 print('SUCCESS:', fdir+'/'+filename)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/download_psmsl.py` & `gnssrefl-1.4.1/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/download_rinex.py` & `gnssrefl-1.4.1/gnssrefl/download_rinex.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,96 +17,90 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("station", help="station name", type=str)
     parser.add_argument("year", help="year", type=int)
     parser.add_argument("month", help="month (or day of year)", type=int)
     parser.add_argument("day", help="day (zero if you use day of year earlier)", type=int)
     # optional arguments
     parser.add_argument("-rate", default='low', metavar='low', type=str, help="sample rate: low or high")
-    parser.add_argument("-archive", default=None, 
-                        help="archive name", type=str)
+    parser.add_argument("-archive", default=None, help="archive name", type=str)
     parser.add_argument("-version", default=None, metavar=2, type=int, help="rinex version (2 or 3)")
-    parser.add_argument("-strip", default=None, type=str,
-                        help="set to True to strip to only SNR observables, gfzrnx used")
+    parser.add_argument("-strip", default=None, type=str, help="set to True to strip to only SNR observables, gfzrnx used")
     parser.add_argument("-doy_end", default=None, type=int, help="last day of year to be downloaded")
-    parser.add_argument("-stream", default=None, type=str,
-                        help="set to True to get stream-defined Rinex3 filename. I know. I know. It is annoying.")
+    parser.add_argument("-stream", default=None, type=str, help="set to True to get stream-defined Rinex3 filename. I know. I know. It is annoying.")
     parser.add_argument("-samplerate", default=None, type=int, help="Sample rate in seconds. For RINEX3 only.")
-    parser.add_argument("-debug", default=None, type=str, help="debugging flag for printout. default is False")
+    parser.add_argument("-screenstats", default=None, type=str, help="debugging flag for printout. default is False")
     parser.add_argument("-dec", default=None, type=int, help="decimation value (seconds). Only for RINEX 3.")
     parser.add_argument("-save_crx", default=None, type=str, help="Save crx version. Only for RINEX 3.")
-    parser.add_argument("-bkg", default=None, type=str, help="bkg directory, only for highrate RINEX 3.")
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['strip','debug','save_crx']
+    boolean_args = ['strip','screenstats','save_crx']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def download_rinex(station: str, year: int, month: int, day: int, rate: str = 'low', archive: str = None,
-                   version: int = 2, strip: bool = False, doy_end: 
-                   int = None, stream: str = 'R', samplerate: int = 30, 
-                   debug: bool = False, dec: int = 1, save_crx: bool = False, bkg: str = None ):
+def download_rinex(station: str, year: int, month: int, day: int, rate: str = 'low', archive: str = 'all',
+                   version: int = 2, strip: bool = False, doy_end: int = None, stream: str = 'R', samplerate: int = 30, 
+                   screenstats : bool = False, dec: int = 1, save_crx: bool = False ):
     """
     Command line interface for downloading RINEX files from global archives.
     Required inputs are station, year, month, and day. If you want to use day of year,
     call it as station, year, doy, 0.
 
-    Example:
-
-    download_rinex mfle 2015 1 1 
+    decimate does not seem to do anything, at least not for RINEX 2.11 files
 
-    Using day of year instead of month/day:
+    bkg option is changed.  now must specify bkg-igs or bkg-euref
 
-    download_rinex mfle 2015 52 0
+    Examples
+    --------
 
-    RINEX 2.11 Files
+    download_rinex mfle 2015 1 1 
+        downloads January 1, 2015
 
-    If you want to specify an archive:
+    download_rinex mfle 2015 52 0
+        Using day of year instead of month/day:
 
     download_rinex p101 2015 52 0 -archive sopac
-
-    RINEX 3 instructions need to be added.
-
-    decimate does not seem to do anything, at least not for RINEX 2.11 files
+        checks only sopac archive
 
     Parameters
     ----------
     station : str
         4 or 9 character ID of the station.
 
     year : int
-        Year
+        full Year
 
     month : int
         month
 
     day : int
-        day
+        day of month
 
     rate : str, optional
         sample rate. value options:
 
             low (default) : standard rate data
 
             high : high rate data
 
     archive : str, optional
         Select which archive to get the files from.
         Default is redirected to all, as defined below. Value options:
 
-            cddis : (NASA's Archive of Space Geodesy Data)
-
+            cddis : (NASA)
 
             bev : (Austria Federal Office of Metrology and Surveying)
 
-            bkg : (German Agency for Cartography and Geodesy)
+            bkg-igs : igs folder of BKG (German Agency for Cartography and Geodesy)
+
+            bkg-euref : Euref folder of BKG (German Agency for Cartography and Geodesy)
 
             bfg : (German Agency for water research, only Rinex 3)
 
             ga : (Geoscience Australia)
 
             gfz : (GFZ)
 
@@ -128,15 +122,15 @@
 
             unavco : now earthscope
 
             all : (searches unavco, sopac, and sonel in that order)
 
     version : int, optional
         Version of Rinex file. Default is 2.
-        Value options  2 or 3 
+        Value options 2 or 3 
 
     strip : bool, optional
         Whether to strip only SNR observables.  Uses teqc or gfzrnx.
         Default is False.
 
     doy_end : int, optional
         End day of year to be downloaded. 
@@ -146,52 +140,61 @@
         Whether to get stream 'S' defined filenames.
         Default is 'R'. 
 
     samplerate : int, optional
         Sample rate in seconds for RINEX3 only.
         Default is 30.
 
-    debug : bool, optional
+    screenstats : bool, optional
         provides screen output helpful for debugging
         Default is False
 
     dec : int, optional
         some highrate file downloads allow decimation. Default is 1 sec, i.e. no decimation
 
     save_crx : bool, option
         saves crx version for Rinex3 downloads. Otherwise they are deleted.
 
-    bkg : str, optional
-        tells you which directory the files live in, EUREF or IGS
-        Default is EUREF.
     """
 
 #   make sure environment variables exist.  set to current directory if not
+
     g.check_environ_variables()
+    debug = screenstats
 
-    if bkg is None:
-        bkg = 'EUREF'
-    else:
-        bkg = bkg.upper()
+
+    if 'bkg' in archive:
+        if (archive == 'bkg'):
+            print('You have not specified which BKG archive you want.')
+            print('You must select bkg-igs or bkg-euref.')
+            sys.exit()
+        if 'euref' in archive:
+            bkg = 'EUREF'
+        else:
+            bkg = 'IGS'
+        # change archive name back to original
+        archive = 'bkg'
 
     if len(str(year)) != 4:
         print('Year must have four characters: ', year)
         sys.exit()
 
     month, day, doy, cyyyy, cyy, cdoy = g.ymd2ch(year,month,day)
 
     # allowed archives, rinex 2.11
     # not really sure bev, gfz, bkg work ???
-    archive_list = ['bkg','bfg','bev','cddis', 'ga', 'gfz', 'jeff', 'ngs', 'nrcan', 'nz','sonel','sopac','special', 'unavco', 'all','unavco2']
+    archive_list = ['bkg','bfg','bev','cddis', 'ga', 'gfz', 'jeff', 'ngs', 
+            'nrcan', 'nz','sonel','sopac','special', 'unavco', 'all','unavco2']
 
     # removed the all archive
-    archive_list_high = ['unavco', 'nrcan', 'cddis','ga','bkg']  # though it is confusing because some are rinex 2.11 and others 3
+    # removed cddis because it is too slow
+    archive_list_high = ['bkg','unavco', 'nrcan', 'ga']  # though it is confusing because some are rinex 2.11 and others 3
 
     # archive list for rinex3 lowrate files
-    archive_list_rinex3 = ['unavco', 'cddis', 'ga', 'bev', 'bkg', 'ign', 'epn', 'bfg','sonel','all','unavco2','nrcan','gfz']
+    archive_list_rinex3 = ['unavco', 'bkg','cddis', 'ga', 'bev', 'ign', 'epn', 'bfg','sonel','all','unavco2','nrcan','gfz']
 
     if doy_end is None:
         doy_end = doy
 
     NS = len(station)
 
     if NS == 9:
@@ -246,40 +249,43 @@
             archive = 'unavco'
 
         if archive not in archive_list_high:
             print('You picked an archive that is not supported by my code. Exiting')
             sys.exit()
 
     if (rate == 'high') and (version == 3):
-        if ((archive == 'cddis') or (archive == 'bkg')) or (archive == 'ga'):
+        if (archive == 'bkg') or (archive == 'ga'):
             print('Highrate RINEX 3 is supported - but it is very slow. Pick up a cup of coffee.')
         else:
             print('I do not support RINEX 3 high rate downloads from your selected archive.')
             sys.exit()
 
     for d in range(doy, doy_end+1):
         # RINEX Version 3
         if version == 3:
             print('Request ', station, year, d, archive, samplerate, stream)
             if rate == 'high':
                 if archive == 'cddis':
-                    print('seek highrate data at CDDIS')
+                    if debug:
+                        print('seek highrate data at CDDIS')
                     ch.cddis_highrate(station, year, d, 0, stream, 1)
                 if archive == 'bkg':                               
-                    print('seek highrate data at BKG')
+                    if debug:
+                        print('seek highrate data at BKG')
                     rnx_filename,foundit = ch.bkg_highrate(station, year, d, 0,stream,dec,bkg)
                 if archive == 'ga':
-                    print('seek highrate data at GA')
+                    if debug:
+                        print('seek highrate data at GA')
                     deleteOld = True
                     r2, foundit = g.ga_highrate(station,year,d,dec,deleteOld)
             else:
                 if archive == 'all':
-                    file_name, foundit = k.universal_all(station, year, d, samplerate, stream)
+                    file_name, foundit = k.universal_all(station, year, d, samplerate, stream,debug)
                     if not foundit:
-                        file_name, foundit = k.universal_all(station, year, d, samplerate, k.swapRS(stream))
+                        file_name, foundit = k.universal_all(station, year, d, samplerate, k.swapRS(stream),debug)
                 else:
                     file_name, foundit = k.universal(station, year, d, archive, samplerate, stream,debug)
                     if not foundit:
                         file_name, foundit = k.universal(station, year, d, archive, samplerate, k.swapRS(stream),debug)
                 if foundit: 
                     print('\n SUCCESS 1: ', file_name)
                     deletecrx = not save_crx
@@ -292,20 +298,21 @@
             # using new karnak code
             rinexfile, rinexfiled = g.rinex_name(station, year, d, 0)
             if rate == 'high':
                 rinexfile, foundit = k.rinex2_highrate(station, year, d, archive, strip)
             else:
                 if archive == 'all':
                     foundit = False
-                    print('cycle thru unavco,sopac,sonel archives')
+                    if debug:
+                        print('cycle thru unavco,sopac,sonel archives')
                     for archiveinput in ['unavco', 'sopac', 'sonel']:
                         if not foundit:
-                            file_name, foundit = k.universal_rinex2(station, year, d, archiveinput)
+                            file_name, foundit = k.universal_rinex2(station, year, d, archiveinput,debug)
                 else:
-                    file_name, foundit = k.universal_rinex2(station, year, d, archive)
+                    file_name, foundit = k.universal_rinex2(station, year, d, archive, debug)
                 if foundit:  # uncompress and make o files ...
                     rinexfile, foundit = k.make_rinex2_ofiles(file_name)  # translate
 
             if foundit:
                 print('SUCCESS:', rinexfile, ' was found')
             else:
                 print('FAILURE:', rinexfile, ' was not found')
```

### Comparing `gnssrefl-1.3.8/gnssrefl/download_teqc.py` & `gnssrefl-1.4.1/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/download_tides.py` & `gnssrefl-1.4.1/gnssrefl/download_tides.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,42 +35,45 @@
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 def download_tides(station: str, network : str, date1: str = None, date2: str = None, output: str = None, plt: bool = False, datum: str = 'mllw', subdir: str = None):
     """
     Downloads tide gauge data from four different networks (see below)
 
-    Output is written to REFL_CODE/Files/ unless subdir optional input is set
-    Plot is sent to the screen if requested.
+    Output is written to REFL_CODE/Files/ unless subdir optional input is set. Plot is sent to the screen if requested.
 
     Examples
     --------
 
     download_tides 8768094 noaa 20210101 20210131
+        NOAA station 876094
 
     download_tides thul ioc 20210101 20210131
+        IOC station thul
 
     download_tides 5970026 wsv 
+        WSV station 5970026
 
     download_tides 10313 psmsl
+        PSMSL station 10313 (downloads one file)
 
     Parameters 
     ----------
     station : str
         station name
     network : str
         name of tide network. Options:
 
             noaa : US NOAA
 
             ioc : UNESCO
 
-            wsv : Germany
+            wsv : Germany, Wasserstrassen-und Schifffahrtsverwaltung
 
-            psmsl : Perm Service Mean Sea Level
+            psmsl : Permanent Service Mean Sea Level
 
     date1 : str, optional
         start date, 20150101, needed for NOAA/IOC
     date2 : str,optional
         end date, 20150110, needed for NOAA/IOC
     output : str, optional
         Optional output filename
```

### Comparing `gnssrefl-1.3.8/gnssrefl/download_unr.py` & `gnssrefl-1.4.1/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/download_wsv.py` & `gnssrefl-1.4.1/gnssrefl/download_wsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,22 @@
     # set up the address for the API call
     xdir = os.environ['REFL_CODE']
     outputdir = xdir + '/Files'  
     if not os.path.isdir(outputdir):
         print('making ', outputdir)
         subprocess.call(['mkdir',outputdir])
 
-    newurl = 'https://www.pegelonline.wsv.de/webservices/rest-api/v2/stations/' + station + '/W/measurements.json?start=P15D'
+    newurl = 'https://www.pegelonline.wsv.de/webservices/rest-api/v2/stations/' + station + '/W/measurements.json?start=P30D'
 
     data = requests.get(newurl).json()
 
     N= len(data)
+    if (N <= 2) :
+        print(data)
+        sys.exit()
     thetime = []; sealevel = [] ; obstimes = [] ; pt = 0
     if output is None:
         # use default
         outfile = outputdir + '/' + station + '.txt'
     else:
         outfile = outputdir + '/' + output
```

### Comparing `gnssrefl-1.3.8/gnssrefl/filesizes.py` & `gnssrefl-1.4.1/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/gnssir.py` & `gnssrefl-1.4.1/gnssrefl/gnssir.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,22 @@
     snr_type : integer
         snr file type
 
     extension : string
         optional subdirectory to save results
 
     lsp : dictionary
-        REQUIRES DESCRIPTION
+        e1 : float
+            min elev angle, deg
+        e2 : float
+            max elev angle, deg
+        NReg : list of floats
+            noise region for RH peak2noise , meters
+        azval : list of floats
+            pairs of azimuth regions, i.e. [0 90 90 180]
         
     """
 
     #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
     # this is also checked in the command line - but for people calling the code ...
@@ -63,14 +70,15 @@
     plot_screen = lsp['plt_screen'] 
     onesat = lsp['onesat']; screenstats = lsp['screenstats']
     gzip = lsp['gzip']
     if 'dec' in lsp.keys():
         dec = lsp['dec']
     else:
         dec = 1 # so Jupyter notebooks do not need to be rewritten
+
     #print('Decimate:', dec)
     #print('Number of azimuths', len(azval))
     for i in range(0,len(azval),2):
         #print(i, azval[i], azval[i+1])
         if (azval[i+1] - azval[i]) > 100:
             print('FATAL WARNING: You are prohibited from having an azimuth range that is larger than 100 degrees.')
             print('Azimuth values:', azval[i], azval[i+1])
@@ -83,15 +91,16 @@
     ann = g.make_nav_dirs(year) # make sure directories are there for orbits
     g.result_directories(station,year,extension) # make directories for the LSP results
 
    # this defines the minimum number of points in an arc.  This depends entirely on the sampling
    # rate for the receiver, so you should not assume this value is relevant to your case.
     minNumPts = 20
     p,T,irefr = set_refraction_params(station, dmjd, lsp)
-    #print(p,T)
+    print('refraction ', irefr)
+    print(p,T)
 
 # only doing one day at a time for now - but have started defining the needed inputs for using it
     twoDays = False
     obsfile2= '' # dummy value for name of file for the day before, when we get to that
     fname, resultExist = g.LSPresult_name(station,year,doy,extension) 
     #print('Results are written to:', fname)
 
@@ -167,15 +176,15 @@
                             if lsp['mmdd']:
                                 ctime = g.nicerTime(UTCtime); ctime2 = ctime[0:2] + ' ' + ctime[3:5]
                                 fout.write(" {0:4.0f} {1:3.0f} {2:6.3f} {3:3.0f} {4:6.3f} {5:6.2f} {6:6.2f} {7:6.2f} {8:6.2f} {9:4.0f} {10:3.0f} {11:2.0f} {12:8.5f} {13:6.2f} {14:7.2f} {15:12.6f} {16:1.0f} {17:2.0f} {18:2.0f} {19:5s} \n".format(year,doy,maxF,satNu, UTCtime, avgAzim,maxAmp,eminObs,emaxObs,Nv, f,riseSet, Edot2, maxAmp/Noise, delT, MJD,irefr,month,day,ctime2)) 
                             else:
                                 fout.write(" {0:4.0f} {1:3.0f} {2:6.3f} {3:3.0f} {4:6.3f} {5:6.2f} {6:6.2f} {7:6.2f} {8:6.2f} {9:4.0f} {10:3.0f} {11:2.0f} {12:8.5f} {13:6.2f} {14:7.2f} {15:12.6f} {16:1.0f} \n".format(year,doy,maxF,satNu, UTCtime, avgAzim,maxAmp,eminObs,emaxObs,Nv, f,riseSet, Edot2, maxAmp/Noise, delT, MJD,irefr)) 
                             gj +=1
                             if screenstats:
-                                print('Writing out ', np.round(Edot2,3), np.round(avgEdot,3))
+                                #print('Writing out ', np.round(Edot2,3), np.round(avgEdot,3))
                                 T = g.nicerTime(UTCtime)
                                 print('SUCCESS Azimuth {0:3.0f} Sat {1:3.0f} RH {2:7.3f} m PkNoise {3:4.1f} Amp {4:4.1f} Fr{5:3.0f} UTC {6:5s} DT {7:3.0f} '.format(iAzim,satNu,maxF,maxAmp/Noise,maxAmp, f,T,round(delT)))
                             if plot_screen:
                                 failed = False
                                 local_update_plot(x,y,px,pz,ax1,ax2,failed)
                         else:
                             rj +=1
```

### Comparing `gnssrefl-1.3.8/gnssrefl/gnssir_cl.py` & `gnssrefl-1.4.1/gnssrefl/gnssir_cl.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import argparse
 import os
 import subprocess
 import sys
 import wget
 
 import gnssrefl.gnssir as guts
+import gnssrefl.gnssir_v2 as guts2
 import gnssrefl.gps as g
 
 from gnssrefl.utils import str2bool
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
@@ -33,148 +34,166 @@
     parser.add_argument("-gzip", default=None, type=str, help="Boolean, gzip SNR files after use")
     parser.add_argument("-screenstats", default=None, type=str, help="Boolean, some stats printed to screen(default is False)")
     parser.add_argument("-delTmax", default=None, type=int, help="Allowed satellite arc length (minutes)")
     parser.add_argument("-e1", default=None, type=float, help="min elev angle (deg)")
     parser.add_argument("-e2", default=None, type=float, help="max elev angle (deg)")
     parser.add_argument("-mmdd", default=None, type=str, help="Boolean, add columns for month,day,hour,minute")
     parser.add_argument("-dec", default=1, type=int, help="decimate SNR file to this sampling rate before computing periodograms")
+    parser.add_argument("-newarcs", default=None, type=str, help="Default is true. set to F to use old way of defining arcs")
 
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['plt', 'screenstats', 'nooverwrite', 'compress', 'screenstats', 'mmdd','gzip']
+    boolean_args = ['plt', 'screenstats', 'nooverwrite', 'compress', 'screenstats', 'mmdd','gzip','newarcs']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def gnssir(station: str, year: int, doy: int, snr: int = 66, plt: bool = False, fr: int = None,
-           ampl: float = None, sat: int = None, doy_end: int = None, year_end: int = None,
-           azim1: int = 0, azim2: int = 360, nooverwrite: bool = False, extension: str = '',
-           compress: bool = False, screenstats: bool = False, delTmax: int = None,
-           e1: float = None, e2: float = None, mmdd: bool = False, gzip: bool = False, dec : int = 1):
+def gnssir(station: str, year: int, doy: int, snr: int = 66, plt: bool = False, fr: int = None, 
+        ampl: float = None, sat: int = None, doy_end: int = None, year_end: int = None, azim1: int = 0, 
+        azim2: int = 360, nooverwrite: bool = False, extension: str = '', compress: bool = False, 
+        screenstats: bool = False, delTmax: int = None, e1: float = None, e2: float = None, 
+        mmdd: bool = False, gzip: bool = False, dec : int = 1, newarcs : bool = True ):
     """
-        gnssir is the main driver for estimating Reflector Heights
-        The user is required to have set up an analysis strategy using "make_json_input" 
+    gnssir is the main driver for estimating reflector heights. The user is required to 
+    have set up an analysis strategy using gnssir_input. 
+
+    Older json versions created by make_json_input will be allowed as long as you set -newarcs F
+
         
-        Examples
-        --------
-        gnssir p041 2021 15 
-            analyzes the data for station p041, year 2021 and day of year 15.
-        gnssir p041 2021 15  -snr 99
-            uses SNR files with a 99 suffix
-        gnssir p041 2021 15  -snr 99 -screenstats T
-            sends debugging information to the screen
-        gnssir p041 2021 15  -nooverwrite T 
-            only runs gnssir if there isn't a previous solution
-        gnssir p041 2021 15  -doy_end 20 
-            Analyzes data from day of year 15 to day of year 20
-
-        Parameters
-        ----------
-        station : str
-            lowercase 4 character ID of the station
-        year : int
-            full Year
-        doy : integer
-            Day of year
-        snr : int, optional
-            SNR format. This tells the code what elevation angles to save data for. Will be the snr file ending.
-            value options:
-                66 (default) : saves all data with elevation angles less than 30 degress
-
-                99 : saves all data with elevation angles between 5 and 30 degrees
-
-                88 : saves all data 
-
-                50 : saves all data with elevation angles less than 10 degrees
-
-        plt : bool, optional
-            Send plots to screen or not. Default is False.
-        fr : int, optional
-            GNSS frequency. Value options:
-                1,2,20,5 : GPS L1, L2, L2C, L5
-
-                101,102 : GLONASS L1, L2
-
-                201, 205,206,207,208 : GALILEO E1, E5a,E6,E5b,E5
-
-                302,306,307 : BEIDOU B1, B3, B2
-
-        ampl : float, optional
-            minimum spectral peak amplitude.
-            default is None
-
-        sat : int, optional
-            satellite number to only look at that single satellite.
-            default is None.
-
-        doy_end : int, optional
-            end day of year. This is to create a range from doy to doy_end of days.
-            If year_end parameter is used - then day_end will end in the day of the year_end.
-            Default is None. (meaning only a single day using the doy parameter)
-
-        year_end : int, optional
-            end year. This is to create a range from year to year_end to get the snr files for more than one year.
-            doy_end will be for year_end.
-            Default is None.
-
-        azim1 : int, optional
-            lower limit azimuth.
-            If the azimuth angles are changed in the json (using 'azval' key) and not here, then the json overrides these.
-            If changed here, then it overrides what you requested in the json.
-            default is 0.
-        azim2 : int, optional
-            upper limit azimuth.
-            If the azimuth angles are changed in the json (using 'azval' key) and not changed here, then the json overrides these.
-            If changed here, then it overrides what you requested in the json.
-            default is 360.
-        nooverwrite : bool, optional
-            Use to overwrite lomb scargle result files or not.
-            Default is True (do not overwrite files).
-        extension : string, optional
-            extension for result file, useful for testing strategies.
-            default is ''. (empty string)
-        compress : boolean, optional
-            xz compress SNR files after use.
-            default is False.
-        screenstats : bool, optional
-            whether to print stats to the screen or not.
-            default is True.
-        delTmax : int, optional
-            maximum satellite arc length in minutes. Set in make_json_input
-        e1 : float, optional
-            use to override the minimum elevation angle.
-        e2 : float, optional
-            use to override the maximum elevation angle.
-        mmdd : boolean, optional
-            adds columns in results for month, day, hour, and minute.
-            default is False.
-        gzip : boolean, optional
-            gzip compress SNR files after use.
-            default is False.
-        dec : int, optional
-            decimate SNR file to this sampling period before the 
-            periodograms are computed. 1 sec is default (i.e. no decimating)
+    Examples
+    --------
+    gnssir p041 2021 15 
+        analyzes the data for station p041, year 2021 and day of year 15.
+        uses new way of defining arcs
+    gnssir p041 2021 15  -snr 99
+        uses SNR files with a 99 suffix
+        uses new way of defining arcs
+    gnssir p041 2021 15  -snr 99 -screenstats T
+        sends debugging information to the screen
+        uses new way of defining arcs
+    gnssir p041 2021 15  -nooverwrite T 
+        only runs gnssir if there isn't a previous solution
+        uses new way of defining arcs
+    gnssir p041 2021 15  -doy_end 20 
+        Analyzes data from day of year 15 to day of year 20
+        uses new way of defining arcs
+    gnssir p041 2021 15  -newarcs F
+        uses old way of picking arcs 
+
+    Parameters
+    ----------
+    station : str
+        lowercase 4 character ID of the station
+    year : int
+        full Year
+    doy : integer
+        Day of year
+    snr : int, optional
+        SNR format. This tells the code what elevation angles to save data for. Input is the snr file ending.
+        Value options:
+
+            66 (default) : saves all data with elevation angles less than 30 degress
+
+            99 : saves all data with elevation angles between 5 and 30 degrees
+
+            88 : saves all data 
+
+            50 : saves all data with elevation angles less than 10 degrees
+
+    plt : bool, optional
+        Send plots to screen or not. Default is False.
+    fr : int, optional
+        GNSS frequency. Value options:
+
+            1,2,20,5 : GPS L1, L2, L2C, L5
+
+            101,102 : GLONASS L1, L2
+
+            201, 205,206,207,208 : GALILEO E1, E5a,E6,E5b,E5
+
+            302,306,307 : BEIDOU B1, B3, B2
+
+    ampl : float, optional
+        minimum spectral peak amplitude. default is None
+    sat : int, optional
+        satellite number to only look at that single satellite. default is None.
+    doy_end : int, optional
+        end day of year. This is to create a range from doy to doy_end of days.
+        If year_end parameter is used - then day_end will end in the day of the year_end.
+        Default is None. (meaning only a single day using the doy parameter)
+    year_end : int, optional
+        end year. This is to create a range from year to year_end to get the snr files for more than one year.
+        doy_end will be for year_end. Default is None.
+    azim1 : int, optional
+        lower limit azimuth.
+        If the azimuth angles are changed in the json (using 'azval' key) and not here, then the json overrides these.
+        If changed here, then it overrides what you requested in the json. default is 0.
+    azim2 : int, optional
+        upper limit azimuth.
+        If the azimuth angles are changed in the json (using 'azval' key) and not changed here, then the json overrides these.
+        If changed here, then it overrides what you requested in the json. default is 360.
+    nooverwrite : bool, optional
+        Use to overwrite lomb scargle result files or not.
+        Default is True (do not overwrite files).
+    extension : string, optional
+        extension for result file, useful for testing strategies. default is empty string
+    compress : boolean, optional
+        xz compress SNR files after use. default is False.
+    screenstats : bool, optional
+        whether to print stats to the screen or not. default is True.
+    delTmax : int, optional
+        maximum satellite arc length in minutes. Set in make_json_input
+    e1 : float, optional
+        use to override the minimum elevation angle.
+    e2 : float, optional
+        use to override the maximum elevation angle.
+    mmdd : boolean, optional
+        adds columns in results for month, day, hour, and minute. default is False.
+    gzip : boolean, optional
+        gzip compress SNR files after use. default is False.
+    dec : int, optional
+        decimate SNR file to this sampling period before the 
+        periodograms are computed. 1 sec is default (i.e. no decimating)
+    newarcs : bool, optional
+        default is to use new way to do rising and setting arcs.
+        if you want to use old way, set newarcs to False
 
     """
 
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
     exitS = g.check_inputs(station, year, doy, snr)
 
     if exitS:
         sys.exit()
 
     lsp = guts.read_json_file(station, extension)
     # now check the overrides to the json instructions
 
+    if newarcs:
+        if 'azval2' not in lsp:
+            print('An azval2 variable was not found in your json. Fix your json ')
+            print('and/or use gnssir_input to make a new one. Exiting')
+            sys.exit()
+
+    else:
+        if 'azval' in lsp:
+            print('An azval variable was found in your json. I will use the old way of defining arcs.')
+        else:
+            print('You chose the old way of setting arcs, but you do not have valid input in your json.')
+            print('I recommend you use gnssir_input to create your json file. Azimuth regions are no ')
+            print('longer required to be regions less than 100 degrees. Exiting.')
+            sys.exit()
+
+
     # plt is False unless user changes
     lsp['plt_screen'] = plt
 
     if delTmax is not None:
         lsp['delTmax'] = delTmax
 
     if ((lsp['maxH'] - lsp['minH']) < 5):
@@ -270,14 +289,15 @@
     args = {'station': station.lower(), 'year': year, 'doy': doy, 'snr_type': snr, 'extension': extension, 'lsp': lsp}
 
     year_list = list(range(year_st, year_end+1))
     # changed to better describe year and doy start/end
 
     print('requested frequencies ', lsp['freqs'])
 
+
     for year in year_list:
         # edits made 2021Sep10 by Makan karegar
         if year != year_end:
             doy_en = 366
         else:
             doy_en = doy_end
 
@@ -286,15 +306,20 @@
             doy_list = list(range(doy, doy_en+1))
         else:
             doy_list = list(range(1, doy_en+1))
 
         args['year'] = year
         for doy in doy_list:
             args['doy'] = doy
-            guts.gnssir_guts(**args)
+            if newarcs:
+                print('Using the New Way of Selecting Arcs')
+                guts2.gnssir_guts_v2(**args)
+            else:
+                print('Using the Old Way of Selecting Arcs')
+                guts.gnssir_guts(**args)
 
 
 def main():
     args = parse_arguments()
     gnssir(**args)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/gnsssnr.f` & `gnssrefl-1.4.1/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.4.1/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/gps.py` & `gnssrefl-1.4.1/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,21 +626,19 @@
     day : integer
 
     pCtr : string
         3 character orbit processing center
 
     Returns
     -------
-    name : string
+    name : str
         filename for the orbits
-
-    fdir : string
+    fdir : str
         directory for the orbits
-
-    fexist : boolean
+    fexist : bool
         whether the orbit file was successfully found
 
     """
     # really should use mgex version
     # returns name and the directory
     name, fdir = sp3_name(year,month,day,pCtr) 
     #print(name, fdir)
@@ -698,14 +696,15 @@
 
     fdir : str
         file directory
 
     foundit : bool
 
     """
+    screenstats = False # for now
     foundit = False
     # this returns sp3 orbit product name
     month, day, doy, cyyyy, cyy, cdoy = ymd2ch(year,month,day)
 
     name, fdir = sp3_name(year,month,day,pCtr) 
     gps_week = name[3:7]
     igps_week = int(gps_week)
@@ -737,43 +736,48 @@
 
      
     # this is the default setting - no file exists
     mgex = 0
     n1 = os.path.isfile(fdir + '/' + name)
     n1c = os.path.isfile(fdir + '/' + name + '.xz')
     if (n1 == True):
-        print('first kind of MGEX sp3file already exists online')
+        if screenstats:
+            print('first kind of MGEX sp3file already exists online')
         mgex = 1
         foundit = True
     elif (n1c  == True): 
-        print('xz first kind of MGEX sp3file already exists online-unxz it')
+        if screenstats:
+            print('xz first kind of MGEX sp3file already exists online-unxz it')
         fx =  fdir + '/' + name + '.xz'
         subprocess.call(['unxz', fx])
         mgex = 1
         foundit = True
 
     n2 = os.path.isfile(fdir + '/' + name2)
     n2c = os.path.isfile(fdir + '/' + name2 + '.xz')
     if (n2 == True):
-        print('MGEX sp3file already exists online')
+        if screenstats:
+            print('MGEX sp3file already exists online')
         mgex = 2 ; foundit = True
     elif (n2c == True):
-        print('MGEX sp3file already exists online')
+        if screenstats:
+            print('MGEX sp3file already exists online')
         mgex = 2 ; foundit = True
         fx =  fdir + '/' + name2 + '.xz'
         subprocess.call(['unxz', fx])
 
     if (mgex == 2):
         name = name2
     if (mgex == 1):
         name = file1[:-2]
 
     if not foundit:
-        print('Type 1 filename',file1)
-        print('Type 2 filename',file2)
+        if screenstats:
+            print('Type 1 filename',file1)
+            print('Type 2 filename',file2)
         if (mgex == 0):
             if not foundit:
                 name = file2[:-3] 
                 secure_file = file2
                 secure_dir = '/gps/products/mgex/' + str(igps_week) + '/'
                 foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
             if not foundit:
@@ -788,38 +792,33 @@
                 secure_dir = '/gps/products/' + str(igps_week) + '/'
                 foundit = orbfile_cddis(name, year, secure_file, secure_dir, file2)
 
     return name, fdir, foundit
 
 def orbfile_cddis(name, year, secure_file, secure_dir, file2):
     """
-    tries to download a file from a directory at CDDIS
-    file2 is like this: GFZ0MGXRAP_' + cyyyy + cdoy + '0000_01D_05M_ORB.SP3.gz
+    tries to download a file from a directory at CDDIS which 
     it then stores it the year directory (with a given name)
 
     Parameters
     ----------
-    name : string
+    name : str
         the name of the orbit file you want to download from CDDIS
-
-    year : integer
+    year : int
         full year
-
-    secure_file : string
+    secure_file : str
         name of the file at CDDIS
- 
-    secure_dir : string
+    secure_dir : str
         where the file lives at CDDIS
-
-    file2 : string
+    file2 : str
         name without the compression???
 
     Returns
     -------
-    foundit : boolean
+    foundit : bool
         whether the file was found
 
     now checks that file size is not zero. allows old file name downloads
 
     """
     # assume file was not found
     foundit = False
@@ -1533,23 +1532,23 @@
     return maxF, maxAmp, eminObs, emaxObs,riseSet, px,pz
 
 def window_data(s1,s2,s5,s6,s7,s8, sat,ele,azi,seconds,edot,f,az1,az2,e1,e2,satNu,pfitV,pele,screenstats):
     """
 
     window the SNR data for a given satellite azimuth and elevation angle range
 
-    also calculates the scale factor for various GNNS frequencies.  currently
+    also calculates the scale factor for various GNSS frequencies.  currently
     returns meanTime in UTC hours and mean azimuth in degrees
     cf, which is the wavelength/2
     currently works for GPS, GLONASS, GALILEO, and Beidou
     new: pele are the elevation angle limits for the polynomial fit. these are appplied
     before you start windowing the data
 
     Parameters
-    -----------
+    ----------
     s1 : numpy array 
         SNR L1 data, floats
     s2 : numpy array 
         SNR L2 data, floats 
     s5 : numpy array
         SNR L5 data
     s6 : numpy array floats
@@ -1564,38 +1563,38 @@
         elevation angle (Degrees)
     azi : numpy array
         azimuth angle (Degrees)
     seconds : numpy array
         seconds of the day (GPS time)
     edot : numpy array
         elev angle time rate of change (units?)
-    f : integer
+    f : int
         requested frequency
     az1 : float
         minimum azimuth limit, degrees
     az2 : float
         maximum azimuth limit, degrees
     e1 : float
         minimum elevation angle limit, degrees
     e2 : float
         maximum elevation angle limit, degrees
-    satNu : integer
+    satNu : int
         requested satellite number
-    pfitV : integer
+    pfitV : int
         polynomial order for DC fit
-    screenstats : boolean
+    screenstats : bool
         Whether statistics come to the screen
 
     Returns
     -------
     x : numpy array of floats 
         elevation angle, deg
     y : numpy array of floats
         SNR, db-Hz
-    Nvv : integer
+    Nvv : int
         number of points in x
     cf : float
         refl scale factor (lambda/2)
     meanTime : float
         UTC hour of the arc
     avgAzim : float
         average azimuth of the track (degrees)
@@ -1852,27 +1851,31 @@
     return pd
 
 def find_satlist_wdate(f,snrExist,year,doy):
     """
     find satellite list for a given frequency and date
 
     Parameters
-    -------------
+    ----------
     f : integer
         frequency
-
-    snrExist : boolean numpy array
+    snrExist : numpy array, bool
         tells you if a signal is (potentially) legal
+    year : int
+        full year
+    doy : int
+        day of year
 
     Returns
-    --------
+    -------
     satlist: numpy list of integers
         satellites to use
 
     june 24, 2021: updated for SVN78
+
     """
     # get list of relevant satellites
     l2c_sat, l5_sat = l2c_l5_list(year,doy)
 
     l1_sat = np.arange(1,33,1)
     satlist = []
     if f == 1:
@@ -1907,19 +1910,29 @@
     #    print('     illegal frequency: no sat list being returned')
     return satlist
 
 
 
 def glonass_channels(f,prn):
     """
-    inputs frequency and prn number
-    returns wavelength for glonass satellite in meters
-    logic from Simon Williams, matlab
-    converted to function by KL, 2017 November
-    converted to python by KL 2018 September
+    Retrieves appropriate wavelength for a given Glonass satellite
+
+    Parameters
+    ----------
+    f : int
+        frequency( 101 or 102)
+    prn : int
+        satellite number
+
+    Returns
+    -------
+    l : float
+        wavelength for glonass satellite in meters
+
+    logic from Simon Williams 
     """
 #   we define glonass by adding 100.  remove this for definition of the wavelength
     if (prn > 100):
         prn = prn - 100
     lightSpeed = 299792458
     slot = [14,15,10,20,19,13,12,1,6,5,22,23,24,16,4,8,3,7,2,18,21,9,17,11]
     channel = [-7,0,-7,2,3,-2,-1,1,-4,1,-3,3,2,-1,6,6,5,5,-4,-3,4,-2,4,0]
@@ -2003,18 +2016,18 @@
             sys.exit()
     frej = 100
 
     return fout, frej
 
 def removeDC(dat,satNu, sat,ele, pele, azi,az1,az2,edot,seconds):
     """
-#   remove direct signal using given elevation angle (pele) and azimuth 
+    remove direct signal using given elevation angle (pele) and azimuth 
     (az1,az2) constraints, return x,y as primary used data and windowed
     azimuth, time, and edot
-#   removed zero points, which 10^0 have value 1.  used 5 to be sure?
+    removed zero points, which 10^0 have value 1.  used 5 to be sure?
 
     Parameters
     ----------
     dat : numpy array of floats 
         SNR data
     satNu : float
         requested satellite number
@@ -2033,20 +2046,26 @@
     edot : numpy array of floats  
         derivative elevation angle (deg/sec)
     seconds : numpy array of floatas
         seconds of the day
 
     Returns
     -------
-    x
-    y
-    sat
-    azi
-    seconds
-    edot
+    x : numpy array of floats
+        sine of elevation angle ( i believed)
+    y : numpy array of floats
+        SNR data in lineer units with DC component removed
+    sat : ??
+        not sure why  this is sent and returned
+    azi : numpy array of flaots
+        azimuth angles
+    seconds : numpy array of flaots
+        seconds of the day
+    edot : numpy array of floats
+        derivative of elevation angle
 
     """
     p1 = pele[0]; p2 = pele[1]
 #   look for data within these azimuth and elevation angle constraints
     #ytest = dat[(sat == satNu)]
     #print(len(ytest))
 
@@ -2611,38 +2630,48 @@
     """
     months = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC']
     return months.index(month) + 1
 
 def char_month_converter(month):
     """
     integer month to 3 character month
+
+    Parameters 
+    ----------
+    month : int
+        integer month (1-12)
+
+    Returns 
+    ----------
+    month : str
+        three char month, uppercase
+
     """
     months = ['JAN', 'FEB', 'MAR', 'APR', 'MAY', 'JUN', 'JUL', 'AUG', 'SEP', 'OCT', 'NOV', 'DEC']
     return months[(month-1)]
 
 def UNR_highrate(station,year,doy):
     """
     picks up the 5 minute time series from UNR website for a given station
 
     Parameters
-    -----------
-    station : string
+    ----------
+    station : str
         4 character station name
+    year : int
+        full year
+    doy : int
+        day of year
 
-    year : integer
-
-    doy : integer
-
-    returns
-    -----------
-    filename : string
+    Returns
+    -------
+    filename : str
         output filename
-
-    goodDownload : boolean
-        whether you were successful
+    goodDownload : bool
+        whether your download was successful
 
     """
     yy,mm,dd, cyyyy, cdoy, YMD = ydoy2useful(year,doy)
     stationUP = station.upper()
     dirdir = 'ftp://gneiss.nbmg.unr.edu/rapids_5min/kenv/' + cyyyy + '/' + cdoy + '/'
     filename = YMD + station.upper() + '_fix.kenv'
     url = dirdir + filename
@@ -2661,15 +2690,15 @@
 
 def mjd_to_date(jd):
     """
     https://gist.github.com/jiffyclub/1294443
 
     Converts Modified Julian Day to y,m,d
     
-    Algorithm from 'Practical Astronomy with your Calculator or Spreadsheet', 
+    Algorithm from Practical Astronomy with your Calculator or Spreadsheet 
         4th ed., Duffet-Smith and Zwart, 2011.
     
     Parameters
     ----------
     jd : float
         Julian Day
         
@@ -2765,15 +2794,15 @@
 def rewrite_tseries(station):
     """
     given a station name, look at a daily blewitt position (ENV) 
     file and write a new file that is more human friendly
 
     Parameters
     ----------
-    station : string
+    station : str
         4 character station name
     """
     siteid = station.upper()
     # NA12 env time series
     fname = 'tseries/' + siteid + '.NA12.tenv3'
     fname_rapid = 'tseries/' + siteid + '.NA12.rapid.tenv3'
     outputfile = 'tseries/' + station+ '_na12.env'
@@ -2824,16 +2853,15 @@
         f.close()
     except:
         print('some problem writing the output')
 
 
 def llh2xyz(lat,lon,height):
     """
-    inputs lat,lon (in degrees) and ellipsoidal height (in meters)
-    returns Cartesian values in meters.
+    converts llh to Cartesian values
 
     Parameters
     -----------
     lat : float
         latitude in degrees
 
     lon : float
@@ -3010,14 +3038,15 @@
     if maxAmp < reqamp:
         print('     Obs Ampl {0:.1f} vs {1:.1f} required '.format(maxAmp,reqamp  ))
     if maxAmp/Noise < PkNoise:
         print('     Obs PkN  {0:.1f} vs {1:.1f} required'.format(maxAmp/Noise, PkNoise ))
         
 def define_quick_filename(station,year,doy,snr):
     """
+    defines SNR File name
 
     Parameters
     ----------
     station : str
         4 ch station name
     year : int
         full year
@@ -3025,15 +3054,15 @@
         day of year
     snr : int
         snr file type (66,88, etc)
 
     Returns 
     -------
     f : str
-        filename
+        SNR filename
 
     """
     cyyyy, cyy, cdoy = ydoych(year,doy)
     f= station + str(cdoy) + '0.' + cyy + '.snr' + str(snr)
     return f
 
 def update_quick_plot(station, f):
@@ -3057,26 +3086,26 @@
 
 def navfile_retrieve(navfile,cyyyy,cyy,cdoy):
     """
     retrieves navfile from either SOPAC or CDDIS
 
     Parameters 
     ----------
-    navfile : string
+    navfile : str
         name of the broadcast orbit file
-    cyyyy :  string
+    cyyyy :  str
         4 character yaer
     cyy : string
         2 character year
-    cdoy : string
+    cdoy : str
         3 character day of year
 
     Returns
     -------
-    FileExists : boolean
+    FileExists : bool
         whether the file was found
 
     """
     navname = navfile
     FileExists = False
     xx=get_sopac_navfile(navfile,cyyyy,cyy,cdoy) 
     
@@ -3258,22 +3287,22 @@
 
 def rinex_ga_highrate(station, year, month, day):
     """
     no longer supported - 
 
     Parameters
     ----------
-    station : string
+    station : str
         4 character station ID, lowercase
-
-    year : integer
-
-    month : integer
-
+    year : int
+        full year
+    month : int
+        calendar month
     day : integer
+        day of the month
 
     """
     crnxpath = hatanaka_version()
     teqcpath = teqc_version()
     alpha='abcdefghijklmnopqrstuvwxyz'
     # if doy is input
     if day == 0:
@@ -3335,14 +3364,15 @@
             subprocess.call(['mv',foutname,rinexname])
     else:
         print('No files were available for you from GA.')
 
 
 def highrate_nz(station, year, month, day):
     """
+    NO LONGER SUPPORTED 
     picks up a high-rate RINEX 2.11 file from GNS New zealand
     requires teqc to convert/merge the files
 
     Parameters
     ----------
     station : str
         station name
@@ -3393,57 +3423,65 @@
 def get_orbits_setexe(year,month,day,orbtype,fortran):
     """
     picks up and stores orbits as needed
     also sets executable location for translation (gpsonly vs multignss)
 
     Parameters
     ----------
-    year : integer
-
-    month : integer
-
-    day : integer
-
-    orbtype : string
+    year : int
+        full year
+    month : int
+        calendar month
+    day : int
+        calendar day
+    orbtype : str
         orbit source, e.g. nav, gps...
-
-    fortran : boolean
-        whether you are using forran code for translation
+    fortran : bool
+        whether you are using fortran code for translation
 
     Returns
     -------
-    foundit : boolean
+    foundit : bool
         whether orbit file was found
-    f : string
+    f : str
         name of the orbit file
-    orbdir : string
+    orbdir : str
         location of the orbit file
-    snrexe : string 
+    snrexe : str 
         location of SNR executable. only relevant for fortran users
 
     """
     #default values
+    # if they ask for gnss or gnss3, always use rapid.
+    # at least for years 2022 and after
+    if year >= 2022:
+        if (orbtype == 'gnss') or (orbtype == 'gnss3'):
+            orbtype = 'rapid'
+        if orbtype == 'gbm':
+            orbtype = 'rapid'
+
     foundit = False
     f=''; orbdir=''
     # define directory for the conversion executables
     exedir = os.environ['EXE']
     if (orbtype == 'grg'):
         # French multi gnss, but there are no Beidou results
         f,orbdir,foundit=getsp3file_mgex(year,month,day,'grg')
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'gfr'):
-        print('uses rapid GFZ orbits, avail as of 2021/137, now pointing to local GFZ directory ')
         f,orbdir,foundit=rapid_gfz_orbits(year,month,day)
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'rapid'):
-        print('uses rapid GFZ orbits, avail as of 2021/137, now pointing to local GFZ directory ')
         f,orbdir,foundit=rapid_gfz_orbits(year,month,day)
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
+    elif (orbtype == 'gnss3'):
+        f,orbdir,foundit=gbm_orbits_direct(year,month,day)
+        snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'sp3'):
-        print('uses default IGS orbits, so only GPS ?')
+        #print('uses default IGS orbits, so only GPS ?')
         f,orbdir,foundit=getsp3file_flex(year,month,day,'igs')
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'gfz'):
         print('using Final gfz sp3 file, GPS and GLONASS') # though I advocate gbm
         f,orbdir,foundit=getsp3file_flex(year,month,day,'gfz')
         snrexe = gnssSNR_version() ; warn_and_exit(snrexe,fortran)
     elif (orbtype == 'igr'):
@@ -3503,14 +3541,16 @@
 
     return foundit, f, orbdir, snrexe
 
 def warn_and_exit(snrexe,fortran):
     """
     if the GNSS/GPS to SNR executable does not exist, exit
 
+    Parameters
+    ----------
     snrexe : str
         name of the executable
     fortran : bool
         whether fortran is being used for translation
     """
     if not fortran:
         ok = 1
@@ -3533,20 +3573,20 @@
     r3_filename : str
          RINEX 3 format filename. Either Hatanaka 
          compressed or uncompressed allowed
     r2_filename : str
          RINEX 2.11 file
     dec : integer
         decimation factor. If 0 or 1, no decimation is done.
-    gpsonly : boolean
+    gpsonly : bool
         whether you want only GPS signals. Default is false
 
     Returns
     -------
-    fexists : boolean
+    fexists : bool
         whether the RINEX 2.11 file was created and exists
 
     """
     fexists = False
     gexe = gfz_version()
     crnxpath = hatanaka_version()
     #lastbit =  r3_filename[-6:]
@@ -3584,24 +3624,24 @@
                    #subprocess.call([gfzpath,'-finp', searchpath, '-fout', tmpname, '-vo',str(version),'-sei','out','-smp',crate,'-f','-q'])
 
                     if (gpsonly):
                         subprocess.call([gexe,'-finp', r3_filename, '-fout', r2_filename, '-vo','2','-ot', gobblygook_gps, '-sei','out','-smp', crate, '-f','-q'])
                     else:
                         subprocess.call([gexe,'-finp', r3_filename, '-fout', r2_filename, '-vo','2','-ot', gobblygook, '-sei','out','-smp', crate, '-f','-q'])
                 if os.path.exists(r2_filename):
-                    print('Look for the rinex 2.11 file here: ', r2_filename)
+                    #print('Look for the rinex 2.11 file here: ', r2_filename)
                     fexists = True
                 else:
                     sigh = 0
             except:
                 print('some kind of problem in translation from RINEX 3 to RINEX 2.11')
         else:
             print('RINEX 3 file does not exist', r3_filename)
         s2=time.time()
-        print('gfzrnx rinex3 to rinex 2:', round(s2-s1,2), ' seconds')
+        #print('gfzrnx rinex3 to rinex 2:', round(s2-s1,2), ' seconds')
 
 
     return fexists
 
 
 def ign_orbits(filename, directory,year):
     """
@@ -3614,15 +3654,15 @@
     directory : str
         location of orbits at the IGN
     year : int
         full year
 
     Returns
     -------
-    foundit : boolean
+    foundit : bool
         whether sp3 file was found
 
     """
     # without gz
     stripped_name = filename[0:-3]
     url = directory + filename
 
@@ -3652,15 +3692,15 @@
     doy : int
         day of year 
     srate : int
         sample rate
 
     Returns
     -------
-    fexist : boolean
+    fexist : bool
         whether file was downloaded
     """
     fexist = False
     crnxpath = hatanaka_version()
     cyyyy, cyy, cdoy = ydoych(year,doy)
 
     csrate = '{:02d}'.format(srate)
@@ -3817,14 +3857,15 @@
     downloads navigation file from SOPAC to be used in a cron job
 
     Parameters
     ----------
     yyyy : int
         full year
     doy : int
+        day of year
 
     Returns
     -------
     filefound : bool
         whether file is found
 
     """
@@ -3871,15 +3912,15 @@
     cdoy : string
         3 char day of year
 
     Returns 
     -------
     navfile : string 
         should be the same name as input. not logical!
-        i have no idea why i did it this way.
+        I have no idea why i did it this way.
 
     """
     foundfile = False
     sopac = 'ftp://garner.ucsd.edu'
     navfile_sopac1 =  navfile   + '.Z' # regular nav file
     navfile_compressed = navfile_sopac1
     url_sopac1 = sopac + '/pub/rinex/' + cyyyy + '/' + cdoy + '/' + navfile_sopac1
@@ -3904,22 +3945,22 @@
     """
 
     downloads GPS broadcast navigation file from ESA
     tries both Z and gz compressed
 
     Parameters
     ----------
-    cyyyy : string
+    cyyyy : str
         4 char year
-    cdoy : string
+    cdoy : str
         3 char day of year
 
     Returns
     -------
-    fstatus : boolean
+    fstatus : bool
         whether file was found or not
 
     """
     fstatus = False
     cyy = cyyyy[2:4]
     year = int(cyyyy)
     navfile_out = 'auto' + cdoy + '0.' + cyy + 'n' 
@@ -4127,24 +4168,25 @@
         ndoy = doy + 1
 
     return nyear, ndoy
 
 def read_sp3file(file_path):
     """ 
     input: file_path is the sp3file name
-    I do not believe this is used
+    this code is from Joakim Strandberg I believe.
+    It is for the python only version of the translator, which 
+    should be deprecated
 
     Returns
     -------
     sp3 : ndarray
     colums are satnum, gpsweek, gps_sow, x,y,z
     x,y,z are in meters
     satnum has 0, 100, 200, 300 added for gps, glonass, galileo,beidou,
     respectively.  all other satellites are ignored
-    some of this code came from joakim
 
     """
     ignorePoint = False
     max_sat = 150 # not used
     # store as satNu, week, sec of week , x, y, and z?
     sp3 = np.empty(shape=[0, 6])
     count = -1
@@ -4741,15 +4783,15 @@
     nr,nc = t.shape
     obstimes = []
 
     # if i read in the file better, would not have to change from float
     # year mon day hour min sealevel doy mjd seconds
     if nr > 0:
         for i in range(0,nr):
-            dtime = datetime.datetime(year=int(t[i,0]), month=int(t[i,1]), day=int(t[i,2]), hour=int(t[i,3]), minute=int(t[i,4]), second=int(t[i,8]) )
+            dtime = datetime.datetime(year=int(t[i,0]), month=int(t[i,1]), day=int(t[i,2]), hour=int(t[i,3]), minute=int(t[i,4]), second=int(t[i,5]) )
             obstimes.append(dtime)
     else:
         print('you sent me an empty variable')
 
     return obstimes
 
 def get_noaa_obstimes_plus(t):
@@ -4830,26 +4872,26 @@
     littlename = 'gbm' + str(wk) + str(int(sec/86400)) + '.sp3'
     #GFZ0MGXRAP_20222740000_01D_05M_ORB.SP3
     #GFZ0OPSFIN
     # GFZ0MGXRAP_20222440000_01D_05M_ORB.SP3
     littlename = 'GFZ0MGXRAP_' + str(year) + cdoy + '0000_01D_05M_ORB.SP3'
 
     url = gns + 'w' + str(wk) + '/' + littlename + '.gz'
-    print(url)
+    #print(url)
 
     fullname = fdir + '/' + littlename + '.xz'
     if os.path.isfile(fullname):
         subprocess.call(['unxz', fullname])
 
     fullname = fdir + '/' + littlename + '.gz'
     if os.path.isfile(fullname):
         subprocess.call(['gunzip', fullname])
 
     if os.path.isfile(fdir + '/' + littlename):
-        print(littlename, ' already exists on disk')
+        #print(littlename, ' already exists on disk')
         return littlename, fdir, True 
 
     try:
         wget.download(url,littlename + '.gz')
         subprocess.call(['gunzip', littlename + '.gz'])
     except:
         print('Problems downloading final multi-GNSS GFZ orbit from GFZ')
@@ -4879,25 +4921,25 @@
 
     gns = 'ftp://ftp.gfz-potsdam.de/pub/GNSS/products/rapid/'
     month, day, doy, cyyyy, cyy, cdoy = ymd2ch(year,month,day)
 
     fdir = os.environ['ORBITS'] + '/' + cyyyy + '/sp3'
     littlename = 'gfz' + str(wk) + str(int(sec/86400)) + '.sp3'
     url = gns + 'w' + str(wk) + '/' + littlename + '.gz'
-    print(url)
+    #print(url)
     if (year + doy/365.25) < dday:
         print('No rapid GFZ orbits until 2021/doy137')
         return '', '', foundit
     fullname = fdir + '/' + littlename + '.xz'
     # look for compressed file
     if os.path.isfile(fullname):
         subprocess.call(['unxz', fullname])
 
     if os.path.isfile(fdir + '/' + littlename):
-        print(littlename, ' already exists on disk')
+        #print(littlename, ' already exists on disk')
         return littlename, fdir, True 
     try:
         wget.download(url,littlename + '.gz')
         subprocess.call(['gunzip', littlename + '.gz'])
     except:
         print('Problems downloading Rapid GFZ orbit')
 
@@ -4936,15 +4978,15 @@
     gns = 'ftp://ftp.gfz-potsdam.de/pub/GNSS/products/ultra/'
     fdir = os.environ['ORBITS'] + '/' + cyyyy + '/sp3'
     # change the hour into two character string
     chr = '{:02d}'.format(hour)
     littlename = 'gfu' + str(wk) + str(int(sec/86400)) + '_' + chr + '.sp3'  
 
     url = gns + 'w' + str(wk) + '/' + littlename + '.gz'
-    print(url)
+    #print(url)
     if (year + doy/365.25) < dday:
         print('No rapid GFZ orbits until 2021/doy137')
         return '', '', foundit
 
     # check to see if the file is there already
     fullname = fdir + '/' + littlename + '.xz'
     if os.path.isfile(fullname):
@@ -4952,15 +4994,15 @@
 
     # check to see if the file is there already
     fullname = fdir + '/' + littlename + '.gz'
     if os.path.isfile(fullname):
         subprocess.call(['gunzip', fullname])
 
     if os.path.isfile(fdir + '/' + littlename):
-        print(littlename, ' already exists on disk')
+        #print(littlename, ' already exists on disk')
         return littlename, fdir, True
 
     try:
         wget.download(url,littlename + '.gz')
         subprocess.call(['gunzip', littlename + '.gz'])
     except:
         print('Problems downloading ultrarapid GFZ orbit')
@@ -5005,17 +5047,15 @@
 
     try:
         wget.download(url1,filename1)
         status = subprocess.call(['uncompress', filename1])
     except:
         okokok =1
 
-    #print('try hatanaka RINEX at unavco')
     if not os.path.exists(rinexfile):
-        #print('look for hatanaka version')
         if os.path.exists(crnxpath):
             try:
                 wget.download(url2,filename2)
                 status = subprocess.call(['uncompress', filename2])
                 status = subprocess.call([crnxpath, rinexfiled])
                 status = subprocess.call(['rm', '-f', rinexfiled])
             except:
@@ -5036,19 +5076,21 @@
     foundit = False; 
     wk,swk = kgpsweek(year, month, day, 0,0,0)
     cwk = '{:04d}'.format(wk); cday = str(int(swk/86400))
     # old file name for precise files
     filenameZ = 'gbm' + cwk + cday + '.sp3.Z'
     filename = 'gbm' + cwk + cday + '.sp3'
     if os.path.isfile(fdir + filename):
-        print(filename,' orbit file already exists on disk'); foundit = True
+        #print(filename,' orbit file already exists on disk'); 
+        foundit = True
         return filename, fdir, foundit
     if os.path.isfile(fdir + filename + '.xz'):
         subprocess.call(['unxz',fdir + filename + '.xz'])
-        print(filename, ' orbit file already exists on disk'); foundit = True
+        #print(filename, ' orbit file already exists on disk'); 
+        foundit = True
         return filename, fdir, foundit
 
     # only use this for weeks < 2050
     if (wk < 2050):
         url = 'ftp://igs.ensg.ign.fr/pub/igs/products/mgex/' + cwk +  '/' + filenameZ
         try:
             wget.download(url,filenameZ)
@@ -5058,19 +5100,21 @@
         except:
             print('could not find ', filename)
     if (not foundit):
         filename = 'GFZ0MGXRAP_' + cyyyy  + cdoy + '0000_01D_05M_ORB.SP3'
         filenamegz = 'GFZ0MGXRAP_' + cyyyy  + cdoy + '0000_01D_05M_ORB.SP3.gz'
 
         if os.path.isfile(fdir + filename):
-            print(filename, ' orbit file already exists on disk'); foundit = True
+            #print(filename, ' orbit file already exists on disk'); 
+            foundit = True
             return filename, fdir, foundit
         if os.path.isfile(fdir + filename + '.xz'):
             subprocess.call(['unxz',fdir + filename + '.xz'])
-            print(filename, ' orbit file already exists on disk'); foundit = True
+            #print(filename, ' orbit file already exists on disk'); 
+            foundit = True
             return filename, fdir, foundit
 
         url = 'ftp://igs.ensg.ign.fr/pub/igs/products/mgex/' + cwk +  '/' + filenamegz
         try:
             wget.download(url, filenamegz)
             if os.path.exists(filenamegz):
                 subprocess.call(['gunzip',filenamegz])
@@ -5084,24 +5128,24 @@
 def rinex_jp(station, year, month, day):
     """
     Picks up RINEX file from Japanese GSI GeoNet archive
     URL : https://www.gsi.go.jp/ENGLISH/index.html
 
     Parameters
     ----------
-    station : string
+    station : str
         station name
 
-    year : integer
+    year : int
         full year
 
-    month: integer
+    month: int
         month or day of year
 
-    day : integer
+    day : int
         day of month or zero
     """
     # allow it to be called with day of year
     doy,cdoy,cyyyy,cyy = ymd2doy(year,month,day)
 
     fdir = os.environ['REFL_CODE']
     if not os.path.isdir(fdir):
@@ -5176,14 +5220,15 @@
 
     """
     lat = 0; lon = 0; ht = 0
     if len(station) != 4:
         print('The station name must be four characters long')
         return lat, lon, ht
 
+    not_in_database = False
     xdir = os.environ['REFL_CODE']
     nfile1 = 'gnssrefl/station_pos.db'
     nfile1_exist = os.path.isfile(nfile1)
     nfile2 = xdir + '/Files/station_pos.db'
     nfile2_exist = os.path.isfile(nfile2)
 
     if (nfile1_exist) or (nfile2_exist):
@@ -5202,34 +5247,49 @@
             wget.download(url1,nfile2)
             nfile2_exist = True
         except:
             print('Could not download the database for you')
             return lat, lon, ht
     # if you used github and run the code from that directory
     if nfile1_exist:
-        print('Database was found at :', nfile1)
+        #print('Database was found at :', nfile1)
         conn = sqlite3.connect(nfile1)
     elif nfile2_exist:
-        print('Database was found at :', nfile2)
+        #print('Database was found at :', nfile2)
         conn = sqlite3.connect(nfile2)
     c=conn.cursor()
     c.execute("SELECT * FROM  stations WHERE station=:station",{'station': station})
     w = c.fetchall()
     if len(w) > 0:
         [(name,lat,lon,ht)] = w
         # if longitude is ridiculous, as it often is in the Nevada Reno database make it less so
         if (lon < -180):
             lon = lon + 360
-        print(lat,lon,ht)
     else:
-        print('Did not find the station in the database:', station)
-        # this returns 0 values
+        not_in_database = True
 
     # close the database
     conn.close()
+    if (station == 'moss'):
+        lat= -16.434464800 ;lon = 145.403622520 ; ht = 71.418
+    elif (station == 'mnis'):
+        lat = -16.667810553; lon  = 139.170597267; ht = 60.367;  
+    elif (station == 'boig'):
+        lat =  -9.24365375 ; lon  = 142.253961217; ht = 82.5;  
+    elif (station == 'glbx'):
+        lat = 58.455146633; lon  = -135.888483766 ; ht = 12.559;  
+    elif (station == 'ugar'):
+        lat = -9.50477824; lon = 143.54686680 ; ht =  81.2
+    elif (station == 'whla'):
+        lat = -33.01640186 ; lon = 137.59157111 ; ht = 7.856
+    elif (station == 'kubn'):
+        lat =-10.23608303 ; lon =142.21446068; ht = 78.2
+
+    if (not_in_database) and (lat == 0):
+        print('Did not find station coordinates :', station)
 
     return lat,lon,ht
 
 def rinex3_nav(year,month,day):
     """
     """
     foundit = False
@@ -5376,19 +5436,19 @@
 
 def bfg_password():
     """
     Picks up BFG userid and password that is stored in a pickle file
     in your REFL_CODE/Files/passwords area
     If it does not exist, it asks you to input the values and stores them for you.
 
-    returns  
-    --------
-    userid : string
+    Returns  
+    -------
+    userid : str
 
-    password : string 
+    password : str 
 
     """
 
     fdir = os.environ['REFL_CODE']
     if not os.path.isdir(fdir):
         print('You need to define the REFL_CODE environment variable')
         return
@@ -5508,15 +5568,14 @@
     if not os.path.exists(crnxpath):
         hatanaka_warning()
     else:
         if os.path.exists(c3): # file exists
             subprocess.call([crnxpath,c3])
     if os.path.exists(rnx): # file exists
         translated = True
-        #print('remove Hatanaka compressed file')
         subprocess.call(['rm','-f',c3])
 
     return translated, rnx
 
 
 
 def ga_highrate(station9,year,doy,dec,deleteOld=True):
@@ -5622,27 +5681,63 @@
         subprocess.call(cm,shell=True)
         searchpath = station9.upper()  + '*' + cyyyy + cdoy + '*crx'
         cm ='rm -f ' + searchpath
         subprocess.call(cm,shell=True)
     return rinex2, fexist
 
 
+def cddis_download_2022B_new(filename,directory):
+    """
+    download code for CDDIS using https and password
+
+    Parameters
+    ----------
+    filename : str
+        name of the rinex file or orbit file
+
+    directory : str
+        where the file lives at CDDIS
+
+    """
+    print('New way of CDDIS downloads')
+    basename = 'https://cddis.nasa.gov/archive'
+    url = basename + directory + filename
+    print(url)
+    # Makes request of URL, stores response in variable r
+    user,passw = cddis_password()
+
+# requests.get('https://httpbin.org/basic-auth/user/pass', auth=('user', 'pass'))
+    r = requests.get(url,auth=('user','passw'))
+
+    if (r.status_code == 200):
+# Opens a local file of same name as remote file for writing to
+        with open(filename, 'wb') as fd:
+            for chunk in r.iter_content(chunk_size=1000):
+                fd.write(chunk)
+
+# Closes local file
+        fd.close()
+    else:
+        print('File does not exist')
+
 def cddis_download_2022B(filename,directory):
     """
-    download code for CDDIS
+    Nth iteration of download code for CDDIS
 
     Parameters
     ----------
     filename : str
         name of the rinex file or orbit file
 
     directory : str
         where the file lives at CDDIS
 
     """
+    print('Original way of accessing CDDIS ')
+
     ftps = FTP_TLS(host = 'gdc.cddis.eosdis.nasa.gov')
     email = 'kristine.larson@colorado.edu'
     ftps.login(user='anonymous', passwd=email)
     ftps.prot_p()
     ftps.cwd(directory)
     ftps.retrbinary("RETR " + filename, open(filename, 'wb').write)
     siz = os.path.getsize(filename)
@@ -5825,15 +5920,15 @@
         print('Making ', localdir)
         subprocess.call('mkdir',localdir)
 
     egm = localdir + matfile
     if 'REFL_CODE' in os.environ:
         egm = localdir + matfile
         if os.path.isfile(egm):
-            print('EGM96 file exists')
+            #print('EGM96 file exists')
             foundfile = True
         else:
             print('EGM96 file does not exist. We will try to download and store it in ',localdir)
             githubdir = 'https://raw.githubusercontent.com/kristinemlarson/gnssrefl/master/docs/'   
             wget.download(githubdir+matfile, localdir + matfile)
             if os.path.isfile(egm):
                 print('successful download, EGM file exists')
@@ -6005,7 +6100,197 @@
         plt.grid()
         fig.autofmt_xdate()
         plt.show()
     else:
         print('no data found - so no plot')
     return
 
+
+def cddis_restriction(iyear, idoy,archive):
+    """
+    CDDIS has announced a restructuring of their archive.
+    After 6 months files are tarred. It would be ok for the code
+    to accommodate this change, but it will have to come from the community.
+    If six months has passed since you ran the code, a warning will come to the 
+    screen and the code will exit.
+
+    updated now that i realize BKG does the same thing
+
+    Parameters
+    ----------
+    iyear : int
+        year you want to download from CDDIS
+    idoy : int
+        day of year you want to download from CDDIS
+
+    archive : str
+        name of archive
+
+    Returns
+    -------
+    bad_day : bool
+        if bad_day is true, you cannot access high-rate data from CDDIS or BKG
+
+    """
+# find out today's date
+    year = int(date.today().strftime("%Y"));
+    month = int(date.today().strftime("%m"));
+    day = int(date.today().strftime("%d"));
+
+    today=datetime.datetime(year,month,day)
+    doy = (today - datetime.datetime(today.year, 1, 1)).days + 1
+    tdate = year + doy/365.25
+
+    # input date
+    idate = iyear + idoy/365.25
+
+    if (tdate - idate) > 0.5:
+        # i.e. half a year is six months
+        bad_day =  True
+        print(archive.upper() + ' does not allow direct access to their high-rate data for this day and year. ')
+        print('They now tar files six months after the data archived. If you are willing to ')
+        print('submit a pull request to fix this issue, we would be very willing to host it.')
+
+    else:
+        bad_day = False
+
+
+    return bad_day
+
+
+def cddis_password():
+    """
+    Picks up cddis userid and password that is stored in a pickle file
+    in your REFL_CODE/Files/passwords area
+    If it does not exist, it asks you to input the values and stores them for you.
+
+    Returns
+    -------
+    userid : str
+        cddis username
+
+    password : str
+        cddis password
+
+    """
+
+    fdir = os.environ['REFL_CODE']
+    if not os.path.isdir(fdir):
+        print('You need to define the REFL_CODE environment variable')
+        return
+
+    # make sure the directory exists to store passwords
+    if not os.path.isdir(fdir + '/Files'):
+        subprocess.call(['mkdir',fdir + '/Files'])
+    if not os.path.isdir(fdir + '/Files/passwords'):
+        subprocess.call(['mkdir',fdir + '/Files/passwords'])
+
+    userinfo_file = fdir + '/Files/passwords/' + 'cddis.pickle'
+    #print('user information file', userinfo_file)
+
+    #print('Will try to pick up BFG account information',userinfo_file)
+    if os.path.exists(userinfo_file):
+        with open(userinfo_file, 'rb') as client_info:
+            login_info = pickle.load(client_info)
+            user_id = login_info[0]
+            passport = login_info[1]
+    else:
+        print('You need a earthdata account to access NASA data.')
+        print('https://urs.earthdata.nasa.gov/')
+        user_id = getpass.getpass(prompt='Userid: ', stream=None)
+        passport= getpass.getpass(prompt='Password: ', stream=None)
+        # save to a file
+        with open(userinfo_file, 'wb') as client_info:
+            pickle.dump((user_id,passport) , client_info)
+        print('User id and password saved to', userinfo_file)
+
+    return user_id, passport
+
+
+
+def gbm_orbits_direct(year,month,day):
+    """
+    downloads gfz multi-gnss orbits, aka gbm orbits, directly from GFZ.
+    thus avoids CDDIS.  it first checks to see if you have the files online.
+    both version of the long name.
+
+    Parameters
+    ----------
+    year : int
+        full year
+    month : int
+        month number or day of year if day is set to zero
+    day : int
+        calendar day of month
+
+    """
+    foundit = False
+    return_name = ''
+
+    month, day, doy, cyyyy, cyy, cdoy = ymd2ch(year,month,day)
+    gpsweek,sec=kgpsweek(year,month,day,0,0,0)
+    cgpsweek = str(gpsweek)
+
+    gns = 'ftp://ftp.gfz-potsdam.de/pub/GNSS/products/mgex/' + cgpsweek + '/'
+
+    fdir = os.environ['ORBITS'] + '/' + cyyyy + '/sp3'
+    littlename = 'gbm' + str(gpsweek) + str(int(sec/86400)) + '.sp3'
+    bigname = 'GFZ0MGXRAP_' + cyyyy + cdoy + '0000_01D_05M_ORB.SP3'
+
+    bigname2 = 'GBM0MGXRAP_' + cyyyy + cdoy + '0000_01D_05M_ORB.SP3'
+
+    # first, do you have it locally?  
+    # look for compressed file
+    fullname = fdir + '/' + littlename 
+    if os.path.isfile(fullname):
+        foundit = True
+        return_name = littlename
+    elif os.path.isfile(fullname + '.gz'):
+        subprocess.call(['gunzip', fullname + '.gz'])
+        foundit = True; 
+        return_name = littlename
+
+    if not foundit:
+        fullname = fdir + '/' + bigname 
+        if os.path.isfile(fullname):
+            foundit = True
+            return_name = bigname
+        elif os.path.isfile(fullname + '.gz'):
+            subprocess.call(['gunzip', fullname + '.gz'])
+            foundit = True; 
+            return_name = littlename
+
+    # checked for the first kind of name because that is how it was stored on CDDIS.
+    # now use the name as how it is stored at GFZ.  I think
+    bigname = bigname2 
+    if not foundit:
+        url = gns + littlename + '.Z'
+        try:
+            wget.download(url,littlename + '.Z')
+            subprocess.call(['uncompress', littlename + '.Z'])
+        except:
+            okok = 1
+        if os.path.isfile(littlename):
+            foundit = True ; return_name = littlename
+        else:
+            url = gns + bigname + '.gz'
+            try:
+                wget.download(url,bigname + '.gz')
+                subprocess.call(['gunzip', bigname + '.gz'])
+                foundit = True ; return_name = bigname
+            except:
+                okok = 1
+
+
+    # store the file
+    if os.path.isfile(littlename):
+        store_orbitfile(littlename,year,'sp3') ; 
+    elif os.path.isfile(bigname):
+        store_orbitfile(bigname,year,'sp3') ; 
+
+    if not foundit:
+        print('Orbit was not found at GFZ or in a local directory')
+    #else:
+    #    print('Orbit found')
+
+    return return_name, fdir, foundit
+
```

### Comparing `gnssrefl-1.3.8/gnssrefl/gpssnr.f` & `gnssrefl-1.4.1/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/gpsweek.py` & `gnssrefl-1.4.1/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.4.1/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/highrate.py` & `gnssrefl-1.4.1/gnssrefl/highrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,14 @@
         return
 
     gns = 'https://cddis.nasa.gov/archive/gnss/data/highrate/' 
     gns = gns + cyyyy + '/'+ cdoy + '/' +cyy + 'd/'
     #YYYY/DDD/YYt/HH/mmmmDDDHMM.YYt.gz
 
     s1=time.time()
-    print('WARNING: CDDIS has changed the directory structure of older datasets. ')
-    print('WARNING: Please help modify this code / submit a pull request. ')
     print('WARNING: Get yourself a cup of coffeee. Downloading 96 files takes a long time.')
     fileF = 0
     streamID  = '_' + stream + '_'
     s1 = time.time()
     for h in range(0,24):
         # subdirectory
         ch = '{:02d}'.format(h)
@@ -76,14 +74,15 @@
                 file_name, crnx_name, file_name2, crnx_name2, exe1, exe2 = variableArchives(station,year,doy,cyyyy,cyy,cdoy,alpha[h],e) 
             else:
                 file_name = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.crx.gz'
                 crnx_name = file_name[:-3] 
                 oname = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.rnx' # do we need this?
 
             new_way_dir = '/gnss/data/highrate/' + cyyyy + '/' + cdoy + '/' + cyy + 'd/' + ch + '/'
+            #print(new_way_dir)
             if os.path.isfile(oname):
                 print('Found it:', new_way_dir,file_name)
                 fileF = fileF + 1
             elif os.path.isfile(file_name):
                 print('Found gzip/hatanaka file:', new_way_dir,file_name)
                 subprocess.call(['gunzip',file_name])
                 subprocess.call([crnxpath, crnx_name])
@@ -275,19 +274,19 @@
     s1 = time.time()
     for h in range(0,24):
         # subdirectory
         ch = '{:02d}'.format(h)
         print('Hour: ', ch)
         for e in ['00', '15', '30', '45']:
             file_name = station.upper() + streamID + cyyyy + cdoy + ch + e + '_15M_01S_MO.crx.gz'
-            print('looking for', file_name)
+            dirname = gns + '/' + alpha[h] + '/'
+            print('looking for', dirname + file_name)
             crnx_name = file_name[:-3] 
             oname = file_name[:-6] + 'rnx'
 
-            dirname = gns + '/' + alpha[h] + '/'
             if os.path.isfile(oname):
                 fileF = fileF + 1
                 print('already have ', oname)
             else:
                 try:
                     wget.download(dirname+file_name,file_name)
                     subprocess.call(['gunzip',file_name]) # unzip
```

### Comparing `gnssrefl-1.3.8/gnssrefl/installexe_cl.py` & `gnssrefl-1.4.1/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/invsnr_cl.py` & `gnssrefl-1.4.1/gnssrefl/invsnr_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,23 @@
     parser.add_argument("doy", default=None, type=int, help="doy")
     parser.add_argument("signal", default=None, type=str, help="L1, L2, L5, L1+L2, L1+L2+L5, etc")
 
     parser.add_argument("-pktnlim", default=None, type=float, help="Peak2noise ratio for Quality Control")
     parser.add_argument("-constel", default=None, type=str, help="Only a single constellation (G,E, or R)")
     parser.add_argument("-screenstats", default=None, type=str, help="screen stats, False is default")
     parser.add_argument("-tempres", default=None, type=int, help="SNR file decimator (seconds)")
-    parser.add_argument("-polydeg", default=None, type=int,
-                        help="polynomial degree for direct signal removal (default is 2)")
+    parser.add_argument("-polydeg", default=None, type=int, help="polynomial degree for direct signal removal (default is 2)")
     parser.add_argument("-snrfit", default=None, type=str, help="Do invsnr fit? True is the default ")
     parser.add_argument("-plt", default=None, type=str, help="Plot to the screen?  default is True")
     parser.add_argument("-doy_end", default=None, type=str, help="day of year to end analysis")
     parser.add_argument("-lspfigs", default=None, type=str, help="Make LSP plots, default False.")
     parser.add_argument("-snrfigs", default=None, type=str, help="Make SNR plots, default False.")
     parser.add_argument("-knot_space", default=None, type=int, help="knot spacing in hours (default is 3)")
     parser.add_argument("-rough_in", default=None, type=str, help="Roughness (default is 0.1)")
-    parser.add_argument("-risky", default=None, type=str,
-                        help="Risky taker related to gaps/knot spacing, False is default)")
+    parser.add_argument("-risky", default=None, type=str, help="Risky taker related to gaps/knot spacing, False is default.")
     parser.add_argument("-snr_ending", default=None, type=str, help="SNR file ending. Default is 66")
     parser.add_argument("-outfile_type", default=None, type=str, help="Output file type (txt or csv)")
     parser.add_argument("-outfile_name", default=None, type=str, help="Output file name")
     parser.add_argument("-outlier_limit", default=None, type=str, help="outliers limit (m)")
     parser.add_argument("-no_dots", default=None, type=str, help="bool, no lomb scargle  results plotted")
     parser.add_argument("-delta_out", default=None, type=str, help="Output increment, in seconds (default is 300)")
     parser.add_argument("-refraction", default=None, type=str, help="bool, Set to False to turn off")
@@ -46,28 +44,26 @@
     boolean_args = ['screenstats', 'snrfit', 'plt', 'lspfigs', 'snrfigs', 'risky', 'no_dots','refraction', 'json_override',]
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def invsnr(station: str, year: int, doy: int, signal: str, pktnlim: float = 4, constel: str = None,
-           screenstats: bool = False, tempres: int = 1, polydeg: int = 2, snrfit: bool = True, plt: bool = True,
-           doy_end: int = None, lspfigs: bool = False, snrfigs: bool = False, knot_space: int = 3,
-           rough_in: float = 0.1, risky: bool = False, snr_ending: int = 66, outfile_type: str = 'txt',
-           outfile_name: str = '', outlier_limit: float = 0.5, no_dots: bool = False, delta_out: int = 300,
-           refraction: bool = True, json_override: bool = False):
-
+def invsnr(station: str, year: int, doy: int, signal: str, pktnlim: float = 4, constel: str = None, 
+        screenstats: bool = False, tempres: int = 1, polydeg: int = 2, snrfit: bool = True, plt: bool = True,
+        doy_end: int = None, lspfigs: bool = False, snrfigs: bool = False, knot_space: int = 3, 
+        rough_in: float = 0.1, risky: bool = False, snr_ending: int = 66, outfile_type: str = 'txt', 
+        outfile_name: str = '', outlier_limit: float = 0.5, no_dots: bool = False, delta_out: int = 300, 
+        refraction: bool = True, json_override: bool = False):
     """
-    Calls invsnr code.
-
-    Note: outfile_name and outfile_type are unnecessary. Consolidate them.
+    You must have run invsnr_input before using this code. This is the wrapper code that does the 
+    invsnr modelling. Note: outfile_name and outfile_type are unnecessary. Consolidate them.
     
     Examples
-    -------
+    --------
     invsnr sc02 2023 15 L1+L2+L5 
         would analyze day of year 15 and the L1, L2, and L5 signals
     invsnr sc02 2023 15 ALL
         would analyze day of year 15 and all signals
     invsnr sc02 2023 15 L1+L2
         would analyze day of year 15 and just L1 and L2
     invsnr sc02 2023 15 L1+L2  -doy_end 18
@@ -78,33 +74,32 @@
     station : str
         four character ID 
     year : int
         Year
     doy : int
         Day of year
     signal : str
-        signal to use.
-        value options: 
-            L1  L2 L5 L6 L7 L1+L2 L1+L2+L5 L1+L5 ALL
+        signal to use, L1  L2 L5 L6 L7 L1+L2 L1+L2+L5 L1+L5 ALL
     pktnlim: float, optional
         Peak2noise ratio limit for Quality Control.
         Default is 4
     constel: str, optional
         Only a single constellation.
         Default is gps, glonass, and galileo.
         value options:
-                G : GPS
 
-                E : Galileo
+            G : GPS
+
+            E : Galileo
 
-                R : Glonass
+            R : Glonass
 
-                C : Beidou
+            C : Beidou
 
-                withBeidou : adds Beidou to the default.
+            withBeidou : adds Beidou to the default.
 
     screenstats: bool, optional
         Whether to print out stats to the screen.
         Default is False
     tempres: int, optional
         SNR file decimator (seconds)
         Default is 1 (everything)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/invsnr_input.py` & `gnssrefl-1.4.1/gnssrefl/invsnr_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,71 +17,78 @@
 
 
 def parse_arguments():
 # user inputs the observation file information
     parser = argparse.ArgumentParser()
 # required arguments
     parser.add_argument("station", help="station name", type=str)
-    parser.add_argument("h1", default=None, type=float, help="Lower limit reflector height (m)")
-    parser.add_argument("h2", default=None, type=float, help="Upper limit reflector height (m)")
-    parser.add_argument("e1", default=None, type=float, help="Lower limit elev. angle (deg)")
-    parser.add_argument("e2", default=None, type=float, help="Upper limit elev. angle (deg)")
+    parser.add_argument("-h1", default=None, type=float, help="Lower limit reflector height (m), default 1")
+    parser.add_argument("-h2", default=None, type=float, help="Upper limit reflector height (m), default 8")
+    parser.add_argument("-e1", default=None, type=float, help="Lower limit elev. angle (deg), default 5")
+    parser.add_argument("-e2", default=None, type=float, help="Upper limit elev. angle (deg), default 15")
 
-    parser.add_argument("-a1", default=None, type=float, help="Lower limit azimuth angle (deg)")
-    parser.add_argument("-a2", default=None, type=float, help="Upper limit azimuth angle (deg)")
+    parser.add_argument("-azim1", default=None, type=float, help="Lower limit azimuth angle (deg), default 0")
+    parser.add_argument("-azim2", default=None, type=float, help="Upper limit azimuth angle (deg), default 360")
 
     parser.add_argument("-lat", help="Latitude (degrees)", type=str, default=None)
     parser.add_argument("-lon", help="Longitude (degrees)", type=str, default=None)
     parser.add_argument("-height", help="Ellipsoidal height (meters)", type=str, default=None)
 # these are the optional inputs 
     args = parser.parse_args().__dict__
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def invsnr_input(station: str, h1: float, h2: float, e1: float, e2: float, a1: float = 0,
-                 a2: float = 360, lat: float = None, lon: float = None, height: float = None):
+def invsnr_input(station: str, h1: float=1, h2: float=8, e1: float=5, e2: float=15, azim1: float = 0,
+                 azim2: float = 360, lat: float = None, lon: float = None, height: float = None):
     """
+    Sets some of the analysis parameters for invnsr. Values are stored in a json in $REFL_CODE/input
+    Note: this code was written independently of gnssrefl. The Quality Control parametesr are thus quite 
+    different from how gnssrefl is done. The LSP RH retrievals are not - and should not - be the same.
+
+    Examples
+    --------
+    invsnr_input sc02 -h1 3 -h2 12 -e1 5 -e2 13 -azim1 40 -azim2 220
+        general Friday Harbor inputs
+    invsnr_input at01 -h1 9 -h2 14 -e1 5 -e2 13 -azim1 20 -azim2 22
+        St Michael inputs 
+
+
+
     Parameters
     ----------
-    station : string
-        Character ID of the station
-
-    h1 : float
+    station : str
+        four ch ID of the station
+    h1 : float, optional
         Lower limit reflector height (m)
-
-    h2 : float
+    h2 : float, optional
         Upper limit reflector height (m)
-
-    e1 : float
+    e1 : float, optional
         Lower limit elev. angle (deg)
-
     e2 : float
         Upper limit elev. angle (deg)
-
-    a1 : float, optional
+    azim1 : float 
         Lower limit azimuth angle (deg)
-
-    a2 : float, optional
+    azim2 : float 
         Upper limit azimuth angle (deg)
-
     lat : float, optional
         Latitude (degrees)
-
     lon : float, optional
         Longitude (degrees)
-
     height : float, optional
         Ellipsoidal height (meters)
 
     """
 
 # rename the user inputs into variables
 #
+    # use old variable names
+    a1=azim1
+    a2=azim2
     NS = len(station)
     if (NS != 4):
         print('station name must be four characters long. Exiting.')
         sys.exit()
     Lat, Long, Height = g.queryUNR_modern(station)
     if Lat == 0:
         if lat is None:
@@ -126,16 +133,16 @@
         subprocess.call(['mkdir', outputdir])
 # 
     lsp['precision'] = 0.005 # precision of RH in meters
 # 
     lsp['l2c_only'] = True
 
     outputfile = outputdir + '/' + station + '.inv.json'
-    print('writing json file to:', outputfile)
-    print(lsp)
+    print('Writing json file to:', outputfile)
+    #print(lsp)
     with open(outputfile, 'w+') as outfile:
         json.dump(lsp, outfile, indent=4)
 
 
 def main():
     args = parse_arguments()
     invsnr_input(**args)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/karnak_libraries.py` & `gnssrefl-1.4.1/gnssrefl/karnak_libraries.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,43 +145,56 @@
         name of rinexfile
 
     foundit : boolean
         whether file was found
 
     """
     # define the file name
-    print('Searching the ', archive, ' archive with rate/filetype', srate, stream)
+    if debug:
+        print('Searching the ', archive, ' archive with rate/filetype', srate, stream)
     foundit = False
 
     file_name,cyyyy,cdoy = filename_plus(station9ch,year,doy,srate,stream)
     print('Filename:', file_name)
     cyy = cyyyy[2:4]
     dir1 = ''
     dir2 = ''
 
     # put this outside the try because I think there is one in the function
     if archive == 'bfg':
         station = station9ch[0:4] ; samplerate = srate; stream = 'R'
+        debug = False
         g.bfg_data(station, year, doy, samplerate,debug)
+        zip_file_name = file_name[0:-2] + 'zip'
         if os.path.exists(file_name):
-            print('File was found: ', file_name )
+            if debug:
+                print('File was found: ', file_name )
+            foundit = True
+        elif os.path.exists(zip_file_name):
+            if debug:
+                print('From zip to gz: ', zip_file_name )
+            subprocess.call(['unzip', zip_file_name])
+            subprocess.call(['gzip', file_name[0:-3]])
+            # cleaning up
+            subprocess.call(['rm', zip_file_name])
             foundit = True
         else:
             print('File was not found: at bfg.')
 
         return file_name,foundit
     cydoy =  cyyyy + '/' + cdoy + '/'
     s1 = time.time()
     if (archive == 'unavco'):
         # original dir1 = 'https://data.unavco.org/archive/gnss/rinex3/obs/' + cyyyy + '/' + cdoy + '/'
         #url1 =      'https://data-idm.unavco.org/archive/gnss/rinex3/obs/' + cydoy + file_name
         url1 =      'https://data.unavco.org/archive/gnss/rinex3/obs/' + cydoy + file_name
         foundit,file_name = kelly.the_kelly_simple_way(url1,file_name)
         s2 = time.time()
-        print('Download took ',np.round(s2-s1,2), ' seconds') 
+        if debug:
+            print('Download took ',np.round(s2-s1,2), ' seconds') 
         return file_name,foundit
 
     try:
         if (archive == 'ign'):
             dir1='ftp://igs.ensg.ign.fr/pub/igs/data/' + cyyyy + '/' + cdoy + '/'
             wget.download(dir1+file_name,file_name)
         elif (archive == 'sonel'):
@@ -212,26 +225,26 @@
             wget.download(dir1+file_name,file_name)
         elif (archive == 'unavco-old'):
             dir1 = 'https://data.unavco.org/archive/gnss/rinex3/obs/' + cyyyy + '/' + cdoy + '/'
             wget.download(dir1+file_name,file_name)
         elif (archive == 'gfz'):
             # no idea
             dir1 = 'ftp://isdcftp.gfz-potsdam.de/gnss/data/daily/' + cyyyy + '/' + cdoy + '/'
-            print(dir1+file_name)
+            #print(dir1+file_name)
             wget.download(dir1+file_name,file_name)
         elif (archive == 'cddis'):
             new_way_dir = '/gnss/data/daily/' + cyyyy + '/' + cdoy + '/' + cyy + 'd/'
             g.cddis_download_2022B(file_name,new_way_dir)
-            #g.cddis_download(file_name,new_way_dir)
         else:
             return '', ''
     except:
         okokok = 1
     s2 = time.time()
-    print('Download took ',np.round(s2-s1,2), ' seconds') 
+    if debug: 
+        print('Download took ',np.round(s2-s1,2), ' seconds') 
     if os.path.exists(file_name):
         siz = os.path.getsize(file_name)
         if (siz == 0):
             subprocess.call(['rm',file_name])
             print('File was not found: ', file_name, ' at ', archive)
         else:
             print('File exists: ', file_name, ' at ', archive)
@@ -322,15 +335,15 @@
     QUERY_PARAMS['endDate'] =   str(year) + '-' + cmonth + '-' + cday + 'T23:59:30Z'
 
     headers = {}
     headers['Accept-Encoding'] = 'gzip'
 
     return QUERY_PARAMS, headers
 
-def universal_all(station9ch, year, doy, srate,stream):
+def universal_all(station9ch, year, doy, srate,stream,screenstats):
     """
     check multiple archives for RINEX 3 data
 
     Parameters
     ----------
     station9ch : str
         9 character station name
@@ -338,14 +351,16 @@
         full year
     doy : int
         doy of year
     srate : int
         receiver sample rate 
     stream : str
         R or S
+    screenstats : bool
+        print statements
 
     Peturns
     -------
     file_name : str
         rinex filename
     foundit : bool
         whether rinex file was found
@@ -396,28 +411,30 @@
     cdoy = '{:03d}'.format(doy)
     f1 = station  + cdoy + '0.' + cyyyy[2:4] + 'd'
     f2 = station  + cdoy + '0.' + cyyyy[2:4] + 'o'
 
     return f1, f2, cyyyy, cdoy
 
 
-def universal_rinex2(station, year, doy, archive):
+def universal_rinex2(station, year, doy, archive,screenstats):
     """
     seamless archive for rinex 2 files ...
 
     Parameters
     ----------
     station : str
         four character station name
     year : int
         full year
     doy : int
         day of year
     archive : str
         name of the GNSS archive
+    screenstats : bool
+        whether print statements come to scree
 
     Returns
     -------
     file_name : str
         filename that was downloaded
     foundit : bool
         whether file was found
@@ -428,15 +445,16 @@
     foundit = False; dir1 = ''; file_name = ''
 
     dname, oname, cyyyy, cdoy = rinex2names(station,year,doy)
     if os.path.exists(oname):
         #print('RINEX o File is already on disk')
         return oname, True 
 
-    print('Searching the ', archive, ' archive for ', station)
+    if screenstats:
+        print('Searching the ', archive, ' archive for ', station)
 
     cydoy = cyyyy + '/' + cdoy + '/'
     cyy = cyyyy[2:4]
 
     s1 = time.time()
     if (archive == 'jp'):
         # i did not want to rewrite the code
@@ -457,15 +475,16 @@
         if not foundit:
             url2 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy + oname + '.Z'
             print(url2)
             foundit,file_name = kelly.the_kelly_simple_way(url2, oname + '.Z')
     elif (archive == 'special'):
         #print('testing out new protocol at unavco')
         url1 = 'https://data.unavco.org/archive/gnss/products/reflectometry/' + cydoy + oname + '.gz'
-        print(url1)
+        if screenstats:
+            print(url1)
         foundit,file_name = kelly.the_kelly_simple_way(url1, oname + '.gz')
         # old way
         #foundit, file_name = gogetit(dir1, oname, '.gz'); 
     elif archive == 'sopac':
         dir1 = 'ftp://garner.ucsd.edu/pub/rinex/' + cydoy
         foundit, file_name = gogetit(dir1, dname, '.Z');
     elif archive == 'sonel':
@@ -516,21 +535,23 @@
                 file_url = query_response_item['fileLocation']
                 file_name = urlparse(file_url).path.rsplit('/', 1)[1]
                 wget.download(file_url,file_name)
     elif (archive == 'nrcan'):
         dir1 = 'ftp://cacsa.nrcan.gc.ca/gps/data/gpsdata/' + cyy + cdoy  + '/' + cyy + 'd' + '/'
         foundit, f = gogetit(dir1, dname, '.Z'); file_name = f
     else:
-         print('I do not recognize your archive')
+         print('I do not recognize your archive', archive)
 
     s2 = time.time()
-    print('Download took ', np.round(s2-s1,2),' seconds') 
+    if screenstats:
+        print('Download took ', np.round(s2-s1,2),' seconds') 
 
-    if not os.path.exists(file_name):
+    if not os.path.exists(file_name) and screenstats:
         print('Did not find the Rinex file')
+
     return file_name,foundit
 
 def make_rinex2_ofiles(file_name):
     """
     take a rinex2 file, gunzip or uncompress it, and 
     then Hatanaka decompress it
 
@@ -583,25 +604,25 @@
     ----------
     rinexfile : string
         name of the rinex2 file
     """
     print('You chose the strip option to reduce the number of observables in the RINEX file')
     teqcv = g.teqc_version()
     if os.path.isfile(teqcv):
-        print('Use teqc to strip the RINEX 2 file')
+        #print('Use teqc to strip the RINEX 2 file')
         foutname = 'tmp.' + rinexfile
         fout = open(foutname,'w')
         subprocess.call([teqcv, '-O.obs','S1+S2+S5+S6+S7+S8', rinexfile],stdout=fout)
         fout.close()
         subprocess.call(['rm','-f',rinexfile])
         subprocess.call(['mv','-f',foutname, rinexfile])
     else:
         gfzrnxpath = g.gfz_version()
         if os.path.isfile(gfzrnxpath):
-            print('Use gfzrnx to strip the RINEX 2 file')
+            #print('Use gfzrnx to strip the RINEX 2 file')
             tempfile = rinexfile + '.tmp'
             # save yourself heartache down the way cause those doppler data are just clogging up the works
             subprocess.call([gfzrnxpath,'-finp', rinexfile, '-fout', tempfile, '-vo','2','-f', '-obs_types', 'S','-q'])
             subprocess.call(['mv', '-f', tempfile, rinexfile])
 
 def gsi_data(station,year,doy):
     """
@@ -718,15 +739,15 @@
     headers = {}
     headers['Accept-Encoding'] = 'gzip'
 
     return QUERY_PARAMS, headers
 
 def serial_cddis_files(dname,cyyyy,cdoy):
     """
-    only looks in the hatanaka decompression section of cddis
+    Looks for rinex files in the hatanaka decompression section of cddis
 
     Parameters
     ----------
     dname : string
         rinex2 filename without compression extension
     cyyyy : string
         four character year
```

### Comparing `gnssrefl-1.3.8/gnssrefl/kelly.py` & `gnssrefl-1.4.1/gnssrefl/kelly.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     s1 = time.time()
     r = requests.get(url, headers=headers)
     s2 = time.time()
     # Opens a local file of same name as remote file for writing to
     # check to see that the file exists
     if (r.status_code == requests.codes.ok):
-        print('File was found', filename)
+        #print('File was found', filename)
         with open(filename, 'wb') as f:
             for data in r:
                 f.write(data)
         #f.close() 
 
         foundit = True
     else:
```

### Comparing `gnssrefl-1.3.8/gnssrefl/llh2xyz.py` & `gnssrefl-1.4.1/gnssrefl/llh2xyz.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import gnssrefl.gps as g
 
 def main():
     """
     Command line tool that converts latitude, longitude, and 
     ellipsoidal ht to Cartesian coordinates  and prints to the screen
 
-    Example
-    -------
+    Examples
+    --------
     llh2xyz  39.949492042 -105.194266387  1728.856
         returns  -1283634.1616   -4726427.8934    4074798.0432
 
     Parameters
     ----------
     lat : float
         latitude in degrees
```

### Comparing `gnssrefl-1.3.8/gnssrefl/make_json_input.py` & `gnssrefl-1.4.1/gnssrefl/make_json_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#
-# set up json input file needed for gnssir
-
 import argparse
 import json
 import os
 import subprocess
 import sys
 
 import gnssrefl.gps as g
@@ -51,20 +48,22 @@
     return {key: value for key, value in args.items() if value is not None}
 
 
 def make_json(station: str, lat: float, long: float, height: float, e1: int = 5, e2: int = 25,
               h1: float = 0.5, h2: float = 8.0, nr1: float = None, nr2: float = None,
               peak2noise: float = 2.8, ampl: float = 5.0, allfreq: bool = False,
               l1: bool = False, l2c: bool = False, xyz: bool = False, refraction: bool = True,
-              extension: str = '', ediff: float=2.0, delTmax: float=75.0, azlist: float=[], frlist: float=[] ):
+              extension: str = '', ediff: float=2.0, delTmax: float=75.0, azlist: float=[], 
+              frlist: float=[]):
 
     """
-    Saves the lomb scargle analysis strategy you will use in gnssrefl. Store in 
-    a json file which by default is saved
-    in REFL_CODE/<station>.json.
+    WE NO LONGER RECOMEND USING THIS CODE. Please see the gnssir_input.py code instead.
+
+    This code saves the Lomb Scargle analysis strategy you will use in gnssrefl. Store in 
+    a json file which by default is saved in REFL_CODE/<station>.json.
 
     Examples
     --------
 
     make_json_input p041 0 0 0 
         uses only GPS frequencies and all azimuths and the coordinates in the UNR database
 
@@ -202,15 +201,14 @@
 
     # where the instructions will be written
     xdir = os.environ['REFL_CODE']
     outputdir = xdir + '/input'
     if not os.path.isdir(outputdir):
         subprocess.call(['mkdir', outputdir])
 
-    print('extension', extension)
     if len(extension) == 0:
         outputfile = outputdir + '/' + station + '.json'
     else:
         outputfile = outputdir + '/' + station + '.' + extension + '.json'
 
     lsp['polyV'] = 4 # polynomial order for DC removal
     # change this so the min elevation angle for polynomial removal is the same as the
```

### Comparing `gnssrefl-1.3.8/gnssrefl/nmea2snr.py` & `gnssrefl-1.4.1/gnssrefl/nmea2snr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,114 @@
 # -*- coding: utf-8 -*-
-"""
-This code is missing full documentation.
-
-"""
 from __future__ import division
+import json
 import numpy as np 
 import os, datetime, traceback
 import subprocess
+import sys
 from scipy.interpolate import interp1d
 
 import gnssrefl.gps as g
+import gnssrefl.decipher_argt as gt
 
 #Last modified Feb 22, 2023 by Taylor Smith (git: tasmi) for additional constellation support
 
-def NMEA2SNR(locdir, fname, snrfile, csnr):
+def NMEA2SNR(locdir, fname, snrfile, csnr,dec,year,doy,llh,sp3):
     """
+    Reads and translates the NMEA file stored in locdir + fname
+
+    Naming convention assumed for NMEA files :  SSSS1520.23.A
+
+    where SSSS is station name, day of year is 152 and year is 2023
+
+    locdir is generally $REFL_CODE/nmea/SSSS/yyyy where yyyy is the year number and SSSS is the station name
+
+    I believe lowercase is also allowed, but the A at the end is still set to be upper case
+
+    (I believe) The SNR files are stored with upper case if given upper case, lower case if given lower case.
+
 
     Parameters
     -----------
     locdir : str
-        directory where your SNR files are kept
-    fname : string
+        directory where your NMEA files are kept
+    fname : str
         NMEA filename 
     snrfile : str
         name of output file for SNR data
     csnr : str
         snr option, i.e. '66' or '99'
+    dec : int
+        decimation value in seconds
+    year : int
+        full year
+    doy : int
+        day of year
+    llh : list of floats
+        station location, lat (deg), lon(deg), height (m)
+    sp3 : bool
+        whether you use multi-GNSS sp3 file to do azimuth elevation angle calculations
+        currently this only uses the GFZ rapid orbit.  
         
     """
     
+    idec = int(dec)
     missing = True
+    station = fname.lower() ; station = station[0:4]
+    yy,month,day, cyyyy, cdoy, YMD = g.ydoy2useful(year,doy)
+
+    foundcoords = False
+    if (llh[0] != 0):
+        # compute Cartesian receiver coordinates in meters
+        x,y,z = g.llh2xyz(llh[0],llh[1],llh[2])
+        recv = [x,y,z]
+        foundcoords = True
+
+    if sp3 and (not foundcoords):
+        # try to get the LLH from json file
+        jfile1  = os.environ['REFL_CODE'] + '/input/' + station.upper() + '.json'
+        jfile2  = os.environ['REFL_CODE'] + '/input/' + station.lower() + '.json'
+        fexists = False
+        if os.path.isfile(jfile1):
+            jfile = jfile1 ; fexists = True
+            print('json file found ',jfile1)
+        elif os.path.isfile(jfile2):
+            jfile = jfile2 ; fexists = True
+            print('json file found ',jfile2)
+
+        if fexists:
+            with open(jfile, 'r') as my_json:
+                fcont = json.load(my_json)
+
+            llh[0] = fcont['lat']; llh[1] = fcont['lon'] ; llh[2] = fcont['ht']
+            x,y,z = g.llh2xyz(llh[0],llh[1],llh[2])
+            recv = [x,y,z]
+            foundcoords = True
+        else:
+            print('This code requires lat/lon/ht inputs. Provide on the command line or')
+            print('make a json file using gnssir_input.  Exiting')
+            return
+
+    if sp3:
+        xf,orbdir,foundit=g.rapid_gfz_orbits(year,month,day)
+        if not foundit: 
+            print('Could not find the rapid orbits. Exiting')
+            return
+        else:
+            orbfile = orbdir + '/' + xf # hopefully
+
+    # this is to help a colleague 
+    if station == 'argt':
+        gt.decipher_argt(station,'jul01.txt',idec,snrfile,orbfile,recv,csnr,year,month,day)
+        if os.path.isfile(snrfile):
+            print('File made, ignoring the rest of the code')
+            return
+        else:
+            print('Translation was unsuccessful'); return
+
 
     #check whether the input file is a uncompressed or compressed     
     if os.path.exists(locdir + fname):
         subprocess.call(['cp', '-f',locdir + fname ,'.'])
         t, prn, az, elv, snr, freq = read_nmea(fname)#read nmea files
         subprocess.call(['rm',fname])
         missing = False
@@ -48,29 +123,34 @@
     if os.path.exists(locdir + fname + '.Z') and missing:
         subprocess.call(['cp', '-f',locdir + fname + '.Z','.'])
         subprocess.call(['uncompress', fname + '.Z'])
         t, prn, az, elv, snr, freq = read_nmea(fname)#read nmea files
         subprocess.call(['rm',fname])
         missing = False
         
-    t = np.array(t);az = np.array(az);elv = np.array(elv);snr = np.array(snr);prn = np.array(prn); freq=np.array(freq)
 
+    # why is there all this going back and forth between lists and np arrays?
+
+    t = np.array(t);az = np.array(az);elv = np.array(elv);snr = np.array(snr);prn = np.array(prn); freq=np.array(freq)
     #remove empty records
-    t = t[az !=''];snr = snr[az !=''];prn = prn[az !=''];elv = elv[az !=''];freq = freq[az != ''];az = az[az !=''];
-    t = t[elv !=''];az = az[elv !=''];snr = snr[elv !=''];prn = prn[elv !=''];freq = freq[elv != ''];elv = elv[elv !='']
-    t = t[snr !=''];az = az[snr !=''];prn = prn[snr !=''];elv = elv[snr !=''];freq = freq[snr != ''];snr = snr[snr !='']
-    t = t[prn !=''];az = az[prn !=''];elv = elv[prn !=''];snr = snr[prn !=''];freq = freq[prn != ''];prn = prn[prn !=''] 
-    t = t[freq !=''];az = az[freq !=''];elv = elv[freq !=''];snr = snr[freq !=''];prn = prn[freq !='']; freq = freq[freq != '']
+    if (station != 'argt'):
+        #????
+        t = t[az !=''];snr = snr[az !=''];prn = prn[az !=''];elv = elv[az !=''];freq = freq[az != ''];az = az[az !=''];
+        t = t[elv !=''];az = az[elv !=''];snr = snr[elv !=''];prn = prn[elv !=''];freq = freq[elv != ''];elv = elv[elv !='']
+        t = t[snr !=''];az = az[snr !=''];prn = prn[snr !=''];elv = elv[snr !=''];freq = freq[snr != ''];snr = snr[snr !='']
+        t = t[prn !=''];az = az[prn !=''];elv = elv[prn !=''];snr = snr[prn !=''];freq = freq[prn != ''];prn = prn[prn !=''] 
+        t = t[freq !=''];az = az[freq !=''];elv = elv[freq !=''];snr = snr[freq !=''];prn = prn[freq !='']; freq = freq[freq != '']
     
     az = az.astype(float)
     elv = elv.astype(float)
     snr = snr.astype(float)
     prn = prn.astype(int)
 
     prn_unique = np.unique(prn) 
+    #print(prn_unique)
 
     T = []; PRN = []; AZ = []; ELV = []; SNR = []; FREQ = []        
     for i_prn in prn_unique:
         # the original code added 100 - but did not take into account the 
         # satellite numbers have been shifted for glonass.
         # also there is an illegal signal at satellite "48" 
         # i do not know what that is, but i am ignoring it.
@@ -83,14 +163,34 @@
         if (len(angle_fixed) == 0 and len(azim_fixed) == 0):
             continue
             
         T.extend(time);AZ.extend(azim_fixed);ELV.extend(angle_fixed);SNR.extend(Snr);PRN.extend(Prn); FREQ.extend(frequency)
         
         del  time, angle, azimuth, Snr, Prn, angle_fixed, azim_fixed, frequency
         
+    if sp3:
+        tmpfile =  station + 'tmp.txt'
+        #print('Opening temporary file : ', tmpfile)
+        fout = open(tmpfile, 'w+')
+        fout.write('{0:15.4f}{1:15.4f}{2:15.4f} \n'.format(recv[0], recv[1],recv[2]) )
+        fout.write('{0:6.0f}{1:6.0f}{2:6.0f} \n'.format(year, month, day) )
+        #(t[i], prn[i], snr[i],freq[i])
+        for i in range(0,len(T)):
+            if ( (int(t[i]) % idec) == 0):
+                sat = PRN[i]
+                # glonass satellites are misnamed by the code
+                if (sat > 100) & (sat < 200):
+                    sat = sat - 64
+                fout.write('{0:8.0f} {1:3.0f} {2:6.2f} {3:s} \n'.format(T[i], sat, SNR[i], freq[i]) )
+        fout.close()
+        # make the snrfile
+        gt.new_azel(station,tmpfile,snrfile,orbfile,csnr)
+        return
+
+
     inx = np.argsort(T)  #Sort data by time
     
     T = np.array(T);PRN = np.array(PRN);ELV = np.array(ELV);SNR = np.array(SNR);AZ = np.array(AZ); FREQ=np.array(FREQ)
     
     T = T[inx];PRN = PRN[inx];ELV = ELV[inx];SNR = SNR[inx];AZ = AZ[inx]; FREQ=FREQ[inx]
                                
     emin,emax = elev_limits(int(csnr))#select snr option 50, 66, 88, 99
@@ -140,36 +240,41 @@
                 #S6 SNR on L6
                 #S1 SNR on L1
                 #S2 SNR on L2
                 #S5 SNR on L5
                 #S7 SNR on L7
                 #S8 SNR on L8        
                 
+                # it is not necessary to write out l7 and l8.  or l6. zero can be put there.
                 l1 = 0; l2 = 0; l5 = 0; l6 = 0; l7 = 0; l8 = 0
                 
                 #Check what frequency we are at to know where to write each line
                 f_store = FREQ[i]
                 if f_store == '1':
                     l1 = float(SNR[i])
                 elif f_store == '2':
                     l2 = float(SNR[i])
                 elif f_store == '5':
                     l5 = float(SNR[i])
-                elif f_store == '6':
-                    l6 = float(SNR[i])
-                elif f_store == '8':
-                    l8 = float(SNR[i])
+                # remove l6 and l7 ... we can add back in if a cheap instrument ever produces these obs
+                #elif f_store == '6':
+                #    l6 = float(SNR[i])
+                #elif f_store == '8':
+                #    l8 = float(SNR[i])
                     
-                #NOTE -- All satellites have a 'mixed/undefined' frequency 0 for NMEA 4.11 (https://gpsd.gitlab.io/gpsd/NMEA.html#_nmea_4_11_system_id_and_signal_id)
+                #NOTE -- All satellites have a 'mixed/undefined' frequency 0 for 
+                # NMEA 4.11 (https://gpsd.gitlab.io/gpsd/NMEA.html#_nmea_4_11_system_id_and_signal_id)
                 #This is never used here so could leave blank snr lines!
                 
                 outline = "%3g %10.4f %10.4f %10g %4s " % (p, float(ELV[i]), float(AZ[i]), float(T[i]), '0')
-                snrline = "%7.2f %7.2f %7.2f %7.2f %7.2f %7.2f" % (l6, l1, l2, l5, l7, l8)
-    
-                fout.write(outline + snrline + '\n')
+                snrline = "%7.2f %7.2f %7.2f %7.2f " % (l6, l1, l2, l5 )
+                 
+                # apply decimating here
+                if ( (int(T[i]) % idec) == 0):
+                    fout.write(outline + snrline + '\n')
                 #fout.write("%3g %10.4f %10.4f %10g %4s %4s %7.2f %4s %4s\n" % (p, float(ELV[i]), float(AZ[i]), float(T[i]),'0', '0', float(SNR[i]),'0', '0')) 
     
 def read_nmea(fname):
     """
     read GPGGA sentence (includes snr data) in NMEA files    
 
     Parameters
@@ -220,15 +325,18 @@
             continue
         
         #line = line.replace('$', '') #Strip leading $
         
         if 'RMC' in line: #Get timing info
             row = line.split(',')
             #sect = int(float(row[1][0:2]) * 60 * 60 + float(row[1][2:4]) * 60 + float(row[1][4:])) #Time in seconds
-            curdt = datetime.datetime(int(row[9][4:6])+2000,int(row[9][2:4]),int(row[9][0:2])) #Current date
+            try:
+                curdt = datetime.datetime(int(row[9][4:6])+2000,int(row[9][2:4]),int(row[9][0:2])) #Current date
+            except:
+                pass
         
         if not curdt: #Skip forward until the first 'RMC' instance which gives a proper date to store
             continue
         
         if 'GGA' in line: #read GPGGA sentence: Global Positioning System Fix Data 
             hr = int(line.split(",")[1][0:2])
             mn = int(line.split(",")[1][2:4])
@@ -418,44 +526,53 @@
     azim_b = azim[1:]
     diff = azimuth_diff2 (azim_b, azim_a);
     #diff = azimuth_diff2 (azima, azimb);  % WRONG!   
     return diff
 
 def azimuth_diff(azim1, azim2):
     """
+    someone should document this
+
     Parameters
     ----------
     azim1 : ??
 
     azim2 : ??
 
+    Returns
+    -------
+    ???
+
     """
     if not(azim2.size):
         diff = azimuth_diff1 (azim1)
     else:
         diff = azimuth_diff2 (azim1, azim2)
 #    diff = np.abs(diff)
     return diff
      
 def angle_range_positive(ang):
     """
+    someone should document this
 
     Parameters
     ----------
     ang : ??
 
     """
 #    idx1 = np.isfinite(ang)
     ang = np.angle(np.exp(1j*ang*np.pi/180))*180/np.pi  
     idx2 = (ang < 0)
     ang[idx2] = 360 + ang[idx2]
     return ang
 
 def azimuth_mean(azim1, azim2):
     """
+    someone should document this
+
     Parameters
     ----------
     azim1 : list of floats ? 
          azimuth degrees
 
     azim2 : list of floats
          azimuth degrees
@@ -476,15 +593,16 @@
         x = ( (x1 + x2)/2.0 )[0];y = ( (y1 + y2)/2.0 )[0]
         azim = 180/np.pi * np.arctan2(x, y)
 
     return azim
 
 def quickname(station,year,cyy, cdoy, csnr):
     """
-    full name of the snr file name (incl path) 
+    Creates a full name of the snr file name (i.e. including the path) 
+    >>>> Checks that directories exist.
 
     Parameters
     ----------
     station : str
         4 ch station name
 
     year : int
@@ -503,24 +621,32 @@
     -------
     fname : str
         output filename
 
     """
     
     xdir  = os.environ['REFL_CODE'] + '/'
-    fname =  xdir + str(year) + '/snr/' + station + '/' + station + cdoy + '0.' + cyy + '.snr' + csnr
-    if not (os.path.exists(xdir + str(year) + '/snr/' + station+'/')):
-        os.system('mkdir -p '+xdir + str(year) + '/snr/' + station+'/')
+    cyyyy = str(year)
+    fname =  xdir + cyyyy + '/snr/' + station + '/' + station + cdoy + '0.' + cyy + '.snr' + csnr
+    d = xdir + cyyyy
+    if not os.path.isdir(d):
+        subprocess.call(['mkdir', d])
+    d = xdir + cyyyy + '/snr'
+    if not os.path.isdir(d):
+        subprocess.call(['mkdir', d])
+    d = xdir + cyyyy + '/snr/' + station
+    if not os.path.isdir(d):
+        subprocess.call(['mkdir', d])
 
     return fname
 
 def elev_limits(snroption):
     """
 
-    given snr option return the elevation angle limits
+    Given a snr option, return the elevation angle limits
 
     Parameters
     ----------
     snroption : int
         snrfile number
 
     Returns
@@ -541,58 +667,73 @@
     elif (snroption == 88):
         emin = 0; emax = 90
     else:
         emin = 5; emax = 30
 
     return emin, emax
   
-def run_nmea2snr(station, year_list, doy_list, isnr, overwrite):
+def run_nmea2snr(station, year_list, doy_list, isnr, overwrite,dec,llh,sp3):
     """
     runs the nmea2snr conversion code
 
+    Looks for NMEA files in $REFL_CODE/nmea/ssss/2023 for station ssss and year 2023.
+    I prefer lowercase station names, but I believe the code allows both upper and lower
+    case. 
+
+    Files are named:  SSSS1520.23.A 
+
+    where SSSS is station name, day of year 152 and 
+    the last two characters of the 2023 as the middle value.
+
+    The SNR files are stored with upper case if given upper case, lower case if given lower case.
+
     Parameters
     ----------
     station : str
-        name of station 
-
+        4 ch name of station 
     year_list : list of integers
         years 
-
     doy_list : list of days of year
         days of years
-
     isnr : int
         snr file type
-
     overwrite : bool
         whether make a new SNR file even if one already exists
+    dec : int
+        decimation in seconds
+    llh : list of floats
+        lat and lon (deg) and ellipsoidal ht (m)
+    sp3 : bool
+        whether you want to use GFZ rapid sp3 file for the orbits
 
     """
     # loop over years and day of years
     for yr in year_list:
         
         locdir= os.environ['REFL_CODE'] + '/nmea/' + station + '/' + str(yr) + '/'
         for dy in doy_list:
             csnr = str(isnr)
             cdoy = '{:03d}'.format(dy)
             cyy = '{:02d}'.format(yr-2000)
             snrfile =  quickname(station,yr,cyy,cdoy,csnr)#snr filename
             snre = g.snr_exist(station,yr,dy,csnr)#check if snrfile already sxists
             if snre:
-                print('SNR file exists', snrfile)
-            if overwrite:
-                subprocess.call(['rm', snrfile])
-                snre = False
+                if overwrite:
+                    print('SNR file exists, but you requested it be overwritten')
+                    subprocess.call(['rm', snrfile])
+                    snre = False
+                else:
+                    print('SNR file already exists', snrfile)
         
             illegal_day = False
             if (float(dy) > g.dec31(yr)):
                 illegal_day = True
         
             if (not illegal_day) and (not snre):
                 r =  station + cdoy + '0.' + cyy + '.A'# nmea file name example:  WESL2120.21.A 
-                
-                if os.path.exists(locdir+r) or os.path.exists(locdir+r+'.gz') or os.path.exists(locdir+r+'.Z'):
-                    print('Creating '+snrfile)
-                    NMEA2SNR(locdir, r, snrfile, csnr)
-                    
+                if os.path.exists(locdir+r) or os.path.exists(locdir+r+'.gz') or os.path.exists(locdir+r+'.Z') or (station == 'argt'):
+                    #print('Creating '+snrfile)
+                    NMEA2SNR(locdir, r, snrfile, csnr,dec,yr,dy,llh,sp3)
+                    if os.path.isfile(snrfile):
+                        print('SUCCESS: SNR file created', snrfile)
                 else:
                     print('NMEA file '+ locdir + r +' does not exist')
```

### Comparing `gnssrefl-1.3.8/gnssrefl/phase_functions.py` & `gnssrefl-1.4.1/gnssrefl/phase_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,15 @@
 
     # this is arbitrary
     min_num_pts = 20
 
 
     # get the SNR filename
     obsfile, obsfilecmp, snrexist = g.define_and_xz_snr(station, year, doy, snr_type)
+    #print(obsfile,obsfilecmp,snrexit)
 
     # noise region - hardwired for normal sites ~ 2-3 meters tall
     noise_region = [0.5, 8]
 
 
     if not snrexist:
         print('No SNR file on this day.')
```

### Comparing `gnssrefl-1.3.8/gnssrefl/prn2gps.py` & `gnssrefl-1.4.1/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/query_unr.py` & `gnssrefl-1.4.1/gnssrefl/query_unr.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,11 @@
     if len(station) != 4:
         print('illegal station name-must be 4 characters')
         sys.exit()
     alat,alon,ht=g.queryUNR_modern(station.lower())
     if (alat+alon+ht) != 0:
         x,y,z=g.llh2xyz(alat,alon,ht)
         print('XYZ', round(x,4),round(y,4),round(z,4) )
+        print('LLH', round(alat,6),round(alon,6),round(ht,3) )
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.3.8/gnssrefl/quickLook_cl.py` & `gnssrefl-1.4.1/gnssrefl/quickLook_cl.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,94 +4,98 @@
 """
 import argparse
 import sys
 
 # internal codes
 import gnssrefl.gps as g
 import gnssrefl.quickLook_function as quick
+import gnssrefl.quickLook_function2 as quick2
 
 from gnssrefl.utils import validate_input_datatypes, str2bool
 
 
 def parse_arguments():
-# user inputs the observation file information
     parser = argparse.ArgumentParser()
     parser.add_argument("station", help="station name", type=str)
     parser.add_argument("year", help="year", type=int)
     parser.add_argument("doy", help="day of year", type=int)
     parser.add_argument("-snr", default=None, type=int, help="snr ending - default is 66")
     parser.add_argument("-fr", default=None, type=int, help="e.g. -fr 1 for GPS L1  or -fr 101 for Glonass L1")
     parser.add_argument("-ampl", default=None, type=float, help="minimum spectral amplitude allowed")
-    parser.add_argument("-e1",  default=None, type=int, help="lower limit elevation angle (default is 5 deg) ")
-    parser.add_argument("-e2",  default=None, type=int, help="upper limit elevation angle (default is 25 deg)")
+    parser.add_argument("-e1",  default=None, type=float, help="lower limit elevation angle (default is 5 deg) ")
+    parser.add_argument("-e2",  default=None, type=float, help="upper limit elevation angle (default is 25 deg)")
     parser.add_argument("-h1",  default=None, type=float, help="lower limit reflector height (default is 0.5m) ")
     parser.add_argument("-h2",  default=None, type=float, help="upper limit reflector height (default is 8 m)")
     parser.add_argument("-azim1",  default=None, type=float, help="lower limit azimuth (default is 0 deg)")
     parser.add_argument("-azim2",  default=None, type=float, help="upper limit azimuth (default is 360 deg)")
     parser.add_argument("-sat", default=None, type=int, help="satellite")
     parser.add_argument("-screenstats", default=None, type=str, help="if True, Success and Failure info printed to the screen")
     parser.add_argument("-peak2noise",  default=None, type=float, help="Quality Control ratio (default is 3)")
     parser.add_argument("-ediff",  default=None, type=float, help="ediff Quality Control parameter (default 2 deg)")
+    parser.add_argument("-delTmax",  default=None, type=float, help="maximum arc length, in minutes, (default is 75 )")
     parser.add_argument("-plt", default=None, type=str, help="Set to false to turn off plots to the screen.")
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
     boolean_args = ['screenstats','plt']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def quicklook(station: str, year: int, doy: int,
               snr: int = 66, fr: int = 1, ampl: float = 7.,
-              e1: int = 5, e2: int = 25, h1: float = 0.5, h2: float = 8., sat: int = None,
+              e1: float = 5, e2: float = 25, h1: float = 0.5, h2: float = 8., sat: int = None,
               peak2noise: float = 3., screenstats: bool = False, fortran: bool = None, 
-              plt: bool = True, azim1: float = 0., azim2: float = 360., ediff: float = 2.0):
+              plt: bool = True, azim1: float = 0., azim2: float = 360., ediff: float = 2.0, delTmax : float=75.0 ):
     """
 
     quickLook assessment of SNR reflectometry data. It creates two plots: one with periodograms for
     four different quadrants (northwest, northeast, southeast, southwest) and the other with the RH
     results shown as a function of azimuth. This plot also summarizes why the RH retrievals were accepted
     or rejected in terms of the quality control parameters.  
 
-    Example:
+    Examples
+    --------
+    quickLook p041 2023 1 
+        analyzes station p041 on day of year 1 in the year 2023 with defaults (L1, e1=5, e2=25)
+
+    quickLook p041 2023 1 -h1 1 -h2 10
+        analyzes station p041 on day of year 1 in the year 2023.  
+        The periodogram would be restricted to RH of 1-10 meters.  
 
-    quickLook p041 2023 1 -h1 1 -h2 8
-
-    would analyze station p041 on day of year 1 in the year 2023.  The periodogram would be 
-    restricted to 1-8 meters.  
 
     No refraction correction is applied at this stage. For this reason, very low elevation angle data at 
     very tall sites will appear to be of very poor quality.
 
     Parameters
     ----------
-    station : string
+    station : str
         4 character ID of the station
-    year : integer
+    year : int
         Year
-    doy : integer
+    doy : int
         Day of year
-    snr : integer, optional
+    snr : int, optional
         SNR format. This tells the code which SNR file to use.  66 is the default.
         Other options: 50, 88, and 99.
 
-    f : integer, optional. 
+    f : int, optional. 
         GNSS frequency. Default is GPS L1
         value options:
 
             1,2,20,5 : GPS L1,L2,L2C,L5 (1 is default)
 
             101,102 : GLONASS L1 and L2
 
             201,205,206,207,208 : GALILEO E1 E5a E6,E5b,E5
 
-            302,306,207 : BEIDOU B1, B3, B2
+            302,306,307 : BEIDOU B1, B3, B2
 
     reqAmp : int or array_like, optional
         Lomb-Scargle Periodogram (LSP) amplitude significance criterion in volts/volts.
         Default is 7 
 
     e1 : int, optional
         elevation angle lower limit in degrees for the LSP.
@@ -134,14 +138,18 @@
         maximum azimuth angle (deg)
         default is 360.
 
     ediff : float, optional
         elevation angle difference, quality control parameter 
         default is 2 degrees.
 
+    delTmax: float, optional
+        maximum allowed arc length, in minutes
+        default is 75 minutes.
+
     """
 
 #   make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
 
     exitS = g.check_inputs(station, year, doy, snr)
 
@@ -154,34 +162,38 @@
         fr = [fr]  # default is to do L1
 
     pele = [5, 30]  # polynomial fit limits
     if ampl is not type(list):
         ampl = [ampl]  # this is arbitrary  - but often true for L1 obs
 
     if e1 < 5:
-        print('have to change the polynomial limits because you went below 5 degrees')
-        print('this restriction is for quickLook only ')
+        print('We have to change the polynomial limits because you went below 5 degrees.')
+        print('This restriction is for quickLook only ')
         pele[0] = e1
 
     pltscreen = plt
     args = {'station': station.lower(), 'year': year, 'doy': doy, 'snr_type': snr, 'f': fr[0], 'reqAmp': ampl, 'e1': e1,
             'e2': e2, 'minH': h1, 'maxH': h2, 'PkNoise': peak2noise, 'satsel': sat, 'fortran': fortran, 'pele': pele,
-            'pltscreen': pltscreen, 'screenstats': screenstats, 'azim1': azim1, 'azim2': azim2, 'ediff': ediff}
+            'pltscreen': pltscreen, 'screenstats': screenstats, 'azim1': azim1, 'azim2': azim2, 'ediff': ediff, 'delTmax': delTmax}
 
     deltaRH = h2-h1
     if (deltaRH <= 0):
         print('Your reflector height region is invalid (i.e. h1 is greater than h2). h1:', h1, ' h2: ',h2)
         print('Exiting')
         sys.exit()
 
     if (deltaRH < 5.5):
         print('The reflector height region must be at least 5.5 meters long. These values are used for computing ')
         print('a valid periodogram and for quality control.  Change h1 or h2 or both. Exiting')
         sys.exit()
-    return quick.quickLook_function(**args)
+
+    if True:
+        return quick2.quickLook_function(**args)
+#    else:
+#        return quick.quickLook_function(**args)
     # returns two variables: data, datakey = quick.quicklook_function(**args)
 
     # the key is saved wth the same keys as the data dictionary, in this order 
     # [avgAzim, RH, satNumber,frequency,maxAmplitude,Peak2Noise, UTChour]
 
 
 def main():
```

### Comparing `gnssrefl-1.3.8/gnssrefl/quickLook_function.py` & `gnssrefl-1.4.1/gnssrefl/quickLook_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-called by quickLook_cl.py
-quickLook functions 
-"""
 import sys
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.figure import Figure
 import subprocess
 import warnings
@@ -13,15 +9,16 @@
 import scipy.interpolate
 import scipy.signal
 
 import gnssrefl.gps as g
 import gnssrefl.rinex2snr as rinex
 
 
-def quickLook_function(station, year, doy, snr_type,f,e1,e2,minH,maxH,reqAmp,pele,satsel,PkNoise,fortran,pltscreen,azim1,azim2,ediff,**kwargs):
+def quickLook_function(station, year, doy, snr_type,f,e1,e2,minH,maxH,reqAmp,pele,satsel,PkNoise,fortran,
+        pltscreen,azim1,azim2,ediff, delTmax,**kwargs):
     """
     This is the main function to compute spectral characteristics of a SNR file.
     It takes in all user inputs and calculates reflector heights. It makes two png files to summarize
     the data.
 
     Parameters
     ----------
@@ -57,14 +54,16 @@
         whether you want plots sent to the terminal
     azim1 : float
          minimum azimuth in degrees
     azim2 : float
          maximum azimuth in degrees
     ediff : float
          QC parameter - restricts length of arcs (degrees)
+    delTmax : float
+         maximum arc length in minutes
 
     """
 
     if ((maxH - minH) < 5.5):
         print('Requested reflector heights (', minH, ',', maxH, ') are too close together. ')
         print('They must be at least 5.5 meters apart - and preferably further than that. Exiting')
         return
@@ -100,15 +99,15 @@
     bx = [0,1,0,1]; by = [0,0,1,1]; bz = [1,3,2,4]
 
     #  fontsize
     fs = 10
     # various defaults - ones the user doesn't change in this quick Look code
     # changed this december 4, 2022
     # changed it back on december 20, 2022
-    delTmax = 75 # this is how long an arc can be in minutes
+    #delTmax = 75 # this is how long an arc can be in minutes
     polyV = 4 # polynomial order for the direct signal
     desiredP = 0.01 # 1 cm precision for a "quick Look"
 
     #four_in_one = True # put the plots together
     minNumPts = 20 
     #noise region for LSP QC. these are meters
     NReg = [minH, maxH]
@@ -125,18 +124,16 @@
 # not sure that that is all that useful as I never let that happen
     obsfile = g.define_quick_filename(station,year,doy,snr_type)
     if os.path.isfile(obsfile):
         print('>>>> The snr file exists ',obsfile)
     else:
         if True:
             obsfile, obsfileCmp, snre =  g.define_and_xz_snr(station,year,doy,snr_type)
-            if snre:
-                dkfjaklj = True
-            else:
-                print('>>>> The SNR the file needs does not exist ',obsfile)
+            if not snre:
+                print('>>>> The SNR file this code needs does not exist ',obsfile)
                 print('Please use rinex2snr to make a SNR file')
                 sys.exit()
     allGood,sat,ele,azi,t,edot,s1,s2,s5,s6,s7,s8,snrE = read_snr_simple(obsfile)
     # this just means the file existed ... not that it had the frequency you want to use
     if allGood == 1:
         # make output file for the quickLook RRH values, just so you can give them a quick look see
         quicklog = 'logs/rh_' + station + '.txt'
@@ -187,19 +184,15 @@
                     ax4=plt.subplot(2,2,bz[a])
 
                 plt.title(titles[a],fontsize=fs)
             az1 = azval[(a*2)] ; az2 = azval[(a*2 + 1)]
 
             # this means no satellite list was given, so get them all
             if satsel == None:
-                #satlist = g.find_satlist(f,snrE)
-                #march 29, 2021 made l2c and l5 time dependent
                 satlist = g.find_satlist_wdate(f,snrE,year,doy)
-                #print(f,year,doy)
-                #print(satlist)
             else:
                 satlist = [satsel]
 
             for satNu in satlist:
                 x,y,Nv,cf,UTCtime,avgAzim,avgEdot,Edot2,delT= g.window_data(s1,s2,s5,s6,s7,s8,sat,ele,azi,t,edot,f,az1,az2,e1,e2,satNu,polyV,pele,screenstats) 
                 allpoints = allpoints + Nv
                 # if screenstats:
```

### Comparing `gnssrefl-1.3.8/gnssrefl/quickPhase.py` & `gnssrefl-1.4.1/gnssrefl/quickPhase.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,29 +29,27 @@
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def quickphase(station: str, year: int, doy: int, year_end: int = None, doy_end: int = None, snr: int = 66, 
-        fr: str = '20', e1: float = 5, e2: float = 30, plt: bool = False, screenstats: bool = False, gzip:bool=False):
+        fr: str = '20', e1: float = 5, e2: float = 30, plt: bool = False, screenstats: bool = False, gzip: bool = False):
     """
-    quickphase computes phase for the given inputs (station, years, doy, elevation angles)
-    These phase results are subquently used in vwc. The command line call is phase
+    quickphase computes phase, which are subquently used in vwc. The command line call is phase
     (which maybe we should change).
     
     Examples
     --------
     phase p038 2021 4
         analyzes data for year 2021 and day of year 4
 
     phase p038 2021 1 -doy_end 365 
         analyzes data for the whole year
 
-
     Parameters
     ----------
     station: str
         4 character ID of the station.
 
     year: int
         full Year to evaluate.
@@ -67,52 +65,51 @@
         Day of year to end analysis. Using this option will create a range of doy-doy_end.
         If also using year_end, then this will be the day to end analysis in the year_end requested.
         Default is None.
 
     snr : int, optional
         SNR format. This tells the code what elevation angles are in the SNR file
         value options:
+
             66 (default) : data with elevation angles less than 30 degrees
 
             99 : data with elevation angles between 5 and 30 degrees
 
             88 : data with all elevation angles 
 
             50 : data with elevation angles less than 10 degrees
 
     fr : str, optional
-        GNSS frequency. Currently only supports L2C.
-        Default is 20 (l2c)
+        GNSS frequency. Currently only supports L2C. Default is 20 (l2c)
 
     e1 : float, optional
-        Elevation angle lower limit in degrees for the LSP.
-        default is 5
+        Elevation angle lower limit in degrees for the LSP. default is 5
 
     e2: float, optional
-        Elevation angle upper limit in degrees for the LSP.
-        default is 30
+        Elevation angle upper limit in degrees for the LSP. default is 30
 
     plt: bool, optional
-        Whether to plot results.
-        Default is False
+        Whether to plot results. Default is False
 
     screenstats: bool, optional
-        Whether to print stats to the screen.
-        Default is False
+        Whether to print stats to the screen. Default is False
 
     Returns
     -------
     Saves a file for each day in the doy-doy_end range: $REFL_CODE/<year>/phase/<station>/<doy>.txt
 
     columns in files:
         year doy hour phase nv azimuth sat ampl emin emax delT aprioriRH freq estRH pk2noise LSPAmp
 
     """
 
     compute_lsp = True # used to be an optional input
+    if len(station) != 4:
+        print('Station name must be four characters long. Exiting.')
+        sys.exit()
 
     if fr == 'all':
         fr_list = [1, 20]
         ex = qp.apriori_file_exist(station,20)
         if (not ex):
             print('No apriori RH file exists. Run vwc_input')
             sys.exit()
```

### Comparing `gnssrefl-1.3.8/gnssrefl/quicklib.py` & `gnssrefl-1.4.1/gnssrefl/quicklib.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/quickplt.py` & `gnssrefl-1.4.1/gnssrefl/quickplt.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         T or True, to reverse y-axis limits
     title : str, optional
         title for plot 
     outfile : str, optional
         name of png file to store plot 
     ylimits: float, optional
         pair of yaxis limits  
+    xlimits: float, optional
+        pair of xaxis limits  
 
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("filename", help="filename", type=str)
     parser.add_argument("xcol", help="x-column", type=str)
     parser.add_argument("ycol",   help="y-column", type=str)
@@ -70,14 +72,15 @@
     parser.add_argument("-ymdhm", help="if True/T, columns 1-4 are year mon day hour minute", type=str,default=None)
     parser.add_argument("-xlabel", type=str, help="optional x-axis label", default=None)
     parser.add_argument("-ylabel", type=str, help="optional y-axis label", default=None)
     parser.add_argument("-symbol", help="plot symbol ", type=str,default=None)
     parser.add_argument("-title", help="optional title", type=str,default=None)
     parser.add_argument("-outfile", help="optional filename for plot", type=str,default=None)
     parser.add_argument("-ylimits", nargs="*",type=float, help="optional ylimits", default=None)
+    parser.add_argument("-xlimits", nargs="*",type=float, help="optional xlimits", default=None)
     parser.add_argument("-ydoy", help="if True/T, columns 1-2 are year and doy", type=str,default=None)
     parser.add_argument("-filename2", help="second filename", type=str, default=None)
 
     args = parser.parse_args()
 
     filename = args.filename
     # change column numbers to pythonese
@@ -171,14 +174,18 @@
     plt.grid()
 
 
     if args.ylimits is not None:
         print('found y-axis limits')
         ylimits = args.ylimits
         plt.ylim((ylimits))
+    if args.xlimits is not None:
+        print('found x-axis limits')
+        xlimits = args.xlimits
+        plt.xlim((xlimits))
 
     if args.outfile is not None:
         plt.savefig(args.outfile,dpi=300)
 
     plt.show()
```

### Comparing `gnssrefl-1.3.8/gnssrefl/read_snr_files.py` & `gnssrefl-1.4.1/gnssrefl/read_snr_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import numpy as np
 import os
 import subprocess 
 import sys
 
 def read_snr_multiday(obsfile,obsfile2,twoDays,dec=1):
     """
+    originally meant to make snr arrays longer than a day to take care
+    of midnight crossing.  not currently invoked.
+
+    Snr data have units changed to linear units I believed.
+
     Parameters
     ----------
     obsfile : string
         name of first SNR input file
 
     obsfile2 : string
         name of second SNR input file
```

### Comparing `gnssrefl-1.3.8/gnssrefl/refl_zones.py` & `gnssrefl-1.4.1/gnssrefl/refl_zones.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from scipy.interpolate import interp1d
 import math
 import numpy as np
 import os
 import subprocess
 import sys
 import time
 import wget
@@ -468,44 +469,52 @@
     """
     finds the file needed to compute orbits for reflection zones
 
     Parameters
     ----------
     system : str
         gps,glonass,beidou, or galileo
+    it : int
+        simple pointer from former code. 1 is GPS, 2 is Glonass etc
 
     Returns
     -------
     orbfile : str
         orbit filename with Cartesian coordinates for one day 
 
     """
+    it = 1
     xdir = os.environ['REFL_CODE'] 
     if not os.path.exists(xdir):
         print('REFL_CODE environment variable must be set. Exiting.')
         sys.exit()
     xdir = os.environ['REFL_CODE'] + '/Files/'
     if not os.path.exists(xdir):
         subprocess.call(['mkdir', xdir])
 
     if (system is None) or (system == 'gps'):
         system = 'gps'
         orbfile = xdir + 'GPSorbits_21sep17.txt'
+        it = 1
     elif (system == 'galileo'):
         orbfile = xdir + 'GALILEOorbits_21sep17.txt'
+        it = 3
     elif (system == 'glonass'):
         orbfile = xdir + 'GLONASSorbits_21sep17.txt'
+        it = 2
     elif (system == 'beidou'):
         orbfile = xdir + 'BEIDOUorbits_21sep17.txt'
+        it = 4
     else:
        print('Using GPS')
        system = 'gps'
+       it = 1
        orbfile = xdir + 'GPSorbits_21sep17.txt'
 
-    return orbfile
+    return orbfile, it 
 
 def save_reflzone_orbits():
     """
     check that orbit files exist for reflection zone code.
     downloads to $REFL_CODE$/Files directory if needed
 
     Returns
@@ -528,21 +537,114 @@
 
     for otypes in ['GPS','GLONASS','GALILEO','BEIDOU']:
         orbfile = otypes + 'orbits_21sep17.txt'
         #print( githubdir+orbfile)
         if not os.path.exists(xdir + orbfile):
             print('download from github and put in local Files directory: ', otypes)
             wget.download(githubdir+orbfile, xdir + orbfile)
-        else:
-            print('file already exists', otypes)
+        #else:
+        #    print('file already exists', otypes)
 
     found = 0 
     for otypes in ['GPS','GLONASS','GALILEO','BEIDOU']:
         orbfile = otypes + 'orbits_21sep17.txt'
         if os.path.exists(xdir + orbfile):
             found = found + 1
 
     foundfiles = False
     if found == 4:
         foundfiles = True
 
     return foundfiles 
+
+def nyquist_simple(t,elev,azims, emin,emax,azriseset,reqsamplerate):
+    """
+    given numpy array of elevation angles (elev)
+    and limtis (emin,emax) and azriseset, reqsamplerate
+
+    Parameters
+    ----------
+    t : ??
+        cannot remember
+    elev : numpy array of floats
+        elevation angle of rising/setting arcs
+    azims : numpy array of floats
+        azimuths of rising/setting arcs
+    emin : float
+        minimum elevation angle, degrees
+    emax : float
+        maximum elevation angle, degrees
+    azriseset : ??
+        cannot remember
+    reqsamplerate : float
+        requested receiver sampling rate
+
+    """
+    # sample rate used for primary orbit calculation.  will scale by requested sample rate
+    samplerate = 30
+    # t is every five minutes
+    ie= interp1d(t, elev, kind='quadratic',bounds_error=False,fill_value='extrapolate')
+    ia= interp1d(t, azims, kind='quadratic',bounds_error=False,fill_value='extrapolate')
+    tnew = np.arange(t[0], t[-1], samplerate)
+    # interporlate el and az
+    enew = ie(tnew)
+    anew = ia(tnew)
+    # window it
+    i = (np.abs(anew-azriseset) < 20); enew = enew[i]
+    i = (enew >= emin) & (enew <= emax); enew = enew[i]
+    # scale factor for L1
+    cf = 0.1902936/2
+    N = len(enew)
+    if (N > 2):
+        maxe = max(enew); mine = min(enew)
+    # highest observation has to be within 0.5 degrees of requested
+        if ( maxe < (emax-0.5)):
+        #print(azriseset, 'max ele ', round(maxe,2), ' Not a significant arc')
+            nyq = np.nan
+        else:
+            diffT = (np.sin( maxe*np.pi/180) - np.sin(mine*np.pi/180) ) /cf
+    # we do 30 sec and then multiple by ratio of requested sample rate
+            nyq = round(N/(2*diffT),2)*(samplerate/reqsamplerate)
+    else:
+        nyq = np.nan
+
+    return nyq
+
+
+def calcAzEl_newish(prn, newf,recv,u,East,North):
+    """
+    should be consolidated with the other function.but who has the time!
+
+    Parameters
+    ----------
+    prn : int
+        satellite number ?
+
+    newf : 
+
+    u : numpy array
+        up unit vector
+    East: 
+
+    North : 
+
+    Returns
+    -------
+    tv : numpy array
+
+    """
+    tv = np.empty(shape=[0, 4])
+    # number of values
+    NV = len(newf)
+    for t in range(0,NV):
+        satv= [newf[t,2], newf[t,3],newf[t,4]]
+        etime = newf[t,1]
+        r=np.subtract(satv,recv) # satellite minus receiver vector
+        eleA = g.elev_angle(u, r)*180/np.pi
+        if ( (eleA >= 0) & (eleA <= 20)):
+            azimA = g.azimuth_angle(r, East, North)
+#            print(etime, eleA, azimA)
+            newl = [prn, eleA, azimA, etime]
+            tv = np.append(tv, [newl],axis=0)
+    nr,nc=tv.shape
+    return tv
+
```

### Comparing `gnssrefl-1.3.8/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.4.1/gnssrefl/refl_zones_cl.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 def parse_arguments():
     parser = argparse.ArgumentParser()
 
     parser.add_argument('station', help='station', type=str)
     parser.add_argument('-lat', help='Latitude (deg), if station not in database', type=float, default=None)
     parser.add_argument('-lon', help='Longitude (deg), if station not in database', type=float, default=None)
     parser.add_argument('-el_height', help='Ellipsoidal height (m) if station not in database', type=float,default=None)
-    parser.add_argument('-fr', help='1, 2, or 5 ', type=int)
+    parser.add_argument('-fr', help='1, 2, or 5 ', type=int,default=None)
     parser.add_argument('-RH', help='Reflector height (meters). Default is sea level', type=str, default=None)
     parser.add_argument('-azim1', help='start azimuth (default is 0, negative values allowed) ', type=int,default=None)
     parser.add_argument('-azim2', help='end azimuth (default is 360) ', type=int,default=None)
     parser.add_argument('-el_list', nargs="*",type=float,  help='elevation angle list, e.g. 5 10 15  (default)')
     parser.add_argument('-azlist', nargs="*",type=float,  help='flexible azimuth angle list, e.g. 0 90 270 360, but must be positive ')
     parser.add_argument('-system', help='default=gps, options are galileo, glonass, beidou', type=str)
     parser.add_argument('-output', help='output filename. default is the station name with kml extension', type=str,default=None)
 
-
     args = parser.parse_args().__dict__
 
+
     return {key: value for key, value in args.items() if value is not None}
 
 def reflzones(station: str, azim1: int=0, azim2: int=360, lat: float=None, lon: float=None, el_height: float=None, 
         RH: str=None, fr: int = 1, el_list: float= [], azlist : float=[], system: str = 'gps', output: str = None):
     """
     Creates a KML file for reflection zones to be used in Google Earth
 
@@ -40,20 +40,22 @@
     with the optional inputs.
 
     The output file will be stored in REFL_CODE/Files/kml unless you specify an output name. In that case
     it will go into your working directory
 
     Examples
     --------
-
     refl_zones p041 -RH 2
+        standard Fresnel zones for all azimuths, GPS and L1 frequency, RH of 2 meters
 
     refl_zones sc02 -fr 2 -azlist 40 240
+        Fresnel zones for limited azimuths, GPS and L2 frequency. RH is mean sea level
 
-    refl_zones p041 -RH 2 -system galileo
+    refl_zones p041 -RH 5 -system galileo
+        Fresnel zones for reflector height of 5 meters and Galileo L1
 
     Parameters
     ----------
     station : str
         station name
     azim1 : int, optional
         min azimuth angle in deg
@@ -65,15 +67,15 @@
         longitude in deg
     el_height : float, optional
         ellipsoidal height in m
     RH : str, optional
         user-defined reflector height (m)
         default is to use sea level as the RH
     fr : int, optional
-        frequency (1,2, or 5 allowed)
+        frequency (only 1,2, or 5 allowed)
     el_list : list of floats
         elevation angles desired (deg)
         default is 5, 10, 15
     azlist : list of floats, optional
         azimuth angle regions (deg) Must be in pairs, i.e. 0 90 180 270
     system : str, optional
         name of constellation (gps,glonass,galileo, beidou allowed)
@@ -82,48 +84,59 @@
         name for kml file 
 
     Returns
     -------
     Creates a KML file
 
     """
+
     # changed name to be consistent with other codes
     az_sectors = azlist
     # check that you have the files for the orbits on your local system
     foundfiles = rf.save_reflzone_orbits()    
     if not foundfiles:
         print('The orbit files needed for this code were either not found')
         print('or not downloaded successfully. They should be in the REFL_CODE/Files directory') 
         sys.exit()
 
 
     # check that EGM96 file is in your local directory
     foundfile = g.checkEGM()
     if (RH == None) and (not foundfile):
-        print('EGM96 file is not online. It should be in the REFL_CODE/Files directory')
+        print('EGM96 file has not been found. It should be in the REFL_CODE/Files directory')
 
     #print(lat,lon,el_height)
     if (lat is None) & (lon is None):
     # check the station coordinates in our database from the station name
         lat, lon, el_height = g.queryUNR_modern(station)
         if (lat == 0) and (lon == 0):
             print('Exiting.')
             sys.exit()
         else:
-            print('using inputs:', lat, lon, el_height)
+            print('Using inputs:', lat, lon, el_height)
     else:
-        print('using inputs:', lat, lon, el_height)
+        print('Using inputs:', lat, lon, el_height)
 
     geoidC = g.geoidCorrection(lat,lon)
     # calculate height above sea level
     sealevel = el_height - geoidC
     
     if fr not in [1,2,5]:
         print('Illegal frequency chosen: ',fr)
         return
+    else:
+        if (system == 'galileo') & (fr == 2):
+            print('Galileo does not have a L2 frequency.')
+            sys.exit()
+        elif (system == 'glonass') & (fr == 5):
+            print('Glonass does not have a L5 frequency.')
+            sys.exit()
+        else:
+            print('Using frequency: ', fr)
+
     # default is to use sea level as reflector height.  if RH is set, use that instead
     if RH == None:
         h = sealevel
     else:
         h = float(RH)
 
     if h < 0:
@@ -149,16 +162,16 @@
     print(all(x < 50 for x in el_list))
 
     if not (all(x < emax for x in el_list)):
         print('Right now we have an emax of 30 degrees. Resubmit your request.')
         sys.exit()
 
 
-    obsfile = rf.set_system(system)
-    print('The code should use this orbit file: ', obsfile)
+    obsfile, it  = rf.set_system(system)
+    print('The code should use this orbit file: ', obsfile )
     x,y,z=g.llh2xyz(lat,lon,el_height)
     recv=np.array([x,y,z])
     # calculate rising and setting arcs for this site and the requested constellation
     azlisttmp= rf.rising_setting_new(recv,el_list,obsfile)
     if len(az_sectors) == 0:
         print('Using one set of azimuths') 
         azlist = rf.set_final_azlist(azim1,azim2,azlisttmp)
@@ -208,16 +221,16 @@
 
     if fz_maps == True:
         print('File is saved in ' , output)
     else:
         print('Something went wrong, and the kml file was not created')
 
 
-
 def main():
     args = parse_arguments()
+    print(args)
     data = reflzones(**args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.3.8/gnssrefl/refraction.py` & `gnssrefl-1.4.1/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/rh_plot.py` & `gnssrefl-1.4.1/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/rinex2snr.py` & `gnssrefl-1.4.1/gnssrefl/rinex2snr.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
     xdir  = os.environ['REFL_CODE'] + '/'
     fname =  xdir + str(year) + '/snr/' + station + '/' + station + cdoy + '0.' + cyy + '.snr' + csnr
 
     return fname
 
 def run_rinex2snr(station, year_list, doy_list, isnr, orbtype, rate,dec_rate,archive,fortran,nol,overwrite,translator,srate,
-        mk,skipit,stream,strip,bkg):
+        mk,skipit,stream,strip,bkg,screenstats):
     """
     main code to convert RINEX files into SNR files 
 
     Parameters
     ----------
     station : string
         4 or 9 character station name. 6 ch allowed for japanese archive
@@ -118,23 +118,25 @@
     strip : boolean
          reduces observables to only SNR (too many observables, particularly in RINEX 2 files
          will break the RINEX translator)
 
     bkg : str
          location of bkg files, EUREF or IGS
 
+    screenstats: bool
+         whether print statements come to screen
+
     """
     #
     # do not allow illegal skipit values
     if skipit < 1:
         skipit = 1
 
     NS = len(station)
     if (NS == 4):
-        #print('Assume RINEX 2.11');
         version = 2
         if not mk:
             station = station.lower()
     elif (NS == 6 and archive == 'jp') :
         version = 2
         if not mk:
             station = station[-4:].upper()
@@ -199,16 +201,19 @@
                     if version == 2:
                         if mk:
                             the_makan_option(station,cyyyy,cyy,cdoy) # looks everywhere in your local directories
                         if not os.path.exists(r):
                             # could try this way? - look for file in localpath2. gunzip if necessary
                             allgood = get_local_rinexfile(r,localpath2)
                         if os.path.exists(r):
+                            if screenstats:
+                                print('Found the RINEX 2.11 file', r)
                             if strip:
-                                print('Testing out stripping the RINEX 2 file here')
+                                if screenstats:
+                                    print('Testing out stripping the RINEX 2 file here')
                                 k.strip_rinexfile(r)
                             conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
                         else:
                             print('You Chose the No Look Option, but did not provide the needed RINEX file.')
                     if version == 3:
                         if rate == 'high':
                             csrate = '01' # high rate assumes 1-sec
@@ -217,81 +222,99 @@
                         streamid = '_' + stream  + '_'
                         # this can be done in a function now ...
                         r3cmpgz = station9ch + streamid + str(year) + cdoy + '0000_01D_' + csrate + 'S_MO.crx.gz'
                         r3 = station9ch + streamid + str(year) + cdoy + '0000_01D_' + csrate + 'S_MO.rnx'
                         r3gz = station9ch + streamid + str(year) + cdoy + '0000_01D_' + csrate + 'S_MO.rnx.gz'
                         r2 = station + cdoy + '0.' + cyy + 'o'
                         if os.path.exists(r3cmpgz):
-                            print('Try to translate', r3cmpgz)
+                            if screenstats: 
+                                print('Try to translate', r3cmpgz)
                             deletecrx = True
                             translated, rnx_filename = go_from_crxgz_to_rnx(r3cmpgz,deletecrx)
                         if os.path.exists(r3gz):
-                            print('Try to gunzip ', r3gz)
+                            if screenstats: 
+                                print('Try to gunzip ', r3gz)
                             subprocess.call(['gunzip', r3gz])
                         if os.path.exists(r3):
-                            print('The RINEX 3 file exists locally', r3)
+                            if screenstats: 
+                                print('The RINEX 3 file exists locally', r3)
                             # convert to RINEX 2.11
                             fexists = g.new_rinex3_rinex2(r3,r2,dec_rate)
                             if fexists:
                                 conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
                             else:
                                 print('Something about the RINEX 3-2 conversion did not work')
                         else:
                             print('You Chose the No Look Option, but did not provide the needed RINEX3 file.')
                             print('I assumed its name was ', r3)
 
                 else:
-                    print('Will seek the RINEX file from an external archive')
+                    if screenstats:
+                        print('Will seek the RINEX file from an external archive')
                     if version == 3:
                         fexists = False
                         rnx_filename = '' # just in  case?
                         print(station9ch, ' year:', year, ' doy:', doy, 'from: ', archive)
                         r2 = station + cdoy + '0.' + cyy + 'o'
                         rinex2exists = False; rinex3name = '';
                         if (rate == 'high'):
-                            print('This code only accesses 1-Hz Rinex 3 data at CDDIS, BKG, and GA')
+                            print('This code only accesses 1-Hz Rinex 3 data at BKG, CDDIS, and GA')
                             if archive == 'ga':
                                 deleteOld = True
                                 # cold should return the new name of the rinex 2 file
                                 r2, foundit = g.ga_highrate(station9ch,year,doy,dec_rate,deleteOld)
-                                if foundit:
+                                if foundit and screenstats:
                                     print('rinex2 file should now exist:', r2)
                             if archive == 'cddis':
-                                rnx_filename,foundit = ch.cddis_highrate(station9ch, year, doy, 0,stream,dec_rate)
+                                bad_day = g.cddis_restriction(year, doy,'cddis')
+                                if not bad_day:
+                                    rnx_filename,foundit = ch.cddis_highrate(station9ch, year, doy, 0,stream,dec_rate)
+                                else: 
+                                    print('No high-rate RINEX data will be downloaded')
+                                    foundit = False; fexists = False; rnx_file = ''
                                 if foundit:
-                                    print('The RINEX 3 file has been downloaded. Try to make ', r2)
+                                    if screenstats:
+                                        print('The RINEX 3 file has been downloaded. Try to make ', r2)
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
                             if archive == 'bkg':
-                                rnx_filename,foundit = ch.bkg_highrate(station9ch, year, doy, 0,stream,dec_rate,bkg)
+                                bad_day = g.cddis_restriction(year, doy,'bkg')
+                                if not bad_day:
+                                    rnx_filename,foundit = ch.bkg_highrate(station9ch, year, doy, 0,stream,dec_rate,bkg)
+                                else:
+                                    print('No high-rate RINEX data will be downloaded')
+                                    foundit = False; fexists = False; rnx_file = ''
                                 if foundit:
-                                    print('The RINEX 3 file has been downloaded and merged. Try to make ', r2)
+                                    if screenstats:
+                                        print('The RINEX 3 file has been downloaded and merged. Try to make ', r2)
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
 
                         else:
                             if (archive == 'all'):
-                                file_name,foundit = k.universal_all(station9ch, year, doy,srate,stream)
+                                file_name,foundit = k.universal_all(station9ch, year, doy,srate,stream,screenstats)
                                 if (not foundit): # try again
-                                    file_name,foundit = k.universal_all(station9ch, year, doy, srate,k.swapRS(stream))
+                                    file_name,foundit = k.universal_all(station9ch, year, doy, srate,k.swapRS(stream),screenstats)
                             else:
                                 #print('stream',stream)
                                 file_name,foundit = k.universal(station9ch, year, doy, archive,srate,stream)
                                 if (not foundit): # try again
                                     #print('stream',stream)
                                     file_name,foundit = k.universal(station9ch, year, doy, archive,srate,k.swapRS(stream))
                             if foundit: # version 3 found - now need to gzip, then hatanaka decompress
                                 deletecrx = True # no point keeping this around
                                 translated, rnx_filename = go_from_crxgz_to_rnx(file_name,deletecrx)
                             # now make rinex2
                                 if translated:
-                                    print('The RINEX 3 file has been downloaded. Try to make ', r2)
+                                    if screenstats:
+                                        print('The RINEX 3 file has been downloaded. Try to make ', r2)
                                     fexists = g.new_rinex3_rinex2(rnx_filename,r2,dec_rate)
                                     #subprocess.call(['rm', '-f',rnx_filename]) # rnx
                         # this means the rinex 2 version exists
                         if fexists:
-                             print('RINEX 2 created from v3', year, doy, ' Now remove RINEX 3 files and convert')
+                             if screenstats:
+                                 print('RINEX 2 created from v3', year, doy, ' Now remove RINEX 3 files and convert')
                              subprocess.call(['rm', '-f',rnx_filename]) # rnx
                              conv2snr(year, doy, station, isnr, orbtype,rate,dec_rate,archive,fortran,translator)
                         else:
                             print('Unsuccessful RINEX 3 retrieval/translation', year, doy)
                     else:
                         print(station, ' year:', year, ' doy:', doy, 'from: ', archive)
                         # this is rinex version 2 - finds rinex and converts it
@@ -328,14 +351,15 @@
     fortran : bool
          whether fortran translator to be used.  this is here for backwards compatability
 
     translator : str
          hybrid, python, or fortran
 
     """
+    screenstats = False # for now
     # define directory for the conversion executables
     if not os.path.isdir('logs'):
         subprocess.call(['mkdir', 'logs'])
     logname = 'logs/' + station + '.txt'
     log = open(logname, 'w+')
     log.write("Receiver rate: {0:5s} \n".format(receiverrate))
     log.write("Decimation rate: {0:3.0f} \n".format(dec_rate))
@@ -364,17 +388,17 @@
                 file_name, foundit = k.rinex2_highrate(station, year, doy,archive,strip_snr)
             else:
                 # added karnak librariies
                 if (archive == 'all'):
                     foundrinex = False
                     for archivechoice in ['unavco','sopac','sonel']:
                         if (not foundrinex):
-                            file_name,foundrinex = k.universal_rinex2(station, year, doy, archivechoice)
+                            file_name,foundrinex = k.universal_rinex2(station, year, doy, archivechoice,screenstats)
                 else:
-                    file_name,foundrinex = k.universal_rinex2(station, year, doy, archive)
+                    file_name,foundrinex = k.universal_rinex2(station, year, doy, archive,screenstats)
 
                 if foundrinex: #uncompress etc  to make o files ...
                     rinexfile, foundit2 = k.make_rinex2_ofiles(file_name) # translate
 
 #           define booleans for various files
             oexist = os.path.isfile(orbdir + '/' + f) == True
             rexist = os.path.isfile(rinexfile) == True
@@ -1219,15 +1243,15 @@
         g.hatanaka_warning()
     else:
         if os.path.exists(c3): # file exists
             subprocess.call([crnxpath,c3])
     if os.path.exists(rnx): # file exists
         translated = True
         if deletecrx:
-            print('remove Hatanaka compressed file')
+            #print('remove Hatanaka compressed file')
             subprocess.call(['rm','-f',c3])
 
     return translated, rnx
 
 def get_local_rinexfile(rfile,localpath2):
     """
     look for a plain or gzipped version of the rinex 2.11 file in the year subdirectories
@@ -1246,21 +1270,27 @@
 
     Returns
     -------
     allgood : bool
         whether file found
     """
     allgood = False
-    r = localpath2 + rfile
-    if os.path.exists(r):
+    # look for gzip veresion in local directory first
+    if os.path.exists(rfile + '.gz'):
+        subprocess.call(['gunzip', rfile + '.gz'])
         allgood = True
-        # cp to the local directory
-        subprocess.call(['cp',r,'.'])
-    else:
-       # did not find noromal rinex, so look for gzip version
-        if os.path.exists(r + '.gz'):
-            subprocess.call(['gunzip', r + '.gz'])
+
+    if not allgood:
+        r = localpath2 + rfile
         if os.path.exists(r):
-            subprocess.call(['cp',r,'.'])
             allgood = True
+        # cp to the local directory
+            subprocess.call(['cp',r,'.'])
+        else:
+       # did not find normal rinex, so look for gzip version
+            if os.path.exists(r + '.gz'):
+                subprocess.call(['gunzip', r + '.gz'])
+            if os.path.exists(r):
+                subprocess.call(['cp',r,'.'])
+                allgood = True
 
     return allgood
```

### Comparing `gnssrefl-1.3.8/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.4.1/gnssrefl/rinex2snr_cl.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def parse_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument("station", help="station name", type=str)
     parser.add_argument("year", help="year", type=int)
     parser.add_argument("doy", help="start day of year", type=int)
     parser.add_argument("-snr", default=None, help="snr file ending, 99: 5-30 deg.; 66: < 30 deg.; 88: all data; 50: < 10 deg.", type=int)
     parser.add_argument("-orb", default=None, type=str,
-                        help="orbit type, e.g. gps, gps+glo, gnss, rapid, ultra")
+                        help="orbit type, e.g. gps, gps+glo, gnss, rapid, ultra, gnss3")
     parser.add_argument("-rate", default=None, metavar='low', type=str, help="RINEX sample rate: low or high. Only used for archive searches.")
     parser.add_argument("-dec", default=None, type=int, help="decimate (seconds)")
     parser.add_argument("-nolook", default=None, metavar='False', type=str,
                         help="True means only use RINEX files on local machine")
     parser.add_argument("-fortran", default=None, metavar='False', type=str,
                         help="True means use Fortran RINEX translators ")
     parser.add_argument("-archive", default=None, metavar='all',
@@ -40,67 +40,74 @@
     parser.add_argument("-overwrite", default=None, help="boolean", type=str)
     parser.add_argument("-translator", default=None, help="translator(fortran,hybrid,python)", type=str)
     parser.add_argument("-samplerate", default=None, help="sample rate in sec (RINEX 3 only)", type=int)
     parser.add_argument("-stream", default=None, help="Set to R or S (RINEX 3 only)", type=str)
     parser.add_argument("-mk", default=None, help="use True for uppercase station names ", type=str)
     parser.add_argument("-weekly", default=None, help="use True for weekly data translation", type=str)
     parser.add_argument("-strip", default=None, help="use True to reduce number of obs", type=str)
-    parser.add_argument("-bkg", default=None, help="Which folder to use for the BKG archive, IGS or EUREF (default)", type=str)
+    parser.add_argument("-screenstats", default=None, help="set to T see more info printed to screen", type=str)
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['nolook', 'fortran', 'overwrite', 'mk', 'weekly','strip']
+    boolean_args = ['nolook', 'fortran', 'overwrite', 'mk', 'weekly','strip','screenstats']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
-def rinex2snr(station: str, year: int, doy: int, snr: int = 66, orb: str = 'nav', rate: str = 'low', dec: int = 0,
+def rinex2snr(station: str, year: int, doy: int, snr: int = 66, orb: str = None, rate: str = 'low', dec: int = 0,
               fortran: bool = False, nolook: bool = False, archive: str = 'all', doy_end: int = None,
               year_end: int = None, overwrite: bool = False, translator: str = 'hybrid', samplerate: int = 30,
-              stream: str = 'R', mk: bool = False, weekly: bool = False, strip: bool = False, bkg: str = 'EUREF'):
+              stream: str = 'R', mk: bool = False, weekly: bool = False, strip: bool = False, screenstats : bool = False):
     """
     rinex2snr translates RINEX files to a new file in SNR format. This function will also fetch orbit files for you.
     RINEX obs files are provided by the user or fetched from a long list of archives. The default is RINEX 2.11 files
 
+    Default is GPS only until day of year 137, 2021 when rapid GFZ orbits became available.  If you still want to use
+    the nav message, i.e. GPS only, you can request it.
+
+    bkg no longer a boolean input - must be specified with archive name, i.e. bkg-igs or bkg-euref
+
     Examples
     --------
+    rinex2snr mchn 2018 15  -archive sopac
+        station mchn, year/doy 2022/15,sopac archive using GPS orbits
 
     rinex2snr mchn 2022 15  -archive sopac
+        station mchn, year/doy 2022/15,sopac archive using multi-GNSS GFZ orbits
+
+    rinex2snr mchn 2022 15  -archive sopac -orb gps
         station mchn, year/doy 2022/15,sopac archive using GPS orbits
 
     rinex2snr mchn 2022 15  -orb rapid -archive sopac
-        now using multi-GNSS orbits
+        now explicitly using multi-GNSS orbits
+
     rinex2snr p041 2022 15  -orb rapid -rate high -archive unavco
         now using high-rate data from unavco and multi-GNSS orbits
 
     rinex2snr p041 2022 15 -nolook T
         using your own data stored as p0410150.22o in the working directory 
-
-    RINEX 2.11 archives listed below
-
-    Examples
-    --------
+        your RINEX o file may also be gzipped.  
 
     rinex2snr mchl00aus 2022 15  -orb rapid -archive ga 
         30 sec data for mchl00aus and Geoscience Australia
 
-    rinex2snr warn00deu 2023 87 -dec 5 -rate high -samplerate 1 -orb rapid -archive bkg -stream S -bkg IGS
-        1 sec data for warn00deu, 1 sec decimated to 5 sec, multi-GNSS, bkg archive, streamed, in IGS folder
+    rinex2snr warn00deu 2023 87 -dec 5 -rate high -samplerate 1 -orb rapid -archive bkg-igs -stream S 
+        1 sec data for warn00deu, 1 sec decimated to 5 sec, multi-GNSS, bkg IGS archive, streamed
 
     RINEX3 30 second archives supported  
-        bev, bkg, cddis, epn, ga, gfz, nrcan, sonel
+        bev, bkg-euref, bkg-igs, cddis, epn, ga, gfz, nrcan, sonel
 
     RINEX3 15 sec archives
         bfg, unavco
 
     RINEX3 1 sec 
-        cddis, bkg, maybe nrcan
+        bkg-igs, bkg-euref, cddis, maybe nrcan 
 
     Parameters
     ----------
     station : str
         4 or 9 character ID of the station, preferably lowercase
     year : int
         Year
@@ -123,14 +130,16 @@
 
             gps (default) : will use GPS broadcast orbit
 
             gps+glos : will use JAXA orbits which have GPS and Glonass (usually available in 48 hours)
 
             gnss : will use GFZ orbits, which is multi-GNSS (available in 3-4 days?)
 
+            gnss3 : test case for GFZ orbits downloaded from GFZ instead of CDDIS
+
             nav : GPS broadcast, perfectly adequate for reflectometry. Same as gps.
 
             igs : IGS precise, GPS only
 
             igr : IGS rapid, GPS only
 
             jax : JAXA, GPS + Glonass, within a few days, missing block III GPS satellites
@@ -146,14 +155,15 @@
             rapid : GFZ rapid, multi-GNSS
 
             ultra: GFZ ultra-rapid, multi-GNSS
 
     rate : str, optional
         The data rate. Rather than numerical value, this tells the code which folder to use
         value options:
+
             low (default) : standard rate data. Usually 30 sec, but sometimes 15 sec.
 
             high : high-rate data
 
     dec : int, optional
         Decimation rate. 0 is default.
 
@@ -167,15 +177,17 @@
         Select which archive to get the files from. Default is all
         value options:
 
             bev : (Austria Federal Office of Metrology and Surveying)
 
             bfg : (German Agency for water research, only Rinex 3, requires password)
 
-            bkg : (German Agency for Cartography and Geodesy)
+            bkg-igs : EUREF for (German Agency for Cartography and Geodesy)
+
+            bkg-euref : IGS for (German Agency for Cartography and Geodesy)
 
             cddis : (NASA's Archive of Space Geodesy Data)
 
             ga : (Geoscience Australia)
 
             gfz : (GFZ, Germany)
 
@@ -226,58 +238,68 @@
         Takes 1 out of every 7 days in the doy-doy_end range (one file per week) - used to save cpu time.
         Default is False.
 
     strip : bool, optional
         Reduces observables since the translator does not allow more than 25
         Default is False.
 
-    bkg : str, optional
-        tells you which directory the files live in, EUREF or IGS 
-        Default is EUREF.
+    screenstats: bool, optional
+        if true, prints more information to the screen
 
     """
 
     # make sure environment variables exist.  set to current directory if not
     g.check_environ_variables()
     #
-    # rename the user inputs as variables
-    #
+
+    # when multi-GNSS orbits are reliably available
+    gfz_avail = 2021 + 137/365.25
+
+    if orb is None:
+        # you asked for default
+        if ((year + doy/365.25) > gfz_avail):
+            orb = 'rapid'
+        else:
+            orb = 'nav'
+
     ns = len(station)
     if (ns == 4) or (ns == 6) or (ns == 9):
         pass
     else:
         print('Illegal input - Station name must have 4 (RINEX 2), 6 (GSI), or 9 (RINEX 3) characters. Exiting.')
         sys.exit()
 
     if len(str(year)) != 4:
         print('Year must be four characters long. Exiting.', year)
         sys.exit()
 
     # currently allowed orbit types - shanghai removed 2020sep08
     #
     orbit_list = ['gps', 'gps+glo', 'gnss', 'nav', 'igs', 'igr', 'jax', 'gbm',
-                  'grg', 'wum', 'gfr', 'esa', 'ultra', 'rapid', 'gnss2','nav-sopac','nav-esa','nav-cddis']
+                  'grg', 'wum', 'gfr', 'esa', 'ultra', 'rapid', 'gnss2','nav-sopac','nav-esa','nav-cddis','gnss3']
     if orb not in orbit_list:
         print('You picked an orbit type I do not recognize. Here are the ones I allow')
         print(orbit_list)
         print('Exiting')
         sys.exit()
 
     # if you choose GPS, you get the nav message
     if orb == 'gps':
         orb = 'nav'
 
-    # if you choose ultra , you get the GFZ rapid 
     if orb == 'rapid':
         orb = 'gfr'
 
     # if you choose GNSS, you get the GFZ sp3 file  (precise)
+    # I think gbm should be changed to 'gnss3' though perhaps not here
     if orb == 'gnss':
         orb = 'gbm'
 
+
+    # get orbit from IGS
     if orb == 'gnss2':
         # this code wants year month day....
         year, month, day = g.ydoy2ymd(year, doy)
         filename, fdir, foundit = g.avoid_cddis(year, month, day)
         orb = 'gbm'
         if not foundit:
             print('You picked the backup multi-GNSS option.')
@@ -338,31 +360,53 @@
         sys.exit()
 
     if doy_end is None:
         doy2 = doy
     else:
         doy2 = doy_end
 
+
+    bkg = 'EUREF' # just so the code doesn't crash later on when variable
+    # is sent to rinex2snr
+    if 'bkg' in archive:
+        if (archive == 'bkg'):
+            print('You have not specified which BKG archive you want.')
+            print('You must select bkg-igs or bkg-euref.')
+            sys.exit()
+        if 'euref' in archive:
+            bkg = 'EUREF'
+        else:
+            bkg = 'IGS'
+        # change archive name back to original name
+        archive = 'bkg'
+
     archive_list_rinex3 = ['unavco', 'cddis', 'bev', 'bkg', 'ga', 'epn', 'bfg','sonel','all','unavco2','nrcan','gfz']
-    archive_list = ['sopac', 'unavco', 'sonel', 'cddis', 'nz', 'ga', 'bkg', 'jeff',
-                    'ngs', 'nrcan', 'special', 'bev', 'jp', 'all','unavco2']
+    archive_list = ['sopac', 'unavco', 'sonel',  'nz', 'ga', 'bkg', 'jeff',
+                    'ngs', 'nrcan', 'special', 'bev', 'jp', 'all','unavco2','cddis']
 
     # no longer allow the all option
     # unavco is only rinex2
     # ga is only rinex3
     # bkg is only rinex 3
     # i cannot remember for nrcan. it is probably rinex2
-    highrate_list = ['unavco', 'nrcan', 'cddis','ga','bkg']  
+    #highrate_list = ['unavco', 'nrcan', 'cddis','ga','bkg']  
+    highrate_list = ['unavco', 'nrcan', 'ga','bkg','cddis']  
 
     if ns == 9:
         # rinex3
-        if archive not in archive_list_rinex3:
-            print('You have chosen an archive not supported by the code.')
-            print(archive_list_rinex3)
-            sys.exit()
+        if rate == 'high':
+            if archive not in highrate_list:
+                print('You have chosen an archive not supported by the code.')
+                print(highrate_list)
+                sys.exit()
+        else:
+            if archive not in archive_list_rinex3:
+                print('You have chosen an archive not supported by the code.')
+                print(archive_list_rinex3)
+                sys.exit()
     else:
         # rinex2
         if rate == 'high':
             if archive not in highrate_list:
                 if nolook:
                     print('You have chosen nolook, so I will proceed assuming you have the RINEX file.')
                     # change to lowrate since the code only uses low vs high for retrieving files from
@@ -395,20 +439,19 @@
 
     # the Makan option
     if mk:
         print('You have invoked the Makan option')
 
     if stream not in ['R', 'S']:
         stream = 'R'
-    bkg = bkg.upper() # make sure it is using uppercase
 
     args = {'station': station, 'year_list': year_list, 'doy_list': doy_list, 'isnr': snr, 'orbtype': orb,
             'rate': rate, 'dec_rate': dec, 'archive': archive, 'fortran': fortran, 'nol': nolook,
             'overwrite': overwrite, 'translator': translator, 'srate': samplerate, 'mk': mk,
-            'skipit': skipit, 'stream': stream, 'strip': strip, 'bkg': bkg}
+            'skipit': skipit, 'stream': stream, 'strip': strip, 'bkg': bkg, 'screenstats': screenstats}
 
     s1 = time.time()
     rnx.run_rinex2snr(**args)
     s2 = time.time()
     print('That took ', round(s2-s1,2), ' seconds')
     print('Feedback written to subdirectory logs')
```

### Comparing `gnssrefl-1.3.8/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.4.1/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/rinex3_snr.py` & `gnssrefl-1.4.1/gnssrefl/rinex3_snr.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 
     Creates SNR file from RINEX 3 file that is stored locally
     Requires the gfzrnx executable to be available.
 
     Parameters
     ----------
     rinex3 : str
-        name of filename
-
+        name of RINEX3 file
     orb : str
         optional orbit choice.  default is gbm
+    snr : int
+        snr file choice. default is 66
+
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("rinex3", help="rinex3 filename", type=str)
     parser.add_argument("-orb", help="orbit choice", default='gbm',type=str)
     parser.add_argument("-snr", help="SNR file ending (default is 66)", default=None,type=str)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/rinpy.py` & `gnssrefl-1.4.1/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.4.1/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/smoosh.py` & `gnssrefl-1.4.1/gnssrefl/smoosh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/snow_functions.py` & `gnssrefl-1.4.1/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.4.1/gnssrefl/snowdepth_cl.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,30 +22,31 @@
     parser.add_argument("-bare_date1", help="bare soil start yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-bare_date2", help="bare soil end yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-plt_enddate", help="end date for the plot/snow solns, yyyy-mm-dd", type=str, default=None)
     parser.add_argument("-plt", help="whether you want the plot to come to the screen", type=str, default=None)
     parser.add_argument("-simple", help="use simple algorithm (default is false)", type=str, default=None)
     parser.add_argument("-medfilter", help="median filter for daily average(m)", type=float, default=None)
     parser.add_argument("-ReqTracks", help="how many arcs needed for daily average)", type=int, default=None)
+    parser.add_argument("-fr", help="if you want to restrict to a single frequency", type=int, default=None)
     parser.add_argument("-barereq_days", help="how many bare soil values req (default is 15)", type=int, default=None)
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    #boolean_args = ['plt', 'csv','test']
     boolean_args = ['longer','plt','simple']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def snowdepth(station: str, year: int, minS: float=None, maxS: float=None,
         longer:bool=False, plt:bool=True, bare_date1:str=None, bare_date2:str=None, 
-        plt_enddate:str=None,simple:bool=False, medfilter:float = None, ReqTracks: int = None, barereq_days: int = 15):
+        plt_enddate:str=None,simple:bool=False, medfilter:float = None, ReqTracks: int = None, 
+        barereq_days: int = 15, fr: int = None):
     """
     Calculates snow depth for a given station and water year.
     Before you run this code you must have run gnssir for each day of interest.  
 
     You can then run daily_avg to concatenate the results or you can input appropriate 
     values to optional inputs medfilter and ReqTracks.  
 
@@ -95,20 +96,25 @@
         to avoid running daily_avg, you can set median filter in meters;
         this is used to remove large outliers
     ReqTracks: int, optional
         to avoid running daily_avg, you can set required number of tracks 
         to create a daily average RH
     barereq_days: int, optional
         how many bare soil days are required to trust the result, default is 15
+    fr : int, optional
+        if you want to restrict to a single frequency at the daily-avg stage (1, 20, etc)
 
     """
     if (medfilter is not None) and (ReqTracks is not None):
         print('Running daily average')
         txtfile=None; pltit = False
-        da.daily_avg(station, medfilter, ReqTracks,  txtfile,pltit,'',2005,2030,0,False,0,360,False,None)
+        if fr is not None:
+            da.daily_avg(station, medfilter, ReqTracks,  txtfile,pltit,'',2005,2030,fr,False,0,360,False,None)
+        else:
+            da.daily_avg(station, medfilter, ReqTracks,  txtfile,pltit,'',2005,2030,0,False,0,360,False,None)
         # do not display these plots
         matplt.close ('all')
 
     # default days of year used for bare soil
     # september from the fall
     doy1 = 244 
     doy2 = 274
```

### Comparing `gnssrefl-1.3.8/gnssrefl/spline_functions.py` & `gnssrefl-1.4.1/gnssrefl/spline_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
                 # here dave is removing the direct signal
                     z = np.polyfit(sinelvt, snrt, polydeg)
                     p = np.poly1d(z)
                 # estimating the periodogram used to compute the dominant reflector 
                 # frequency, and thus RH
                     snrdt = snrt - p(sinelvt)
                     pgram = LombScargle(sinelvt, snrdt, normalization='psd').power(f)
-
+                    pgram = 2 * np.sqrt(pgram/len(sinelvt))
                 # converting it into the proper units of RH (meters)
                     reflh = 0.5 * f * lcar
                 # this is a very simplistic outlier detector
                     tfilter = np.logical_and(reflh > rhlims[0], reflh < rhlims[1])
                     pgram_sub = pgram[tfilter]
                     reflh_sub = reflh[tfilter]
                     maxind = np.argmax(pgram_sub)
@@ -1065,29 +1065,29 @@
 
 def invsnr_header(xdir, outfile_type,station,outfile_name):
     """
     Makes header for output of invsnr analysis
 
     Parameters
     ----------
-    xdir : string 
+    xdir : str
         directory for the output file
-    outfile_type : string
+    outfile_type : str
         csv or txt
-    station : string
+    station : str
         4 character name
-    outfile_name : string
-        name of output - if '', it uses default
+    outfile_name : str
+        name of output - if empty string, it uses default
 
     Returns 
     -------
-    fileID : ? 
+    fileID : file
         used for writing to file
-    usetxt : boolean
-        - boolean for the code calling this function to use
+    usetxt : bool
+        boolean for the code calling this function to use
         if you write out special files, they go in the working directory
 
     """
     if outfile_type == 'txt':
         usetxt = True; 
         if (len(outfile_name) == 0):
             ioutputfile= xdir + station + '_invsnr.txt'
```

### Comparing `gnssrefl-1.3.8/gnssrefl/subdaily.py` & `gnssrefl-1.4.1/gnssrefl/subdaily.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,23 @@
     """
     nr,nc=tvd_bad.shape
     if nr > 0:
         f = txtdir + '/' + filename
         print(nr, ' Outliers written to: ', f)
         fout = open(f, 'w+')
         # put in a header
-        fout.write('{0:3s} sat azim deltT-min outlier-m fracDOY MJD\n'.format('%'))
-        fout.write('{0:3s} (1) (2)   (3)        (4)      (5)    (6) D\n'.format('%'))
+        fout.write('{0:3s} sat azim deltT-min outlier-m fracDOY MJD  OrigRH meanE PkNoise \n'.format('%'))
+        fout.write('{0:3s} (1) (2)   (3)        (4)      (5)    (6)   (7)    (8)   (9)\n'.format('%'))
         for w in range(0,nr):
             fy = tvd_bad[w,1] + tvd_bad[w,4]/24 # fractional day of year
             deltaT = tvd_bad[w,14]
             mjd = tvd_bad[w,15]
-            fout.write('{0:3.0f} {1:7.2f} {2:7.2f} {3:7.2f} {4:9.3f} {5:15.7f} {6:7.2f} \n'.format( 
-                tvd_bad[w,3], tvd_bad[w,5], deltaT,residual[w],fy,mjd,tvd_bad[w,2] ))
+            elAv = 0.5*(tvd_bad[w,8] + tvd_bad[w,7])
+            fout.write('{0:3.0f} {1:7.2f} {2:7.2f} {3:7.2f} {4:9.3f} {5:15.7f} {6:7.2f} {7:7.2f} {8:5.2f}\n'.format( 
+                tvd_bad[w,3], tvd_bad[w,5], deltaT,residual[w],fy,mjd,tvd_bad[w,2],elAv,tvd_bad[w,13]))
         fout.close()
 
     return
 
 def mirror_plot(tnew,ynew,spl_x,spl_y,txtdir,station,beginT,endT):
     """
     Makes a plot of the spline fit to the mirrored RH data
@@ -134,17 +135,17 @@
 
     Parameters
     ----------
     txtdir : str
         the directory where the results should be written out
     txtfile : str
         name of the output file 
-    csvfile : boolean
+    csvfile : bool
         cl input whether the output file should be csv format
-    jsonfile : boolean
+    jsonfile : bool
         cl input for whether the output file should be in the json format
 
     Returns
     -------
     writetxt : bool
         whether output should be plain txt
     writecsv : bool
@@ -188,17 +189,17 @@
     ----------
     input : str
         output filename
     station : str
         4 character station name, lowercase
     nvt : numpy multi-dimensional
         the variable with the LSP results read via np.loadtxt
-    writecsv : boolean
+    writecsv : bool
         whether the file output is csv
-    extraline: boolean
+    extraline: bool
         whether the header has an extra line
 
     """
     # this is lazy - should use shape
     RHdot_corr= kwargs.get('RHdot_corr',[])
 
     newRH = kwargs.get('newRH',[])
@@ -208,19 +209,19 @@
     original = False
     if len(RHdot_corr) + len(newRH) + len(newRH_IF) == 0:
         original = True
         print('LSP series being written')
     # 
     write_IF_corrected = False
     if len(newRH_IF) > 0:
-        print('IF corrected values being written')
+        print('IF corrected values being written - make sure you use the correct column!')
         write_IF_corrected = True
     extra = False
     if len(RHdot_corr) > 0:
-        print('RH corrected values being written')
+        print('RHdot corrected values being written - make sure you use the correct column')
         extra = True
 
     N= len(ntv)
     nr,nc = ntv.shape
     if nr == 0:
         print('No results in this file, so nothing to write out.')
         return
@@ -270,15 +271,15 @@
                 fout.write(" {0:4.0f} {1:3.0f} {2:7.3f} {3:3.0f} {4:6.3f} {5:6.2f} {6:6.2f} {7:6.2f} {8:6.2f} {9:4.0f} {10:3.0f} {11:2.0f} {12:8.5f} {13:6.2f} {14:7.2f} {15:12.6f} {16:1.0f} {17:2.0f} {18:2.0f} {19:2.0f} {20:2.0f} {21:2.0f} \n".format(year, doy, rh,ntv[i,3],UTCtime,ntv[i,5],
                     ntv[i,6],ntv[i,7],ntv[i,8], ntv[i,9], ntv[i,10],ntv[i,11], ntv[i,12],ntv[i,13], ntv[i,14], 
                     ntv[i,15], ntv[i,16],month,day,hour,minute, int(second)))
     fout.close()
 
 
 def readin_and_plot(station, year,d1,d2,plt2screen,extension,sigma,writecsv,azim1,azim2,ampl,
-        peak2noise,txtfile,h1,h2,kplt,txtdir,default_usage):
+        peak2noise,txtfile,h1,h2,kplt,txtdir,default_usage,hires_figs):
     """
     Reads in RH results and makes various plots to help users assess the quality of the solution
 
     This is basically "section 1" of the code
 
     Parameters
     ----------
@@ -315,14 +316,16 @@
     kplt : bool
         special plot made 
     txtdir : str
         directory where the results will be written
     default_usage : bool
         flat as to whether you are using this code for subdaily or for rh_plot.
         this changes the plots a bit.
+    hires_figs: bool
+        whether to switch from png to eps
 
     Returns
     -------
     tv : numpy array
         LSP results (augmented)
     otimes : datetime object 
         times of observations 
@@ -412,16 +415,22 @@
         #print( len(tmp[ri,1])) print( len(tmp[ei,1]))
 
         if (n > 0):
             rhavg = np.mean(tv[ii,2]); 
             rhstd = np.std(tv[ii,2]); 
             newl = [dtime, rhavg, rhstd]
             stats = np.append(stats, [newl], axis=0)
+            #print(newl)
+            #??
+            if rhstd == 0:
+                rhstd = 1
+                
             b = ( tv[ii,2] - rhavg*np.ones( len(tv[ii,2]) ))/ rhstd
             bb =  tv[ii,2] - rhavg*np.ones( len(tv[ii,2]) )
+            
             residuals = np.append(residuals, b)
             real_residuals = np.append(real_residuals, bb)
             Gval = np.append(Gval, len(tmp[gi,1]))
             Eval = np.append(Eval, len(tmp[ei,1]))
             Rval = np.append(Rval, len(tmp[ri,1]))
             Cval = np.append(Cval, len(tmp[ci,1]))
         else:
@@ -434,17 +443,17 @@
     jj = (np.absolute(residuals) < sigma) # data you do not like ;-)
 
     if plt2screen:
 
         minAz = float(np.min(tv[:,5])) ; maxAz = float(np.max(tv[:,5]))
 
         if default_usage:
-            numsats_plot(station,tval,nval,Gval,Rval,Eval,Cval,txtdir,fs)
-            two_stacked_plots(otimes,tv,station,txtdir,year,d1,d2)
-            stack_two_more(otimes,tv,ii,jj,stats, station, txtdir,sigma,kplt)
+            numsats_plot(station,tval,nval,Gval,Rval,Eval,Cval,txtdir,fs,hires_figs)
+            two_stacked_plots(otimes,tv,station,txtdir,year,d1,d2,hires_figs)
+            stack_two_more(otimes,tv,ii,jj,stats, station, txtdir,sigma,kplt,hires_figs)
             print_badpoints(tv[ii,:],residuals[ii],txtdir,real_residuals[ii])
         else:
             # make both plots cause life is short
             rh_plots(otimes,tv,station,txtdir,year,d1,d2,True)
             rh_plots(otimes,tv,station,txtdir,year,d1,d2,False)
 
         #plt.show()
@@ -703,15 +712,15 @@
     outf = outfile
     with open(outf,'w+') as outf:
         json.dump(o,outf,indent=4)
 
     return True
 
 
-def two_stacked_plots(otimes,tv,station,txtdir,year,d1,d2):
+def two_stacked_plots(otimes,tv,station,txtdir,year,d1,d2,hires_figs):
     """
     This actually makes three stacked plots - not two, LOL
     It gives an overview for quality control
 
     Parameters
     ----------
     otimes : numpy array of datetime objects
@@ -724,14 +733,16 @@
         where the plots will be written to
     year: int
         what year is being analyzed
     d1 : int
         minimum day of year
     d2 : int
         maximum day of year
+    hires_figs : bool
+        true for eps instead of png
 
     """
     if d1 == 1 and d2 == 366:
         # these are the defaults
         setlimits = False
     else:
         setlimits = True
@@ -791,42 +802,42 @@
     ax3.invert_yaxis()
     ax3.grid(True)
     if setlimits:
         ax3.set_xlim((th1, th2))
     fig.autofmt_xdate()
 
     plotname = txtdir + '/' + station + '_combined.png'
-    plt.savefig(plotname,dpi=300)
-    print('png file saved as: ', plotname)
+    if hires_figs:
+        plotname = txtdir + '/' + station + '_combined.eps'
+        plt.savefig(plotname,dpi=300)
+    else:
+        plt.savefig(plotname,dpi=300)
+    print('Plot file saved as: ', plotname)
 
-def stack_two_more(otimes,tv,ii,jj,stats, station, txtdir, sigma,kplt):
+def stack_two_more(otimes,tv,ii,jj,stats, station, txtdir, sigma,kplt,hires_figs):
     """
     makes a plot of the reflector heights before and after minimal editing
 
     Parameters
     ----------
     otimes : numpy array of datetime objects 
         observation times
-
-    tv : variable with the gnssrefl results
-
-    ii : good data?
-
-    jj : bad data?
-
-    station : string
+    tv : numpy array
+        variable with the gnssrefl LSP results
+    ii : numpy array
+        indices of good data
+    jj : numpy array
+        indices of bad data
+    station : str
         station name
-
-    txtdir : string
+    txtdir : str
         directory where plots will be written
-
     sigma : float
         what kind of standard deviation is used for outliers (3sigma, 2.5 sigma etc)
-
-    kplt : boolean
+    kplt : bool
         make extra plot for kristine
     """
     fs = 10
     otimesarray = np.asarray(otimes)
     # new plot 
     plt.figure()
     plt.plot(tv[:,5],tv[:,2], '.',markersize=4,label='obs')
@@ -834,15 +845,15 @@
     plt.xlabel('Azimuth (degrees)')
     plt.ylabel('Reflector Height (m)')
     plt.title('Quick Plot of RH with respect to Azimuth')
     plt.gca().invert_yaxis()
     plt.legend(loc="best")
     plt.grid()
     plotname = txtdir + '/' + station + '_outliers_wrt_az.png'
-    plt.savefig(plotname,dpi=150)
+    plt.savefig(plotname,dpi=300)
     print('png file saved as: ', plotname)
 
     #    fig=plt.figure(figsize=(10,6))
     fig = plt.figure(figsize=(10,6))
     colors = tv[:,5]
 # put some amplitude information on it
 # ax.plot( otimes, tv[:,2], '.')
@@ -871,15 +882,20 @@
     plt.plot(otimesarray[jj],tv[jj,2], '.',color='green',label='arcs')
     plt.gca().invert_yaxis()
     plt.ylabel('meters',fontsize=8)
     plt.xticks(rotation =45,fontsize=8); plt.yticks(fontsize=8)
     plt.title('Edited ' + station.upper() + ' Reflector Heights', fontsize=8)
     plt.grid() ; fig.autofmt_xdate()
     plotname = txtdir + '/' + station + '_outliers.png'
-    plt.savefig(plotname,dpi=300)
+    if hires_figs:
+        plotname = txtdir + '/' + station + '_outliers.png'
+        plt.savefig(plotname,dpi=300)
+    else:
+        plt.savefig(plotname,dpi=300)
+
     plt.ylim((savey1, savey2))
     print('png file saved as: ', plotname)
     if kplt:
         fig = plt.figure()
         ax1 = fig.add_subplot(211)
         ddd = - (tv[jj,2] - np.max(tv[jj,2]))
         plt.plot(otimesarray[jj],ddd, '.',color='blue')
@@ -1135,40 +1151,38 @@
 
 def rhdot_correction2(station,fname,fname_new,pltit,outlierV,outlierV2,**kwargs):
     """
     Improved code to compute rhdot correction and bias correction for subdaily
 
     Parameters
     ----------
-    station : string
+    station : str
         4 char station name
-
-    fname : string
+    fname : str
         input filename for results
-
-    fname_new : string
+    fname_new : str
         output filename for results
-
-    pltit : boolean 
+    pltit : bool
         whether you want plots to the screen
-
     outlierV : float
        outlier criterion, in meters  used in first go thru
        if None, then use 3 sigma (which is the default)
     outlierV2 : float
        outlier criterion, in meters  used in second go thru
        if None, then use 3 sigma (which is the default)
-
     delta_out : float, optional
         seconds for smooth output
     txtdir : str
         if wanting to set your own output directory
     apply_if_corr : bool, optional
         whether you want to apply the IF correction
         default is true
+    apply_rhdot : bool, optional
+        whether you want to apply the rhdot correction
+        default is true
 
     """
     # output will go to REFL_CODE/Files unless txtdir provided
     xdir = os.environ['REFL_CODE']
 
     val = kwargs.get('txtdir',[])
     if len(val) == 0:
@@ -1185,14 +1199,28 @@
 
     if_corr = kwargs.get('if_corr',True)
     if if_corr:
         apply_if_corr = True
     else:
         apply_if_corr = False
 
+    apply_rhdot  = kwargs.get('apply_rhdot',True)
+    if apply_rhdot:
+        apply_rhdot_corr = True
+    else:
+        apply_rhdot_corr = False
+
+    # probably a better way - but this is it for now ....
+    gotit = kwargs.get('hires_figs',True)
+    if gotit:
+        hires_figs = True
+        print('Requested high resolution figures')
+    else:
+        hires_figs = False
+
     #print('output directory: ', txtdir)
 
 #   how often do you want velocity computed (per day)
     perday = 24*20 # so every 3 minutes
     fs = 10 # fontsize
     # making a knot every three hours ...
     # knots_per_day = 8
@@ -1357,14 +1385,15 @@
     residual_after = residual_after[ii]
 
     # make the RHdot plot as well
     rhdot_plots(th,correction,rhdot_at_th, tvel,yvel,fs,station,txtdir)
 
     writecsv = False ; extraline = ''
     # write out the new solutions with RHdot and without 3 sigma outliers
+    # this should be changed to take into account apply_rhdot_corr
     write_subdaily(fname_new,station,tvd_new,writecsv,extraline,newRH=correctedRH_new, RHdot_corr=correction_new)
     nr,nc = tvd_new.shape
     print('Percent of observations removed:', round(100*(NV-nr)/NV,2))
 
     # now make yet another vector - this time to apply bias corrections
     # this is horrible code and needs to be fixed
     biasCorrected_RH = correctedRH_new
@@ -1476,15 +1505,19 @@
 
     plt.legend(loc="upper left")
     plt.grid()
     plt.gca().invert_yaxis()
     plt.ylabel('meters')
     plt.title('Station: ' + station + ', new spline, RHdot corr/InterFreq corr/outliers removed')
     plt.xlabel('days of the year')
-    g.save_plot(txtdir + '/' + station + '_rhdot4.png')
+    # put hires_figs boolean here
+    if hires_figs:
+        g.save_plot(txtdir + '/' + station + '_rhdot4.eps')
+    else:
+        g.save_plot(txtdir + '/' + station + '_rhdot4.png')
 
     fig=plt.figure(figsize=(10,5))
     #plt.subplot(2,1,1)
     plt.plot(th, biasCor_rh - spline_at_GPS, 'b.',label='all residuals')
     plt.title('Station:' + station + ' Residuals to new spline fit')
     plt.grid()
     plt.ylabel('meters')
@@ -1654,16 +1687,17 @@
     fig.autofmt_xdate()
 
     if percent99:
         plotname = txtdir + '/' + station + '_rh2_99.png'
     else:
         plotname = txtdir + '/' + station + '_rh2.png'
 
+
     print('png file saved as: ', plotname)
-    plt.savefig(plotname,dpi=150)
+    plt.savefig(plotname,dpi=300)
 
 def my_percentile(rh,p1, p2):
     """
     numpy percentile was crashing docker build
     this is a quick work around
 
     Parameters
@@ -1691,15 +1725,15 @@
 
     # calculate the low and high values at these percentiles
     lowv = sorted_rh[N1] 
     highv = sorted_rh[N2]
 
     return  lowv, highv
 
-def numsats_plot(station,tval,nval,Gval,Rval,Eval,Cval,txtdir,fs):
+def numsats_plot(station,tval,nval,Gval,Rval,Eval,Cval,txtdir,fs,hires_figs):
     """
     makes the plot that summarizes the number of satellites in each
     constellation per epoch
 
     Parameters
     ----------
     station : str
@@ -1716,14 +1750,16 @@
         number of galileo satellites at an epoch
     Cval : numpy array
         number of beidou satellites at an epoch
     txtdir : str
         where results are stored
     fs : int
         fontsize for the plots
+    hires_figs : bool
+        try to plot high resolution
 
     """
 
     fig,ax=plt.subplots()
     ax.plot(tval,nval,'ko',label='Total',markersize=3)
     if (np.sum(Gval) > 0):
         ax.plot(tval,Gval,'bo',label='GPS',markersize=3)
@@ -1735,10 +1771,14 @@
         ax.plot(tval,Cval,'co',label='BEI',markersize=3)
     plt.legend(loc="upper left")
     plt.title(station + ': number of RH retrievals each day',fontsize=fs)
     plt.xticks(rotation =45,fontsize=fs); plt.yticks(fontsize=fs)
     plt.grid()
     fig.autofmt_xdate()
     plotname = txtdir + '/' + station + '_Subnvals.png'
-    plt.savefig(plotname,dpi=150)
+    if hires_figs:
+        plotname = txtdir + '/' + station + '_Subnvals.eps'
+        plt.savefig(plotname,dpi=300)
+    else:
+        plt.savefig(plotname,dpi=300)
     print('png file saved as: ', plotname)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/subdaily_cl.py` & `gnssrefl-1.4.1/gnssrefl/subdaily_cl.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,34 +36,48 @@
     parser.add_argument("-h2", default=None, type=float, help="max RH (m)")
     parser.add_argument("-peak2noise", default=None, type=float, help="new peak2noise constraint")
     parser.add_argument("-kplt", default=None, type=str, help="special plot for kristine")
     parser.add_argument("-subdir", default=None, type=str, help="non-default subdirectory for output")
     parser.add_argument("-delta_out", default=None, type=int, help="Output interval for spline fit, seconds (default is 1800)")
     parser.add_argument("-if_corr", default=None, type=str, help="Interfrequency correction applied, optional")
     parser.add_argument("-knots_test", default=None, type=int, help="test knots")
+    parser.add_argument("-hires_figs", default=None, type=str, help="hi-res figures")
+    parser.add_argument("-apply_rhdot", default=None, type=str, help="apply rhdot, default is True")
 
     args = parser.parse_args().__dict__
 
     # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['csvfile', 'plt', 'rhdot', 'testing','kplt','if_corr']
+    boolean_args = ['csvfile', 'plt', 'rhdot', 'testing','kplt','if_corr','hires_figs','apply_rhdot']
     args = str2bool(args, boolean_args)
 
     # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
     return {key: value for key, value in args.items() if value is not None}
 
 
 def subdaily(station: str, year: int, txtfile_part1: str = '', txtfile_part2: str = None, csvfile: bool = False, 
         plt: bool = True, spline_outlier1: float = None, spline_outlier2: float = None, 
         knots: int = 8, sigma: float = 2.5, extension: str = '', rhdot: bool = True, doy1: int = 1, 
-        doy2: int = 366, testing: bool = True, ampl: float = 0, h1: float=0.0, h2: float=300.0, 
+        doy2: int = 366, testing: bool = True, ampl: float = 0, h1: float=0.4, h2: float=300.0, 
         azim1: int=0, azim2: int = 360, peak2noise: float = 0, kplt: bool = False, 
-        subdir: str = None, delta_out : int = 1800, if_corr: bool = True, knots_test: int = 0):
+        subdir: str = None, delta_out : int = 1800, if_corr: bool = True, knots_test: int = 0, 
+        hires_figs : bool=False, apply_rhdot : bool=True):
     """
-    subdaily combines multiple day gnssir solutions and applies relevant corrections. 
-    It works on one year at a time; you can restricts time periods within a year with -doy1 and -doy2
+    Subdaily combines multiple day gnssir solutions and applies relevant corrections. 
+    It only works for one year at a time; you can restricts time periods within a year with -doy1 and -doy2
+
+    WARNING: this code is meant to be used at sites with tidal signals. If you have a site without it, you 
+    should probably use daily_avg instead. If you insist on using this code on such sites (rivers and lakes),
+    you should think about how this code is implemented - it is using splines with 8 knots as the default 
+    (i.e. knot every three hours).  This is very unlikely to be acceptable for a lake or non-tidal river.
+    You should change the knot setting.
+
+    WARNING: this code calculates and applies various corrections. New Reflector Height values are added 
+    to the output files as new columns. If you run the code but continue to assume the "good answers" are
+    in column 2, you are essentially not using the code at all.
+
 
     Examples
     --------
 
     subdaily at01 2023 -plt F
         for station at01, all solutions in 2023  but no plots to the screen
 
@@ -90,15 +104,14 @@
     txtfile_part1 is optional input if you want to skip part 1 and use your own file (but in the same format).
 
     txtfile_part2 is optional input to the second part of the code.
 
 
     Parameters
     ----------
-
     station : str
         4 character id of the station.
     year : int
         full year
     txtfile_part1 : str, optional
         input File name.
     txtfile_part2 : str, optional
@@ -115,51 +128,54 @@
         Outlier criterion used in second splinefit, after IF & RHdot (meters)
     knots : integer, optional
         Knots per day, spline fit only.
         default is 8.
     sigma : float, optional
         Simple sigma outlier criterion (e.g. 1 for 1sigma, 3 for 3sigma)
         default is 2.5
-    extension : string, optional
+    extension : str, optional
         Solution subdirectory.
         default is empty string.
-    rhdot : boolean, optional
+    rhdot : bool, optional
         Set to True to turn on spline fitting for RHdot correction.
         default is True.
-    doy1 : integer, optional
-        Initial day of year
-        default is 1.
-    doy2 : integer, optional
-        End day of year.
-        default is 366.
-    testing : boolean, optional
+    doy1 : int, optional
+        Initial day of year, default is 1.
+    doy2 : int, optional
+        End day of year. Default is 366.
+    testing : bool, optional
         Set to False for older code.
         default is now True.
     ampl : float, optional
-        New amplitude constraint
-        default is 0.
+        New amplitude constraint. Default is 0.
     azim1: int, optional
-        New min azimuth
-        default is 0.
+        minimum azimuth. Default is 0.
     azim2: int, optional
-        New max azimuth
-        default is 360.
-    h1: float optional 
-        lowest allowed reflector height
-        default is 0
-    h2: float optional 
-        highest allowed reflector height
-        default is 300
+        Max azimuth. Default is 360.
+    h1: float, optional 
+        lowest allowed reflector height in meters. Default is 0.4
+    h2: float, optional 
+        highest allowed reflector height in meters. Default is 300
     peak2noise: float, optional
-        New peak to noise constraint
-        default is 0.
-    kplt: boolean, optional
+        New peak to noise constraint. Default is 0.
+    kplt: bool, optional
         plot for kristine
     subdir : str, optional
         name for output subdirectory in REFL_CODE/Files
+    delta_out : int, optional
+        how frequently - in seconds - you want smooth spline model output written
+        default is 1800 seconds
+    if_corr : bool, option
+        whether you want the inter-frequency removed
+        default is true
+    hires_figs : bool, optional
+        whether high resolution figures are made
+    apply_rhdot : bool, optional
+        whether you want the RH dot correction applied
+        for a lake or river you would not want it to be.
 
     """
 
     if len(station) != 4:
         print('station names must be four characters long')
         sys.exit()
 
@@ -191,15 +207,16 @@
             print('Will pick up and concatenate daily result files')
         else:
             print('Using ', txtfile_part1)
         # if txtfile provided, you can use that as your starting dataset 
         
         default_usage = True
         ntv, obstimes, fname, fname_new = t.readin_and_plot(station, year, doy1, doy2, plt, 
-                extension, sigma, writecsv, azim1, azim2, ampl, peak2noise, txtfile_part1,h1,h2,kplt,txtdir,default_usage)
+                extension, sigma, writecsv, azim1, azim2, ampl, peak2noise, txtfile_part1, 
+                h1,h2,kplt,txtdir,default_usage,hires_figs)
         haveObstimes = True
     else:
         haveObstimes = False
         fname_new = txtfile_part2
         if not os.path.isfile(fname_new):
             print('Input subdaily RH file you provided does not exist:', fname_new)
             sys.exit()
@@ -209,15 +226,16 @@
         if plt:
             mplt.show()
     input2spline = fname_new; output4spline = fname_new + '.withrhdot'
 
     # not sure why tv and corr are being returned.
     if rhdot:
        tv, corr = t.rhdot_correction2(station, input2spline, output4spline, plt, spline_outlier1, spline_outlier2, 
-                   knots=knots,txtdir=txtdir,testing=testing,delta_out=delta_out,if_corr=if_corr,knots_test=knots_test)
+                   knots=knots,txtdir=txtdir,testing=testing,delta_out=delta_out,
+                   if_corr=if_corr,knots_test=knots_test,hires_figs=hires_figs,apply_rhdot=apply_rhdot)
        if plt:
            mplt.show()
 
 def main():
     args = parse_arguments()
     subdaily(**args)
```

### Comparing `gnssrefl-1.3.8/gnssrefl/utils.py` & `gnssrefl-1.4.1/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/veg_multiyr.py` & `gnssrefl-1.4.1/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/vwc.py` & `gnssrefl-1.4.1/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/vwc_input.py` & `gnssrefl-1.4.1/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/xyz2llh.py` & `gnssrefl-1.4.1/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/ydoy.py` & `gnssrefl-1.4.1/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl/ymd.py` & `gnssrefl-1.4.1/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.4.1/gnssrefl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.8
+Version: 1.4.1
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.8** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.4.1** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
-Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
-The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
+Our documentation is available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
 
 [Youtube videos for beginners](https://www.youtube.com/channel/UCC1NW5oS7liG7C8NBK148Bg).
 
-New discussion page started about [modern GNSS signals](docs/pages/signal_issues.md).
+If you want to access CDDIS, including orbits, you should make [an account](https://urs.earthdata.nasa.gov/users/new).
+
+If you want to access to any Earthscope data, [an account is required](https://data-idm.unavco.org/user/profile/login).
 
 <HR> 
 
 GNSS-IR was developed with funding from NSF (ATM 0740515, EAR 0948957, AGS 0935725, EAR 1144221, AGS 1449554) and 
 NASA (NNX12AK21G and NNX13AF43G). <code>gnssrefl</code> was initially developed 
 as a fun post-retirement project, followed by support from NASA (80NSSC20K1731).
 
-This documentation was updated on March 24, 2023
+As of August 31, 2023, we will be an independent (unfunded) software package. Please help us maintain/improve this code. 
 
 Kristine M. Larson
 
+July 2, 2023
+
 <HR>
```

### Comparing `gnssrefl-1.3.8/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.4.1/gnssrefl.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 setup.py
 gnssrefl/EGM96.py
 gnssrefl/__init__.py
 gnssrefl/check_rinex_file.py
 gnssrefl/computemp1mp2.py
 gnssrefl/daily_avg.py
 gnssrefl/daily_avg_cl.py
+gnssrefl/decipher_argt.py
 gnssrefl/download_ioc.py
 gnssrefl/download_noaa.py
 gnssrefl/download_orbits.py
 gnssrefl/download_psmsl.py
 gnssrefl/download_rinex.py
 gnssrefl/download_teqc.py
 gnssrefl/download_tides.py
 gnssrefl/download_unr.py
 gnssrefl/download_wsv.py
-gnssrefl/felipe.py
 gnssrefl/filesizes.py
 gnssrefl/gnssir.py
 gnssrefl/gnssir_cl.py
+gnssrefl/gnssir_input.py
+gnssrefl/gnssir_v2.py
 gnssrefl/gnsssnr.f
 gnssrefl/gnsssnrbigger.f
 gnssrefl/gps.py
 gnssrefl/gpssnr.f
 gnssrefl/gpsweek.py
 gnssrefl/gpt_1wA.pickle
 gnssrefl/highrate.py
@@ -34,45 +36,50 @@
 gnssrefl/invsnr_input.py
 gnssrefl/karnak_libraries.py
 gnssrefl/kelly.py
 gnssrefl/llh2xyz.py
 gnssrefl/make_json_input.py
 gnssrefl/nmea2snr.py
 gnssrefl/nmea2snr_cl.py
+gnssrefl/nyquist_cl.py
+gnssrefl/nyquist_libs.py
 gnssrefl/phase_functions.py
 gnssrefl/pickle_dilemma.py
 gnssrefl/prn2gps.py
 gnssrefl/query_unr.py
 gnssrefl/quickLook_cl.py
 gnssrefl/quickLook_function.py
+gnssrefl/quickLook_function2.py
 gnssrefl/quickPhase.py
-gnssrefl/quickPhase_function.py
 gnssrefl/quicklib.py
 gnssrefl/quickplt.py
 gnssrefl/read_snr_files.py
 gnssrefl/refl_zones.py
 gnssrefl/refl_zones_cl.py
 gnssrefl/refraction.py
 gnssrefl/rh_plot.py
 gnssrefl/rinex2snr.py
 gnssrefl/rinex2snr_cl.py
 gnssrefl/rinex3_rinex2.py
 gnssrefl/rinex3_snr.py
 gnssrefl/rinpy.py
 gnssrefl/rt_rinex3_snr.py
 gnssrefl/smoosh.py
+gnssrefl/smoosh_snr.py
 gnssrefl/snow_functions.py
 gnssrefl/snowdepth_cl.py
 gnssrefl/spline_functions.py
 gnssrefl/subdaily.py
 gnssrefl/subdaily_cl.py
 gnssrefl/utils.py
 gnssrefl/veg_multiyr.py
 gnssrefl/vwc.py
+gnssrefl/vwc_cl.py
 gnssrefl/vwc_input.py
+gnssrefl/xnmeasnr.f
 gnssrefl/xyz2llh.py
 gnssrefl/ydoy.py
 gnssrefl/ymd.py
 gnssrefl.egg-info/PKG-INFO
 gnssrefl.egg-info/SOURCES.txt
 gnssrefl.egg-info/dependency_links.txt
 gnssrefl.egg-info/entry_points.txt
```

### Comparing `gnssrefl-1.3.8/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.4.1/gnssrefl.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 download_orbits = gnssrefl.download_orbits:main
 download_rinex = gnssrefl.download_rinex:main
 download_teqc = gnssrefl.download_teqc:main
 download_tides = gnssrefl.download_tides:main
 download_unr = gnssrefl.download_unr:main
 filesizes = gnssrefl.filesizes:main
 gnssir = gnssrefl.gnssir_cl:main
+gnssir_input = gnssrefl.gnssir_input:main
 gpsweek = gnssrefl.gpsweek:main
 installexe = gnssrefl.installexe_cl:main
 invsnr = gnssrefl.invsnr_cl:main
 invsnr_input = gnssrefl.invsnr_input:main
 llh2xyz = gnssrefl.llh2xyz:main
-make_json_input = gnssrefl.make_json_input:main
 mp1mp2 = gnssrefl.computemp1mp2:main
 nmea2snr = gnssrefl.nmea2snr_cl:main
+nyquist = gnssrefl.nyquist_cl:main
 phase = gnssrefl.quickPhase:main
 pickle_dilemma = gnssrefl.pickle_dilemma:main
 prn2gps = gnssrefl.prn2gps:main
 query_unr = gnssrefl.query_unr:main
 quickLook = gnssrefl.quickLook_cl:main
 quickplt = gnssrefl.quickplt:main
 refl_zones = gnssrefl.refl_zones_cl:main
 rh_plot = gnssrefl.rh_plot:main
 rinex2snr = gnssrefl.rinex2snr_cl:main
 rinex3_rinex2 = gnssrefl.rinex3_rinex2:main
 rinex3_snr = gnssrefl.rinex3_snr:main
 rt_rinex3_snr = gnssrefl.rt_rinex3_snr:main
 smoosh = gnssrefl.smoosh:main
+smoosh_snr = gnssrefl.smoosh_snr:main
 snowdepth = gnssrefl.snowdepth_cl:main
 subdaily = gnssrefl.subdaily_cl:main
 veg_multiyr = gnssrefl.veg_multiyr:main
-vwc = gnssrefl.vwc:main
+vwc = gnssrefl.vwc_cl:main
 vwc_input = gnssrefl.vwc_input:main
 xyz2llh = gnssrefl.xyz2llh:main
 ydoy = gnssrefl.ydoy:main
 ymd = gnssrefl.ymd:main
```

### Comparing `gnssrefl-1.3.8/pyproject.toml` & `gnssrefl-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.8/setup.py` & `gnssrefl-1.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,26 @@
         sources=['gnssrefl/gnsssnr.f'], 
         f2py_options=['--verbose'],
         )
 ext3 = Extension(name='gnssrefl.gnsssnrbigger', 
         sources=['gnssrefl/gnsssnrbigger.f'], 
         f2py_options=['--verbose'],
         )
+ext4 = Extension(name='gnssrefl.xnmeasnr', 
+        sources=['gnssrefl/xnmeasnr.f'], 
+        f2py_options=['--verbose'],
+        )
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.8",
+    version="1.4.1",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
@@ -35,15 +39,15 @@
         'console_scripts': [ 
             'gnssir = gnssrefl.gnssir_cl:main',
             'rinex2snr = gnssrefl.rinex2snr_cl:main',
             'daily_avg = gnssrefl.daily_avg_cl:main',
             'quickLook= gnssrefl.quickLook_cl:main',
             'download_rinex = gnssrefl.download_rinex:main',
             'download_orbits = gnssrefl.download_orbits:main',
-            'make_json_input = gnssrefl.make_json_input:main',
+            'gnssir_input = gnssrefl.gnssir_input:main',
             'ymd = gnssrefl.ymd:main',
             'ydoy = gnssrefl.ydoy:main',
             'xyz2llh = gnssrefl.xyz2llh:main',
             'llh2xyz = gnssrefl.llh2xyz:main',
             'prn2gps = gnssrefl.prn2gps:main',
             'download_tides = gnssrefl.download_tides:main',
             'subdaily= gnssrefl.subdaily_cl:main',
@@ -61,22 +65,24 @@
             'rt_rinex3_snr= gnssrefl.rt_rinex3_snr:main',
             'filesizes= gnssrefl.filesizes:main',
             'invsnr= gnssrefl.invsnr_cl:main',
             'invsnr_input= gnssrefl.invsnr_input:main',
             'vwc_input= gnssrefl.vwc_input:main',
             'phase= gnssrefl.quickPhase:main',
             'refl_zones= gnssrefl.refl_zones_cl:main',
-            'vwc= gnssrefl.vwc:main',
+            'vwc= gnssrefl.vwc_cl:main',
             'smoosh= gnssrefl.smoosh:main',
+            'smoosh_snr= gnssrefl.smoosh_snr:main',
             'quickplt= gnssrefl.quickplt:main',
             'snowdepth= gnssrefl.snowdepth_cl:main',
             'rh_plot= gnssrefl.rh_plot:main',
+            'nyquist= gnssrefl.nyquist_cl:main',
             'pickle_dilemma= gnssrefl.pickle_dilemma:main',
             ], 
         },
     install_requires=requirements,
-    ext_modules = [ext1,ext2,ext3],
+    ext_modules = [ext1,ext2,ext3,ext4],
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 )
```

### Comparing `gnssrefl-1.3.8/test/test_gps.py` & `gnssrefl-1.4.1/test/test_gps.py`

 * *Files identical despite different names*


# Comparing `tmp/foxes-0.4.0.tar.gz` & `tmp/foxes-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.4.0.tar", last modified: Mon Jun 12 12:59:15 2023, max compression
+gzip compressed data, was "foxes-0.4.1.tar", last modified: Fri Jul  7 09:25:33 2023, max compression
```

## Comparing `foxes-0.4.0.tar` & `foxes-0.4.1.tar`

### file list

```diff
@@ -1,262 +1,263 @@
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2023-06-02 08:05:39.000000 foxes-0.4.0/LICENSE
--rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2023-06-02 08:05:43.000000 foxes-0.4.0/Logo_FOXES.svg
--rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2023-06-02 08:05:43.000000 foxes-0.4.0/MANIFEST.in
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-12 12:59:15.634295 foxes-0.4.0/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5769 2023-06-12 12:58:21.000000 foxes-0.4.0/README.md
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/VERSION
--rw-r--r--   0 jonas     (1000) jonas     (1000)      717 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      188 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/downwind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2023-06-02 08:05:44.000000 foxes-0.4.0/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17305 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/downwind/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2023-06-02 08:05:44.000000 foxes-0.4.0/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-06-06 06:30:42.000000 foxes-0.4.0/foxes/algorithms/downwind/models/calc_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3329 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4391 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1876 2023-06-02 08:05:44.000000 foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1500 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/iterative/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-06 06:30:42.000000 foxes-0.4.0/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2016 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/algorithms/iterative/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      161 2023-06-06 06:30:42.000000 foxes-0.4.0/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5050 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3266 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4064 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/algorithms/iterative/models/loop_runner.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1568 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/constants.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      811 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    16552 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/algorithm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2951 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7859 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/data_calc_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12097 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/farm_controller.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7251 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/farm_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      269 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/farm_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5554 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5135 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/partial_wakes_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6923 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/point_data_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12744 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/rotor_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8120 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3059 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/turbine.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1069 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/turbine_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1418 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/turbine_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1637 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/vertical_profile.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6492 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wake_frame.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2908 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wake_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2547 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wake_superposition.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1713 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/core/wind_farm.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/data/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/farms/
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/farms/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2957 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/data/parse.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/power_ct_curves/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/data/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/data/states/wind_rotation.nc
--rw-r--r--   0 jonas     (1000) jonas     (1000)      543 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/data/static_data.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/input/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/farm_layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3189 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_csv.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      578 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_df.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1578 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1646 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/from_json.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1469 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1196 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/farm_layout/row.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/states/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      302 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/states/create/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2023-06-02 08:05:43.000000 foxes-0.4.0/foxes/input/states/create/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3270 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    16107 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/field_data_nc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12501 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/multi_height.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4459 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/scan_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5850 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/single.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10640 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/states/states_table.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/input/windio/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/input/windio/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8680 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/input/windio/windio.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/farm_controllers/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       71 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      253 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/farm_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       65 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/farm_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3439 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    13207 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/model_book.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/partial_wakes/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      241 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10485 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10792 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/distsliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2695 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7519 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/mapped.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6214 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9670 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/point_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      130 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/point_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4548 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1403 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2027 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/rotor_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5607 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/rotor_models/centre.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4993 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/rotor_models/grid.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/turbine_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      457 2023-06-12 12:58:21.000000 foxes-0.4.0/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2658 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2892 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5888 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/lookup_table.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5509 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4510 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/rotor_centre_calc.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7695 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3500 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/set_XYHD.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4533 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5247 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2162 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1613 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1584 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes/models/turbine_types/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1567 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/CpCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2285 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/CpCt_from_two.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7884 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     9027 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/PCt_from_two.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      248 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1316 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11215 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/turbine_types/wsrho2PCt_from_two.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/vertical_profiles/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      314 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1121 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_neutral_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1200 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_stable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1212 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_unstable_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2534 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/abl_log_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1245 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/sheared_ws.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1202 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_frames/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      164 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4754 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3816 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11983 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8304 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_models/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_models/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2693 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2659 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_models/ti/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      124 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8485 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6242 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5136 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/top_hat.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_models/wind/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5597 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/bastankhah.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5073 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    15626 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/porte_agel.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    12164 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/models/wake_superpositions/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      236 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6016 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/linear.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6781 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/max.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3889 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/product.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6574 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/quadratic.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4858 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/models/wake_superpositions/ti_superp.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      171 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/constraints/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      158 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/constraints/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6176 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7538 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/core/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      288 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/core/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2017 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2047 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_objective.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10624 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7778 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5684 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/objectives/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/objectives/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8998 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4156 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/problems/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      103 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/problems/layout/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5772 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      385 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    22671 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     8176 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7598 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10115 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    14234 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    17906 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    11816 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10637 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    19431 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/output/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      391 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/output/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10647 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/farm_layout.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    15752 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/farm_results_eval.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    45090 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/flow_plots_2d.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2204 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/output.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2670 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/results_writer.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    10073 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/rose_plot.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2425 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/state_turbine_map.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5526 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      480 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/__init__.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/abl/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/abl/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1370 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/neutral.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      451 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/sheared.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1834 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/stable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1611 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/abl/unstable.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3321 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/cubic_roots.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5306 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/data_book.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      898 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/dict.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/geom2d/
--rw-r--r--   0 jonas     (1000) jonas     (1000)      251 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)    19159 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4538 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/circle.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1626 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1750 2023-06-06 06:32:22.000000 foxes-0.4.0/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6175 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     5542 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7915 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     4631 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/pandas_helpers.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      373 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/plotly_helpers.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.634295 foxes-0.4.0/foxes/utils/runners/
--rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/runners/__init__.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6523 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/runners/runners.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)      384 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/subclasses.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2818 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/two_circles.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     2829 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/utils/wind_dir.py
--rw-r--r--   0 jonas     (1000) jonas     (1000)     3576 2023-06-12 12:58:24.000000 foxes-0.4.0/foxes/variables.py
-drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-06-12 12:59:15.624295 foxes-0.4.0/foxes.egg-info/
--rw-r--r--   0 jonas     (1000) jonas     (1000)     6589 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/PKG-INFO
--rw-r--r--   0 jonas     (1000) jonas     (1000)     7734 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)      195 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/requires.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/top_level.txt
--rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-06-12 12:59:15.000000 foxes-0.4.0/foxes.egg-info/zip-safe
--rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2023-06-02 08:05:39.000000 foxes-0.4.0/pyproject.toml
--rw-r--r--   0 jonas     (1000) jonas     (1000)     1131 2023-06-12 12:59:15.634295 foxes-0.4.0/setup.cfg
--rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2023-06-02 08:05:43.000000 foxes-0.4.0/setup.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1071 2023-06-02 08:05:39.000000 foxes-0.4.1/LICENSE
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    40774 2023-06-02 08:05:43.000000 foxes-0.4.1/Logo_FOXES.svg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      215 2023-06-02 08:05:43.000000 foxes-0.4.1/MANIFEST.in
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7287 2023-07-07 09:25:33.591802 foxes-0.4.1/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6468 2023-07-07 09:20:16.000000 foxes-0.4.1/README.md
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/VERSION
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      717 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      188 2023-07-04 09:56:46.000000 foxes-0.4.1/foxes/algorithms/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/downwind/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       53 2023-06-02 08:05:44.000000 foxes-0.4.1/foxes/algorithms/downwind/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17768 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/downwind.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/downwind/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      242 2023-06-02 08:05:44.000000 foxes-0.4.1/foxes/algorithms/downwind/models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2292 2023-06-06 06:30:42.000000 foxes-0.4.1/foxes/algorithms/downwind/models/calc_order.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3382 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4400 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1701 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1500 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/iterative/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      137 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4876 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/iterative.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/algorithms/iterative/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6272 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/models/convergence.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3355 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2373 2023-07-07 09:22:06.000000 foxes-0.4.1/foxes/constants.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/core/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      811 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/core/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17540 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/algorithm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5843 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/data.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9387 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/data_calc_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12417 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/farm_controller.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7534 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/farm_data_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      265 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/farm_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    13023 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5857 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/partial_wakes_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7210 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/point_data_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12866 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/rotor_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8109 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/states.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3055 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/turbine.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1069 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/core/turbine_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1410 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/turbine_type.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1633 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/vertical_profile.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6465 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wake_frame.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3171 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wake_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2760 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wake_superposition.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1709 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/core/wind_farm.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/data/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/data/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/data/farms/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/farms/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1872 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/farms/test_farm_67.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2949 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/data/parse.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes/data/power_ct_curves/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      410 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      300 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      851 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      401 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/power_ct_curves/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/data/states/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   427815 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        0 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)   126124 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/abl_states_6000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      501 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/data/states/timeseries_100.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    29085 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/timeseries_3000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    78694 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/timeseries_8000.csv.gz
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4943 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/wind_rose_bremen.csv
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10990 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/data/states/wind_rotation.nc
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      539 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/data/static_data.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      125 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/farm_layout/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      250 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/farm_layout/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3185 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/from_csv.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      574 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/from_df.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1578 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/farm_layout/from_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1642 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/from_json.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1465 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/farm_layout/grid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1196 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/farm_layout/row.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/states/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      302 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/states/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/states/create/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       81 2023-06-02 08:05:43.000000 foxes-0.4.1/foxes/input/states/create/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3262 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/create/random_abl_states.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    16099 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/field_data_nc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12490 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/multi_height.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4455 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/scan_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5842 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/single.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10625 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/states/states_table.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/input/windio/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       88 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/input/windio/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8676 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/input/windio/windio.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      375 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/farm_controllers/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       71 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/farm_controllers/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      249 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/farm_controllers/basic.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/farm_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       65 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/farm_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3427 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/farm_models/turbine2farm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14000 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/model_book.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/partial_wakes/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      241 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/partial_wakes/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11367 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/axiwake.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11820 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/distsliced.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2518 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/grid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8717 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/mapped.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5656 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/rotor_points.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10173 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/partial_wakes/top_hat.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/point_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      130 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/point_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4540 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/point_models/set_uniform_data.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1399 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/point_models/tke2ti.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2027 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/point_models/wake_deltas.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/rotor_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       82 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/rotor_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5607 2023-07-07 09:07:29.000000 foxes-0.4.1/foxes/models/rotor_models/centre.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4985 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/rotor_models/grid.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/turbine_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      457 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/turbine_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2650 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/calculator.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3136 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/kTI_model.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5969 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/lookup_table.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5501 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/power_mask.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4464 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7688 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/sector_management.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3492 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/set_XYHD.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4543 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/set_farm_vars.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5239 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/table_factors.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2139 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/thrust2ct.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1780 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/yaw2yawm.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1751 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_models/yawm2yaw.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/turbine_types/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1559 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/CpCt_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2277 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/CpCt_from_two.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7803 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/PCt_file.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8954 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/PCt_from_two.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      248 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/turbine_types/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1312 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/turbine_types/null_type.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11215 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/turbine_types/wsrho2PCt_from_two.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/vertical_profiles/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      314 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/vertical_profiles/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1117 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1196 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_stable_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1208 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2530 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/abl_log_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1225 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/sheared_ws.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1191 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/vertical_profiles/uniform.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_frames/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      197 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4760 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/farm_order.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3857 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/rotor_wd.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    12397 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/streamlines.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9995 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/timelines.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8452 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_frames/yawed_wakes.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_models/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_models/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2990 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/axisymmetric.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7349 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/dist_sliced.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2951 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/gaussian.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_models/ti/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      124 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_models/ti/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     9069 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6718 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/ti/iec_ti.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5603 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/top_hat.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_models/wind/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      212 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_models/wind/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6051 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/bastankhah.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5710 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/jensen.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17035 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/porte_agel.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    13025 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_models/wind/turbopark.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/models/wake_superpositions/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      236 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/models/wake_superpositions/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7258 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/linear.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8021 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/max.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4054 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/product.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7814 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/quadratic.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5068 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/models/wake_superpositions/ti_superp.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      171 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/constraints/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      158 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/constraints/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6156 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/constraints/area_geometry.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7531 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/constraints/min_dist.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/core/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      288 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/core/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2009 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_constraint.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2039 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_objective.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10671 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_opt_problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7774 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/farm_vars_problem.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5676 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/core/pop_states.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/objectives/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      152 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/objectives/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8983 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/objectives/farm_vars.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4149 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/objectives/max_n_turbines.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/problems/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      102 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/problems/layout/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      228 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/problems/layout/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5768 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/farm_layout.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      385 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    22624 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     8164 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7586 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10104 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    14222 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    17858 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    11804 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/reggrids_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10629 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/layout/regular_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    19425 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/opt/problems/opt_farm_vars.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/output/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      391 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/output/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10639 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/farm_layout.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    15744 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/farm_results_eval.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    46575 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/flow_plots_2d.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2204 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/output/output.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2662 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/results_writer.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    10065 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/rose_plot.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2421 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/state_turbine_map.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5514 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/output/turbine_type_curves.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.581802 foxes-0.4.1/foxes/utils/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      480 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/__init__.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/foxes/utils/abl/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      134 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/abl/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1358 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/abl/neutral.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      446 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/abl/sheared.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1830 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/abl/stable.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1611 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/abl/unstable.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     3321 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/cubic_roots.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5302 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/data_book.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      886 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/dict.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/foxes/utils/geom2d/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      251 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/geom2d/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)    19120 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/area_geometry.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4530 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/circle.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1626 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/geom2d/example_intersection.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1750 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/geom2d/example_union.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6167 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/half_plane.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     5534 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geom2d/polygon.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7895 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/geopandas_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4627 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/pandas_helpers.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      369 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/plotly_helpers.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.591802 foxes-0.4.1/foxes/utils/runners/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       55 2023-06-15 07:11:55.000000 foxes-0.4.1/foxes/utils/runners/__init__.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     6502 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/runners/runners.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      380 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/subclasses.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2810 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/two_circles.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     2825 2023-07-07 09:20:20.000000 foxes-0.4.1/foxes/utils/wind_dir.py
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     4261 2023-07-07 09:22:17.000000 foxes-0.4.1/foxes/variables.py
+drwxr-xr-x   0 jonas     (1000) jonas     (1000)        0 2023-07-07 09:25:33.571802 foxes-0.4.1/foxes.egg-info/
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7287 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/PKG-INFO
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     7763 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/SOURCES.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/dependency_links.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      200 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/requires.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        6 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/top_level.txt
+-rw-r--r--   0 jonas     (1000) jonas     (1000)        1 2023-07-07 09:25:33.000000 foxes-0.4.1/foxes.egg-info/zip-safe
+-rw-r--r--   0 jonas     (1000) jonas     (1000)      185 2023-06-02 08:05:39.000000 foxes-0.4.1/pyproject.toml
+-rw-r--r--   0 jonas     (1000) jonas     (1000)     1136 2023-07-07 09:25:33.591802 foxes-0.4.1/setup.cfg
+-rw-r--r--   0 jonas     (1000) jonas     (1000)       69 2023-06-02 08:05:43.000000 foxes-0.4.1/setup.py
```

### Comparing `foxes-0.4.0/LICENSE` & `foxes-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/Logo_FOXES.svg` & `foxes-0.4.1/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/PKG-INFO` & `foxes-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: foxes
-Version: 0.4.0
-Summary: Farm Optimization and eXtended yield Evaluation Software
-Author: Fraunhofer IWES
-Author-email: jonas.schmidt@iwes.fraunhofer.de
-License: MIT
-Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
-Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
-Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
-Keywords: Wind farm,Wake modelling,Wind farm optimization
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: doc
-Provides-Extra: scripts
-License-File: LICENSE
-
 # Welcome to foxes
 
 ![FOXES Logo](Logo_FOXES.svg)
 
 ## Overview
 
 The software `foxes` is a modular wind farm simulation and wake modelling toolbox which is based on engineering wake models. It has many applications, for example
@@ -43,14 +21,38 @@
 
 Source code: [https://github.com/FraunhoferIWES/foxes](https://github.com/FraunhoferIWES/foxes)
 
 PyPi reference: [https://pypi.org/project/foxes/](https://pypi.org/project/foxes/)
 
 Anaconda reference: [https://anaconda.org/conda-forge/foxes](https://anaconda.org/conda-forge/foxes)
 
+## Citation
+
+Please cite the JOSS paper `"FOXES: Farm Optimization and eXtended yield
+Evaluation Software"` 
+
+ [![DOI](https://joss.theoj.org/papers/10.21105/joss.05464/status.svg)](https://doi.org/10.21105/joss.05464)
+
+ Bibtex:
+ ```
+@article{
+    Schmidt2023, 
+    author = {Jonas Schmidt and Lukas Vollmer and Martin Dörenkämper and Bernhard Stoevesandt}, 
+    title = {FOXES: Farm Optimization and eXtended yield Evaluation Software}, 
+    doi = {10.21105/joss.05464}, 
+    url = {https://doi.org/10.21105/joss.05464}, 
+    year = {2023}, 
+    publisher = {The Open Journal}, 
+    volume = {8}, 
+    number = {86}, 
+    pages = {5464}, 
+    journal = {Journal of Open Source Software} 
+}
+ ```
+
 ## Requirements
 
 The supported Python versions are: 
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foxes-0.4.0/README.md` & `foxes-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: foxes
+Version: 0.4.1
+Summary: Farm Optimization and eXtended yield Evaluation Software
+Author: Fraunhofer IWES
+Author-email: jonas.schmidt@iwes.fraunhofer.de
+License: MIT
+Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
+Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
+Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
+Keywords: Wind farm,Wake modelling,Wind farm optimization
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: scripts
+License-File: LICENSE
+
 # Welcome to foxes
 
 ![FOXES Logo](Logo_FOXES.svg)
 
 ## Overview
 
 The software `foxes` is a modular wind farm simulation and wake modelling toolbox which is based on engineering wake models. It has many applications, for example
@@ -21,14 +43,38 @@
 
 Source code: [https://github.com/FraunhoferIWES/foxes](https://github.com/FraunhoferIWES/foxes)
 
 PyPi reference: [https://pypi.org/project/foxes/](https://pypi.org/project/foxes/)
 
 Anaconda reference: [https://anaconda.org/conda-forge/foxes](https://anaconda.org/conda-forge/foxes)
 
+## Citation
+
+Please cite the JOSS paper `"FOXES: Farm Optimization and eXtended yield
+Evaluation Software"` 
+
+ [![DOI](https://joss.theoj.org/papers/10.21105/joss.05464/status.svg)](https://doi.org/10.21105/joss.05464)
+
+ Bibtex:
+ ```
+@article{
+    Schmidt2023, 
+    author = {Jonas Schmidt and Lukas Vollmer and Martin Dörenkämper and Bernhard Stoevesandt}, 
+    title = {FOXES: Farm Optimization and eXtended yield Evaluation Software}, 
+    doi = {10.21105/joss.05464}, 
+    url = {https://doi.org/10.21105/joss.05464}, 
+    year = {2023}, 
+    publisher = {The Open Journal}, 
+    volume = {8}, 
+    number = {86}, 
+    pages = {5464}, 
+    journal = {Journal of Open Source Software} 
+}
+ ```
+
 ## Requirements
 
 The supported Python versions are: 
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foxes-0.4.0/foxes/__init__.py` & `foxes-0.4.1/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/algorithms/downwind/downwind.py` & `foxes-0.4.1/foxes/algorithms/downwind/downwind.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from foxes.core import Algorithm, FarmDataModelList
 from foxes.core import PointDataModel, PointDataModelList
-import foxes.algorithms.downwind.models as dm
 import foxes.models as fm
 import foxes.variables as FV
 import foxes.constants as FC
+from . import models as dm
+
 
 class Downwind(Algorithm):
     """
     The downwind algorithm.
 
     The turbines are evaluated once, in the order
     that is calculated by the provided `TurbineOrder`
@@ -37,15 +38,15 @@
         The farm controller. Will be
         looked up in the model book
     chunks : dict
         The chunks choice for running in parallel with dask,
         e.g. `{"state": 1000}` for chunks of 1000 states
     dbook : foxes.DataBook, optional
         The data book, or None for default
-    keep_models : list of str
+    keep_models : set of str
         Keep these models data in memory and do not finalize them
     verbosity : int
         The verbosity level, 0 means silent
 
     Attributes
     ----------
     states : foxes.core.States
@@ -77,15 +78,15 @@
         wake_models,
         rotor_model="centre",
         wake_frame="rotor_wd",
         partial_wakes_model="auto",
         farm_controller="basic_ctrl",
         chunks={FC.STATE: 1000},
         dbook=None,
-        keep_models=[],
+        keep_models=set(),
         verbosity=1,
     ):
         super().__init__(mbook, farm, chunks, verbosity, dbook, keep_models)
 
         self.states = states
         self.n_states = None
         self.states_data = None
@@ -165,15 +166,14 @@
             self.partial_wakes_model,
         ] + self.wake_models
 
         self.update_idata(mdls)
 
     def _collect_farm_models(
         self,
-        vars_to_amb,
         calc_parameters,
         ambient,
     ):
         """
         Helper function that creates model list
         """
         # prepare:
@@ -214,55 +214,71 @@
         # 5) run post-rotor turbine models via farm controller:
         mlist.models.append(self.farm_controller)
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
         calc_pars[-1]["pre_rotor"] = False
 
         # 6) copy results to ambient, requires self.farm_vars:
         self.farm_vars = mlist.output_farm_vars(self)
-        mlist.models.append(dm.SetAmbFarmResults(vars_to_amb))
+        mlist.models.append(dm.SetAmbFarmResults())
         mlist.models[-1].name = "set_amb_results"
         calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
         # 7) calculate wake effects:
         if not ambient:
             mlist.models.append(self.FarmWakesCalculation())
             mlist.models[-1].name = "calc_wakes"
             calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
+        # initialize models:
+        self.update_idata(mlist)
+
         # update variables:
-        self.farm_vars = [FV.WEIGHT] + mlist.output_farm_vars(self)
+        self.farm_vars = sorted(list(set([FV.WEIGHT] + mlist.output_farm_vars(self))))
 
         return mlist, calc_pars
 
+    def _run_farm_calc(self, mlist, *data, **kwargs):
+        """Helper function for running the main farm calculation"""
+        self.print(
+            f"\nCalculating {self.n_states} states for {self.n_turbines} turbines"
+        )
+        farm_results = mlist.run_calculation(
+            self, *data, out_vars=self.farm_vars, **kwargs
+        )
+        farm_results[FC.TNAME] = ((FC.TURBINE,), self.farm.turbine_names)
+        if FV.ORDER in farm_results:
+            farm_results[FV.ORDER] = farm_results[FV.ORDER].astype(FC.ITYPE)
+
+        return farm_results
+
     def calc_farm(
         self,
-        vars_to_amb=None,
         calc_parameters={},
         persist=True,
         finalize=True,
         ambient=False,
+        chunked_results=False,
     ):
         """
         Calculate farm data.
 
         Parameters
         ----------
-        vars_to_amb : list of str, optional
-            Variables for which ambient variables should
-            be stored. None means all.
         calc_parameters : dict
             Parameters for model calculation.
             Key: model name str, value: parameter dict
         persist : bool
             Switch for forcing dask to load all model data
             into memory
         finalize : bool
             Flag for finalization after calculation
         ambient : bool
             Flag for ambient instead of waked calculation
+        chunked_results: bool
+            Flag for chunked results
 
         Returns
         -------
         farm_results : xarray.Dataset
             The farm results. The calculated variables have
             dimensions (state, turbine)
 
@@ -271,49 +287,42 @@
         if not self.initialized:
             self.initialize()
 
         # welcome:
         self._print_deco("calc_farm")
 
         # collect models:
-        mlist, calc_pars = self._collect_farm_models(
-            vars_to_amb, calc_parameters, ambient
-        )
+        mlist, calc_pars = self._collect_farm_models(calc_parameters, ambient)
 
-        # initialize models and get input model data:
-        self.update_idata(mlist)
+        # get input model data:
         models_data = self.get_models_data()
         if persist:
             models_data = models_data.persist()
         self.print("\nInput data:\n\n", models_data, "\n")
         self.print(f"\nOutput farm variables:", ", ".join(self.farm_vars))
         self.print(f"\nChunks: {self.chunks}\n")
 
         # run main calculation:
-        self.print(
-            f"\nCalculating {self.n_states} states for {self.n_turbines} turbines"
-        )
-        farm_results = mlist.run_calculation(
-            self, models_data, out_vars=self.farm_vars, parameters=calc_pars
-        )
-        farm_results[FC.TNAME] = ((FC.TURBINE,), self.farm.turbine_names)
-        if FV.ORDER in farm_results:
-            farm_results[FV.ORDER] = farm_results[FV.ORDER].astype(FC.ITYPE)
+        farm_results = self._run_farm_calc(mlist, models_data, parameters=calc_pars)
         del models_data
 
         # finalize models:
         if finalize:
             self.print("\n")
             self.finalize_model(mlist)
             self.finalize()
+        self.cleanup()
 
         if ambient:
             dvars = [v for v in farm_results.data_vars.keys() if v in FV.var2amb]
             farm_results = farm_results.drop_vars(dvars)
 
+        if chunked_results:
+            farm_results = self.chunked(farm_results)
+
         return farm_results
 
     def _collect_point_models(
         self,
         vars,
         vars_to_amb,
         calc_parameters,
@@ -363,28 +372,32 @@
 
         # 3) calc wake effects:
         if not ambient:
             mlist.models.append(dm.PointWakesCalculation(vars, emodels, emodels_cpars))
             mlist.models[-1].name = "calc_wakes"
             calc_pars.append(calc_parameters.get(mlist.models[-1].name, {}))
 
+        # initialize models:
+        self.update_idata(mlist)
+
         return mlist, calc_pars
 
     def calc_points(
         self,
         farm_results,
         points,
         vars=None,
         vars_to_amb=None,
         point_models=None,
         calc_parameters={},
         persist_mdata=True,
         persist_pdata=False,
         finalize=True,
         ambient=False,
+        chunked_results=False,
     ):
         """
         Calculate data at a given set of points.
 
         Parameters
         ----------
         farm_results : xarray.Dataset
@@ -409,14 +422,16 @@
         persist_fdata : bool
             Switch for forcing dask to load all farm data
             into memory
         finalize : bool
             Flag for finalization after calculation
         ambient : bool
             Flag for ambient instead of waked calculation
+        chunked_results: bool
+            Flag for chunked results
 
         Returns
         -------
         point_results : xarray.Dataset
             The point results. The calculated variables have
             dimensions (state, point)
 
@@ -428,31 +443,30 @@
             raise ValueError(
                 f"Cannot calculate point results without farm results for ambient = {ambient}"
             )
 
         # welcome:
         self._print_deco("calc_points", n_points=points.shape[1])
 
-        # collect models:
+        # collect models and initialize:
         mlist, calc_pars = self._collect_point_models(
             vars, vars_to_amb, calc_parameters, point_models, ambient
         )
 
-        # initialize models and get input model data:
-        self.update_idata(mlist)
+        # get input model data:
         models_data = self.get_models_data()
         if persist_mdata:
             models_data = models_data.persist()
         self.print("\nInput data:\n\n", models_data, "\n")
         self.print(f"\nOutput farm variables:", ", ".join(self.farm_vars))
         self.print(f"\nChunks: {self.chunks}\n")
 
         # chunk farm results:
         if self.chunks is not None:
-            farm_results = farm_results.chunk(chunks={FC.STATE: self.chunks[FC.STATE]})
+            farm_results = self.chunked(farm_results)
         self.print("\nInput farm data:\n\n", farm_results, "\n")
 
         # get point data:
         if FC.STATE in farm_results.coords:
             sinds = farm_results.coords[FC.STATE]
         elif models_data is not None and FC.STATE in models_data.coords:
             sinds = models_data.coords[FC.STATE]
@@ -481,38 +495,46 @@
             self,
             models_data,
             farm_results,
             point_data,
             out_vars=vars,
             parameters=calc_pars,
         )
+
         del models_data, farm_results, point_data
 
         # finalize models:
         if finalize:
             self.print("\n")
-            mlist.finalize(self, self.verbosity)
+            self.finalize_model(mlist, self.verbosity)
             self.finalize()
+        self.cleanup()
 
         if ambient:
             dvars = [v for v in point_results.data_vars.keys() if v in FV.var2amb]
             point_results = point_results.drop_vars(dvars)
 
+        if chunked_results:
+            point_results = self.chunked(point_results)
+
         return point_results
 
     def finalize(self, clear_mem=False):
         """
         Finalizes the algorithm.
 
         Parameters
         ----------
         clear_mem : bool
             Clear idata memory, including keep_models entries
 
         """
+        if clear_mem:
+            self.keep_models = set()
+
         mdls = [
             self.states,
             self.rotor_model,
             self.farm_controller,
             self.wake_frame,
             self.partial_wakes_model,
         ] + self.wake_models
```

### Comparing `foxes-0.4.0/foxes/algorithms/downwind/models/calc_order.py` & `foxes-0.4.1/foxes/algorithms/downwind/models/calc_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.4.1/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,19 +51,15 @@
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.pwakes = algo.partial_wakes_model
-
-        idata = super().initialize(algo, verbosity)
-        algo.update_idata(self.pwakes, idata=idata, verbosity=verbosity)
-
-        return idata
+        return super().initialize(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
@@ -84,29 +80,33 @@
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         torder = fdata[FV.ORDER]
         n_order = torder.shape[1]
         n_states = mdata.n_states
 
-        wdeltas = self.pwakes.new_wake_deltas(algo, mdata, fdata)
+        def _evaluate(algo, mdata, fdata, pdata, wdeltas, o):
+            self.pwakes.evaluate_results(
+                algo, mdata, fdata, pdata, wdeltas, states_turbine=o
+            )
+
+            trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
+            np.put_along_axis(trbs, o[:, None], True, axis=1)
+
+            res = algo.farm_controller.calculate(
+                algo, mdata, fdata, pre_rotor=False, st_sel=trbs
+            )
+            fdata.update(res)
 
+        wdeltas, pdata = self.pwakes.new_wake_deltas(algo, mdata, fdata)
         for oi in range(n_order):
             o = torder[:, oi]
 
             if oi > 0:
-                self.pwakes.evaluate_results(
-                    algo, mdata, fdata, wdeltas, states_turbine=o
-                )
-
-                trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
-                np.put_along_axis(trbs, o[:, None], True, axis=1)
-
-                res = algo.farm_controller.calculate(
-                    algo, mdata, fdata, pre_rotor=False, st_sel=trbs
-                )
-                fdata.update(res)
+                _evaluate(algo, mdata, fdata, pdata, wdeltas, o)
 
             if oi < n_order - 1:
-                self.pwakes.contribute_to_wake_deltas(algo, mdata, fdata, o, wdeltas)
+                self.pwakes.contribute_to_wake_deltas(
+                    algo, mdata, fdata, pdata, o, wdeltas
+                )
 
         return {v: fdata[v] for v in self.output_farm_vars(algo)}
```

### Comparing `foxes-0.4.0/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.4.1/foxes/algorithms/downwind/models/point_wakes_calc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import foxes.variables as FV
 import foxes.constants as FC
 from foxes.core import PointDataModel
 
+
 class PointWakesCalculation(PointDataModel):
     """
     This model calculates wake effects at points of interest.
 
     Parameters
     ----------
     point_vars : list of str, optional
@@ -107,36 +108,37 @@
         results : dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_points)
 
         """
         torder = fdata[FV.ORDER].astype(FC.ITYPE)
         n_order = torder.shape[1]
-        points = pdata[FC.POINTS]
 
         wdeltas = {}
         wmodels = []
         for w in algo.wake_models:
             hdeltas = {}
-            w.init_wake_deltas(algo, mdata, fdata, pdata.n_points, hdeltas)
+            w.init_wake_deltas(algo, mdata, fdata, pdata, hdeltas)
             if len(set(self.pvars).intersection(hdeltas.keys())):
                 wdeltas.update(hdeltas)
                 wmodels.append(w)
             del hdeltas
 
         for oi in range(n_order):
             o = torder[:, oi]
-            wcoos = algo.wake_frame.get_wake_coos(algo, mdata, fdata, o, points)
+            wcoos = algo.wake_frame.get_wake_coos(algo, mdata, fdata, pdata, o)
 
             for w in wmodels:
-                w.contribute_to_wake_deltas(algo, mdata, fdata, o, wcoos, wdeltas)
+                w.contribute_to_wake_deltas(
+                    algo, mdata, fdata, pdata, o, wcoos, wdeltas
+                )
 
         amb_res = {v: pdata[FV.var2amb[v]] for v in wdeltas}
         for w in wmodels:
-            w.finalize_wake_deltas(algo, mdata, fdata, amb_res, wdeltas)
+            w.finalize_wake_deltas(algo, mdata, fdata, pdata, amb_res, wdeltas)
 
         for v in self.pvars:
             if v in wdeltas:
                 pdata[v] = amb_res[v] + wdeltas[v]
 
         if self.emodels is not None:
             self.emodels.calculate(algo, mdata, fdata, pdata, self.emodels_cpars)
```

### Comparing `foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 from foxes.core import FarmDataModel
 
 
 class SetAmbFarmResults(FarmDataModel):
     """
     This model copies farm data results to ambient results.
 
-    Parameters
-    ----------
-    vars_to_amb : list of str, optional
-        The variables to be copied, or `None` for all
-
     Attributes
     ----------
     vars : list of str
         The variables to be copied, or `None` for all
 
     """
 
-    def __init__(self, vars_to_amb=None):
+    def __init__(self):
+        """
+        Constructor.
+        """
         super().__init__()
-        self.vars = vars_to_amb
+        self.vars = None
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -35,15 +33,14 @@
         -------
         output_vars : list of str
             The output variable names
 
         """
         if self.vars is None:
             self.vars = set([v for v in algo.farm_vars if v in FV.var2amb])
-            self.vars -= set(algo.rotor_model.output_farm_vars(algo))
         return [FV.var2amb[v] for v in self.vars]
 
     def calculate(self, algo, mdata, fdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
```

### Comparing `foxes-0.4.0/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.4.1/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.4.1/foxes/algorithms/iterative/models/convergence.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,208 +1,270 @@
-import numpy as np
 from abc import ABCMeta, abstractmethod
+import numpy as np
 
 import foxes.variables as FV
 from foxes.utils import delta_wd
 
 
 class ConvCrit(metaclass=ABCMeta):
     """
     Abstract base class for convergence criteria
 
-    Parameters
+    Attributes
     ----------
-    name : str, optional
-        The convergence criteria name
-
-    Attribute
-    ---------
-    name : str, optional
+    name: str, optional
         The convergence criteria name
 
     """
 
     def __init__(self, name=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        name: str, optional
+            The convergence criteria name
+
+        """
         self.name = name if name is not None else type(self).__name__
 
     @abstractmethod
-    def check_converged(self, algo, fdata0, fdata1, verbosity=0):
+    def check_converged(self, algo, prev_results, results, verbosity=0):
         """
         Check convergence criteria.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        fdata0 : foxes.core.Data
-            The farm data results of previous
-            iteration, or None if first
-        fdata1 : foxes.core.Data
-            The farm data results of current
+        prev_results: xarray.Dataset
+            The farm results of previous
             iteration, or None if first
-        verbosity : int
+        results: xarray.Dataset
+            The farm results of current
+            iteration
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        convergence : bool
+        convergence: bool
             Convergence flag, true if converged
 
         """
         pass
 
+    @abstractmethod
+    def get_deltas(self):
+        """
+        Get the most recent evaluation deltas.
+
+        Returns
+        -------
+        deltas: dict
+            The most recent evaluation deltas
+
+        """
+        pass
+
 
 class ConvCritList(ConvCrit):
     """
     A list of convergence criteria
 
-    Parameters
-    ----------
-    crits : list of ConvCrit
-        The criteria
-    name : str, optional
-        The convergence criteria name
-
     Attributes
     ----------
-    crits : list of ConvCrit
+    crits: list of ConvCrit
         The criteria
 
     """
 
     def __init__(self, crits=[], name=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        crits: list of ConvCrit
+            The criteria
+        name: str, optional
+            The convergence criteria name
+
+        """
         super().__init__(name)
         self.crits = crits
 
     def add_crit(self, crit):
         """
         Add a convergence criterion
 
         Parameters
         ----------
-        crit : ConvCrit
+        crit: ConvCrit
             The criterion
 
         """
         self.crits.append(crit)
 
-    def check_converged(self, algo, fdata0, fdata1, verbosity=0):
+    def check_converged(self, algo, prev_results, results, verbosity=0):
         """
         Check convergence criteria.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        fdata0 : foxes.core.Data
-            The farm data results of previous
+        prev_results: xarray.Dataset
+            The farm results of previous
             iteration, or None if first
-        fdata1 : foxes.core.Data
-            The farm data results of current
-            iteration, or None if first
-        verbosity : int
+        results: xarray.Dataset
+            The farm results of current
+            iteration
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        convergence : bool
+        convergence: bool
             Convergence flag, true if converged
 
         """
+        self._failed = None
         for c in self.crits:
-            if not c.check_converged(algo, fdata0, fdata1, verbosity):
+            if not c.check_converged(algo, prev_results, results, verbosity):
+                self._failed = c
                 return False
 
         return True
 
+    def get_deltas(self):
+        """
+        Get the most recent evaluation deltas.
+
+        Returns
+        -------
+        deltas: dict
+            The most recent evaluation deltas
+
+        """
+        if self._failed is not None:
+            return self._failed.get_deltas()
+        return {}
+
 
 class ConvVarDelta(ConvCrit):
     """
     Requires convergence of a selection of variables.
 
-    Parameters
-    ----------
-    limits : dict
-        The convergence limits. Keys: variables str,
-        values: float values
-    wd_vars : list of str, optional
-        The wind direction type variables (unit deg)
-    name : str, optional
-        The convergence criteria name
-
     Attributes
     ----------
-    limits : dict
+    limits: dict
         The convergence limits. Keys: variables str,
         values: float values
-    wd_vars : list of str
+    wd_vars: list of str
         The wind direction type variables (unit deg)
 
     """
 
     def __init__(self, limits, wd_vars=None, name=None):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        limits: dict
+            The convergence limits. Keys: variables str,
+            values: float values
+        wd_vars: list of str, optional
+            The wind direction type variables (unit deg)
+        name: str, optional
+            The convergence criteria name
+
+        """
         super().__init__(name)
         self.limits = limits
         if wd_vars is None:
             self.wd_vars = [FV.WD, FV.AMB_WD, FV.YAW, FV.AMB_YAW]
         else:
             self.wd_vars = wd_vars
 
-    def check_converged(self, algo, fdata0, fdata1, verbosity=0):
+        self._deltas = {}
+
+    def check_converged(self, algo, prev_results, results, verbosity=0):
         """
         Check convergence criteria.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        fdata0 : foxes.core.Data
-            The farm data results of previous
-            iteration, or None if first
-        fdata1 : foxes.core.Data
-            The farm data results of current
+        prev_results: xarray.Dataset
+            The farm results of previous
             iteration, or None if first
-        verbosity : int
+        results: xarray.Dataset
+            The farm results of current
+            iteration
+        verbosity: int
             The verbosity level, 0 = silent
 
         Returns
         -------
-        convergence : bool
+        convergence: bool
             Convergence flag, true if converged
 
         """
-        if fdata0 is None:
+        if prev_results is None:
             return False
 
         if verbosity > 0:
             print(f"\n{self.name}: Convergence check")
+            L = max([len(v) for v in self.limits.keys()])
 
         ok = True
+        self._deltas = {}
         for v, lim in self.limits.items():
+            x0 = prev_results[v].to_numpy()
+            x = results[v].to_numpy()
             if v in self.wd_vars:
-                check = np.max(np.abs(delta_wd(fdata0[v], fdata1[v])))
+                self._deltas[v] = np.max(np.abs(delta_wd(x0, x)))
             else:
-                check = np.max(np.abs(fdata1[v] - fdata0[v]))
+                self._deltas[v] = np.max(np.abs(x - x0))
+            check = self._deltas[v]
             ok = ok and (check <= lim)
 
             if verbosity > 0:
                 r = "FAILED" if check > lim else "OK"
-                print(f"  {v}: delta = {check}, lim = {lim}  --  {r}")
+                print(f"  {v:<{L}}: delta = {check:.3e}, lim = {lim:.3e}  --  {r}")
             elif not ok:
                 break
 
         return ok
 
+    def get_deltas(self):
+        """
+        Get the most recent evaluation deltas.
+
+        Returns
+        -------
+        deltas: dict
+            The most recent evaluation deltas
+
+        """
+        return self._deltas
+
 
 class DefaultConv(ConvVarDelta):
     """
     Default convergence criteria.
     """
 
     def __init__(self):
+        """
+        Constructor.
+        """
         super().__init__(
             {
                 FV.REWS: 1e-5,
-                FV.WD: 1e-4,
                 FV.TI: 1e-6,
             }
         )
```

### Comparing `foxes-0.4.0/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.4.1/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from copy import deepcopy
 
 import foxes.variables as FV
+import foxes.constants as FC
 from foxes.core import FarmDataModel
 
 
 class FarmWakesCalculation(FarmDataModel):
     """
     This model calculates wakes effects on farm data.
     """
@@ -51,19 +52,15 @@
         idata : dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         self.pwakes = algo.partial_wakes_model
-
-        idata = super().initialize(algo, verbosity)
-        algo.update_idata(self.pwakes, idata=idata, verbosity=verbosity)
-
-        return idata
+        return super().initialize(algo, verbosity)
 
     def calculate(self, algo, mdata, fdata):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
@@ -84,26 +81,30 @@
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
 
         torder = fdata[FV.ORDER]
         n_order = torder.shape[1]
         n_states = mdata.n_states
-        wdeltas = self.pwakes.new_wake_deltas(algo, mdata, fdata)
 
-        for oi in range(n_order):
-            o = torder[:, oi]
-            self.pwakes.contribute_to_wake_deltas(algo, mdata, fdata, o, wdeltas)
-
-        for oi in range(n_order):
-            o = torder[:, oi]
-            self.pwakes.evaluate_results(algo, mdata, fdata, wdeltas, states_turbine=o)
+        def _evaluate(algo, mdata, fdata, pdata, wdeltas, o):
+            self.pwakes.evaluate_results(
+                algo, mdata, fdata, pdata, wdeltas, states_turbine=o
+            )
 
             trbs = np.zeros((n_states, algo.n_turbines), dtype=bool)
             np.put_along_axis(trbs, o[:, None], True, axis=1)
 
             res = algo.farm_controller.calculate(
                 algo, mdata, fdata, pre_rotor=False, st_sel=trbs
             )
             fdata.update(res)
 
+        wdeltas, pdata = self.pwakes.new_wake_deltas(algo, mdata, fdata)
+        for oi in range(n_order):
+            o = torder[:, oi]
+            self.pwakes.contribute_to_wake_deltas(algo, mdata, fdata, pdata, o, wdeltas)
+
+        for oi in range(n_order):
+            _evaluate(algo, mdata, fdata, pdata, wdeltas, torder[:, oi])
+
         return {v: fdata[v] for v in self.output_farm_vars(algo)}
```

### Comparing `foxes-0.4.0/foxes/algorithms/iterative/models/loop_runner.py` & `foxes-0.4.1/foxes/models/turbine_models/set_farm_vars.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,134 +1,167 @@
-from copy import deepcopy
+import numpy as np
 
-from foxes.core import FarmDataModelList
+from foxes.core import TurbineModel
+import foxes.constants as FC
 
 
-class LoopRunner(FarmDataModelList):
+class SetFarmVars(TurbineModel):
     """
-    This model runs the loop of iterations
-    within each individual chunk.
-
-    Parameters
-    ----------
-    mlist : foxes.core.FarmDataModelList
-        The models to be iterated
-    conv : foxes.algorithm.iterative.models.ConvCrit
-        The convergence criteria
-    model_wflag : list of bool, optional
-        True for models that should be run during wake iteration
-    max_its : int, optional
-        Set the maximal number of iterations, None means
-        number of turbines + 1
-    conv_error : bool
-        Throw error if not converging
-    verbosity : int
-        The verbosity level, 0 = silent
+    Set farm data variables to given data.
 
     Attributes
     ----------
-    conv : foxes.algorithm.iterative.models.ConvCrit
-        The convergence criteria
-    models : list of foxes.core.FarmDataModel
-        The model list
-    model_wflag : list of bool
-        True for models that should be run during wake iterations
-    max_its : int
-        Set the maximal number of iterations, None means
-        number of turbines + 1
-    conv_error : bool
-        Throw error if not converging
-    verbosity : int
-        The verbosity level, 0 = silent
+    vars: list of str
+        The variables to be set
+
+    :group: models.turbine_models
 
     """
 
-    def __init__(
-        self,
-        conv,
-        models=[],
-        model_wflag=None,
-        max_its=None,
-        conv_error=True,
-        verbosity=0,
-    ):
-        super().__init__(models=models)
-        self.conv = conv
-        self.verbosity = verbosity
-        self.model_wflag = (
-            [False for m in models] if model_wflag is None else model_wflag
-        )
-        self.max_its = max_its
-        self.conv_error = conv_error
+    def __init__(self, pre_rotor=False):
+        """
+        Constructor.
+
+        Parameters
+        ----------
+        pre_rotor: bool
+            Flag for running this model before
+            running the rotor model.
 
-    def append(self, model, wflag=False):
         """
-        Add a model to the list
+        super().__init__(pre_rotor=pre_rotor)
+        self.reset()
+
+    def add_var(self, var, data):
+        """
+        Add data for a variable.
 
         Parameters
         ----------
-        model : foxes.core.FarmDataModel
-            The model to add
-        wflag : bool
-            True if model should be run during wake iterations
+        var: str
+            The variable name
+        data: numpy.ndarray
+            The data, shape: (n_states, n_turbines)
+
+        """
+        self.vars.append(var)
+        self._vdata.append(np.asarray(data, dtype=FC.DTYPE))
 
+    def reset(self):
+        """
+        Remove all variables.
         """
-        super().append(model)
-        self.model_wflag.append(wflag)
+        self.vars = []
+        self._vdata = []
+
+    def output_farm_vars(self, algo):
+        """
+        The variables which are being modified by the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
 
-    def calculate(self, algo, mdata, fdata, parameters=[]):
+        Returns
+        -------
+        output_vars: list of str
+            The output variable names
+
+        """
+        return self.vars
+
+    def initialize(self, algo, verbosity=0):
+        """
+        Initializes the model.
+
+        This includes loading all required data from files. The model
+        should return all array type data as part of the idata return
+        dictionary (and not store it under self, for memory reasons). This
+        data will then be chunked and provided as part of the mdata object
+        during calculations.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
+
+        Returns
+        -------
+        idata: dict
+            The dict has exactly two entries: `data_vars`,
+            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
+            and `coords`, a dict with entries `dim_name_str -> dim_array`
+
+        """
+        idata = super().initialize(algo, verbosity)
+
+        for i, v in enumerate(self.vars):
+            data = np.full((algo.n_states, algo.n_turbines), np.nan, dtype=FC.DTYPE)
+            vdata = self._vdata[i]
+
+            # handle special case of call during vectorized optimization:
+            if (
+                np.ndim(vdata)
+                and vdata.shape[0] != algo.n_states
+                and hasattr(algo.states, "n_pop")
+            ):
+                n_pop = algo.states.n_pop
+                n_ost = algo.states.states.size()
+                n_trb = algo.n_turbines
+                vdata = np.zeros((n_pop, n_ost, n_trb), dtype=FC.DTYPE)
+                vdata[:] = self._vdata[i][None, :]
+                vdata = vdata.reshape(n_pop * n_ost, n_trb)
+
+            data[:] = vdata
+            idata["data_vars"][self.var(v)] = ((FC.STATE, FC.TURBINE), data)
+
+        return idata
+
+    def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
-        algo : foxes.core.Algorithm
+        algo: foxes.core.Algorithm
             The calculation algorithm
-        mdata : foxes.core.Data
+        mdata: foxes.core.Data
             The model data
-        fdata : foxes.core.Data
+        fdata: foxes.core.Data
             The farm data
-        parameters : list of dict, optional
-            A list of parameter dicts, one for each model
+        st_sel: numpy.ndarray of bool
+            The state-turbine selection,
+            shape: (n_states, n_turbines)
 
         Returns
         -------
-        results : dict
+        results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        fdata0 = None
-        it = 0
-        max_its = algo.n_turbines + 1 if self.max_its is None else self.max_its
-        while it < max_its:
-            if self.verbosity > 0:
-                print(f"\n{self.name}: Running iteration {it} (max_its = {max_its})\n")
-
-            # run all models at first iteration:
-            if fdata0 is None:
-                results = super().calculate(algo, mdata, fdata, parameters)
-                fdata.update(results)
+        n_states = fdata.n_states
+        n_turbines = fdata.n_turbines
+        allt = np.all(st_sel)
+
+        for v in self.vars:
+            data = mdata[self.var(v)]
+            hsel = ~np.isnan(data)
+            hallt = np.all(hsel)
 
-            # only run wake relevant models after first iteration:
-            else:
-                for mi, m in enumerate(self.models):
-                    if self.model_wflag[mi]:
-                        results = m.calculate(algo, mdata, fdata, **parameters[mi])
-                        fdata.update(results)
-            del results
+            if allt and hallt:
+                fdata[v][:] = data
 
-            if self.conv.check_converged(self, fdata0, fdata, verbosity=self.verbosity):
-                break
             else:
-                fdata0 = deepcopy(fdata)
-                it += 1
+                if v not in fdata:
+                    fdata[v] = np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
 
-        if it >= max_its and self.conv_error:
-            raise ValueError(
-                f"{self.name}: Maximal numer of iterations {max_its} reached, not converging."
-            )
+                tsel = st_sel & hsel
+                fdata[v][tsel] = data[tsel]
 
-        return {v: fdata[v] for v in self.output_farm_vars(algo)}
+        return {v: fdata[v] for v in self.vars}
```

### Comparing `foxes-0.4.0/foxes/core/__init__.py` & `foxes-0.4.1/foxes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/core/algorithm.py` & `foxes-0.4.1/foxes/core/algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     chunks: dict
         The chunks choice for running in parallel with dask,
         e.g. `{"state": 1000}` for chunks of 1000 states
     verbosity: int
         The verbosity level, 0 means silent
     dbook: foxes.DataBook
         The data book, or None for default
-    keep_models: list of str
+    keep_models: set of str
         Keep these models data in memory and do not finalize them
-    
+
     :group: core
 
     """
 
-    def __init__(self, mbook, farm, chunks, verbosity, dbook=None, keep_models=[]):
+    def __init__(self, mbook, farm, chunks, verbosity, dbook=None, keep_models=set()):
         """
         Constructor.
 
         Parameters
         ----------
         mbook: foxes.models.ModelBook
             The model book
@@ -52,15 +52,15 @@
         chunks: dict
             The chunks choice for running in parallel with dask,
             e.g. `{"state": 1000}` for chunks of 1000 states
         verbosity: int
             The verbosity level, 0 means silent
         dbook: foxes.DataBook, optional
             The data book, or None for default
-        keep_models: list of str
+        keep_models: set of str
             Keep these models data in memory and do not finalize them
 
         """
         super().__init__()
 
         self.name = type(self).__name__
         self.mbook = mbook
@@ -69,20 +69,31 @@
         self.verbosity = verbosity
         self.n_states = None
         self.n_turbines = farm.n_turbines
         self.dbook = StaticData() if dbook is None else dbook
         self.keep_models = keep_models
 
         self._idata_mem = Dict()
+        self._idata_cl = Dict()
 
-    def print(self, *args, **kwargs):
+    def print(self, *args, vlim=1, **kwargs):
         """
         Print function, based on verbosity.
+
+        Parameters
+        ----------
+        args: tuple, optional
+            Arguments for the print function
+        kwargs: dict, optional
+            Keyword arguments for the print function
+        vlim: int
+            The verbosity limit
+
         """
-        if self.verbosity > 0:
+        if self.verbosity >= vlim:
             print(*args, **kwargs)
 
     def __get_sizes(self, idata, mtype):
         """
         Private helper function
         """
 
@@ -157,14 +168,21 @@
                     f"Dimension '{FC.RPOINT}' cannot be chunked, got chunks {self.chunks}"
                 )
             xrdata = xrdata.chunk(
                 chunks={c: v for c, v in self.chunks.items() if c in sizes}
             )
         return xrdata
 
+    def chunked(self, ds):
+        return (
+            ds.chunk(chunks={c: v for c, v in self.chunks.items() if c in ds.coords})
+            if self.chunks is not None
+            else ds
+        )
+
     def initialize(self):
         """
         Initializes the algorithm.
         """
         self._idata_mem[self.name] = super().initialize(self, self.verbosity)
 
     def update_idata(self, models, idata=None, verbosity=None):
@@ -202,14 +220,16 @@
                         f"Model '{m.name}' initialized but not found in idata memory"
                     )
 
             else:
                 self.print(f"Initializing model '{m.name}'")
                 hidata = m.initialize(self, verbosity)
                 self._idata_mem[m.name] = hidata
+                if m.name != self.name and m.name not in self.keep_models:
+                    self._idata_cl[m.name] = m
 
                 pr = False
                 if isinstance(m, FarmController):
                     if verbosity > 1:
                         print(f"-- {m.name}: Starting sub-model initialization -- ")
                         pr = True
                     self.update_idata(m.pre_rotor_models, idata, verbosity)
@@ -226,14 +246,25 @@
             if idata is not None:
                 idata["coords"].update(hidata["coords"])
                 idata["data_vars"].update(hidata["data_vars"])
 
             if pr:
                 print(f"-- {m.name}: Finished sub-model initialization -- ")
 
+    def cleanup(self):
+        """
+        Cleanup after calculation
+        """
+        mnames = list(self._idata_cl.keys())
+        for mname in mnames:
+            m = self._idata_cl[mname]
+            if m.initialized and mname not in self._idata_mem:
+                self.finalize_model(m, self.verbosity)
+                del self._idata_cl[mname]
+
     @property
     def idata_mem(self):
         """
         The current idata memory
 
         Returns
         -------
@@ -317,18 +348,18 @@
 
         """
         if idata is None:
             if not self.initialized:
                 raise ValueError(
                     f"Algorithm '{self.name}': get_models_data called before initialization"
                 )
-            idata = self._idata_mem.pop(self.name)
+            idata = self._idata_mem.get(self.name)
             mnames = [mname for mname in self._idata_mem.keys() if mname[:2] != "__"]
             for mname in mnames:
-                if mname in self.keep_models:
+                if mname in self.keep_models or mname == self.name:
                     hidata = self._idata_mem.get(mname)
                 else:
                     hidata = self._idata_mem.pop(mname)
                 idata["coords"].update(hidata["coords"])
                 idata["data_vars"].update(hidata["data_vars"])
 
         sizes = self.__get_sizes(idata, "models")
@@ -361,15 +392,15 @@
             len(points.shape) != 3
             or points.shape[0] != self.n_states
             or points.shape[2] != 3
         ):
             raise ValueError(
                 f"points have wrong dimensions, expecting ({self.n_states}, n_points, 3), got {points.shape}"
             )
-        idata["data_vars"][FC.POINTS] = ((FC.STATE, FC.POINT, FV.XYH), points)
+        idata["data_vars"][FC.POINTS] = ((FC.STATE, FC.POINT, FC.XYH), points)
 
         sizes = self.__get_sizes(idata, "point")
         return self.__get_xrdata(idata, sizes)
 
     def finalize_model(self, model, verbosity=None):
         """
         Call the finalization routine of the model,
```

### Comparing `foxes-0.4.0/foxes/core/data_calc_model.py` & `foxes-0.4.1/foxes/core/data_calc_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dask.distributed import progress
 from dask.diagnostics import ProgressBar
 
 from .model import Model
 from .data import Data
 from foxes.utils.runners import DaskRunner
 import foxes.constants as FC
+import foxes.variables as FV
 
 
 class DataCalcModel(Model):
     """
     Abstract base class for models with
     that run calculation on xarray Dataset
     data.
@@ -63,28 +64,33 @@
         evars,
         edims,
         edata,
         loop_dims,
         out_vars,
         out_dims,
         calc_pars,
+        init_vars,
     ):
         """
         Wrapper that mitigates between apply_ufunc and `calculate`.
         """
 
+        n_prev = len(init_vars)
+        if n_prev:
+            prev = ldata[:n_prev]
+            ldata = ldata[n_prev:]
+
         # reconstruct original data:
         data = []
         for hvars in dvars:
             v2l = {v: lvars.index(v) for v in hvars if v in lvars}
             v2e = {v: evars.index(v) for v in hvars if v in evars}
 
             hdata = {v: ldata[v2l[v]] if v in v2l else edata[v2e[v]] for v in hvars}
             hdims = {v: ldims[v2l[v]] if v in v2l else edims[v2e[v]] for v in hvars}
-
             data.append(Data(hdata, hdims, loop_dims))
 
             del hdata, hdims, v2l, v2e
 
         # deduce output shape:
         oshape = []
         for li, l in enumerate(out_dims):
@@ -95,25 +101,47 @@
             if len(oshape) != li + 1:
                 raise ValueError(f"Model '{self.name}': Failed to find loop dimension")
 
         # add zero output data arrays:
         odims = {v: out_dims for v in out_vars}
         odata = {
             v: np.full(oshape, np.nan, dtype=FC.DTYPE)
+            if v not in init_vars
+            else prev[init_vars.index(v)].copy()
             for v in out_vars
             if v not in data[-1]
         }
+        if (
+            n_prev
+            and FV.TXYH not in odata
+            and FV.X in odata
+            and FV.X in odata
+            and FV.Y in odata
+            and FV.H in odata
+        ):
+            txyh = np.zeros((data[0].n_states, data[0].n_turbines, 3), dtype=FC.DTYPE)
+            txyh[..., 0] = odata[FV.X]
+            txyh[..., 1] = odata[FV.Y]
+            txyh[..., 2] = odata[FV.H]
+            odata[FV.TXYH] = txyh
+            odims[FV.TXYH] = (FC.STATE, FC.TURBINE, FC.XYH)
+            del txyh
         if len(data) == 1:
             data.append(Data(odata, odims, loop_dims))
         else:
             odata.update(data[-1])
             odims.update(data[-1].dims)
             data[-1] = Data(odata, odims, loop_dims)
         del odims, odata
 
+        # link chunk state indices from mdata to fdata and pdata:
+        if FC.STATE in data[0]:
+            for d in data[1:]:
+                d[FC.STATE] = data[0][FC.STATE]
+
         # run model calculation:
         results = self.calculate(algo, *data, **calc_pars)
 
         # replace missing results by first input data with matching shape:
         missing = set(out_vars).difference(results.keys())
         if len(missing):
             found = set()
@@ -135,15 +163,22 @@
         data = np.zeros(oshape + [n_vars], dtype=FC.DTYPE)
         for v in out_vars:
             data[..., out_vars.index(v)] = results[v]
 
         return data
 
     def run_calculation(
-        self, algo, *data, out_vars, loop_dims, out_core_vars, **calc_pars
+        self,
+        algo,
+        *data,
+        out_vars,
+        loop_dims,
+        out_core_vars,
+        initial_results=None,
+        **calc_pars,
     ):
         """
         Starts the model calculation in parallel, via
         xarray's `apply_ufunc`.
 
         Typically this function is called by algorithms.
 
@@ -159,14 +194,16 @@
             List of the loop dimensions during xarray's
             `apply_ufunc` calculations
         out_core_vars: list of str
             The core dimensions of the output data, use
             `FC.VARS` for variables dimension (required)
         calc_pars: dict, optional
             Additional arguments for the `calculate` function
+        initial_results: xarray.Dataset, optional
+            Initial results
 
         Returns
         -------
         results: xarray.Dataset
             The calculation results
 
         """
@@ -183,14 +220,23 @@
         ldata = []
         lvars = []
         ldims = []
         edata = []
         evars = []
         edims = []
         dvars = []
+        ivars = []
+        idims = []
+        if initial_results is not None:
+            ds = initial_results
+            hvarsl = [v for v, d in ds.items() if len(loopd.intersection(d.dims))]
+            ldata += [ds[v] for v in hvarsl]
+            idims += [ds[v].dims for v in hvarsl]
+            ivars += hvarsl
+
         for ds in data:
             hvarsl = [v for v, d in ds.items() if len(loopd.intersection(d.dims))]
             ldata += [ds[v] for v in hvarsl]
             ldims += [ds[v].dims for v in hvarsl]
             lvars += hvarsl
 
             hvarse = [v for v in ds.keys() if v not in hvarsl]
@@ -229,22 +275,24 @@
             evars=evars,
             edims=edims,
             edata=edata,
             loop_dims=loop_dims,
             out_vars=out_vars,
             out_dims=out_dims,
             calc_pars=calc_pars,
+            init_vars=ivars,
         )
 
         # run parallel computation:
+        iidims = [[c for c in d if c not in loopd] for d in idims]
         icdims = [[c for c in d if c not in loopd] for d in ldims]
         results = xr.apply_ufunc(
             self._wrap_calc,
             *ldata,
-            input_core_dims=icdims,
+            input_core_dims=iidims + icdims,
             output_core_dims=[out_core_vars],
             output_dtypes=[FC.DTYPE],
             dask="parallelized",
             dask_gufunc_kwargs=dargs,
             kwargs=wargs,
         )
```

### Comparing `foxes-0.4.0/foxes/core/farm_controller.py` & `foxes-0.4.1/foxes/core/farm_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 
 from .farm_data_model import FarmDataModelList, FarmDataModel
 from .turbine_model import TurbineModel
 from .turbine_type import TurbineType
 import foxes.constants as FC
 
+
 class FarmController(FarmDataModel):
     """
     Analyses selected turbine models and handles their call.
 
     Attributes
     ----------
     turbine_types: list of foxes.core.TurbineType
@@ -23,21 +24,21 @@
     post_rotor_models: foxes.core.FarmDataModelList
         The turbine models without pre-rotor flag
     pars: dict
         Parameters for the turbine models, stored
         under their respecitve name
 
     :group: core
-    
+
     """
 
     def __init__(self, pars={}):
         """
         Constructor.
-        
+
         Parameters
         ----------
         pars: dict
             Parameters for the turbine models, stored
             under their respective name
 
         """
@@ -47,14 +48,29 @@
         self.turbine_model_names = None
         self.turbine_model_sels = None
         self.pre_rotor_models = None
         self.post_rotor_models = None
 
         self.pars = pars
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        super().keep(algo)
+        self.pre_rotor_models.keep(algo)
+        self.post_rotor_models.keep(algo)
+
     def set_pars(self, model_name, init_pars, calc_pars, final_pars):
         """
         Set parameters for a turbine model
 
         Parameters
         ----------
         model_name: str
```

### Comparing `foxes-0.4.0/foxes/core/farm_data_model.py` & `foxes-0.4.1/foxes/core/farm_data_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from abc import abstractmethod
 
 from .data_calc_model import DataCalcModel
 import foxes.constants as FC
 
+
 class FarmDataModel(DataCalcModel):
     """
     Abstract base class for models that modify
     farm data.
 
     Attributes
     ----------
     pre_rotor: bool
         Flag for running this model before
         running the rotor model.
 
     :group: core
-    
+
     """
 
     def __init__(self, pre_rotor=False):
         """
         Constructor.
 
         Parameters
@@ -126,23 +127,23 @@
     `calculate` functions are called together
     under one common call of xarray's `apply_ufunc`.
 
     Attributes
     ----------
     models: list of foxes.core.FarmDataModel
         The model list
-    
+
     :group: core
 
     """
 
     def __init__(self, models=[]):
         """
         Constructor.
-        
+
         Parameters
         ----------
         models: list of foxes.core.FarmDataModel
             The model list
 
         """
         super().__init__()
@@ -156,14 +157,27 @@
         ----------
         model: foxes.core.FarmDataModel
             The model to add
 
         """
         self.models.append(model)
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        algo.keep_models.update([self.name] + [m.name for m in self.models])
+
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
```

### Comparing `foxes-0.4.0/foxes/core/model.py` & `foxes-0.4.1/foxes/opt/core/pop_states.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,46 @@
 import numpy as np
-from abc import ABCMeta
-from itertools import count
 
+from foxes.core import States, Data
+import foxes.constants as FC
+import foxes.variables as FV
 
-class Model(metaclass=ABCMeta):
+
+class PopStates(States):
     """
-    Base class for all models.
+    Helper class for vectorized opt population
+    calculation, via artificial states of length
+    n_pop times n_states.
 
     Attributes
     ----------
-    name: str
-        The model name
-    
-    :group: core
+    states: foxes.core.States
+        The original states
+    n_pop: int
+        The population size
 
-    """
+    :group: opt.core
 
-    _ids = {}
+    """
 
-    def __init__(self):
+    def __init__(self, states, n_pop):
         """
         Constructor.
-        """
-        t = type(self).__name__
-        if t not in self._ids:
-            self._ids[t] = count(0)
-        self._id = next(self._ids[t])
-
-        ext = "" if self._id == 0 else f"{self._id}"
-        self.name = f"{type(self).__name__}{ext}"
-
-        self.__initialized = False
-
-    def __repr__(self):
-        t = type(self).__name__
-        return f"{self.name} ({t})"
-
-    @property
-    def model_id(self):
-        """
-        Unique id based on the model type.
-
-        Returns
-        -------
-        int
-            Unique id of the model object
-
-        """
-        return self._id
-
-    def var(self, v):
-        """
-        Creates a model specific variable name.
 
         Parameters
         ----------
-        v: str
-            The variable name
-
-        Returns
-        -------
-        str
-            Model specific variable name
-
-        """
-        return f"{self.name}_{v}"
+        states: foxes.core.States
+            The original states
+        n_pop: int
+            The population size
 
-    @property
-    def initialized(self):
         """
-        Initialization flag.
-
-        Returns
-        -------
-        bool :
-            True if the model has been initialized.
-
-        """
-        return self.__initialized
+        super().__init__()
+        self.states = states
+        self.n_pop = n_pop
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -100,112 +59,142 @@
         -------
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
-        if self.initialized:
-            raise ValueError(
-                f"Model '{self.name}': initialize called for already initialized object"
+        self.STATE0 = self.var(FC.STATE + "0")
+        self.SMAP = self.var("SMAP")
+
+        idata = super().initialize(algo, verbosity)
+        self._update_idata(algo, idata)
+
+        if not self.states.name in algo._idata_mem:
+            raise KeyError(
+                f"States idata '{self.states.name}' not found in algo idata memory"
             )
-        self.__initialized = True
-        return {"coords": {}, "data_vars": {}}
+        else:
+            idata0 = algo._idata_mem[self.states.name]
+
+        for cname, coord in idata0["coords"].items():
+            if cname != FC.STATE:
+                idata["coords"][cname] = coord
+            else:
+                idata["coords"][self.STATE0] = coord
+
+        for dname, (dims0, data0) in idata0["data_vars"].items():
+            if dname != FV.WEIGHT:
+                hdims = tuple([d if d != FC.STATE else self.STATE0 for d in dims0])
+                idata["data_vars"][dname] = (hdims, data0)
+
+        smap = np.zeros((self.n_pop, self.states.size()), dtype=np.int32)
+        smap[:] = np.arange(self.states.size())[None, :]
+        smap = smap.reshape(self.size())
+        idata["data_vars"][self.SMAP] = ((FC.STATE,), smap)
+
+        found = False
+        for dname, (dims0, data0) in idata["data_vars"].items():
+            if self.STATE0 in dims0:
+                found = True
+                break
+        if not found:
+            del idata["coords"][self.STATE0]
+
+        return idata
+
+    def size(self):
+        """
+        The total number of states.
 
-    def finalize(self, algo, verbosity=0):
+        Returns
+        -------
+        int:
+            The total number of states
+
+        """
+        return self.states.size() * self.n_pop
+
+    def weights(self, algo):
         """
-        Finalizes the model.
+        The statistical weights of all states.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
+
+        Returns
+        -------
+        weights: numpy.ndarray
+            The weights, shape: (n_states, n_turbines)
 
         """
-        if not self.initialized:
-            raise ValueError(
-                f"Model '{self.name}': Finalization called for uninitialized object"
-            )
-        self.__initialized = False
+        weights = np.zeros(
+            (self.n_pop, self.states.size(), algo.n_turbines), dtype=FC.DTYPE
+        )
+        weights[:] = self.states.weights(algo)[None, :, :] / self.n_pop
+        return weights.reshape(self.size(), algo.n_turbines)
 
-    def get_data(
-        self,
-        variable,
-        data,
-        st_sel=None,
-        upcast=None,
-        data_prio=False,
-        accept_none=False,
-    ):
+    def output_point_vars(self, algo):
         """
-        Getter for a data entry in either the given
-        data source, or the model object.
+        The variables which are being modified by the model.
 
         Parameters
         ----------
-        variable: str
-            The variable, serves as data key
-        data: dict
-            The data source
-        st_sel: numpy.ndarray of bool, optional
-            If given, get the specified state-turbine subset
-        upcast: str, optional
-            Either 'farm' or 'points', broadcasts potential
-            scalar data to numpy.ndarray with dimensions
-            (n_states, n_turbines) or (n_states, n_points),
-            respectively
-        data_prio: bool
-            First search the data source, then the object
-        accept_none: bool
-            Do not throw an error if data entry is None or np.nan
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        output_vars: list of str
+            The output variable names
 
         """
+        return self.states.output_point_vars(algo)
 
-        sources = ("data", "self") if data_prio else ("self", "data")
-
-        out = None
-        for s in sources:
-            if s == "self":
-                try:
-                    out = getattr(self, variable)
-                except AttributeError:
-                    pass
-            else:
-                try:
-                    out = data[variable]
-                except KeyError:
-                    pass
-            if out is not None:
-                break
+    def calculate(self, algo, mdata, fdata, pdata):
+        """ "
+        The main model calculation.
 
-        if out is None:
-            raise KeyError(
-                f"Model '{self.name}': Variable '{variable}' neither found in data {sorted(list(data.keys()))} nor among attributes"
-            )
+        This function is executed on a single chunk of data,
+        all computations should be based on numpy arrays.
 
-        if upcast is not None and not isinstance(out, np.ndarray):
-            if upcast == "farm":
-                out = np.full((data.n_states, data.n_turbines), out)
-            elif upcast == "points":
-                out = np.full((data.n_states, data.n_points), out)
-            else:
-                raise ValueError(
-                    f"Model '{self.name}': Illegal upcast '{upcast}', select 'farm' or 'points'"
-                )
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        pdata: foxes.core.Data
+            The point data
 
-        if st_sel is not None:
-            try:
-                out = out[st_sel]
-            except TypeError:
-                pass
+        Returns
+        -------
+        results: dict
+            The resulting data, keys: output variable str.
+            Values: numpy.ndarray with shape (n_states, n_points)
+
+        """
 
-        if not accept_none:
-            try:
-                if np.all(np.isnan(np.atleast_1d(out))):
-                    raise ValueError(
-                        f"Model '{self.name}': Variable '{variable}' requested but not provided."
-                    )
-            except TypeError:
+        hdata = {}
+        hdims = {}
+        smap = mdata[self.SMAP]
+        for dname, data in mdata.items():
+            dms = mdata.dims[dname]
+            if dname == self.SMAP or dname == self.STATE0:
                 pass
-        return out
+            elif dms[0] == self.STATE0:
+                hdata[dname] = data[smap]
+                hdims[dname] = tuple([FC.STATE] + list(dms)[1:])
+            elif self.STATE0 in dms:
+                raise ValueError(
+                    f"States '{self.name}': Found states variable not at dimension 0 for mdata entry '{dname}': {dms}"
+                )
+            else:
+                hdata[dname] = data
+                hdims[dname] = dms
+        hmdata = Data(hdata, hdims, mdata.loop_dims)
+
+        return self.states.calculate(algo, hmdata, fdata, pdata)
```

### Comparing `foxes-0.4.0/foxes/core/partial_wakes_model.py` & `foxes-0.4.1/foxes/core/partial_wakes_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
     Attributes
     ----------
     wake_models: list of foxes.core.WakeModel
         The wake model selection
     wake_frame: foxes.core.WakeFrame, optional
         The wake frame
-    
+
     :group: core
 
     """
 
     def __init__(self, wake_models=None, wake_frame=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         wake_models: list of foxes.core.WakeModel
             The wake model selection, None for all
             from algorithm.
         wake_frame: foxes.core.WakeFrame, optional
             The wake frame, None takes from algorithm
@@ -69,14 +69,30 @@
         self.wake_frame = algo.wake_frame if self._wframe is None else self._wframe
 
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self.wake_models, idata=idata, verbosity=verbosity)
 
         return idata
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        super().keep(algo)
+        for w in self.wake_models:
+            w.keep(algo)
+        self.wake_frame.keep(algo)
+
     @abstractmethod
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
@@ -88,71 +104,91 @@
         fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
         wake_deltas: dict
             Keys: Variable name str, values: any
+        pdata: foxes.core.Data
+            The evaluation point data
 
         """
         pass
 
     @abstractmethod
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         pass
 
     @abstractmethod
     def evaluate_results(
-        self, algo, mdata, fdata, wake_deltas, states_turbine, update_amb_res=False
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        wake_deltas,
+        states_turbine,
+        amb_res=None,
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
         states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res: bool
-            Flag for updating ambient results
+        amb_res: dict, optional
+            Ambient states results. Keys: var str, values:
+            numpy.ndarray of shape (n_states, n_points)
 
         """
         pass
 
     @classmethod
     def new(cls, pwake_type, **kwargs):
         """
```

### Comparing `foxes-0.4.0/foxes/core/point_data_model.py` & `foxes-0.4.1/foxes/core/point_data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import abstractmethod
 
 from .data_calc_model import DataCalcModel
 import foxes.constants as FC
 
+
 class PointDataModel(DataCalcModel):
     """
     Abstract base class for models that modify
     point based data.
 
     :group: core
-    
+
     """
 
     @abstractmethod
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
@@ -111,15 +112,15 @@
     :group: core
 
     """
 
     def __init__(self, models=[]):
         """
         Constructor.
-        
+
         Parameters
         ----------
         models: list of foxes.core.PointDataModel
             The model list
 
         """
         super().__init__()
@@ -133,14 +134,27 @@
         ----------
         model: foxes.core.PointDataModel
             The model to add
 
         """
         self.models.append(model)
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        algo.keep_models.update([self.name] + [m.name for m in self.models])
+
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
```

### Comparing `foxes-0.4.0/foxes/core/rotor_model.py` & `foxes-0.4.1/foxes/core/rotor_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import foxes.variables as FV
 import foxes.constants as FC
 from .farm_data_model import FarmDataModel
 from .data import Data
 from foxes.utils import wd2uv, uv2wd
 
+
 class RotorModel(FarmDataModel):
     """
     Abstract base class of rotor models.
 
     Rotor models calculate ambient farm data from
     states, and provide rotor points and weights
     for the calculation of rotor effective quantities.
@@ -24,15 +25,15 @@
     :group: core
 
     """
 
     def __init__(self, calc_vars):
         """
         Constructor.
-        
+
         Parameters
         ----------
         calc_vars: list of str
             The variables that are calculated by the model
             (Their ambients are added automatically)
 
         """
@@ -50,17 +51,20 @@
 
         Returns
         -------
         output_vars: list of str
             The output variable names
 
         """
-        return self.calc_vars + [
-            FV.var2amb[v] for v in self.calc_vars if v in FV.var2amb
-        ]
+        return list(
+            set(
+                self.calc_vars
+                + [FV.var2amb[v] for v in self.calc_vars if v in FV.var2amb]
+            )
+        )
 
     @abstractmethod
     def n_rotor_points(self):
         """
         The number of rotor points
 
         Returns
@@ -223,17 +227,14 @@
             ws = rpoint_results[FV.WS]
             uvp = wd2uv(wd, ws, axis=-1)
             uv = np.einsum("stpd,p->std", uvp, weights)
 
         wd = None
         vdone = []
         for v in self.calc_vars:
-            if v not in fdata:
-                fdata[v] = np.zeros((n_states, n_turbines), dtype=FC.DTYPE)
-
             if v == FV.WD or v == FV.YAW:
                 if wd is None:
                     wd = uv2wd(uv, axis=-1)
                 self._set_res(fdata, v, wd, stsel)
                 vdone.append(v)
 
             elif v == FV.WS:
@@ -354,35 +355,37 @@
             results dict. Keys: Variable name str. Values:
             numpy.ndarray with results, shape: (n_states, n_turbines)
 
         """
 
         if rpoints is None:
             rpoints = mdata.get(FC.RPOINTS, self.get_rotor_points(algo, mdata, fdata))
+        if store_rpoints:
+            mdata[FC.RPOINTS] = rpoints
+            mdata.dims[FC.RPOINTS] = (FC.STATE, FC.TURBINE, FC.RPOINT, FC.XYH)
+            self.data_to_store(FC.RPOINTS, algo, mdata)
+
         if states_turbine is not None:
             n_states = mdata.n_states
             stsel = (np.arange(n_states), states_turbine)
             rpoints = rpoints[stsel][:, None]
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         n_points = n_turbines * n_rpoints
 
         if weights is None:
             weights = mdata.get(FC.RWEIGHTS, self.rotor_point_weights())
-
-        if store_rpoints:
-            mdata[FC.RPOINTS] = rpoints
-            mdata.dims[FC.RPOINTS] = (FC.STATE, FC.TURBINE, FC.RPOINT, FV.XYH)
         if store_rweights:
             mdata[FC.RWEIGHTS] = weights
             mdata.dims[FC.RWEIGHTS] = (FC.RPOINT,)
+            self.data_to_store(FC.RWEIGHTS, algo, mdata)
 
         svars = algo.states.output_point_vars(algo)
         points = rpoints.reshape(n_states, n_points, 3)
         pdata = {FC.POINTS: points}
-        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
+        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
         pdata.update(
             {v: np.full((n_states, n_points), np.nan, dtype=FC.DTYPE) for v in svars}
         )
         pdims.update({v: (FC.STATE, FC.POINT) for v in svars})
         pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         del pdims, points
 
@@ -392,14 +395,15 @@
 
         rpoint_results = {}
         for v in svars:
             rpoint_results[v] = pdata[v].reshape(n_states, n_turbines, n_rpoints)
 
         if store_amb_res:
             mdata[FC.AMB_RPOINT_RESULTS] = rpoint_results
+            self.data_to_store(FC.AMB_RPOINT_RESULTS, algo, mdata)
 
         self.eval_rpoint_results(
             algo,
             mdata,
             fdata,
             rpoint_results,
             weights,
```

### Comparing `foxes-0.4.0/foxes/core/states.py` & `foxes-0.4.1/foxes/core/states.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
 
 from .point_data_model import PointDataModel, PointDataModelList
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class States(PointDataModel):
     """
     Abstract base class for states.
 
     States describe ambient meteorological data,
     typically wind speed, wind direction, turbulence
     intensity and air density.
@@ -129,23 +130,23 @@
 
     Attributes
     ----------
     states: foxes.core.States
         The base states to start from
     pmodels: foxes.core.PointDataModelList
         The point models, including states as first model
-    
+
     :group: core
 
     """
 
     def __init__(self, states, point_models=[]):
         """
         Constructor.
-        
+
         Parameters
         ----------
         states: foxes.core.States
             The base states to start from
         point_models: list of foxes.core.PointDataModel, optional
             The point models, executed after states
```

### Comparing `foxes-0.4.0/foxes/core/turbine.py` & `foxes-0.4.1/foxes/core/turbine.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         The rotor diameter. Overwrites turbine type
         settings if given
     H: float, optional
         The hub height. Overwrites turbine type
         settings if given
 
     :group: foxes
-    
+
     """
 
     def __init__(
         self,
         xy,
         turbine_models=[],
         index=None,
```

### Comparing `foxes-0.4.0/foxes/core/turbine_model.py` & `foxes-0.4.1/foxes/core/turbine_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/core/turbine_type.py` & `foxes-0.4.1/foxes/core/turbine_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :group: core
 
     """
 
     def __init__(self, name=None, D=None, H=None, P_nominal=None, P_unit="kW"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         name: str, optional
             The model name
         D: float, optional
             The rotor diameter
         H: float, optional
```

### Comparing `foxes-0.4.0/foxes/core/vertical_profile.py` & `foxes-0.4.1/foxes/core/vertical_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class VerticalProfile(Model):
     """
     Abstract base class for vertical profiles.
 
     :group: core
-    
+
     """
 
     @abstractmethod
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
```

### Comparing `foxes-0.4.0/foxes/core/wake_frame.py` & `foxes-0.4.1/foxes/core/wake_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from scipy.interpolate import interpn
 
 from .data import Data
 from .model import Model
 import foxes.constants as FC
 import foxes.variables as FV
 
+
 class WakeFrame(Model):
     """
     Abstract base class for wake frames.
 
     Wake frames translate global coordinates into
     wake frame coordinates, which are then evaluated
     by wake models.
@@ -44,31 +45,31 @@
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         pass
 
     @abstractmethod
-    def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
+    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points: numpy.ndarray
-            The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
             points, shape: (n_states, n_points, 3)
 
@@ -162,15 +163,15 @@
         xpts[:] = xs[None, 1:]
         pts = self.get_centreline_points(
             algo, mdata, fdata, states_source_turbine, xpts
         )
 
         # run ambient calculation:
         pdata = {FC.POINTS: pts}
-        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
+        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
         pdata.update(
             {v: np.full((n_states, n_steps), np.nan, dtype=FC.DTYPE) for v in vrs}
         )
         pdims.update({v: (FC.STATE, FC.POINT) for v in vrs})
         pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         res = algo.states.calculate(algo, mdata, fdata, pdata)
         pdata.update(res)
```

### Comparing `foxes-0.4.0/foxes/core/wake_model.py` & `foxes-0.4.1/foxes/models/wake_models/gaussian.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,108 @@
+import numpy as np
 from abc import abstractmethod
 
-from .model import Model
+from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
 
 
-class WakeModel(Model):
+class GaussianWakeModel(AxisymmetricWakeModel):
     """
-    Abstract base class for wake models.
+    Abstract base class for Gaussian wake models.
 
-    :group: core
-    
-    """
-
-    @abstractmethod
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
-        """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        n_points: int
-            The number of wake evaluation points
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+    :group: models.wake_models
 
-        """
-        pass
+    """
 
     @abstractmethod
-    def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_coos, wake_deltas
+    def calc_amplitude_sigma_spsel(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
     ):
         """
-        Calculate the contribution to the wake deltas
-        by this wake model.
-
-        Modifies wake_deltas on the fly.
+        Calculate the amplitude and the sigma,
+        both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        wake_coos: numpy.ndarray
-            The wake frame coordinates of the evaluation
-            points, shape: (n_states, n_points, 3)
-        wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_points)
+
+        Returns
+        -------
+        amsi: tuple
+            The amplitude and sigma, both numpy.ndarray
+            with shape (n_sp_sel,)
+        sp_sel: numpy.ndarray of bool
+            The state-point selection, for which the wake
+            is non-zero, shape: (n_states, n_points)
 
         """
         pass
 
-    def finalize_wake_deltas(self, algo, mdata, fdata, amb_results, wake_deltas):
+    def calc_wakes_spsel_x_r(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        r,
+    ):
         """
-        Finalize the wake calculation.
-
-        Modifies wake_deltas on the fly.
+        Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        amb_results: dict
-            The ambient results, key: variable name str,
-            values: numpy.ndarray with shape (n_states, n_points)
-        wake_deltas: dict
-            The wake deltas, are being modified ob the fly.
-            Key: Variable name str, for which the wake delta
-            applies, values: numpy.ndarray with shape
-            (n_states, n_points, ...) before evaluation,
-            numpy.ndarray with shape (n_states, n_points) afterwards
+        pdata: foxes.core.Data
+            The evaluation point data
+        states_source_turbine: numpy.ndarray
+            For each state, one turbine index for the
+            wake causing turbine. Shape: (n_states,)
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_points)
+        r: numpy.ndarray
+            The radial values for each x value, shape:
+            (n_states, n_points, n_r_per_x, 2)
+
+        Returns
+        -------
+        wdeltas: dict
+            The wake deltas. Key: variable name str,
+            value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
+        sp_sel: numpy.ndarray of bool
+            The state-point selection, for which the wake
+            is non-zero, shape: (n_states, n_points)
+
+        """
+        amsi, sp_sel = self.calc_amplitude_sigma_spsel(
+            algo, mdata, fdata, pdata, states_source_turbine, x
+        )
+        wdeltas = {}
+        rsel = r[sp_sel]
+        for v in amsi.keys():
+            ampld, sigma = amsi[v]
+            wdeltas[v] = ampld[:, None] * np.exp(-0.5 * (rsel / sigma[:, None]) ** 2)
 
-        """
-        pass
+        return wdeltas, sp_sel
```

### Comparing `foxes-0.4.0/foxes/core/wake_superposition.py` & `foxes-0.4.1/foxes/core/wake_superposition.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
     Note that it is a matter of the wake model
     if superposition models are used, or if the
     wake model computes the total wake result by
     other means.
 
     :group: core
-    
+
     """
 
     @abstractmethod
     def calc_wakes_plus_wake(
         self,
         algo,
         mdata,
         fdata,
+        pdata,
         states_source_turbine,
         sel_sp,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
@@ -35,14 +36,16 @@
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
         variable: str
             The variable name for which the wake deltas applies
@@ -58,28 +61,37 @@
             The updated wake deltas, shape: (n_states, n_points)
 
         """
         pass
 
     @abstractmethod
     def calc_final_wake_delta(
-        self, algo, mdata, fdata, variable, amb_results, wake_delta
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
         wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
```

### Comparing `foxes-0.4.0/foxes/core/wind_farm.py` & `foxes-0.4.1/foxes/core/wind_farm.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ----------
     name: str
         The wind farm name
     turbines: list of foxes.core.Turbine
         The wind turbines
     boundary: foxes.utils.geom2d.AreaGeometry, optional
         The wind farm boundary
-    
+
     :group: foxes
 
     """
 
     def __init__(self, name="wind_farm", boundary=None):
         """
         Constructor.
```

### Comparing `foxes-0.4.0/foxes/data/farms/test_farm_67.csv` & `foxes-0.4.1/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/parse.py` & `foxes-0.4.1/foxes/data/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     file_name: str or pathlib.Path
         Path to the file
 
     Returns
     -------
     parsed_data: dict
         dict with data parsed from file name
-    
+
     :group: foxes
 
     """
     sname = Path(file_name).stem
     pars = {"name": sname.split(".")[0]}
 
     i = sname.find(".")
@@ -80,15 +80,15 @@
     file_name_B: str or pathlib.Path
         Path to the second file
 
     Returns
     -------
     parsed_data: dict
         dict with data parsed from file name
-    
+
     :group: foxes
 
     """
     pars_A = parse_Pct_file_name(file_name_A)
     pars_B = parse_Pct_file_name(file_name_B)
     name = pars_A["name"]
     name_ct = pars_B["name"]
```

### Comparing `foxes-0.4.0/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.4.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.4.1/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.4.1/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.4.1/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.4.1/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.4.1/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/states/wind_rotation.nc` & `foxes-0.4.1/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/data/static_data.py` & `foxes-0.4.1/foxes/data/static_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class StaticData(DataBook):
     """
     A DataBook filled with static data from
     this directory.
 
     :group: foxes
-    
+
     """
 
     def __init__(self):
         super().__init__()
 
         self.add_data_package(FARM, farms, ".csv")
         self.add_data_package(STATES, states, [".csv", ".csv.gz", ".nc"])
```

### Comparing `foxes-0.4.0/foxes/input/farm_layout/from_csv.py` & `foxes-0.4.1/foxes/input/farm_layout/from_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         index
     turbine_base_name_count_shift: bool, optional
         Start turbine names by 1 instead of 0
     verbosity: int
         The verbosity level, 0 = silent
     turbine_parameters: dict, optional
         Additional parameters are forwarded to the WindFarm.add_turbine().
-    
+
     :group: input.farm_layout
 
     """
 
     if isinstance(data_source, pd.DataFrame):
         data = data_source
     else:
```

### Comparing `foxes-0.4.0/foxes/input/farm_layout/from_df.py` & `foxes-0.4.1/foxes/input/farm_layout/from_df.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,12 +16,12 @@
         The wind farm
     data_source: str or pandas.DataFrame
         The input csv file or data source
     args: tuple, optional
         Additional parameters for add_from_csv()
     kwargs: dict, optional
         Additional parameters for add_from_csv()
-    
+
     :group: input.farm_layout
 
     """
     add_from_csv(farm, data_source, *args, **kwargs)
```

### Comparing `foxes-0.4.0/foxes/input/farm_layout/from_file.py` & `foxes-0.4.1/foxes/input/farm_layout/from_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/input/farm_layout/from_json.py` & `foxes-0.4.1/foxes/input/farm_layout/from_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Path to the file
     set_farm_name: bool
         Flag for inferring wind farm name from data
     verbosity: int
         The verbosity level, 0 = silent
     turbine_parameters: dict, optional
         Parameters forwarded to `foxes.core.Turbine`
-    
+
     :group: input.farm_layout
 
     """
 
     if verbosity:
         print("Reading file", file_path)
     with open(file_path) as f:
```

### Comparing `foxes-0.4.0/foxes/input/farm_layout/grid.py` & `foxes-0.4.1/foxes/input/farm_layout/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         The turbine indices
     names: list of str, optional
         The turbine names
     verbosity: int
         The verbosity level, 0 = silent
     turbine_parameters: dict, optional
         Parameters forwarded to `foxes.core.Turbine`
-    
+
     :group: input.farm_layout
 
     """
 
     inds = list(np.ndindex(*steps))
     n_turbines = len(inds)
```

### Comparing `foxes-0.4.0/foxes/input/farm_layout/row.py` & `foxes-0.4.1/foxes/input/farm_layout/row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/input/states/create/random_abl_states.py` & `foxes-0.4.1/foxes/input/states/create/random_abl_states.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     var2col: dict, optional
         Mapping from variables to column names
     mol_abs_range: tuple
         Min and max of allowed MOL values, set to
         nan if exceeded (i.e., neutral stratification)
     normalize: bool
         Normalize weights to 1
-        
+
     Returns
     -------
     data: pandas.DataFrame
         The created states data
 
     :group: input.states
```

### Comparing `foxes-0.4.0/foxes/input/states/field_data_nc.py` & `foxes-0.4.1/foxes/input/states/field_data_nc.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         fill_value=None,
         time_format="%Y-%m-%d_%H:%M:%S",
         sel=None,
         verbosity=1,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or xarray.Dataset
             The data or the file search pattern, should end with
             suffix '.nc'. One or many files.
         output_vars: list of str
             The output variables
```

### Comparing `foxes-0.4.0/foxes/input/states/multi_height.py` & `foxes-0.4.1/foxes/input/states/multi_height.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         pandas file reading parameters
     states_sel: slice or range or list of int
         States subset selection
     states_loc: list
         State index selection via pandas loc function
     RDICT: dict
         Default pandas file reading parameters
-    
+
     :group: input.states
 
     """
 
     RDICT = {"index_col": 0}
 
     def __init__(
@@ -60,15 +60,15 @@
         pd_read_pars={},
         states_sel=None,
         states_loc=None,
         ipars={},
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             Either path to a file or data
         output_vars: list of str
             The output variables
         heights: list of float
@@ -410,8 +410,9 @@
 class MultiHeightTimeseries(MultiHeightStates):
     """
     Multi-height timeseries states data.
 
     :group: input.states
 
     """
+
     RDICT = {"index_col": 0, "parse_dates": [0]}
```

### Comparing `foxes-0.4.0/foxes/input/states/scan_ws.py` & `foxes-0.4.1/foxes/input/states/scan_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ----------
     wd: float
         The wind direction
     ti: float
         The TI value
     rho: float
         The air density
-    
+
     :group: input.states
 
     """
 
     def __init__(self, ws_list, wd, ti=None, rho=None):
         """
         Constructor.
```

### Comparing `foxes-0.4.0/foxes/input/states/single.py` & `foxes-0.4.1/foxes/input/states/single.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     :group: input.states
 
     """
 
     def __init__(self, ws, wd, ti=None, rho=None, profiles={}, **profdata):
         """
         Constructor.
-        
+
         Parameters
         ----------
         ws: float
             The wind speed
         wd: float
             The wind direction
         ti: float, optional
```

### Comparing `foxes-0.4.0/foxes/input/states/states_table.py` & `foxes-0.4.1/foxes/input/states/states_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         pandas file reading parameters
     states_sel: slice or range or list of int
         States subset selection
     states_loc: list
         State index selection via pandas loc function
     RDICT: dict
         Default pandas file reading parameters
-    
+
     :group: input.states
 
     """
 
     RDICT = {"index_col": 0}
 
     def __init__(
@@ -51,15 +51,15 @@
         profiles={},
         pd_read_pars={},
         states_sel=None,
         states_loc=None,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             Either path to a file or data
         output_vars: list of str
             The output variables
         var2col: dict
@@ -347,10 +347,11 @@
 
 
 class Timeseries(StatesTable):
     """
     Timeseries states data.
 
     :group: input.states
-    
+
     """
+
     RDICT = {"index_col": 0, "parse_dates": [0]}
```

### Comparing `foxes-0.4.0/foxes/input/windio/windio.py` & `foxes-0.4.1/foxes/input/windio/windio.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         The model book
     farm: foxes.WindFarm
         The wind farm
     states: foxes.states.States
         The states object
     algo: foxes.core.Algorithm
         The algorithm
-    
+
     :group: input.windio
 
     """
     case_yaml = Path(case_yaml)
 
     with open(case_yaml, "r") as file:
         case = yaml.load(file, Loader=yaml.loader.BaseLoader)
```

### Comparing `foxes-0.4.0/foxes/models/farm_models/turbine2farm.py` & `foxes-0.4.1/foxes/models/farm_models/turbine2farm.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     into farm models, simply by selecting
     all turbines.
 
     Attributes
     ----------
     turbine_model: foxes.core.TurbineModel
         The turbine model
-    
+
     :group: models.farm_models
 
     """
 
     def __init__(self, turbine_model):
         """
         Constructor.
-        
+
         Parameters
         ----------
         turbine_model: foxes.core.TurbineModel
             The turbine model
 
         """
         super().__init__()
```

### Comparing `foxes-0.4.0/foxes/models/model_book.py` & `foxes-0.4.1/foxes/models/model_book.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         The wake superposition models. Keys: model name str,
         values: foxes.core.WakeSuperposition
     wake_models: foxes.utils.Dict
         The wake models. Keys: model name str,
         values: foxes.core.WakeModel
     sources: foxes.utils.Dict
         All sources dict
-    
+
     :group: foxes
 
     """
 
     def __init__(self, Pct_file=None):
         """
         Constructor.
@@ -106,20 +106,22 @@
             kTI_amb_04=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.4),
             kTI_amb_05=fm.turbine_models.kTI(ti_var=FV.AMB_TI, kTI=0.5),
             thrust2ct=fm.turbine_models.Thrust2Ct(),
             PMask=fm.turbine_models.PowerMask(),
             yaw2yawm=fm.turbine_models.YAW2YAWM(),
             yawm2yaw=fm.turbine_models.YAWM2YAW(),
         )
-        self.turbine_models["hubh_data"] = fm.turbine_models.RotorCentreCalc({
-            f"{FV.WD}_HH": FV.WD,
-            f"{FV.WS}_HH": FV.WS,
-            f"{FV.TI}_HH": FV.TI,
-            f"{FV.RHO}_HH": FV.RHO,
-        })
+        self.turbine_models["hubh_data"] = fm.turbine_models.RotorCentreCalc(
+            {
+                f"{FV.WD}_HH": FV.WD,
+                f"{FV.WS}_HH": FV.WS,
+                f"{FV.TI}_HH": FV.TI,
+                f"{FV.RHO}_HH": FV.RHO,
+            }
+        )
 
         self.farm_models = Dict(
             name="farm_models",
             **{
                 f"farm_{mname}": fm.farm_models.Turbine2FarmModel(m)
                 for mname, m in self.turbine_models.items()
             },
@@ -162,14 +164,25 @@
             self.wake_frames[f"streamlines_{int(s)}_yawed"] = fm.wake_frames.YawedWakes(
                 base_frame=fm.wake_frames.Streamlines(step=s)
             )
         for s in stps:
             self.wake_frames[f"streamlines_{int(s)}_farmo"] = fm.wake_frames.FarmOrder(
                 base_frame=fm.wake_frames.Streamlines(step=s)
             )
+        self.wake_frames["timelines"] = fm.wake_frames.Timelines()
+        self.wake_frames["timelines_1s"] = fm.wake_frames.Timelines(dt_min=1 / 60)
+        self.wake_frames["timelines_10s"] = fm.wake_frames.Timelines(dt_min=1 / 6)
+        self.wake_frames["timelines_30s"] = fm.wake_frames.Timelines(dt_min=0.5)
+        self.wake_frames["timelines_1min"] = fm.wake_frames.Timelines(dt_min=1)
+        self.wake_frames["timelines_10min"] = fm.wake_frames.Timelines(dt_min=10)
+        self.wake_frames["timelines_30min"] = fm.wake_frames.Timelines(dt_min=30)
+        self.wake_frames["timelines_60min"] = fm.wake_frames.Timelines(dt_min=60)
+        self.wake_frames["timelines_1km"] = fm.wake_frames.Timelines(
+            max_wake_length=1000.0
+        )
 
         self.wake_superpositions = Dict(
             name="wake_superpositions",
             linear=fm.wake_superpositions.LinearSuperposition(
                 scalings=f"source_turbine_{FV.REWS}"
             ),
             linear_lim=fm.wake_superpositions.LinearSuperposition(
```

### Comparing `foxes-0.4.0/foxes/models/partial_wakes/axiwake.py` & `foxes-0.4.1/foxes/models/partial_wakes/axiwake.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from foxes.core import PartialWakesModel
+from foxes.core import PartialWakesModel, Data
 from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
 from foxes.utils.two_circles import calc_area
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class PartialAxiwake(PartialWakesModel):
@@ -28,15 +28,15 @@
     :group: models.partial_wakes
 
     """
 
     def __init__(self, n, wake_models=None, wake_frame=None, rotor_model=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         n: int
             The number of radial evaluation points
         wake_models: list of foxes.core.WakeModel, optional
             The wake models, default are the ones from the algorithm
         wake_frame: foxes.core.WakeFrame, optional
@@ -89,14 +89,28 @@
             if not isinstance(w, AxisymmetricWakeModel):
                 raise TypeError(
                     f"Partial wakes '{self.name}': Cannot be applied to wake model '{w.name}', since not an AxisymmetricWakeModel"
                 )
 
         return idata
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        super().keep(algo)
+        self.rotor_model.keep(algo)
+
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
@@ -107,38 +121,49 @@
         fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
         wake_deltas: dict
             Keys: Variable name str, values: any
+        pdata: foxes.core.Data
+            The evaluation point data
 
         """
-        n_points = fdata.n_turbines
+        pdata = Data.from_points(points=fdata[FV.TXYH])
+
         wake_deltas = {}
         for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, n_points, wake_deltas)
+            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
 
-        return wake_deltas
+        return wake_deltas, pdata
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
@@ -146,15 +171,15 @@
         # prepare:
         n_states = mdata.n_states
         n_turbines = algo.n_turbines
         D = fdata[FV.D]
 
         # calc coordinates to rotor centres:
         wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, states_source_turbine, fdata[FV.TXYH]
+            algo, mdata, fdata, pdata, states_source_turbine
         )
 
         # prepare x and r coordinates:
         x = wcoos[:, :, 0]
         n = wcoos[:, :, 1:3]
         R = np.linalg.norm(n, axis=-1)
         r = np.zeros((n_states, n_turbines, self.n), dtype=FC.DTYPE)
@@ -184,15 +209,16 @@
             R1[:] = Dsel / 2
             steps = np.linspace(0.0, 1.0, self.n + 1, endpoint=True) - 0.5
             R2 = np.zeros_like(R1)
             R2[:] = Rsel + Dsel * steps[None, :]
             r[sel] = 0.5 * (R2[:, 1:] + R2[:, :-1])
 
             hA = calc_area(R1, R2, Rsel)
-            hA = hA[:, 1:] - hA[:, :-1]
+            hA = hA[:, 1:] - hA[:, :-1] + 1e-15
+
             weights[sel] = hA / np.sum(hA, axis=-1)[:, None]
             del hA, Rsel, Dsel, R1, R2
 
         # case wake centre inside rotor disk:
         sel = (x > 1e-5) & (R < D / 2)
         if np.any(sel):
             n_sel = np.sum(sel)
@@ -218,15 +244,15 @@
             hA = hA[:, 1:] - hA[:, :-1]
             weights[sel] = hA / np.sum(hA, axis=-1)[:, None]
             del hA, hr, Rsel, Dsel, R1, R2
 
         # evaluate wake models:
         for w in self.wake_models:
             wdeltas, sp_sel = w.calc_wakes_spsel_x_r(
-                algo, mdata, fdata, states_source_turbine, x, r
+                algo, mdata, fdata, pdata, states_source_turbine, x, r
             )
 
             for v, wdel in wdeltas.items():
                 d = np.einsum("ps,ps->p", wdel, weights[sp_sel])
 
                 try:
                     superp = w.superp[v]
@@ -235,71 +261,87 @@
                         f"Model '{self.name}': Missing wake superposition entry for variable '{v}' in wake model '{w.name}', found {sorted(list(w.superp.keys()))}"
                     )
 
                 wake_deltas[v] = superp.calc_wakes_plus_wake(
                     algo,
                     mdata,
                     fdata,
+                    pdata,
                     states_source_turbine,
                     sp_sel,
                     v,
                     wake_deltas[v],
                     d,
                 )
 
     def evaluate_results(
-        self, algo, mdata, fdata, wake_deltas, states_turbine, update_amb_res=False
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        wake_deltas,
+        states_turbine,
+        amb_res=None,
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
         states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res: bool
-            Flag for updating ambient results
+        amb_res: dict, optional
+            Ambient states results. Keys: var str, values:
+            numpy.ndarray of shape (n_states, n_points)
 
         """
-        weights = self.get_data(FC.RWEIGHTS, mdata)
-        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FC.RPOINTS, mdata)
+
+        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
+        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
 
+        amb_res_in = amb_res is not None
+        if not amb_res_in:
+            amb_res = algo.rotor_model.from_data_or_store(
+                FC.AMB_RPOINT_RESULTS, algo, mdata
+            )
+
         wres = {}
         st_sel = (np.arange(n_states), states_turbine)
         for v, ares in amb_res.items():
             wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-        del amb_res
 
         wdel = {}
         for v, d in wake_deltas.items():
             wdel[v] = d.reshape(n_states, n_turbines, 1)[st_sel]
         for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
+            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
-                if update_amb_res:
-                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                if amb_res_in:
+                    amb_res[v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         self.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, weights, states_turbine=states_turbine
         )
 
     def finalize(self, algo, verbosity=0):
```

### Comparing `foxes-0.4.0/foxes/models/partial_wakes/distsliced.py` & `foxes-0.4.1/foxes/models/partial_wakes/distsliced.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from foxes.core import PartialWakesModel
+from foxes.core import PartialWakesModel, Data
 from foxes.models.wake_models.dist_sliced import DistSlicedWakeModel
 from foxes.models.rotor_models.grid import GridRotor
 from foxes.utils import wd2uv, uv2wd
 import foxes.variables as FV
 import foxes.constants as FC
 
 
@@ -28,15 +28,15 @@
     """
 
     def __init__(
         self, n=None, wake_models=None, wake_frame=None, rotor_model=None, **kwargs
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         n: int, optional
             The `GridRotor`'s `n` parameter
         wake_models: list of foxes.core.WakeModel, optional
             The wake models, default are the ones from the algorithm
         wake_frame: foxes.core.WakeFrame, optional
@@ -103,14 +103,29 @@
 
         algo.update_idata(
             [self.rotor_model, self.grotor], idata=idata, verbosity=verbosity
         )
 
         return idata
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        super().keep(algo)
+        self.rotor_model.keep(algo)
+        self.grotor.keep(algo)
+
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
@@ -121,74 +136,86 @@
         fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
         wake_deltas: dict
             Keys: Variable name str, values: any
+        pdata: foxes.core.Data
+            The evaluation point data
 
         """
+
+        n_states = fdata.n_states
         n_rpoints = self.grotor.n_rotor_points()
         n_points = fdata.n_turbines * n_rpoints
+        points = self.grotor.get_rotor_points(algo, mdata, fdata).reshape(
+            n_states, n_points, 3
+        )
+        pdata = Data.from_points(points=points)
+
         wake_deltas = {}
         for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, n_points, wake_deltas)
+            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
 
-        return wake_deltas
+        return wake_deltas, pdata
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
-        # calc coordinates to rotor centres:
-        wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, states_source_turbine, fdata[FV.TXYH]
-        )
 
-        # get x coordinates:
-        x = wcoos[:, :, 0]
-        del wcoos
+        # calc x-coordinates of rotor centres:
+        hpdata = Data.from_points(points=fdata[FV.TXYH])
+        x = self.wake_frame.get_wake_coos(
+            algo, mdata, fdata, hpdata, states_source_turbine
+        )[:, :, 0]
 
         # evaluate grid rotor:
         n_states = fdata.n_states
         n_turbines = fdata.n_turbines
         n_rpoints = self.grotor.n_rotor_points()
-        n_points = n_turbines * n_rpoints
-        points = self.grotor.get_rotor_points(algo, mdata, fdata).reshape(
-            n_states, n_points, 3
-        )
+        n_points = fdata.n_turbines * n_rpoints
         wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, states_source_turbine, points
+            algo, mdata, fdata, pdata, states_source_turbine
         )
         yz = wcoos.reshape(n_states, n_turbines, n_rpoints, 3)[:, :, :, 1:3]
-        del points, wcoos
+        del wcoos
 
         # evaluate wake models:
         for w in self.wake_models:
             wdeltas, sp_sel = w.calc_wakes_spsel_x_yz(
-                algo, mdata, fdata, states_source_turbine, x, yz
+                algo, mdata, fdata, hpdata, states_source_turbine, x, yz
             )
 
             wsps = np.zeros((n_states, n_turbines, n_rpoints), dtype=bool)
             wsps[:] = sp_sel[:, :, None]
             wsps = wsps.reshape(n_states, n_points)
 
             for v, wdel in wdeltas.items():
@@ -203,52 +230,70 @@
                         f"Model '{self.name}': Missing wake superposition entry for variable '{v}' in wake model '{w.name}', found {sorted(list(w.superp.keys()))}"
                     )
 
                 wake_deltas[v] = superp.calc_wakes_plus_wake(
                     algo,
                     mdata,
                     fdata,
+                    hpdata,
                     states_source_turbine,
                     wsps,
                     v,
                     wake_deltas[v],
                     d,
                 )
 
     def evaluate_results(
-        self, algo, mdata, fdata, wake_deltas, states_turbine, update_amb_res=False
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        wake_deltas,
+        states_turbine,
+        amb_res=None,
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
         states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res: bool
-            Flag for updating ambient results
+        amb_res: dict, optional
+            Ambient states results. Keys: var str, values:
+            numpy.ndarray of shape (n_states, n_points)
 
         """
-        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FC.RPOINTS, mdata)
-        rweights = self.get_data(FC.RWEIGHTS, mdata)
+        rweights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
+        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
+        n_states, n_turbines, n_rpoints, __ = rpoints.shape
+
+        amb_res_in = amb_res is not None
+        if not amb_res_in:
+            amb_res = algo.rotor_model.from_data_or_store(
+                FC.AMB_RPOINT_RESULTS, algo, mdata
+            )
+
         wweights = self.grotor.rotor_point_weights()
         n_wpoints = self.grotor.n_rotor_points()
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         st_sel = (np.arange(n_states), states_turbine)
 
         uv = None
         if (FV.WS in amb_res and FV.WD not in amb_res) or (
@@ -273,29 +318,29 @@
                 wres[v] = np.linalg.norm(uv, axis=-1)
             elif v == FV.WD and uv is not None:
                 wres[v] = uv2wd(uv, axis=-1)
             else:
                 wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
                 wres[v] = np.einsum("sp,p->s", wres[v], rweights)
             wres[v] = wres[v][:, None]
-        del amb_res, uv
+        del uv
 
         wdel = {}
         for v, d in wake_deltas.items():
             wdel[v] = d.reshape(n_states, n_turbines, n_wpoints)[st_sel]
         for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
+            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
         for v in wdel.keys():
             wdel[v] = np.einsum("sp,p->s", wdel[v], wweights)[:, None]
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
-                if update_amb_res:
-                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                if amb_res_in:
+                    amb_res[v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         self.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, np.array([1.0]), states_turbine=states_turbine
         )
 
     def finalize(self, algo, verbosity=0):
```

### Comparing `foxes-0.4.0/foxes/models/partial_wakes/grid.py` & `foxes-0.4.1/foxes/models/partial_wakes/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     def __init__(
         self, n, wake_models=None, wake_frame=None, rotor_model=None, **kwargs
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         n: int, optional
             The `GridRotor`'s `n` parameter
         wake_models: list of foxes.core.WakeModel, optional
             The wake models, default are the ones from the algorithm
         wake_frame: foxes.core.WakeFrame, optional
@@ -35,47 +35,48 @@
 
         if not isinstance(self.grotor, GridRotor):
             raise ValueError(
                 f"Wrong grotor type, expecting {GridRotor.__name__}, got {type(self.grotor).__name__}"
             )
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
+
         # evaluate grid rotor:
-        n_states = fdata.n_states
-        n_turbines = fdata.n_turbines
-        n_rpoints = self.grotor.n_rotor_points()
-        n_points = n_turbines * n_rpoints
-        points = self.grotor.get_rotor_points(algo, mdata, fdata).reshape(
-            n_states, n_points, 3
-        )
         wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, states_source_turbine, points
+            algo, mdata, fdata, pdata, states_source_turbine
         )
-        del points
 
         # evaluate wake models:
         for w in self.wake_models:
             w.contribute_to_wake_deltas(
-                algo, mdata, fdata, states_source_turbine, wcoos, wake_deltas
+                algo, mdata, fdata, pdata, states_source_turbine, wcoos, wake_deltas
             )
```

### Comparing `foxes-0.4.0/foxes/models/partial_wakes/mapped.py` & `foxes-0.4.1/foxes/models/partial_wakes/mapped.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from foxes.models.partial_wakes.rotor_points import RotorPoints
 from foxes.models.partial_wakes.top_hat import PartialTopHat
 from foxes.models.partial_wakes.axiwake import PartialAxiwake
 from foxes.models.partial_wakes.distsliced import PartialDistSlicedWake
 from foxes.models.wake_models.top_hat import TopHatWakeModel
 from foxes.models.wake_models.dist_sliced import DistSlicedWakeModel
 from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
+import foxes.constants as FC
 
 
 class Mapped(PartialWakesModel):
     """
     Partial wake models depending on the wake model (type).
 
     This is required if more than one wake models are
@@ -23,25 +24,25 @@
         Mapping from wake model name to partial wakes.
         Key: model name str, value: Tuple of length 2,
         (Partial wake class name, parameter dict)
     wtype2pwake: dict
         Mapping from wake model class name to partial wakes.
         Key: wake model class name str, value: Tuple of length 2,
         (Partial wake class name, parameter dict)
-    
+
     :group: models.partial_wakes
 
     """
 
     def __init__(
         self, wname2pwake={}, wtype2pwake=None, wake_models=None, wake_frame=None
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         wname2pwake: dict, optional
             Mapping from wake model name to partial wakes.
             Key: model name str, value: Tuple of length 2,
             (Partial wake class name, parameter dict)
         wtype2pwake: dict, optional
@@ -126,14 +127,29 @@
                 )
             self._pwakes.append(PartialWakesModel.new(pname, **pars))
 
         algo.update_idata(self._pwakes, idata=idata, verbosity=verbosity)
 
         return idata
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        super().keep(algo)
+        for pw in self._pwakes:
+            pw.keep(algo)
+
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
         ----------
@@ -144,77 +160,116 @@
         fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
         wake_deltas: dict
             Keys: Variable name str, values: any
+        pdata: foxes.core.Data
+            The evaluation point data
 
         """
-        return [pw.new_wake_deltas(algo, mdata, fdata) for pw in self._pwakes]
+        wdeltas = []
+        pdatas = []
+        for pw in self._pwakes:
+            w, p = pw.new_wake_deltas(algo, mdata, fdata)
+            wdeltas.append(w)
+            pdatas.append(p)
+
+        return wdeltas, pdatas
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
         for pwi, pw in enumerate(self._pwakes):
             pw.contribute_to_wake_deltas(
-                algo, mdata, fdata, states_source_turbine, wake_deltas[pwi]
+                algo, mdata, fdata, pdata[pwi], states_source_turbine, wake_deltas[pwi]
             )
 
     def evaluate_results(
-        self, algo, mdata, fdata, wake_deltas, states_turbine, update_amb_res=True
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        wake_deltas,
+        states_turbine,
+        amb_res=None,
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
         states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res: bool
-            Flag for updating ambient results
+        amb_res: dict, optional
+            Ambient states results. Keys: var str, values:
+            numpy.ndarray of shape (n_states, n_points)
 
         """
+        if amb_res is None:
+            ares = algo.rotor_model.from_data_or_store(
+                FC.AMB_RPOINT_RESULTS, algo, mdata
+            ).copy()
+            amb_res = {v: d.copy() for v, d in ares.items()}
+
         for pwi, pw in enumerate(self._pwakes):
             pw.evaluate_results(
-                algo, mdata, fdata, wake_deltas[pwi], states_turbine, update_amb_res
+                algo,
+                mdata,
+                fdata,
+                pdata[pwi],
+                wake_deltas[pwi],
+                states_turbine,
+                amb_res=amb_res,
             )
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
```

### Comparing `foxes-0.4.0/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.4.1/foxes/models/partial_wakes/rotor_points.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,36 @@
 import numpy as np
 
-from foxes.core import PartialWakesModel
-import foxes.variables as FV
+from foxes.core import PartialWakesModel, Data
 import foxes.constants as FC
 
+
 class RotorPoints(PartialWakesModel):
     """
     Partial wakes calculation directly by the
     rotor model.
 
     :group: models.partial_wakes
 
     """
 
     def __init__(self, wake_models=None, wake_frame=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         wake_models: list of foxes.core.WakeModel, optional
             The wake models, default are the ones from the algorithm
         wake_frame: foxes.core.WakeFrame, optional
             The wake frame, default is the one from the algorithm
 
         """
         super().__init__(wake_models, wake_frame)
 
-    def initialize(self, algo, verbosity=0):
-        """
-        Initializes the model.
-
-        This includes loading all required data from files. The model
-        should return all array type data as part of the idata return
-        dictionary (and not store it under self, for memory reasons). This
-        data will then be chunked and provided as part of the mdata object
-        during calculations.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
-
-        Returns
-        -------
-        idata: dict
-            The dict has exactly two entries: `data_vars`,
-            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
-            and `coords`, a dict with entries `dim_name_str -> dim_array`
-
-        """
-        self.WPOINTS = self.var("WPOINTS")
-
-        idata = super().initialize(algo, verbosity)
-        algo.update_idata(algo.rotor_model, idata=idata, verbosity=verbosity)
-
-        return idata
-
     def get_wake_points(self, algo, mdata, fdata):
         """
         Get the wake calculation points.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
@@ -74,15 +42,15 @@
 
         Returns
         -------
         rpoints: numpy.ndarray
             All rotor points, shape: (n_states, n_points, 3)
 
         """
-        rpoints = self.get_data(FC.RPOINTS, mdata)
+        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
         return rpoints.reshape(n_states, n_turbines * n_rpoints, 3)
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
@@ -96,106 +64,129 @@
         fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
         wake_deltas: dict
             Keys: Variable name str, values: any
+        pdata: foxes.core.Data
+            The evaluation point data
 
         """
-        mdata[self.WPOINTS] = self.get_wake_points(algo, mdata, fdata)
-        n_points = mdata[self.WPOINTS].shape[1]
+        points = self.get_wake_points(algo, mdata, fdata)
+        pdata = Data.from_points(points=points)
 
         wake_deltas = {}
         for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, n_points, wake_deltas)
+            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
 
-        return wake_deltas
+        return wake_deltas, pdata
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
         """
-        points = mdata[self.WPOINTS]
         wcoos = self.wake_frame.get_wake_coos(
-            algo, mdata, fdata, states_source_turbine, points
+            algo, mdata, fdata, pdata, states_source_turbine
         )
 
         for w in self.wake_models:
             w.contribute_to_wake_deltas(
-                algo, mdata, fdata, states_source_turbine, wcoos, wake_deltas
+                algo, mdata, fdata, pdata, states_source_turbine, wcoos, wake_deltas
             )
 
     def evaluate_results(
-        self, algo, mdata, fdata, wake_deltas, states_turbine, update_amb_res=False
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        wake_deltas,
+        states_turbine,
+        amb_res=None,
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
         states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res: bool
-            Flag for updating ambient results
+        amb_res: dict, optional
+            Ambient states results. Keys: var str, values:
+            numpy.ndarray of shape (n_states, n_points)
 
         """
-        weights = self.get_data(FC.RWEIGHTS, mdata)
-        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FC.RPOINTS, mdata)
+        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
+        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
 
+        amb_res_in = amb_res is not None
+        if not amb_res_in:
+            amb_res = algo.rotor_model.from_data_or_store(
+                FC.AMB_RPOINT_RESULTS, algo, mdata
+            )
+
         wres = {}
         st_sel = (np.arange(n_states), states_turbine)
         for v, ares in amb_res.items():
             wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-        del amb_res
 
         wdel = {}
         for v, d in wake_deltas.items():
             wdel[v] = d.reshape(n_states, n_turbines, n_rpoints)[st_sel]
         for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
+            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
-                if update_amb_res:
-                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                if amb_res_in:
+                    amb_res[v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         algo.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, weights, states_turbine=states_turbine
         )
```

### Comparing `foxes-0.4.0/foxes/models/partial_wakes/top_hat.py` & `foxes-0.4.1/foxes/models/partial_wakes/top_hat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from foxes.core import PartialWakesModel
+from foxes.core import PartialWakesModel, Data
 from foxes.models.wake_models.top_hat import TopHatWakeModel
 from foxes.utils.two_circles import calc_area
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class PartialTopHat(PartialWakesModel):
@@ -22,15 +22,15 @@
     :group: models.partial_wakes
 
     """
 
     def __init__(self, wake_models=None, wake_frame=None, rotor_model=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         wake_models: list of foxes.core.WakeModel, optional
             The wake models, default are the ones from the algorithm
         wake_frame: foxes.core.WakeFrame, optional
             The wake frame, default is the one from the algorithm
         rotor_model: foxes.core.RotorModel, optional
@@ -80,34 +80,27 @@
         self.WCOOS_X = self.var("WCOOS_X")
         self.WCOOS_R = self.var("WCOOS_R")
 
         algo.update_idata(self.rotor_model, idata=idata, verbosity=verbosity)
 
         return idata
 
-    def get_wake_points(self, algo, mdata, fdata):
+    def keep(self, algo):
         """
-        Get the wake calculation points.
+        Add model and all sub models to
+        the keep_models list
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-
-        Returns
-        -------
-        rpoints: numpy.ndarray
-            All rotor points, shape: (n_states, n_points, 3)
+            The algorithm
 
         """
-        return fdata[FV.TXYH]
+        super().keep(algo)
+        self.rotor_model.keep(algo)
 
     def new_wake_deltas(self, algo, mdata, fdata):
         """
         Creates new initial wake deltas, filled
         with zeros.
 
         Parameters
@@ -119,38 +112,49 @@
         fdata: foxes.core.Data
             The farm data
 
         Returns
         -------
         wake_deltas: dict
             Keys: Variable name str, values: any
+        pdata: foxes.core.Data
+            The evaluation point data
 
         """
-        n_points = fdata.n_turbines
+        pdata = Data.from_points(points=fdata[FV.TXYH])
+
         wake_deltas = {}
         for w in self.wake_models:
-            w.init_wake_deltas(algo, mdata, fdata, n_points, wake_deltas)
+            w.init_wake_deltas(algo, mdata, fdata, pdata, wake_deltas)
 
-        return wake_deltas
+        return wake_deltas, pdata
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_deltas,
     ):
         """
         Modifies wake deltas by contributions from the
         specified wake source turbines.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray of int
             For each state, one turbine index corresponding
             to the wake causing turbine. Shape: (n_states,)
         wake_deltas: Any
             The wake deltas object created by the
             `new_wake_deltas` function
 
@@ -159,23 +163,21 @@
         n_points = fdata.n_turbines
         stsel = (np.arange(n_states), states_source_turbine)
 
         if (
             self.WCOOS_ID not in mdata
             or mdata[self.WCOOS_ID] != states_source_turbine[0]
         ):
-            points = self.get_wake_points(algo, mdata, fdata)
             wcoos = self.wake_frame.get_wake_coos(
-                algo, mdata, fdata, states_source_turbine, points
+                algo, mdata, fdata, pdata, states_source_turbine
             )
             mdata[self.WCOOS_ID] = states_source_turbine[0]
             mdata[self.WCOOS_X] = wcoos[:, :, 0]
             mdata[self.WCOOS_R] = np.linalg.norm(wcoos[:, :, 1:3], axis=-1)
             wcoos[:, :, 1:3] = 0
-            del points
         else:
             wcoos = np.zeros((n_states, n_points), dtype=FC.DTYPE)
             wcoos[:, :, 0] = mdata[self.WCOOS_X]
 
         ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
         ct[:] = fdata[FV.CT][stsel][:, None]
         x = mdata[self.WCOOS_X]
@@ -184,25 +186,33 @@
         if np.any(sel0):
             R = mdata[self.WCOOS_R]
             r = np.zeros_like(R)
             D = fdata[FV.D]
 
             for w in self.wake_models:
                 wr = w.calc_wake_radius(
-                    algo, mdata, fdata, states_source_turbine, x, ct
+                    algo, mdata, fdata, pdata, states_source_turbine, x, ct
                 )
 
                 sel_sp = sel0 & (wr > R - D / 2)
                 if np.any(sel_sp):
                     hx = x[sel_sp]
                     hct = ct[sel_sp]
                     hwr = wr[sel_sp]
 
                     clw = w.calc_centreline_wake_deltas(
-                        algo, mdata, fdata, states_source_turbine, sel_sp, hx, hwr, hct
+                        algo,
+                        mdata,
+                        fdata,
+                        pdata,
+                        states_source_turbine,
+                        sel_sp,
+                        hx,
+                        hwr,
+                        hct,
                     )
                     del hx, hct
 
                     hR = R[sel_sp]
                     hD = D[sel_sp]
                     weights = calc_area(hD / 2, hwr, hR) / (np.pi * (hD / 2) ** 2)
                     del hD, hwr, hR
@@ -215,71 +225,86 @@
                                 f"Model '{self.name}': Missing wake superposition entry for variable '{v}' in wake model '{w.name}', found {sorted(list(w.superp.keys()))}"
                             )
 
                         wake_deltas[v] = superp.calc_wakes_plus_wake(
                             algo,
                             mdata,
                             fdata,
+                            pdata,
                             states_source_turbine,
                             sel_sp,
                             v,
                             wake_deltas[v],
                             weights * d,
                         )
 
     def evaluate_results(
-        self, algo, mdata, fdata, wake_deltas, states_turbine, update_amb_res=False
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        wake_deltas,
+        states_turbine,
+        amb_res=None,
     ):
         """
         Updates the farm data according to the wake
         deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
             Modified in-place by this function
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: Any
             The wake deltas object, created by the
             `new_wake_deltas` function and filled
             by `contribute_to_wake_deltas`
         states_turbine: numpy.ndarray of int
             For each state, the index of one turbine
             for which to evaluate the wake deltas.
             Shape: (n_states,)
-        update_amb_res: bool
-            Flag for updating ambient results
+        amb_res: dict, optional
+            Ambient states results. Keys: var str, values:
+            numpy.ndarray of shape (n_states, n_points)
 
         """
-        weights = self.get_data(FC.RWEIGHTS, mdata)
-        amb_res = self.get_data(FC.AMB_RPOINT_RESULTS, mdata)
-        rpoints = self.get_data(FC.RPOINTS, mdata)
+        weights = algo.rotor_model.from_data_or_store(FC.RWEIGHTS, algo, mdata)
+        rpoints = algo.rotor_model.from_data_or_store(FC.RPOINTS, algo, mdata)
         n_states, n_turbines, n_rpoints, __ = rpoints.shape
 
+        amb_res_in = amb_res is not None
+        if not amb_res_in:
+            amb_res = algo.rotor_model.from_data_or_store(
+                FC.AMB_RPOINT_RESULTS, algo, mdata
+            )
+
         wres = {}
         st_sel = (np.arange(n_states), states_turbine)
         for v, ares in amb_res.items():
             wres[v] = ares.reshape(n_states, n_turbines, n_rpoints)[st_sel]
-        del amb_res
 
         wdel = {}
         for v, d in wake_deltas.items():
             wdel[v] = d.reshape(n_states, n_turbines, 1)[st_sel]
         for w in self.wake_models:
-            w.finalize_wake_deltas(algo, mdata, fdata, wres, wdel)
+            w.finalize_wake_deltas(algo, mdata, fdata, pdata, wres, wdel)
 
         for v in wres.keys():
             if v in wake_deltas:
                 wres[v] += wdel[v]
-                if update_amb_res:
-                    mdata[FC.AMB_RPOINT_RESULTS][v][st_sel] = wres[v]
+                if amb_res_in:
+                    amb_res[v][st_sel] = wres[v]
             wres[v] = wres[v][:, None]
 
         self.rotor_model.eval_rpoint_results(
             algo, mdata, fdata, wres, weights, states_turbine=states_turbine
         )
 
     def finalize(self, algo, verbosity=0):
```

### Comparing `foxes-0.4.0/foxes/models/point_models/set_uniform_data.py` & `foxes-0.4.1/foxes/models/point_models/set_uniform_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         data_source,
         output_vars,
         var2col={},
         pd_read_pars={},
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame or dict
             Either a file name, or a data frame, both assuming
             state dependent data. Or a dict for state independent
             uniform data (i.e., scalars)
         output_vars: list of str
```

### Comparing `foxes-0.4.0/foxes/models/point_models/tke2ti.py` & `foxes-0.4.1/foxes/models/point_models/tke2ti.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class TKE2TI(PointDataModel):
     """
     Calculates TI from TKE, using TI = sqrt( 3/2 * TKE) / WS
 
     :group: models.point_models
-    
+
     """
 
     def output_point_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
```

### Comparing `foxes-0.4.0/foxes/models/point_models/wake_deltas.py` & `foxes-0.4.1/foxes/models/point_models/wake_deltas.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/models/rotor_models/centre.py` & `foxes-0.4.1/foxes/models/rotor_models/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/models/rotor_models/grid.py` & `foxes-0.4.1/foxes/models/rotor_models/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :group: models.rotor_models
 
     """
 
     def __init__(self, n, calc_vars, reduce=True, nint=200):
         """
         Constructor.
-        
+
         Parameters
         ----------
         n: int
             The number of points along one direction,
             maximal number of points is N = n * n
         calc_vars: list of str
             The variables that are calculated by the model
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/calculator.py` & `foxes-0.4.1/foxes/models/turbine_models/calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     :group: models.turbine_models
 
     """
 
     def __init__(self, in_vars, out_vars, func, **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         in_vars: list of str
             The input farm vairables
         out_vars: list of str
             The output variables
         func: Function
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/kTI_model.py` & `foxes-0.4.1/foxes/models/turbine_models/kTI_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     :group: models.turbine_models
 
     """
 
     def __init__(self, kTI=None, kb=None, ti_var=FV.TI, ti_val=None, k_var=FV.K):
         """
         Constructor.
-        
+
         Parameters
         ----------
         kTI: float, optional
             Uniform value for `kTI`. If not given it
             will be searched in farm data
         kb: float, optional
             Uniform value for `kb`. If not given it
@@ -47,15 +47,18 @@
         self.ti_var = ti_var
         self.k_var = k_var
         setattr(self, ti_var, ti_val)
         setattr(self, FV.KTI, kTI)
         setattr(self, FV.KB, 0 if kb is None else kb)
 
     def __repr__(self):
-        return super().__repr__() + f"({self.k_var}, kTI={getattr(self, FV.KTI)}, ti={self.ti_var})"
+        return (
+            super().__repr__()
+            + f"({self.k_var}, kTI={getattr(self, FV.KTI)}, ti={self.ti_var})"
+        )
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
@@ -92,17 +95,23 @@
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        kTI = self.get_data(FV.KTI, fdata, st_sel)
-        kb = self.get_data(FV.KB, fdata, st_sel)
-        ti = self.get_data(self.ti_var, fdata, st_sel)
+        kTI = self.get_data(
+            FV.KTI, FC.STATE_TURBINE, lookup="sf", fdata=fdata, upcast=True
+        )[st_sel]
+        kb = self.get_data(
+            FV.KB, FC.STATE_TURBINE, lookup="sf", fdata=fdata, upcast=True
+        )[st_sel]
+        ti = self.get_data(
+            self.ti_var, FC.STATE_TURBINE, lookup="sf", fdata=fdata, upcast=True
+        )[st_sel]
 
         k = fdata.get(
             self.k_var, np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.DTYPE)
         )
 
         k[st_sel] = kTI * ti + kb
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/lookup_table.py` & `foxes-0.4.1/foxes/models/turbine_models/lookup_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,26 @@
         to column names in the data_source
 
     :group: models.turbine_models
 
     """
 
     def __init__(
-            self, 
-            data_source,
-            input_vars,
-            output_vars,
-            varmap={},
-            pd_file_read_pars={},
-            xr_interp_args={},
-            **kwargs
-        ):
+        self,
+        data_source,
+        input_vars,
+        output_vars,
+        varmap={},
+        pd_file_read_pars={},
+        xr_interp_args={},
+        **kwargs,
+    ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             The lookup-table data
         input_vars: list of str
             The foxes input variables
         output_vars: list of str
@@ -53,15 +53,15 @@
             Mapping from foxes variable names
             to column names in the data_source
         pd_file_read_pars: dict
             Parameters for pandas file reading
         xr_interp_args: dict
             Parameters for xarray interpolation method
         kwargs: dict, optional
-            Additional parameters, added as default 
+            Additional parameters, added as default
             values if not in data
 
         """
         super().__init__()
 
         self.data_source = data_source
         self.input_vars = input_vars
@@ -70,15 +70,17 @@
 
         self._rpars = pd_file_read_pars
         self._xargs = xr_interp_args
         self._data = None
 
         for v, d in kwargs.items():
             if v not in input_vars:
-                raise KeyError(f"{self.name}: Default input parameter '{v}' not in list of inputs {input_vars}")
+                raise KeyError(
+                    f"{self.name}: Default input parameter '{v}' not in list of inputs {input_vars}"
+                )
             setattr(self, v, d)
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
@@ -116,47 +118,50 @@
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         if self._data is None:
-            
             if isinstance(self.data_source, pd.DataFrame):
                 data = self.data_source
             else:
                 if verbosity > 0:
                     print(f"{self.name}: Reading file {self.data_source}")
                 data = PandasFileHelper.read_file(self.data_source, **self._rpars)
-        
+
             if verbosity > 0:
                 print(f"{self.name}: Preparing interpolation data")
             if len(self.varmap):
                 data = data.rename(columns={c: v for v, c in self.varmap.items()})
             data = data[self.input_vars + self.output_vars]
             data.sort_values(by=self.input_vars, inplace=True)
-            coords = {v: np.asarray(data[v].unique(), dtype=FC.DTYPE) for v in self.input_vars}
+            coords = {
+                v: np.asarray(data[v].unique(), dtype=FC.DTYPE) for v in self.input_vars
+            }
 
             dvars = {}
             for oname in self.output_vars:
                 pivot_matrix = data.pivot_table(index=self.input_vars, values=[oname])
                 dvars[oname] = (
-                    self.input_vars, 
-                    pivot_matrix.to_numpy(FC.DTYPE).reshape(pivot_matrix.index.levshape)
+                    self.input_vars,
+                    pivot_matrix.to_numpy(FC.DTYPE).reshape(
+                        pivot_matrix.index.levshape
+                    ),
                 )
-            
-            self._data = xr.Dataset(coords=coords, data_vars=dvars)        
-             
+
+            self._data = xr.Dataset(coords=coords, data_vars=dvars)
+
             if verbosity > 1:
                 print()
                 print(self._data)
                 print()
 
         return super().initialize(algo, verbosity)
-    
+
     def calculate(self, algo, mdata, fdata, st_sel):
         """ "
         The main model calculation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
@@ -177,17 +182,20 @@
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         indata = {
             v: xr.DataArray(
-                self.get_data(v, fdata, data_prio=True, upcast="farm")[st_sel],
-                dims=["_z"]
-            ) for v in self.input_vars
+                self.get_data(
+                    v, FC.STATE_TURBINE, lookup="fs", fdata=fdata, upcast=True
+                )[st_sel],
+                dims=["_z"],
+            )
+            for v in self.input_vars
         }
 
         odata = self._data.interp(**indata, **self._xargs)
 
         out = {}
         for v in self.output_vars:
             out[v] = fdata[v]
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/power_mask.py` & `foxes-0.4.1/foxes/models/turbine_models/power_mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     :group: models.turbine_models
 
     """
 
     def __init__(self, var_ws_P=FV.REWS3, factor_P=1.0e3):
         """
         Constructor.
-        
+
         Parameters
         ----------
         var_ws_P: str
             The wind speed variable for power lookup
         factor_P: float
             The power unit factor, e.g. 1000 for kW
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/rotor_centre_calc.py` & `foxes-0.4.1/foxes/models/turbine_models/rotor_centre_calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import numpy as np
 
 from foxes.core import TurbineModel, Data
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class RotorCentreCalc(TurbineModel):
     """
     Calculates data at the rotor centre
 
     Attributes
     ----------
     calc_vars: dict
         The variables that are calculated by the model,
         keys: var names, values: rotor var names
-        
+
     :group: models.turbine_models
 
     """
 
     def __init__(self, calc_vars):
         """
         Constructor.
-        
+
         Parameters
         ----------
         calc_vars: dict
             The variables that are calculated by the model,
             keys: var names, values: rotor var names
 
         """
         super().__init__()
-        
+
         if isinstance(calc_vars, dict):
             self.calc_vars = calc_vars
         else:
             self.calc_vars = {v: v for v in calc_vars}
 
     def initialize(self, algo, verbosity=0):
         """
@@ -64,15 +65,15 @@
         pvars = list(self.calc_vars.values())
         self._wcalc = algo.PointWakesCalculation(point_vars=pvars)
 
         idata = super().initialize(algo, verbosity)
         algo.update_idata(self._wcalc, idata=idata, verbosity=verbosity)
 
         return idata
-        
+
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
@@ -110,36 +111,36 @@
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         # prepare point data:
         pdata = {FC.POINTS: fdata[FV.TXYH]}
-        dims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
+        dims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
         for v in self.calc_vars.values():
             pdata[v] = np.zeros_like(pdata[FC.POINTS][:, :, 0])
             dims[v] = (FC.STATE, FC.POINT)
         pdata = Data(
             name=f"{self.name}_pdata",
             data=pdata,
             dims=dims,
-            loop_dims=[FC.STATE, FC.POINT]
+            loop_dims=[FC.STATE, FC.POINT],
         )
         del dims
 
         # run ambient calculation:
         res = algo.states.calculate(algo, mdata, fdata, pdata)
         for v, a in FV.var2amb.items():
             if v in res:
                 res[a] = res[v].copy()
         pdata.update(res)
 
         # run wake calculation:
         res = self._wcalc.calculate(algo, mdata, fdata, pdata)
-        
+
         # extract results:
         out = {v: fdata[v] for v in self.calc_vars.keys()}
         for v in out.keys():
             out[v][st_sel] = res[self.calc_vars[v]][st_sel]
 
         return out
 
@@ -153,8 +154,7 @@
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
 
         """
         algo.finalize_model(self._wcalc, verbosity)
         super().finalize(algo, verbosity)
-
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/sector_management.py` & `foxes-0.4.1/foxes/models/turbine_models/sector_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 
 from foxes.core import TurbineModel
 from foxes.utils import PandasFileHelper
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class SectorManagement(TurbineModel):
     """
     Changes variables based on variable range conditions.
 
     Attributes
     ----------
     source: str or pandas.DataFrame
@@ -28,15 +29,15 @@
         col_tnames=None,
         colmap={},
         var_periods={FV.WD: 360.0, FV.AMB_WD: 360.0},
         pd_file_read_pars={},
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             The file path or data
         range_vars: list of str
             The variables for which (min, max) ranges
             are specified in the data
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/set_XYHD.py` & `foxes-0.4.1/foxes/models/turbine_models/set_XYHD.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     :group: models.turbine_models
 
     """
 
     def __init__(self, set_XY=True, set_H=True, set_D=True):
         """
         Constructor.
-        
+
         Parameters
         ----------
         set_XY: bool
             Flag for (x,y) data
         set_H: bool
             Flag for height data
         set_D: bool
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.4.1/foxes/models/wake_frames/farm_order.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,44 @@
 import numpy as np
 
-from foxes.core import TurbineModel
 import foxes.constants as FC
+from .rotor_wd import RotorWD
+from foxes.core import WakeFrame
 
-class SetFarmVars(TurbineModel):
+
+class FarmOrder(WakeFrame):
     """
-    Set farm data variables to given data.
+    Invokes turbine ordering as defined
+    by the wind farm.
+
+    Warning: This is for testing purposes only, and in general
+    only gives correct calculation results when used
+    in an iterative algorithm.
 
     Attributes
     ----------
-    vars: list of str
-        The variables to be set
+    base_frame: foxes.core.WakeFrame
+        The wake frame from which to start
 
-    :group: models.turbine_models
+    :group: models.wake_frames
 
     """
 
-    def __init__(self, pre_rotor=False):
+    def __init__(self, base_frame=RotorWD()):
         """
         Constructor.
-        
-        Parameters
-        ----------
-        pre_rotor: bool
-            Flag for running this model before
-            running the rotor model.
-
-        """
-        super().__init__(pre_rotor=pre_rotor)
-        self.reset()
-
-    def add_var(self, var, data):
-        """
-        Add data for a variable.
-
-        Parameters
-        ----------
-        var: str
-            The variable name
-        data: numpy.ndarray
-            The data, shape: (n_states, n_turbines)
-
-        """
-        self.vars.append(var)
-        self._vdata.append(np.asarray(data, dtype=FC.DTYPE))
-
-    def reset(self):
-        """
-        Remove all variables.
-        """
-        self.vars = []
-        self._vdata = []
-
-    def output_farm_vars(self, algo):
-        """
-        The variables which are being modified by the model.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-
-        Returns
-        -------
-        output_vars: list of str
-            The output variable names
+        base_frame: foxes.core.WakeFrame
+            The wake frame from which to start
 
         """
-        return self.vars
+        super().__init__()
+        self.base_frame = base_frame
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -91,75 +58,111 @@
         idata: dict
             The dict has exactly two entries: `data_vars`,
             a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
             and `coords`, a dict with entries `dim_name_str -> dim_array`
 
         """
         idata = super().initialize(algo, verbosity)
-
-        for i, v in enumerate(self.vars):
-            data = np.full((algo.n_states, algo.n_turbines), np.nan, dtype=FC.DTYPE)
-            vdata = self._vdata[i]
-
-            # handle special case of call during vectorized optimization:
-            if (np.ndim(vdata) and 
-                vdata.shape[0] != algo.n_states and 
-                hasattr(algo.states, "n_pop")):
-
-                n_pop = algo.states.n_pop
-                n_ost = algo.states.states.size()
-                n_trb = algo.n_turbines
-                vdata = np.zeros((n_pop, n_ost, n_trb), dtype=FC.DTYPE)
-                vdata[:] = self._vdata[i][None, :]
-                vdata = vdata.reshape(n_pop*n_ost, n_trb)
-            
-            data[:] = vdata
-            idata["data_vars"][self.var(v)] = ((FC.STATE, FC.TURBINE), data)
+        algo.update_idata(self.base_frame, idata=idata, verbosity=verbosity)
 
         return idata
 
-    def calculate(self, algo, mdata, fdata, st_sel):
+    def calc_order(self, algo, mdata, fdata):
         """ "
-        The main model calculation.
+        Calculates the order of turbine evaluation.
 
         This function is executed on a single chunk of data,
         all computations should be based on numpy arrays.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        st_sel: numpy.ndarray of bool
-            The state-turbine selection,
-            shape: (n_states, n_turbines)
 
         Returns
         -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_turbines)
+        order: numpy.ndarray
+            The turbine order, shape: (n_states, n_turbines)
 
         """
-        n_states = fdata.n_states
-        n_turbines = fdata.n_turbines
-        allt = np.all(st_sel)
+        order = np.zeros((fdata.n_states, fdata.n_turbines), dtype=FC.ITYPE)
+        order[:] = np.arange(fdata.n_turbines)[None, :]
 
-        for v in self.vars:
-            data = mdata[self.var(v)]
-            hsel = ~np.isnan(data)
-            hallt = np.all(hsel)
+        return order
 
-            if allt and hallt:
-                fdata[v][:] = data
+    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
+        """
+        Calculate wake coordinates.
 
-            else:
-                if v not in fdata:
-                    fdata[v] = np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE)
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
+        states_source_turbine: numpy.ndarray
+            For each state, one turbine index for the
+            wake causing turbine. Shape: (n_states,)
+
+        Returns
+        -------
+        wake_coos: numpy.ndarray
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_points, 3)
+
+        """
+        return self.base_frame.get_wake_coos(
+            algo, mdata, fdata, pdata, states_source_turbine
+        )
+
+    def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
+        """
+        Gets the points along the centreline for given
+        values of x.
 
-                tsel = st_sel & hsel
-                fdata[v][tsel] = data[tsel]
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        states_source_turbine: numpy.ndarray
+            For each state, one turbine index for the
+            wake causing turbine. Shape: (n_states,)
+        x: numpy.ndarray
+            The wake frame x coordinates, shape: (n_states, n_points)
 
-        return {v: fdata[v] for v in self.vars}
+        Returns
+        -------
+        points: numpy.ndarray
+            The centreline points, shape: (n_states, n_points, 3)
+
+        """
+        return self.base_frame.get_centreline_points(
+            algo, mdata, fdata, states_source_turbine, x
+        )
+
+    def finalize(self, algo, verbosity=0):
+        """
+        Finalizes the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        verbosity: int
+            The verbosity level, 0 = silent
+
+        """
+        if self.base_frame.initialized:
+            self.base_frame.finalize(algo, verbosity)
+        super().finalize(algo, verbosity)
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/table_factors.py` & `foxes-0.4.1/foxes/models/turbine_models/table_factors.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         col_var,
         output_vars,
         pd_file_read_pars={},
         **ipars,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             Either path to a file or data
         row_var: str
             The row-wise variable
         col_var: str
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.4.1/foxes/models/turbine_models/thrust2ct.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :group: models.turbine_models
 
     """
 
     def __init__(self, thrust_var=FV.T, var_ws_ct=FV.REWS2):
         """
         Constructor.
-        
+
         Parameters
         ----------
         thrust_var: str
             Name of the thrust variable
         var_ws_ct: str
             The wind speed variable for ct lookup
 
@@ -76,15 +76,15 @@
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
         ct = fdata[FV.CT]
 
-        T = self.get_data(self.thrust_var, fdata, st_sel)
+        T = fdata[self.thrust_var][st_sel]
         rho = fdata[FV.RHO][st_sel]
         A = np.pi * (fdata[FV.D][st_sel] / 2) ** 2
         ws = fdata[self.WSCT][st_sel]
 
         ct[st_sel] = 2 * T / (rho * A * ws**2)
 
         return {FV.CT: ct}
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.4.1/foxes/models/turbine_models/yaw2yawm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 
 from foxes.core import TurbineModel
 import foxes.variables as FV
+import foxes.constants as FC
 from foxes.utils import delta_wd
 
 
 class YAW2YAWM(TurbineModel):
     """
     Calculates delta yaw (i.e. YAWM) from absolute
     yaw (i.e. YAW)
 
     :group: models.turbine_models
-    
+
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
@@ -53,14 +54,18 @@
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        yaw = self.get_data(FV.YAW, fdata, st_sel)
-        wd = self.get_data(FV.WD, fdata, st_sel)
+        yaw = self.get_data(
+            FV.YAW, FC.STATE_TURBINE, lookup="f", fdata=fdata, upcast=True
+        )[st_sel]
+        wd = self.get_data(
+            FV.WD, FC.STATE_TURBINE, lookup="f", fdata=fdata, upcast=True
+        )[st_sel]
 
         yawm = fdata[FV.YAWM]
         yawm[st_sel] = delta_wd(wd, yaw)
 
         return {FV.YAWM: yawm}
```

### Comparing `foxes-0.4.0/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.4.1/foxes/models/turbine_models/yawm2yaw.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
 
 from foxes.core import TurbineModel
 import foxes.variables as FV
+import foxes.constants as FC
 
 
 class YAWM2YAW(TurbineModel):
     """
     Calculates absolute yaw (i.e. YAWM) from delta
     yaw (i.e. YAWM)
 
     :group: models.turbine_models
-    
+
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
@@ -52,14 +53,18 @@
         Returns
         -------
         results: dict
             The resulting data, keys: output variable str.
             Values: numpy.ndarray with shape (n_states, n_turbines)
 
         """
-        yawm = self.get_data(FV.YAWM, fdata, st_sel)
-        wd = self.get_data(FV.WD, fdata, st_sel)
+        yawm = self.get_data(
+            FV.YAWM, FC.STATE_TURBINE, lookup="f", fdata=fdata, upcast=True
+        )[st_sel]
+        wd = self.get_data(
+            FV.WD, FC.STATE_TURBINE, lookup="f", fdata=fdata, upcast=True
+        )[st_sel]
 
         yaw = fdata[FV.YAW]
         yaw[st_sel] = np.mod(wd + yawm, 360.0)
 
         return {FV.YAW: yaw}
```

### Comparing `foxes-0.4.0/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.4.1/foxes/models/turbine_types/CpCt_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         col_cp="cp",
         rho=1.225,
         pd_file_read_pars={},
         **parameters,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             The file path, static name, or data
         col_ws: str
             The wind speed column
         col_cp: str
```

### Comparing `foxes-0.4.0/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.4.1/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         rho=1.225,
         pd_file_read_pars_cp={},
         pd_file_read_pars_ct={},
         **parameters,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source_cp: str or pandas.DataFrame
             The file path, static name, or data
         data_source_ct: str or pandas.DataFrame
             The file path, static name, or data
         col_ws_cp_file: str
```

### Comparing `foxes-0.4.0/foxes/models/turbine_types/PCt_file.py` & `foxes-0.4.1/foxes/models/turbine_types/PCt_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         var_ws_ct=FV.REWS2,
         var_ws_P=FV.REWS3,
         pd_file_read_pars={},
         **parameters,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         data_source: str or pandas.DataFrame
             The file path, static name, or data
         col_ws: str
             The wind speed column
         col_P: str
@@ -224,16 +224,16 @@
             if self.p_ct is not None:
                 rews2 *= (cosm**self.p_ct) ** 0.5
             if self.p_P is not None:
                 rews3 *= (cosm**self.p_P) ** (1.0 / 3.0)
             del yawm, cosm
 
         out = {
-            FV.P: fdata.get(FV.P, np.zeros_like(fdata[self.WSCT])),
-            FV.CT: fdata.get(FV.CT, np.zeros_like(fdata[self.WSP])),
+            FV.P: fdata[FV.P],
+            FV.CT: fdata[FV.CT],
         }
 
         out[FV.P][st_sel] = np.interp(
             rews3, self.data_ws, self.data_P, left=0.0, right=0.0
         )
         out[FV.CT][st_sel] = np.interp(
             rews2, self.data_ws, self.data_ct, left=0.0, right=0.0
```

### Comparing `foxes-0.4.0/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.4.1/foxes/models/turbine_types/PCt_from_two.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,16 +247,16 @@
             if self.p_ct is not None:
                 rews2 *= (cosm**self.p_ct) ** 0.5
             if self.p_P is not None:
                 rews3 *= (cosm**self.p_P) ** (1.0 / 3.0)
             del yawm, cosm
 
         out = {
-            FV.P: fdata.get(FV.P, np.zeros_like(fdata[self.WSP])),
-            FV.CT: fdata.get(FV.CT, np.zeros_like(fdata[self.WSCT])),
+            FV.P: fdata[FV.P],
+            FV.CT: fdata[FV.CT],
         }
         out[FV.P][st_sel] = np.interp(
             rews3, self._data_ws_P, self._data_P, left=0.0, right=0.0
         )
         out[FV.CT][st_sel] = np.interp(
             rews2, self._data_ws_ct, self._data_ct, left=0.0, right=0.0
         )
```

### Comparing `foxes-0.4.0/foxes/models/turbine_types/null_type.py` & `foxes-0.4.1/foxes/models/turbine_types/null_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class NullType(TurbineType):
     """
     A turbine type that does not compute any data.
 
     :group: models.turbine_types
-    
+
     """
 
     def output_farm_vars(self, algo):
         """
         The variables which are being modified by the model.
 
         Parameters
```

### Comparing `foxes-0.4.0/foxes/models/turbine_types/wsrho2PCt_from_two.py` & `foxes-0.4.1/foxes/models/turbine_types/wsrho2PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_neutral_ws.py` & `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class ABLLogNeutralWsProfile(VerticalProfile):
     """
     The neutral ABL wind speed log profile.
 
     :group: models.vertical_profiles
-    
+
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
```

### Comparing `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_stable_ws.py` & `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_stable_ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class ABLLogStableWsProfile(VerticalProfile):
     """
     The stable ABL wind speed log profile.
 
     :group: models.vertical_profiles
-    
+
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
```

### Comparing `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_unstable_ws.py` & `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class ABLLogUnstableWsProfile(VerticalProfile):
     """
     The unstable ABL wind speed log profile.
 
     :group: models.vertical_profiles
-    
+
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
```

### Comparing `foxes-0.4.0/foxes/models/vertical_profiles/abl_log_ws.py` & `foxes-0.4.1/foxes/models/vertical_profiles/abl_log_ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     The neutral/stable/unstable ABL wind speed log profile.
 
     This profile picks the profile according to the mol value
     (neutral: mol = None or mol = 0)
 
     :group: models.vertical_profiles
-    
+
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
```

### Comparing `foxes-0.4.0/foxes/models/vertical_profiles/sheared_ws.py` & `foxes-0.4.1/foxes/models/vertical_profiles/sheared_ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from foxes.utils import abl
 import foxes.variables as FV
 
 
 class ShearedProfile(VerticalProfile):
     """
     A wind shear profile, based on a shear exponent.
-    
+
     :group: models.vertical_profiles
-    
+
     """
 
     def input_vars(self):
         """
         The input variables needed for the profile
         calculation.
 
         Returns
         -------
         vars: list of str
             The variable names
-            
+
         """
         return [FV.WS, FV.H, FV.SHEAR]
 
     def calculate(self, data, heights):
         """
         Run the profile calculation.
```

### Comparing `foxes-0.4.0/foxes/models/vertical_profiles/uniform.py` & `foxes-0.4.1/foxes/models/vertical_profiles/uniform.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,23 @@
     """
     A profile with uniform values.
 
     Attributes
     ----------
     var: float
         The value
-    
+
     :group: models.vertical_profiles
 
     """
+
     def __init__(self, variable):
         """
         Constructor
-        
+
         Parameters
         ----------
         variable: float
             The value
 
         """
         super().__init__(self)
```

### Comparing `foxes-0.4.0/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.4.1/foxes/models/wake_frames/rotor_wd.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :group: models.wake_frames
 
     """
 
     def __init__(self, var_wd=FV.WD):
         """
         Constructor.
-        
+
         Parameters
         ----------
         var_wd: str
             The wind direction variable
 
         """
         super().__init__()
@@ -58,38 +58,40 @@
         n = np.mean(wd2uv(fdata[self.var_wd], axis=1), axis=-1)
         xy = fdata[FV.TXYH][:, :, :2]
 
         order = np.argsort(np.einsum("std,sd->st", xy, n), axis=-1)
 
         return order
 
-    def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
+    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points: numpy.ndarray
-            The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
         wake_coos: numpy.ndarray
-            The wake coordinates, shape: (n_states, n_points, 3)
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_points, 3)
 
         """
+        points = pdata[FC.POINTS]
         n_states = mdata.n_states
         stsel = (np.arange(n_states), states_source_turbine)
 
         xyz = fdata[FV.TXYH][stsel]
         delta = points - xyz[:, None, :]
         del xyz
```

### Comparing `foxes-0.4.0/foxes/models/wake_frames/streamlines.py` & `foxes-0.4.1/foxes/models/wake_frames/streamlines.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     n_delstor: int
         The streamline point storage increase
     max_length: float
         The maximal streamline length
     cl_ipars: dict
         Interpolation parameters for centre line
         point interpolation
-    
+
     :group: models.wake_frames
 
     """
 
     def __init__(self, step, n_delstor=100, max_length=1e5, cl_ipars={}):
         """
         Constructor.
-        
+
         Parameters
         ----------
         step: float
             The streamline step size in m
         n_delstor: int
             The streamline point storage increase
         max_length: float
@@ -136,15 +136,15 @@
         slen[:, :, n_spts] = slen[:, :, n_spts - 1] + self.step
         newpts = spts[:, :, n_spts]
         del p0, n0
 
         # calculate next tangential vector:
         svars = algo.states.output_point_vars(algo)
         pdata = {FC.POINTS: newpts}
-        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FV.XYH)}
+        pdims = {FC.POINTS: (FC.STATE, FC.POINT, FC.XYH)}
         pdata.update(
             {v: np.full((n_states, n_turbines), np.nan, dtype=FC.DTYPE) for v in svars}
         )
         pdims.update({v: (FC.STATE, FC.POINT) for v in svars})
         pdata = Data(pdata, pdims, loop_dims=[FC.STATE, FC.POINT])
         data[:, :, n_spts, 5] = 0.0
         data[:, :, n_spts, 3:5] = wd2uv(
@@ -166,24 +166,30 @@
         n_points = points.shape[1]
         n_spts = int(mdata[self.CNTR])
         data = mdata[self.DATA]
         spts = data[..., :3]
         sn = data[..., 3:6]
 
         # find minimal distances to existing streamline points:
-        # n_states, n_turbines, n_points, n_spts
-        dists = np.linalg.norm(
-            points[:, None, :, None] - spts[:, :, None, :n_spts], axis=-1
-        )
-        if tcase:
-            for ti in range(n_turbines):
-                dists[:, ti, ti] = 1e20
-        inds = np.argmin(dists, axis=3)
-        dists = np.take_along_axis(dists, inds[:, :, :, None], axis=3)[..., 0]
-        done = inds < n_spts - 1
+        # (loop over target points, since otherwise this blows memory)
+        done = np.zeros((n_states, n_turbines, n_points), dtype=bool)
+        inds = np.full((n_states, n_turbines, n_points), -1, dtype=FC.ITYPE)
+        dists = np.full((n_states, n_turbines, n_points), np.nan, dtype=FC.DTYPE)
+        for pi in range(n_points):
+            hdists = np.linalg.norm(
+                points[:, None, pi, None] - spts[:, :, :n_spts], axis=-1
+            )
+            if tcase:
+                hdists[:, pi] = np.inf
+            inds[:, :, pi] = np.argmin(hdists, axis=2)
+            dists[:, :, pi] = np.take_along_axis(hdists, inds[:, :, pi, None], axis=2)[
+                ..., 0
+            ]
+            done[:, :, pi] = inds[:, :, pi] < n_spts - 1
+            del hdists
 
         # calc streamline points, as many as needed:
         maxl = np.nanmax(data[:, :, n_spts - 1, 6])
         while maxl + self.step <= self.max_length and not np.all(done):
             # print("CALC STREAMLINES, TODO", np.sum(~done))
 
             # add next streamline point:
@@ -202,15 +208,15 @@
             # rotation:
             done = inds < n_spts - 1
             maxl = np.nanmax(data[:, :, n_spts - 1, 6])
             del newpts
 
         # shrink to size:
         mdata[self.DATA] = data[:, :, :n_spts]
-        del data, spts, sn
+        del data, spts, sn, dists, done
 
         # select streamline points:
         # n_states, n_turbines, n_points, 7
         data = np.take_along_axis(
             mdata[self.DATA][:, :, :, None], inds[:, :, None, :, None], axis=2
         )[:, :, 0]
         spts = data[..., :3]
@@ -282,42 +288,44 @@
         # TODO: Remove loop over states
         order = np.zeros((n_states, n_turbines), dtype=FC.ITYPE)
         for si in range(n_states):
             order[si] = np.lexsort(keys=coosx[si])
 
         return order
 
-    def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
+    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points: numpy.ndarray
-            The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
         wake_coos: numpy.ndarray
-            The wake coordinates, shape: (n_states, n_points, 3)
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_points, 3)
 
         """
 
         # prepare:
         n_states = mdata.n_states
         stsel = (np.arange(n_states), states_source_turbine)
+        points = pdata[FC.POINTS]
         pid = id(points)
 
         # initialize storage:
         if self.DATA not in mdata:
             self._init_data(mdata, fdata)
 
         # calc streamlines, once for given points:
```

### Comparing `foxes-0.4.0/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.4.1/foxes/models/wake_frames/yawed_wakes.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,31 +23,31 @@
     YAWM: float
         The yaw misalignment YAWM. If not given here
         it will be searched in the farm data.
     base_frame: foxes.core.WakeFrame
         The wake frame from which to start
     k_var: str
         The variable name for k
-    
+
     :group: models.wake_frames
 
     """
 
     def __init__(
         self,
         k=None,
         ct_max=0.9999,
-        alpha=0.58, 
+        alpha=0.58,
         beta=0.07,
         base_frame=RotorWD(),
         k_var=FV.K,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         k: float, optional
             The wake growth parameter k. If not given here
             it will be searched in the farm data, by default None
         ct_max: float, optional
             The maximal value for ct, values beyond will be limited
@@ -121,36 +121,48 @@
         -------
         order: numpy.ndarray
             The turbine order, shape: (n_states, n_turbines)
 
         """
         return self.base_frame.calc_order(algo, mdata, fdata)
 
-    def _update_y(self, mdata, fdata, states_source_turbine, x, y):
+    def _update_y(self, algo, mdata, fdata, pdata, states_source_turbine, x, y):
         """
         Helper function for y deflection
         """
-        # prepare:
-        n_states = mdata.n_states
-        n_points = x.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
 
         # get gamma:
-        gamma = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        gamma[:] = self.get_data(FV.YAWM, fdata, upcast="farm", data_prio=True)[st_sel][
-            :, None
-        ]
+        gamma = self.get_data(
+            FV.YAWM,
+            FC.STATE_POINT,
+            lookup="fs",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
         gamma *= np.pi / 180
 
         # get k:
-        k = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        k[:] = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_POINT,
+            lookup="sf",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
 
         # run model calculation:
-        self.model.calc_data(mdata, fdata, states_source_turbine, x, gamma, k)
+        self.model.calc_data(
+            algo, mdata, fdata, pdata, states_source_turbine, x, gamma, k
+        )
 
         # select targets:
         sp_sel = self.model.get_data(PorteAgelModel.SP_SEL, mdata)
         if np.any(sp_sel):
             # prepare:
             n_sp_sel = np.sum(sp_sel)
             ydef = np.zeros((n_sp_sel,), dtype=FC.DTYPE)
@@ -174,47 +186,49 @@
 
                 # set deflection:
                 ydef[far] = delta
 
             # apply deflection:
             y[sp_sel] -= ydef
 
-    def get_wake_coos(self, algo, mdata, fdata, states_source_turbine, points):
+    def get_wake_coos(self, algo, mdata, fdata, pdata, states_source_turbine):
         """
         Calculate wake coordinates.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        points: numpy.ndarray
-            The evaluation points, shape: (n_states, n_points, 3)
 
         Returns
         -------
         wake_coos: numpy.ndarray
-            The wake coordinates, shape: (n_states, n_points, 3)
+            The wake frame coordinates of the evaluation
+            points, shape: (n_states, n_points, 3)
 
         """
+
         # get unyawed results:
         xyz = self.base_frame.get_wake_coos(
-            algo, mdata, fdata, states_source_turbine, points
+            algo, mdata, fdata, pdata, states_source_turbine
         )
         x = xyz[:, :, 0]
         y = xyz[:, :, 1]
 
         # apply deflection:
-        self._update_y(mdata, fdata, states_source_turbine, x, y)
+        self._update_y(algo, mdata, fdata, pdata, states_source_turbine, x, y)
 
         return xyz
 
     def get_centreline_points(self, algo, mdata, fdata, states_source_turbine, x):
         """
         Gets the points along the centreline for given
         values of x.
@@ -253,15 +267,15 @@
 
         nz = np.zeros_like(nx)
         nz[:, :, 2] = 1
         ny = np.cross(nz, nx, axis=-1)
         del nx, nz
 
         y = np.zeros_like(x)
-        self._update_y(mdata, fdata, states_source_turbine, x, y)
+        self._update_y(algo, mdata, fdata, None, states_source_turbine, x, y)
 
         points += y[:, :, None] * ny
 
         return points
 
     def finalize(self, algo, verbosity=0):
         """
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/axisymmetric.py` & `foxes-0.4.1/foxes/models/wake_models/axisymmetric.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,30 +9,41 @@
     Abstract base class for wake models
     that depend on (x, r) separately.
 
     The ability to evaluate multiple r values per x
     is used by the `PartialAxiwake` partial wakes model.
 
     :group: models.wake_models
-    
+
     """
 
     @abstractmethod
-    def calc_wakes_spsel_x_r(self, algo, mdata, fdata, states_source_turbine, x, r):
+    def calc_wakes_spsel_x_r(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        r,
+    ):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         r: numpy.ndarray
             The radial values for each x value, shape:
@@ -46,26 +57,37 @@
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         pass
 
-    def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
+    def calc_wakes_spsel_x_yz(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        yz,
+    ):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         yz: numpy.ndarray
             The yz values for each x value, shape:
@@ -79,9 +101,9 @@
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         r = np.linalg.norm(yz, axis=-1)
         return self.calc_wakes_spsel_x_r(
-            algo, mdata, fdata, states_source_turbine, x, r
+            algo, mdata, fdata, pdata, states_source_turbine, x, r
         )
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/dist_sliced.py` & `foxes-0.4.1/foxes/models/wake_models/dist_sliced.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     :group: models.wake_models
 
     """
 
     def __init__(self, superpositions):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
 
@@ -71,27 +71,53 @@
         }
 
         idata = super().initialize(algo, verbosity)
         algo.update_idata(list(self.superp.values()), idata=idata, verbosity=verbosity)
 
         return idata
 
+    def keep(self, algo):
+        """
+        Add model and all sub models to
+        the keep_models list
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The algorithm
+
+        """
+        super().keep(algo)
+        for v in self.superp.values():
+            v.keep(algo)
+
     @abstractmethod
-    def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
+    def calc_wakes_spsel_x_yz(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        yz,
+    ):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         yz: numpy.ndarray
             The yz values for each x value, shape:
@@ -106,15 +132,22 @@
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
         pass
 
     def contribute_to_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, wake_coos, wake_deltas
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        wake_coos,
+        wake_deltas,
     ):
         """
         Calculate the contribution to the wake deltas
         by this wake model.
 
         Modifies wake_deltas on the fly.
 
@@ -122,14 +155,16 @@
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         wake_coos: numpy.ndarray
             The wake frame coordinates of the evaluation
             points, shape: (n_states, n_points, 3)
         wake_deltas: dict
@@ -139,64 +174,75 @@
             shape (n_states, n_points, ...)
 
         """
         x = wake_coos[:, :, 0]
         yz = wake_coos[:, :, None, 1:3]
 
         wdeltas, sp_sel = self.calc_wakes_spsel_x_yz(
-            algo, mdata, fdata, states_source_turbine, x, yz
+            algo, mdata, fdata, pdata, states_source_turbine, x, yz
         )
 
         for v, hdel in wdeltas.items():
             try:
                 superp = self.superp[v]
             except KeyError:
                 raise KeyError(
                     f"Model '{self.name}': Missing wake superposition entry for variable '{v}', found {sorted(list(self.superp.keys()))}"
                 )
 
             wake_deltas[v] = superp.calc_wakes_plus_wake(
                 algo,
                 mdata,
                 fdata,
+                pdata,
                 states_source_turbine,
                 sp_sel,
                 v,
                 wake_deltas[v],
                 hdel[:, 0],
             )
 
-    def finalize_wake_deltas(self, algo, mdata, fdata, amb_results, wake_deltas):
+    def finalize_wake_deltas(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        amb_results,
+        wake_deltas,
+    ):
         """
         Finalize the wake calculation.
 
         Modifies wake_deltas on the fly.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         amb_results: dict
             The ambient results, key: variable name str,
             values: numpy.ndarray with shape (n_states, n_points)
         wake_deltas: dict
             The wake deltas, are being modified ob the fly.
             Key: Variable name str, for which the wake delta
             applies, values: numpy.ndarray with shape
             (n_states, n_points, ...) before evaluation,
             numpy.ndarray with shape (n_states, n_points) afterwards
 
         """
         for v, s in self.superp.items():
             wake_deltas[v] = s.calc_final_wake_delta(
-                algo, mdata, fdata, v, amb_results[v], wake_deltas[v]
+                algo, mdata, fdata, pdata, v, amb_results[v], wake_deltas[v]
             )
 
     def finalize(self, algo, verbosity=0):
         """
         Finalizes the model.
 
         Parameters
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.4.1/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import foxes.variables as FV
 import foxes.constants as FC
 
 
 class CrespoHernandezTIWake(TopHatWakeModel):
     """
     The Crespo and Hernandez TI empirical correlation
-    
+
     Source: https://doi.org/10.1016/0167-6105(95)00033-X
 
     For the wake diameter we use Eqns. (17), (15), (4), (5) from
             doi:10.1088/1742-6596/625/1/012039
 
     Attributes
     ----------
@@ -53,19 +53,19 @@
         near_wake_D=None,
         ct_max=0.9999,
         a_near=0.362,
         a_far=0.73,
         e1=0.83,
         e2=-0.0325,
         e3=-0.32,
-        k_var=FV.K
+        k_var=FV.K,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
         k: float, optional
@@ -112,52 +112,63 @@
 
     def __repr__(self):
         k = getattr(self, self.k_var)
         s = super().__repr__()
         s += f"({self.k_var}={k}, sp={self.superpositions[FV.TI]})"
         return s
 
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
+    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        n_points: int
-            The number of wake evaluation points
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
-        wake_deltas[FV.TI] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        wake_deltas[FV.TI] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
 
-    def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
+    def calc_wake_radius(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        ct,
+    ):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         r: numpy.ndarray
             The radial values for each x value, shape:
@@ -168,46 +179,72 @@
 
         Returns
         -------
         wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
-        # prepare:
-        n_states = fdata.n_states
-        st_sel = (np.arange(n_states), states_source_turbine)
 
         # get D:
-        D = fdata[FV.D][st_sel][:, None]
+        D = self.get_data(
+            FV.D,
+            FC.STATE_POINT,
+            lookup="f",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
 
         # get k:
-        k = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_POINT,
+            lookup="sf",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
 
         # calculate:
         sbeta = np.sqrt(0.5 * (1 + np.sqrt(1 - ct)) / np.sqrt(1 - ct))
         sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
         sbeta[sbeta > sblim] = sblim
         radius = 2 * (k * x + self.sbeta_factor * sbeta * D)
 
         return radius
 
     def calc_centreline_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        sp_sel,
+        x,
+        wake_r,
+        ct,
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
         x: numpy.ndarray
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.4.1/foxes/models/wake_models/top_hat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,65 @@
 import numpy as np
+from abc import abstractmethod
 
-from foxes.models.wake_models.top_hat import TopHatWakeModel
+from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class IECTIWake(TopHatWakeModel):
+class TopHatWakeModel(AxisymmetricWakeModel):
     """
-    The TI wake model from IEC-64100-1-2005-8 (2005):
+    Abstract base class for top-hat wake models.
 
-    source: http://orbit.dtu.dk/files/3750291/2009_31.pdf
-    v2: VolLuk: corrected implementation following: IEC-64100-1-2005-8
-    (Appearently an error in the document by DTU)
-
-    and the Frandsen wake TI model, from IEC-64100 (2019):
-
-    Source: http://orbit.dtu.dk/files/3750291/2009_31.pdf
-
-    Attributes
-    ----------
-    opening_angle: float
-        The wake opening angle. The wake growth parameter k is calculated
-        based on the wake opening angle.
-    k_var: str
-        The variable name for k
-
-    :group: models.wake_models.ti
+    :group: models.wake_models
 
     """
 
-    def __init__(
-        self,
-        superposition,
-        opening_angle=21.6,
-        ct_max=0.9999,
-        iec_type="2019",
-        k_var=FV.K
-    ):
+    def __init__(self, superpositions, ct_max=0.9999):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
-        opening_angle: float
-            The wake opening angle. The wake growth parameter k is calculated
-            based on the wake opening angle.
         ct_max: float
             The maximal value for ct, values beyond will be limited
             to this number
-        k_var: str
-            The variable name for k
-
-        """
-        super().__init__(superpositions={FV.TI: superposition}, ct_max=ct_max)
-
-        k = float(np.tan(np.deg2rad(opening_angle / 2.0)))
-
-        self.iec_type = iec_type
-        self.k_var = k_var
-        setattr(self, k_var, k)
-
-    def __repr__(self):
-        k = getattr(self, self.k_var)
-        s = super().__repr__()
-        s += f"({self.k_var}={k}, sp={self.superpositions[FV.TI]})"
-        return s
-
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
-        """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        n_points: int
-            The number of wake evaluation points
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
 
         """
-        n_states = mdata.n_states
-        wake_deltas[FV.TI] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        super().__init__(superpositions)
+        self.ct_max = ct_max
 
-    def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
+    @abstractmethod
+    def calc_wake_radius(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        ct,
+    ):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         r: numpy.ndarray
             The radial values for each x value, shape:
@@ -122,42 +70,42 @@
 
         Returns
         -------
         wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
-        # prepare:
-        n_states = fdata.n_states
-        st_sel = (np.arange(n_states), states_source_turbine)
-
-        # get k:
-        k = self.get_data(self.k_var, fdata, st_sel, data_prio=False)
-        if isinstance(k, np.ndarray):
-            k = k[:, None]
-
-        # calculate:
-        radius = k * x
-
-        return radius
+        pass
 
+    @abstractmethod
     def calc_centreline_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        sp_sel,
+        x,
+        wake_r,
+        ct,
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
         x: numpy.ndarray
@@ -171,33 +119,82 @@
         Returns
         -------
         cl_del: dict
             The centre line wake deltas. Key: variable name str,
             varlue: numpy.ndarray, shape: (n_sp_sel,)
 
         """
-        # prepare:
-        n_states = fdata.n_states
-        n_points = sp_sel.shape[1]
+        pass
+
+    def calc_wakes_spsel_x_r(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        r,
+    ):
+        """
+        Calculate wake deltas.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
+        states_source_turbine: numpy.ndarray
+            For each state, one turbine index for the
+            wake causing turbine. Shape: (n_states,)
+        x: numpy.ndarray
+            The x values, shape: (n_states, n_points)
+        r: numpy.ndarray
+            The radial values for each x value, shape:
+            (n_states, n_points, n_r_per_x, 2)
+
+        Returns
+        -------
+        wdeltas: dict
+            The wake deltas. Key: variable name str,
+            value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
+        sp_sel: numpy.ndarray of bool
+            The state-point selection, for which the wake
+            is non-zero, shape: (n_states, n_points)
+
+        """
+        n_states = mdata.n_states
+        n_points = x.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
 
-        # read D from extra data:
-        D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        D[:] = fdata[FV.D][st_sel][:, None]
-        D = D[sp_sel]
-
-        # get ws:
-        ws = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ws[:] = fdata[FV.REWS][st_sel][:, None]
-        ws = ws[sp_sel]
-
-        # calculate wind deficit:
-        if self.iec_type == "2005":
-            cl_deltas = np.sqrt(0.9) / (1.5 + 0.3 * x / D * np.sqrt(ws))
-        elif self.iec_type == "2019" or self.iec_type == "Frandsen":
-            cl_deltas = 1.0 / (1.5 + 0.8 * x / D / np.sqrt(ct))
-        else:
-            raise TypeError(
-                f"Type of IEC {self.iec_type} not found. Select '2015' or '2019'/'Frandsen'."
+        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        ct[:] = fdata[FV.CT][st_sel][:, None]
+        ct[ct > self.ct_max] = self.ct_max
+
+        wake_r = self.calc_wake_radius(
+            algo, mdata, fdata, pdata, states_source_turbine, x, ct
+        )
+
+        wdeltas = {}
+        sp_sel = (ct > 0.0) & (x > 1e-5) & np.any(r < wake_r[:, :, None], axis=2)
+        if np.any(sp_sel):
+            x = x[sp_sel]
+            r = r[sp_sel]
+            ct = ct[sp_sel]
+            wake_r = wake_r[sp_sel]
+
+            cl_del = self.calc_centreline_wake_deltas(
+                algo, mdata, fdata, pdata, states_source_turbine, sp_sel, x, wake_r, ct
             )
 
-        return {FV.TI: cl_deltas}
+            nsel = r >= wake_r[:, None]
+            for v, wdel in cl_del.items():
+                wdeltas[v] = np.zeros_like(r)
+                wdeltas[v][:] = wdel[:, None]
+                wdeltas[v][nsel] = 0.0
+
+        return wdeltas, sp_sel
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/top_hat.py` & `foxes-0.4.1/foxes/models/wake_models/wind/jensen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,110 @@
 import numpy as np
-from abc import abstractmethod
 
-from foxes.models.wake_models.axisymmetric import AxisymmetricWakeModel
+from foxes.models.wake_models.top_hat import TopHatWakeModel
 import foxes.variables as FV
 import foxes.constants as FC
 
 
-class TopHatWakeModel(AxisymmetricWakeModel):
+class JensenWake(TopHatWakeModel):
     """
-    Abstract base class for top-hat wake models.
-    
-    :group: models.wake_models
+    The Jensen wake model.
+
+    Attributes
+    ----------
+    k: float, optional
+        The wake growth parameter k. If not given here
+        it will be searched in the farm data.
+    k_var: str
+        The variable name for k
+
+    :group: models.wake_models.wind
 
     """
 
-    def __init__(self, superpositions, ct_max=0.9999):
+    def __init__(self, superposition, k=None, ct_max=0.9999, k_var=FV.K):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
+        k: float, optional
+            The wake growth parameter k. If not given here
+            it will be searched in the farm data.
         ct_max: float
             The maximal value for ct, values beyond will be limited
             to this number
+        k_var: str
+            The variable name for k
+
+        """
+        super().__init__(superpositions={FV.WS: superposition}, ct_max=ct_max)
+
+        self.k_var = k_var
+        setattr(self, k_var, k)
+
+    def __repr__(self):
+        k = getattr(self, self.k_var)
+        s = super().__repr__()
+        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
+        return s
+
+    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
+        """
+        Initialize wake delta storage.
+
+        They are added on the fly to the wake_deltas dict.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+        mdata: foxes.core.Data
+            The model data
+        fdata: foxes.core.Data
+            The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
+        wake_deltas: dict
+            The wake deltas storage, add wake deltas
+            on the fly. Keys: Variable name str, for which the
+            wake delta applies, values: numpy.ndarray with
+            shape (n_states, n_points, ...)
 
         """
-        super().__init__(superpositions)
-        self.ct_max = ct_max
+        n_states = mdata.n_states
+        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
 
-    @abstractmethod
-    def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
+    def calc_wake_radius(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        ct,
+    ):
         """
         Calculate the wake radius, depending on x only (not r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         r: numpy.ndarray
             The radial values for each x value, shape:
@@ -59,31 +115,67 @@
 
         Returns
         -------
         wake_r: numpy.ndarray
             The wake radii, shape: (n_states, n_points)
 
         """
-        pass
 
-    @abstractmethod
+        R = (
+            self.get_data(
+                FV.D,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
+            / 2
+        )
+
+        k = self.get_data(
+            self.k_var,
+            FC.STATE_POINT,
+            lookup="sf",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
+
+        return R + k * x
+
     def calc_centreline_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        sp_sel,
+        x,
+        wake_r,
+        ct,
     ):
         """
         Calculate centre line results of wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
         x: numpy.ndarray
@@ -97,69 +189,16 @@
         Returns
         -------
         cl_del: dict
             The centre line wake deltas. Key: variable name str,
             varlue: numpy.ndarray, shape: (n_sp_sel,)
 
         """
-        pass
-
-    def calc_wakes_spsel_x_r(self, algo, mdata, fdata, states_source_turbine, x, r):
-        """
-        Calculate wake deltas.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
-        r: numpy.ndarray
-            The radial values for each x value, shape:
-            (n_states, n_points, n_r_per_x, 2)
-
-        Returns
-        -------
-        wdeltas: dict
-            The wake deltas. Key: variable name str,
-            value: numpy.ndarray, shape: (n_sp_sel, n_r_per_x)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
-
-        """
         n_states = mdata.n_states
-        n_points = x.shape[1]
+        n_points = sp_sel.shape[1]
         st_sel = (np.arange(n_states), states_source_turbine)
 
-        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ct[:] = fdata[FV.CT][st_sel][:, None]
-        ct[ct > self.ct_max] = self.ct_max
-
-        wake_r = self.calc_wake_radius(algo, mdata, fdata, states_source_turbine, x, ct)
-
-        wdeltas = {}
-        sp_sel = (ct > 0.0) & (x > 1e-5) & np.any(r < wake_r[:, :, None], axis=2)
-        if np.any(sp_sel):
-            x = x[sp_sel]
-            r = r[sp_sel]
-            ct = ct[sp_sel]
-            wake_r = wake_r[sp_sel]
-
-            cl_del = self.calc_centreline_wake_deltas(
-                algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
-            )
-
-            nsel = r >= wake_r[:, None]
-            for v, wdel in cl_del.items():
-                wdeltas[v] = np.zeros_like(r)
-                wdeltas[v][:] = wdel[:, None]
-                wdeltas[v][nsel] = 0.0
+        R = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        R[:] = fdata[FV.D][st_sel][:, None] / 2
+        R = R[sp_sel]
 
-        return wdeltas, sp_sel
+        return {FV.WS: -((R / wake_r) ** 2) * (1.0 - np.sqrt(1.0 - ct))}
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/wind/bastankhah.py` & `foxes-0.4.1/foxes/models/wake_models/wind/bastankhah.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     k_var: str
         The variable name for k
 
     :group: models.wake_models.wind
 
     """
 
-    def __init__(self, superposition, k=None, sbeta_factor=0.25, ct_max=0.9999, k_var=FV.K):
+    def __init__(
+        self, superposition, k=None, sbeta_factor=0.25, ct_max=0.9999, k_var=FV.K
+    ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
         k: float, optional
@@ -63,53 +65,62 @@
 
     def __repr__(self):
         k = getattr(self, self.k_var)
         s = super().__repr__()
         s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
         return s
 
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
+    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        n_points: int
-            The number of wake evaluation points
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
-        n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        wake_deltas[FV.WS] = np.zeros((mdata.n_states, pdata.n_points), dtype=FC.DTYPE)
 
-    def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
+    def calc_amplitude_sigma_spsel(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+    ):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
@@ -118,39 +129,59 @@
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
-        # prepare:
-        n_states = mdata.n_states
-        n_points = x.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
 
         # get ct:
-        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ct[:] = self.get_data(FV.CT, fdata)[st_sel][:, None]
+        ct = self.get_data(
+            FV.CT,
+            FC.STATE_POINT,
+            lookup="f",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
             # apply selection:
             x = x[sp_sel]
             ct = ct[sp_sel]
 
             # get D:
-            D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            D[:] = self.get_data(FV.D, fdata)[st_sel][:, None]
+            D = self.get_data(
+                FV.D,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
             D = D[sp_sel]
 
             # get k:
-            k = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            k[:] = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
+            k = self.get_data(
+                self.k_var,
+                FC.STATE_POINT,
+                lookup="sf",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
             k = k[sp_sel]
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
             sbeta[sbeta > sblim] = sblim
             sigma = k * x + self.sbeta_factor * sbeta * D
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/wind/jensen.py` & `foxes-0.4.1/foxes/models/wake_superpositions/ti_superp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,165 +1,170 @@
 import numpy as np
 
-from foxes.models.wake_models.top_hat import TopHatWakeModel
-import foxes.variables as FV
-import foxes.constants as FC
+from foxes.core import WakeSuperposition
 
 
-class JensenWake(TopHatWakeModel):
+class TISuperposition(WakeSuperposition):
     """
-    The Jensen wake model.
+    A collection of superpositions for TI.
 
     Attributes
     ----------
-    k: float, optional
-        The wake growth parameter k. If not given here
-        it will be searched in the farm data.
-    k_var: str
-        The variable name for k
+    ti_superp: str
+        The method choice: linear, quadratic, max
+    superp_to_amb: str
+        The method for combining ambient with wake deltas:
+        linear or quadratic
 
-    :group: models.wake_models.wind
+    :group: models.wake_superpositions
 
     """
 
-    def __init__(self, superposition, k=None, ct_max=0.9999, k_var=FV.K):
+    def __init__(self, ti_superp, superp_to_amb="quadratic"):
         """
         Constructor.
-        
-        Parameters
-        ----------
-        superpositions: dict
-            The superpositions. Key: variable name str,
-            value: The wake superposition model name,
-            will be looked up in model book
-        k: float, optional
-            The wake growth parameter k. If not given here
-            it will be searched in the farm data.
-        ct_max: float
-            The maximal value for ct, values beyond will be limited
-            to this number
-        k_var: str
-            The variable name for k
-
-        """
-        super().__init__(superpositions={FV.WS: superposition}, ct_max=ct_max)
-
-        self.k_var = k_var
-        setattr(self, k_var, k)
-
-    def __repr__(self):
-        k = getattr(self, self.k_var)
-        s = super().__repr__()
-        s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
-        return s
-
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
-        """
-        Initialize wake delta storage.
-
-        They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        n_points: int
-            The number of wake evaluation points
-        wake_deltas: dict
-            The wake deltas storage, add wake deltas
-            on the fly. Keys: Variable name str, for which the
-            wake delta applies, values: numpy.ndarray with
-            shape (n_states, n_points, ...)
-
-        """
-        n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-
-    def calc_wake_radius(self, algo, mdata, fdata, states_source_turbine, x, ct):
+        ti_superp: str
+            The method choice: linear, quadratic, max
+        superp_to_amb: str
+            The method for combining ambient with wake deltas:
+            linear or quadratic
+
+        """
+        super().__init__()
+
+        self.ti_superp = ti_superp
+        self.superp_to_amb = superp_to_amb
+
+    def calc_wakes_plus_wake(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        sel_sp,
+        variable,
+        wake_delta,
+        wake_model_result,
+    ):
         """
-        Calculate the wake radius, depending on x only (not r).
+        Add a wake delta to previous wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
-        x: numpy.ndarray
-            The x values, shape: (n_states, n_points)
-        r: numpy.ndarray
-            The radial values for each x value, shape:
-            (n_states, n_points, n_r_per_x, 2)
-        ct: numpy.ndarray
-            The ct values of the wake-causing turbines,
-            shape: (n_states, n_points)
+        sel_sp: numpy.ndarray of bool
+            The selection of points, shape: (n_states, n_points)
+        variable: str
+            The variable name for which the wake deltas applies
+        wake_delta: numpy.ndarray
+            The original wake deltas, shape: (n_states, n_points)
+        wake_model_result: numpy.ndarray
+            The new wake deltas of the selected points,
+            shape: (n_sel_sp,)
 
         Returns
         -------
-        wake_r: numpy.ndarray
-            The wake radii, shape: (n_states, n_points)
+        wdelta: numpy.ndarray
+            The updated wake deltas, shape: (n_states, n_points)
 
         """
-        n_states = mdata.n_states
-        st_sel = (np.arange(n_states), states_source_turbine)
-
-        R = fdata[FV.D][st_sel][:, None] / 2
-        k = self.get_data(self.k_var, fdata, st_sel)
 
-        if isinstance(k, np.ndarray):
-            k = k[:, None]
-
-        return R + k * x
-
-    def calc_centreline_wake_deltas(
-        self, algo, mdata, fdata, states_source_turbine, sp_sel, x, wake_r, ct
+        # superposition of every turbines efect at each target point
+        # linear ti delta:
+        if self.ti_superp == "linear":
+            wake_delta[sel_sp] += wake_model_result
+
+        # quadratic ti delta:
+        elif self.ti_superp == "quadratic":
+            wake_delta[sel_sp] += wake_model_result**2
+
+        # max ti delta:
+        elif self.ti_superp == "max":
+            wake_delta[sel_sp] = np.maximum(wake_model_result, wake_delta[sel_sp])
+
+        # unknown ti delta:
+        else:
+            raise ValueError(
+                f"Unknown ti_superp = '{self.ti_superp}', valid choices: linear, quadratic, max"
+            )
+
+        return wake_delta
+
+    def calc_final_wake_delta(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
-        Calculate centre line results of wake deltas.
+        Calculate the final wake delta after adding all
+        contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        states_source_turbine: numpy.ndarray
-            For each state, one turbine index for the
-            wake causing turbine. Shape: (n_states,)
-        sp_sel: numpy.ndarray of bool
-            The state-point selection, for which the wake
-            is non-zero, shape: (n_states, n_points)
-        x: numpy.ndarray
-            The x values, shape: (n_sp_sel,)
-        wake_r: numpy.ndarray
-            The wake radii, shape: (n_sp_sel,)
-        ct: numpy.ndarray
-            The ct values of the wake-causing turbines,
-            shape: (n_sp_sel,)
+        pdata: foxes.core.Data
+            The evaluation point data
+        variable: str
+            The variable name for which the wake deltas applies
+        amb_results: numpy.ndarray
+            The ambient results, shape: (n_states, n_points)
+        wake_delta: numpy.ndarray
+            The wake deltas, shape: (n_states, n_points)
 
         Returns
         -------
-        cl_del: dict
-            The centre line wake deltas. Key: variable name str,
-            varlue: numpy.ndarray, shape: (n_sp_sel,)
-
-        """
-        n_states = mdata.n_states
-        n_points = sp_sel.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
-
-        R = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        R[:] = fdata[FV.D][st_sel][:, None] / 2
-        R = R[sp_sel]
-
-        return {FV.WS: -((R / wake_r) ** 2) * (1.0 - np.sqrt(1.0 - ct))}
+        final_wake_delta: numpy.ndarray
+            The final wake delta, which will be added to the ambient
+            results by simple plus operation. Shape: (n_states, n_points)
+
+        """
+        # linear superposition to ambient:
+        if self.superp_to_amb == "linear":
+            if self.ti_superp == "linear" or self.ti_superp == "max":
+                return wake_delta
+            elif self.ti_superp == "quadratic":
+                return np.sqrt(wake_delta)
+            else:
+                raise ValueError(
+                    f"Unknown ti_superp = '{self.ti_superp}', valid choices: linear, quadratic, max"
+                )
+
+        # quadratic superposition to ambient:
+        elif self.superp_to_amb == "quadratic":
+            if self.ti_superp == "linear" or self.ti_superp == "max":
+                return np.sqrt(wake_delta**2 + amb_results**2) - amb_results
+            elif self.ti_superp == "quadratic":
+                return np.sqrt(wake_delta + amb_results**2) - amb_results
+            else:
+                raise ValueError(
+                    f"Unknown ti_superp = '{self.ti_superp}', valid choices: linear, quadratic, max"
+                )
+
+        # unknown ti delta:
+        else:
+            raise ValueError(
+                f"Unknown superp_to_amb = '{self.superp_to_amb}', valid choices: linear, quadratic"
+            )
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/wind/porte_agel.py` & `foxes-0.4.1/foxes/models/wake_models/wind/porte_agel.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 
 class PorteAgelModel(Model):
     """
     Common calculations for the wake model and the wake
     frame, such that code repetitions can be avoided.
 
-    Based on Bastankhah & Porte-Agel, 2016, 
+    Based on Bastankhah & Porte-Agel, 2016,
     https://doi.org/10.1017/jfm.2016.595
 
     Attributes
     ----------
     ct_max: float
         The maximal value for ct, values beyond will be limited
         to this number, by default 0.9999
     alpha: float
         model parameter used to determine onset of far wake region
     beta: float
         model parameter used to determine onset of far wake region
-    
+
     :group: models.wake_models.wind
 
     """
 
     MDATA_KEY = "PorteAgelModel"
     PARS = "pars"
     CHECK = "check"
@@ -44,15 +44,15 @@
     SIGMA_Y_FAR = "sigma_y_far"
     SIGMA_Z_FAR = "sigma_z_far"
     DELTA_FAR = "delta_far"
 
     def __init__(self, ct_max=0.9999, alpha=0.58, beta=0.07):
         """
         Constructor.
-        
+
         Parameters
         ----------
         ct_max: float
             The maximal value for ct, values beyond will be limited
             to this number, by default 0.9999
         alpha: float
             model parameter used to determine onset of far wake region
@@ -78,94 +78,143 @@
         """
         alpha = getattr(self, FV.PA_ALPHA)
         beta = getattr(self, FV.PA_BETA)
         return dict(alpha=alpha, beta=beta, ct_max=self.ct_max)
 
     def calc_data(
         self,
+        algo,
         mdata,
         fdata,
+        pdata,
         states_source_turbine,
         x,
         gamma,
         k,
     ):
         """
         Calculate common model data, store it in mdata.
 
         Parameters
         ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         gamma: numpy.ndarray
             The YAWM angles in radiants, shape: (n_states, n_points)
         k: numpy.ndarray
             The k parameter values, shape: (n_states, n_points)
 
         """
-        # prepare:
-        n_states = mdata.n_states
-        n_points = x.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
-
 
         # store parameters:
         out = {self.PARS: self.pars}
         out[self.CHECK] = (
             mdata[FC.STATE][0],
             states_source_turbine[0],
             x.shape,
         )
 
         # get D:
-        D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        D[:] = fdata[FV.D][st_sel][:, None]
+        D = super().get_data(
+            FV.D,
+            FC.STATE_POINT,
+            lookup="f",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
 
         # get ct:
-        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ct[:] = fdata[FV.CT][st_sel][:, None]
+        ct = super().get_data(
+            FV.CT,
+            FC.STATE_POINT,
+            lookup="f",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
             # get ws:
-            ws = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            ws[:] = fdata[FV.REWS][st_sel][:, None]
+            ws = super().get_data(
+                FV.REWS,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
 
             # get TI:
-            ti = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            ti[:] = fdata[FV.TI][st_sel][:, None]
+            ti = super().get_data(
+                FV.TI,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
 
             # get alpha:
-            alpha = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            alpha[:] = Model.get_data(self, FV.PA_ALPHA, fdata, data_prio=True, upcast="farm")[st_sel][:, None]
+            alpha = super().get_data(
+                FV.PA_ALPHA,
+                FC.STATE_POINT,
+                lookup="fs",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
 
             # get beta:
-            beta = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            beta[:] = Model.get_data(self, FV.PA_BETA, fdata, data_prio=True, upcast="farm")[st_sel][:, None]
+            beta = super().get_data(
+                FV.PA_BETA,
+                FC.STATE_POINT,
+                lookup="fs",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
 
             # apply filter:
             x = x[sp_sel]
             D = D[sp_sel]
             ct = ct[sp_sel]
             ws = ws[sp_sel]
             ti = ti[sp_sel]
             k = k[sp_sel]
             gamma = gamma[sp_sel]
             alpha = alpha[sp_sel]
             beta = beta[sp_sel]
-        
+
             # calc theta_c0, Eq. (6.12):
             cosg = np.cos(gamma)
             theta = 0.3 * gamma / cosg * (1 - np.sqrt(1 - ct * cosg))
 
             # calculate x0, Eq. (7.3):
             sqomct = np.sqrt(1 - ct)
             x0 = (
@@ -306,15 +355,15 @@
         del mdata[self.MDATA_KEY]
 
 
 class PorteAgelWake(DistSlicedWakeModel):
     """
     The Bastankhah PorteAgel wake model
 
-    Based on Bastankhah & Porte-Agel, 2016, 
+    Based on Bastankhah & Porte-Agel, 2016,
     https://doi.org/10.1017/jfm.2016.595
 
     Attributes
     ----------
     model: PorteAgelModel
         The model for computing common data
     K: float
@@ -327,25 +376,25 @@
         The variable name for k
 
     :group: models.wake_models.wind
 
     """
 
     def __init__(
-            self, 
-            superposition, 
-            k=None, 
-            ct_max=0.9999, 
-            alpha=0.58, 
-            beta=0.07, 
-            k_var=FV.K,
-        ):
+        self,
+        superposition,
+        k=None,
+        ct_max=0.9999,
+        alpha=0.58,
+        beta=0.07,
+        k_var=FV.K,
+    ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superposition: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
         k: float
@@ -372,52 +421,63 @@
 
     def __repr__(self):
         k = getattr(self, self.k_var)
         s = super().__repr__()
         s += f"({self.k_var}={k}, sp={self.superpositions[FV.WS]})"
         return s
 
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
+    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        n_points: int
-            The number of wake evaluation points
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
 
-    def calc_wakes_spsel_x_yz(self, algo, mdata, fdata, states_source_turbine, x, yz):
+    def calc_wakes_spsel_x_yz(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+        yz,
+    ):
         """
         Calculate wake deltas.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
         yz: numpy.ndarray
             The yz values for each x value, shape:
@@ -429,35 +489,52 @@
             The wake deltas. Key: variable name str,
             value: numpy.ndarray, shape: (n_sp_sel, n_yz_per_x)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
+
         # prepare:
         n_states = mdata.n_states
         n_points = x.shape[1]
         n_y_per_z = yz.shape[2]
         st_sel = (np.arange(n_states), states_source_turbine)
 
         # calculate model data:
         if not self.model.has_data(mdata, states_source_turbine, x):
             # get gamma:
-            gamma = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            gamma[:] = self.get_data(FV.YAWM, fdata, upcast="farm", data_prio=True)[
-                st_sel
-            ][:, None]
+            gamma = self.get_data(
+                FV.YAWM,
+                FC.STATE_POINT,
+                lookup="fs",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
             gamma *= np.pi / 180
 
             # get k:
-            k = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            k[:] = self.get_data(self.k_var, fdata, upcast="farm")[st_sel][:, None]
+            k = self.get_data(
+                self.k_var,
+                FC.STATE_POINT,
+                lookup="sf",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
 
             # run calculation:
-            self.model.calc_data(mdata, fdata, states_source_turbine, x, gamma, k)
+            self.model.calc_data(
+                algo, mdata, fdata, pdata, states_source_turbine, x, gamma, k
+            )
 
         # select targets:
         sp_sel = self.model.get_data(PorteAgelModel.SP_SEL, mdata)
         n_sp_sel = np.sum(sp_sel)
         wdeltas = {FV.WS: np.zeros((n_sp_sel, n_y_per_z), dtype=FC.DTYPE)}
         if np.any(sp_sel):
             # apply filter:
```

### Comparing `foxes-0.4.0/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.4.1/foxes/models/wake_models/wind/turbopark.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
 
     def __init__(
         self, superposition, A, sbeta_factor=0.25, ct_max=0.9999, c1=1.5, c2=0.8
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
         A: float
@@ -63,53 +63,63 @@
         self.c2 = c2
 
     def __repr__(self):
         s = super().__repr__()
         s += f"(A={self.A}, sp={self.superpositions[FV.WS]})"
         return s
 
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
+    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        n_points: int
-            The number of wake evaluation points
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
 
-    def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
+    def calc_amplitude_sigma_spsel(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+    ):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
@@ -118,39 +128,59 @@
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
-        # prepare:
-        n_states = mdata.n_states
-        n_points = x.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
 
         # get ct:
-        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ct[:] = fdata[FV.CT][st_sel][:, None]
+        ct = self.get_data(
+            FV.CT,
+            FC.STATE_POINT,
+            lookup="f",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
             # apply selection:
             x = x[sp_sel]
             ct = ct[sp_sel]
 
             # get D:
-            D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            D[:] = fdata[FV.D][st_sel][:, None]
+            D = self.get_data(
+                FV.D,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
             D = D[sp_sel]
 
             # get TI:
-            ati = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            ati[:] = fdata[FV.AMB_TI][st_sel][:, None]
+            ati = self.get_data(
+                FV.AMB_TI,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
             ati = ati[sp_sel]
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             # sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
             # sbeta[sbeta > sblim] = sblim
             epsilon = self.sbeta_factor * sbeta
@@ -237,15 +267,15 @@
         sbeta_factor=0.25,
         ct_max=0.9999,
         ti_var=FV.TI,
         **ipars,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         superpositions: dict
             The superpositions. Key: variable name str,
             value: The wake superposition model name,
             will be looked up in model book
         dx: float
@@ -273,53 +303,63 @@
         self.ipars = ipars
 
     def __repr__(self):
         s = super().__repr__()
         s += f"(ti={self.ti_var}, dx={self.dx}, A={self.A}, sp={self.superpositions[FV.WS]})"
         return s
 
-    def init_wake_deltas(self, algo, mdata, fdata, n_points, wake_deltas):
+    def init_wake_deltas(self, algo, mdata, fdata, pdata, wake_deltas):
         """
         Initialize wake delta storage.
 
         They are added on the fly to the wake_deltas dict.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
-        n_points: int
-            The number of wake evaluation points
+        pdata: foxes.core.Data
+            The evaluation point data
         wake_deltas: dict
             The wake deltas storage, add wake deltas
             on the fly. Keys: Variable name str, for which the
             wake delta applies, values: numpy.ndarray with
             shape (n_states, n_points, ...)
 
         """
         n_states = mdata.n_states
-        wake_deltas[FV.WS] = np.zeros((n_states, n_points), dtype=FC.DTYPE)
+        wake_deltas[FV.WS] = np.zeros((n_states, pdata.n_points), dtype=FC.DTYPE)
 
-    def calc_amplitude_sigma_spsel(self, algo, mdata, fdata, states_source_turbine, x):
+    def calc_amplitude_sigma_spsel(
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        states_source_turbine,
+        x,
+    ):
         """
         Calculate the amplitude and the sigma,
         both depend only on x (not on r).
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         x: numpy.ndarray
             The x values, shape: (n_states, n_points)
 
         Returns
@@ -328,34 +368,46 @@
             The amplitude and sigma, both numpy.ndarray
             with shape (n_sp_sel,)
         sp_sel: numpy.ndarray of bool
             The state-point selection, for which the wake
             is non-zero, shape: (n_states, n_points)
 
         """
-        # prepare:
-        n_states = mdata.n_states
-        n_points = x.shape[1]
-        st_sel = (np.arange(n_states), states_source_turbine)
 
         # get ct:
-        ct = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-        ct[:] = fdata[FV.CT][st_sel][:, None]
+        ct = self.get_data(
+            FV.CT,
+            FC.STATE_POINT,
+            lookup="f",
+            algo=algo,
+            fdata=fdata,
+            pdata=pdata,
+            upcast=True,
+            states_source_turbine=states_source_turbine,
+        )
         ct[ct > self.ct_max] = self.ct_max
 
         # select targets:
         sp_sel = (x > 1e-5) & (ct > 0.0)
         if np.any(sp_sel):
             # apply selection:
             # x = x[sp_sel]
             ct = ct[sp_sel]
 
             # get D:
-            D = np.zeros((n_states, n_points), dtype=FC.DTYPE)
-            D[:] = fdata[FV.D][st_sel][:, None]
+            D = self.get_data(
+                FV.D,
+                FC.STATE_POINT,
+                lookup="f",
+                algo=algo,
+                fdata=fdata,
+                pdata=pdata,
+                upcast=True,
+                states_source_turbine=states_source_turbine,
+            )
             D = D[sp_sel]
 
             # calculate sigma:
             sbeta = np.sqrt(0.5 * (1 + np.sqrt(1.0 - ct)) / np.sqrt(1.0 - ct))
             # sblim = 1 / (np.sqrt(8) * self.sbeta_factor)
             # sbeta[sbeta > sblim] = sblim
             epsilon = self.sbeta_factor * sbeta
```

### Comparing `foxes-0.4.0/foxes/models/wake_superpositions/linear.py` & `foxes-0.4.1/foxes/models/wake_superpositions/linear.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,50 +17,87 @@
         The scaling rules
     lim_low: dict
         Lower limits of the final wake deltas. Key: variable str,
         value: float
     lim_high: dict
         Higher limits of the final wake deltas. Key: variable str,
         value: float
+    svars: list of str
+        The scaling vafriables
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, scalings, lim_low=None, lim_high=None):
+    def __init__(self, scalings, lim_low=None, lim_high=None, svars=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         scalings: dict or number or str
             Scaling rules. If `dict`, key: variable name str,
             value: number or str. If `str`:
             - `source_turbine`: Scale by source turbine value of variable
             - `source_turbine_amb`: Scale by source turbine ambient value of variable
             - `source_turbine_<var>`: Scale by source turbine value of variable <var>
         lim_low: dict, optional
             Lower limits of the final wake deltas. Key: variable str,
             value: float
         lim_high: dict, optional
             Higher limits of the final wake deltas. Key: variable str,
             value: float
+        svars: list of str, optional
+            The scaling vafriables
 
         """
         super().__init__()
 
         self.scalings = scalings
         self.lim_low = lim_low
         self.lim_high = lim_high
+        self.svars = svars
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        if self.svars is not None:
+            return self.svars
+        elif isinstance(self.scalings, dict):
+            return list(self.scalings.keys())
+        elif (
+            isinstance(self.scalings, str)
+            and len(self.scalings) > 15
+            and self.scalings[:15] == "source_turbine_"
+        ):
+            return [self.scalings[15:]]
+        else:
+            raise ValueError(
+                f"{self.name}: Unable to determine scaling variable for scaling = '{self.scalings}'"
+            )
 
     def calc_wakes_plus_wake(
         self,
         algo,
         mdata,
         fdata,
+        pdata,
         states_source_turbine,
         sel_sp,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
@@ -70,14 +107,16 @@
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
         variable: str
             The variable name for which the wake deltas applies
@@ -148,28 +187,37 @@
 
         else:
             raise ValueError(
                 f"Model '{self.name}': Invalid scaling choice '{scaling}' for wake variable '{variable}', valid choices: None, <scalar>, 'source_turbine', 'source_turbine_amb', 'source_turbine_<var>'"
             )
 
     def calc_final_wake_delta(
-        self, algo, mdata, fdata, variable, amb_results, wake_delta
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
         wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
```

### Comparing `foxes-0.4.0/foxes/models/wake_superpositions/max.py` & `foxes-0.4.1/foxes/models/wake_superpositions/max.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,71 @@
     Maximum supersposition of wake model results,
     optionally rescaled.
 
     Attributes
     ----------
     scalings: dict or number or str
         The scaling rules
+    svars: list of str
+        The scaling variables
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, scalings):
+    def __init__(self, scalings, svars=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         scalings: dict or number or str
             Scaling rules. If `dict`, key: variable name str,
             value: number or str. If `str`:
             - `source_turbine`: Scale by source turbine value of variable
             - `source_turbine_amb`: Scale by source turbine ambient value of variable
             - `source_turbine_<var>`: Scale by source turbine value of variable <var>
+        svars: list of str, optional
+            The scaling variables
 
         """
         super().__init__()
         self.scalings = scalings
+        self.svars = svars
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        if self.svars is not None:
+            return self.svars
+        elif isinstance(self.scalings, dict):
+            return list(self.scalings.keys())
+        elif (
+            isinstance(self.scalings, str)
+            and len(self.scalings) > 15
+            and self.scalings[:15] == "source_turbine_"
+        ):
+            return [self.scalings[15:]]
+        else:
+            raise ValueError(
+                f"{self.name}: Unable to determine scaling variable for scaling = '{self.scalings}'"
+            )
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -66,14 +102,15 @@
         return super().initialize(algo, verbosity)
 
     def calc_wakes_plus_wake(
         self,
         algo,
         mdata,
         fdata,
+        pdata,
         states_source_turbine,
         sel_sp,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
@@ -83,14 +120,16 @@
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
         variable: str
             The variable name for which the wake deltas applies
@@ -175,28 +214,37 @@
 
         else:
             raise ValueError(
                 f"Model '{self.name}': Invalid scaling choice '{scaling}' for wake variable '{variable}', valid choices: None, <scalar>, 'source_turbine', 'source_turbine_amb', 'source_turbine_<var>'"
             )
 
     def calc_final_wake_delta(
-        self, algo, mdata, fdata, variable, amb_results, wake_delta
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
         wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
```

### Comparing `foxes-0.4.0/foxes/models/wake_superpositions/product.py` & `foxes-0.4.1/foxes/models/wake_superpositions/product.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
-import numbers
 
 from foxes.core import WakeSuperposition
 import foxes.variables as FV
-import foxes.constants as FC
 
 
 class ProductSuperposition(WakeSuperposition):
     """
     Product wind wake superposition.
 
     This is based on the idea that the dimensionless
@@ -30,15 +28,15 @@
     :group: models.wake_superpositions
 
     """
 
     def __init__(self, lim_low=None, lim_high=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         lim_low: dict, optional
             Lower limits of the final wake deltas. Key: variable str,
             value: float
         lim_high: dict, optional
             Higher limits of the final wake deltas. Key: variable str,
@@ -50,14 +48,15 @@
         self.lim_high = lim_high
 
     def calc_wakes_plus_wake(
         self,
         algo,
         mdata,
         fdata,
+        pdata,
         states_source_turbine,
         sel_sp,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
@@ -67,14 +66,16 @@
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
         variable: str
             The variable name for which the wake deltas applies
@@ -93,28 +94,37 @@
 
         if np.max(np.abs(wake_delta)) < 1e-14:
             wake_delta[:] = 1
         wake_delta[sel_sp] *= 1 + wake_model_result
         return wake_delta
 
     def calc_final_wake_delta(
-        self, algo, mdata, fdata, variable, amb_results, wake_delta
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
         wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
```

### Comparing `foxes-0.4.0/foxes/models/wake_superpositions/quadratic.py` & `foxes-0.4.1/foxes/models/wake_superpositions/quadratic.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,35 +11,71 @@
     Quadratic supersposition of wake model results,
     optionally rescaled.
 
     Attributes
     ----------
     scalings: dict or number or str
         The scaling rules
+    svars: list of str
+        The scaling variables
 
     :group: models.wake_superpositions
 
     """
 
-    def __init__(self, scalings):
+    def __init__(self, scalings, svars=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         scalings: dict or number or str
             Scaling rules. If `dict`, key: variable name str,
             value: number or str. If `str`:
             - `source_turbine`: Scale by source turbine value of variable
             - `source_turbine_amb`: Scale by source turbine ambient value of variable
             - `source_turbine_<var>`: Scale by source turbine value of variable <var>
+        svars: list of str, optional
+            The scaling variables
 
         """
         super().__init__()
         self.scalings = scalings
+        self.svars = svars
+
+    def input_farm_vars(self, algo):
+        """
+        The variables which are needed for running
+        the model.
+
+        Parameters
+        ----------
+        algo: foxes.core.Algorithm
+            The calculation algorithm
+
+        Returns
+        -------
+        input_vars: list of str
+            The input variable names
+
+        """
+        if self.svars is not None:
+            return self.svars
+        elif isinstance(self.scalings, dict):
+            return list(self.scalings.keys())
+        elif (
+            isinstance(self.scalings, str)
+            and len(self.scalings) > 15
+            and self.scalings[:15] == "source_turbine_"
+        ):
+            return [self.scalings[15:]]
+        else:
+            raise ValueError(
+                f"{self.name}: Unable to determine scaling variable for scaling = '{self.scalings}'"
+            )
 
     def initialize(self, algo, verbosity=0):
         """
         Initializes the model.
 
         This includes loading all required data from files. The model
         should return all array type data as part of the idata return
@@ -66,14 +102,15 @@
         return super().initialize(algo, verbosity)
 
     def calc_wakes_plus_wake(
         self,
         algo,
         mdata,
         fdata,
+        pdata,
         states_source_turbine,
         sel_sp,
         variable,
         wake_delta,
         wake_model_result,
     ):
         """
@@ -83,14 +120,16 @@
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         states_source_turbine: numpy.ndarray
             For each state, one turbine index for the
             wake causing turbine. Shape: (n_states,)
         sel_sp: numpy.ndarray of bool
             The selection of points, shape: (n_states, n_points)
         variable: str
             The variable name for which the wake deltas applies
@@ -169,28 +208,37 @@
 
         else:
             raise ValueError(
                 f"Model '{self.name}': Invalid scaling choice '{scaling}' for wake variable '{variable}', valid choices: None, <scalar>, 'source_turbine', 'source_turbine_amb', 'source_turbine_<var>'"
             )
 
     def calc_final_wake_delta(
-        self, algo, mdata, fdata, variable, amb_results, wake_delta
+        self,
+        algo,
+        mdata,
+        fdata,
+        pdata,
+        variable,
+        amb_results,
+        wake_delta,
     ):
         """
         Calculate the final wake delta after adding all
         contributions.
 
         Parameters
         ----------
         algo: foxes.core.Algorithm
             The calculation algorithm
         mdata: foxes.core.Data
             The model data
         fdata: foxes.core.Data
             The farm data
+        pdata: foxes.core.Data
+            The evaluation point data
         variable: str
             The variable name for which the wake deltas applies
         amb_results: numpy.ndarray
             The ambient results, shape: (n_states, n_points)
         wake_delta: numpy.ndarray
             The wake deltas, shape: (n_states, n_points)
```

### Comparing `foxes-0.4.0/foxes/opt/constraints/area_geometry.py` & `foxes-0.4.1/foxes/opt/constraints/area_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         The selected turbines
     geometry: foxes.utils.geom2d.AreaGeometry
         The area geometry
     disc_inside: bool
         Ensure full rotor disc inside boundary
     D: float
         Use this radius for rotor disc inside condition
-    
+
     :group: opt.constraints
 
     """
 
     def __init__(
         self,
         problem,
@@ -34,15 +34,15 @@
         sel_turbines=None,
         disc_inside=False,
         D=None,
         **kwargs,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem : foxes.opt.FarmOptProblem
             The underlying optimization problem
         name : str
             The name of the constraint
         geometry : foxes.utils.geom2d.AreaGeometry
@@ -194,15 +194,15 @@
     :group: opt.constraints
 
     """
 
     def __init__(self, problem, name="boundary", **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
             The underlying optimization problem
         name: str
             The name of the constraint
         kwargs: dict, optional
```

### Comparing `foxes-0.4.0/foxes/opt/constraints/min_dist.py` & `foxes-0.4.1/foxes/opt/constraints/min_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
 from foxes.opt.core.farm_constraint import FarmConstraint
 import foxes.variables as FV
 import foxes.constants as FC
 
+
 class MinDistConstraint(FarmConstraint):
     """
     Turbines must keep at least a minimal
     spatial distance.
 
     Attributes
     ----------
@@ -31,15 +32,15 @@
         min_dist_unit="m",
         name="dist",
         sel_turbines=None,
         **kwargs,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
             The underlying optimization problem
         min_dist: float
             The minimal distance
         min_dist_unit: str
```

### Comparing `foxes-0.4.0/foxes/opt/core/farm_constraint.py` & `foxes-0.4.1/foxes/opt/core/farm_constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     :group: opt.core
 
     """
 
     def __init__(self, problem, name, sel_turbines=None, **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
             The underlying optimization problem
         name: str
             The name of the constraint
         sel_turbines: list of int, optional
```

### Comparing `foxes-0.4.0/foxes/opt/core/farm_objective.py` & `foxes-0.4.1/foxes/opt/core/farm_objective.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     :group: opt.core
 
     """
 
     def __init__(self, problem, name, sel_turbines=None, **kwargs):
         """
         Constraints.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
             The underlying optimization problem
         name: str
             The name of the objective function
         sel_turbines: list of int, optional
```

### Comparing `foxes-0.4.0/foxes/opt/core/farm_opt_problem.py` & `foxes-0.4.1/foxes/opt/core/farm_opt_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         sel_turbines=None,
         calc_farm_args={},
         points=None,
         **kwargs,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         name: str
             The problem's name
         algo: foxes.core.Algorithm
             The algorithm
         runner: foxes.core.Runner, optional
@@ -192,27 +192,27 @@
             is original states and problem model names
         verbosity: int
             The verbosity level, 0 = silent
 
         """
         if exclude is None:
             exclude = [self._org_states_name]
-        self.algo.keep_models.append(self._org_states_name)
+        self.algo.keep_models.add(self._org_states_name)
         for mname, idata in self.algo.idata_mem.items():
             if mname not in exclude and self.name not in mname:
                 keep = True
                 for d in idata["data_vars"].values():
                     for dropv in drop_vars:
                         if dropv in d[0]:
                             keep = False
                             break
                     if not keep:
                         break
                 if keep:
-                    self.algo.keep_models.append(mname)
+                    self.algo.keep_models.add(mname)
 
     def initialize(self, drop_vars=[FC.STATE], exclude=None, verbosity=1):
         """
         Initialize the object.
 
         Parameters
         ----------
@@ -321,15 +321,17 @@
         self._count += 1
         self.update_problem_individual(vars_int, vars_float)
         farm_results = self.runner.run(self.algo.calc_farm, kwargs=self.calc_farm_args)
 
         if self.points is None:
             return farm_results
         else:
-            point_results = self.runner.run(self.algo.calc_points, args=(farm_results, self.points))
+            point_results = self.runner.run(
+                self.algo.calc_points, args=(farm_results, self.points)
+            )
             return farm_results, point_results
 
     def apply_population(self, vars_int, vars_float):
         """
         Apply new variables to the problem,
         for a whole population.
 
@@ -356,17 +358,19 @@
 
         if self.points is None:
             return farm_results
         else:
             n_pop = farm_results["n_pop"].values
             n_states, n_points = self.points.shape[:2]
             pop_points = np.zeros((n_pop, n_states, n_points, 3), dtype=FC.DTYPE)
-            pop_points[:] = self.points[None, :, : , :]
-            pop_points = pop_points.reshape(n_pop*n_states, n_points, 3)
-            point_results = self.runner.run(self.algo.calc_points, args=(farm_results, pop_points))
+            pop_points[:] = self.points[None, :, :, :]
+            pop_points = pop_points.reshape(n_pop * n_states, n_points, 3)
+            point_results = self.runner.run(
+                self.algo.calc_points, args=(farm_results, pop_points)
+            )
             return farm_results, point_results
 
     def add_to_layout_figure(self, ax, **kwargs):
         """
         Add to a layout figure
 
         Parameters
```

### Comparing `foxes-0.4.0/foxes/opt/core/farm_vars_problem.py` & `foxes-0.4.1/foxes/opt/core/farm_vars_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class FarmVarsProblem(FarmOptProblem):
     """
     Abstract base class for models that optimize
     farm variables.
 
     :group: opt.core
-    
+
     """
 
     def initialize(self, pre_rotor_vars, post_rotor_vars, verbosity=1, **kwargs):
         """
         Initialize the object.
 
         Parameters
```

### Comparing `foxes-0.4.0/foxes/opt/core/pop_states.py` & `foxes-0.4.1/foxes/core/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,200 +1,221 @@
 import numpy as np
 
-from foxes.core import States, Data
-import foxes.constants as FC
+from foxes.utils import Dict
 import foxes.variables as FV
+import foxes.constants as FC
 
 
-class PopStates(States):
+class Data(Dict):
     """
-    Helper class for vectorized opt population
-    calculation, via artificial states of length
-    n_pop times n_states.
+    Container for data and meta data.
+
+    Used during the calculation of single chunks,
+    usually for numpy data (not xarray data).
 
     Attributes
     ----------
-    states: foxes.core.States
-        The original states
-    n_pop: int
-        The population size
+    dims: dict
+        The dimensions tuples, same or subset
+        of data keys
+    loop_dims: array_like of str
+        List of the loop dimensions during xarray's
+        `apply_ufunc` calculations
+    sizes: dict
+        The dimension sizes
 
-    :group: opt.core
+    :group: core
 
     """
 
-    def __init__(self, states, n_pop):
+    def __init__(self, data, dims, loop_dims, name="data"):
         """
         Constructor.
-        
+
         Parameters
         ----------
-        states: foxes.core.States
-            The original states
-        n_pop: int
-            The population size
+        data: dict
+            The initial data to be stored
+        dims: dict
+            The dimensions tuples, same or subset
+            of data keys
+        loop_dims: array_like of str
+            List of the loop dimensions during xarray's
+            `apply_ufunc` calculations
+        name: str
+            The data container name
+
+        """
+        super().__init__(name=name)
+
+        self.update(data)
+        self.dims = dims
+        self.loop_dims = loop_dims
+
+        self.sizes = {}
+        for v, d in data.items():
+            self.__run_entry_checks(v, d, dims[v])
 
-        """
-        super().__init__()
-        self.states = states
-        self.n_pop = n_pop
+        self.__auto_update()
 
-    def initialize(self, algo, verbosity=0):
+    @property
+    def n_states(self):
         """
-        Initializes the model.
-
-        This includes loading all required data from files. The model
-        should return all array type data as part of the idata return
-        dictionary (and not store it under self, for memory reasons). This
-        data will then be chunked and provided as part of the mdata object
-        during calculations.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        verbosity: int
-            The verbosity level, 0 = silent
+        The number of states
 
         Returns
         -------
-        idata: dict
-            The dict has exactly two entries: `data_vars`,
-            a dict with entries `name_str -> (dim_tuple, data_ndarray)`;
-            and `coords`, a dict with entries `dim_name_str -> dim_array`
+        int:
+            The number of states
 
         """
-        self.STATE0 = self.var(FC.STATE + "0")
-        self.SMAP = self.var("SMAP")
-
-        idata = super().initialize(algo, verbosity)
-        self._update_idata(algo, idata)
-
-        if not self.states.name in algo._idata_mem:
-            raise KeyError(
-                f"States idata '{self.states.name}' not found in algo idata memory"
-            )
-        else:
-            idata0 = algo._idata_mem[self.states.name]
-
-        for cname, coord in idata0["coords"].items():
-            if cname != FC.STATE:
-                idata["coords"][cname] = coord
-            else:
-                idata["coords"][self.STATE0] = coord
-
-        for dname, (dims0, data0) in idata0["data_vars"].items():
-            if dname != FV.WEIGHT:
-                hdims = tuple([d if d != FC.STATE else self.STATE0 for d in dims0])
-                idata["data_vars"][dname] = (hdims, data0)
-
-        smap = np.zeros((self.n_pop, self.states.size()), dtype=np.int32)
-        smap[:] = np.arange(self.states.size())[None, :]
-        smap = smap.reshape(self.size())
-        idata["data_vars"][self.SMAP] = ((FC.STATE,), smap)
-
-        found = False
-        for dname, (dims0, data0) in idata["data_vars"].items():
-            if self.STATE0 in dims0:
-                found = True
-                break
-        if not found:
-            del idata["coords"][self.STATE0]
-
-        return idata
+        return self.sizes[FC.STATE] if FC.STATE in self.sizes else None
 
-    def size(self):
+    @property
+    def n_turbines(self):
         """
-        The total number of states.
+        The number of turbines
 
         Returns
         -------
         int:
-            The total number of states
+            The number of turbines
 
         """
-        return self.states.size() * self.n_pop
+        return self.sizes[FC.TURBINE] if FC.TURBINE in self.sizes else None
 
-    def weights(self, algo):
+    @property
+    def n_points(self):
         """
-        The statistical weights of all states.
-
-        Parameters
-        ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+        The number of points
 
         Returns
         -------
-        weights: numpy.ndarray
-            The weights, shape: (n_states, n_turbines)
+        int:
+            The number of points
 
         """
-        weights = np.zeros(
-            (self.n_pop, self.states.size(), algo.n_turbines), dtype=FC.DTYPE
-        )
-        weights[:] = self.states.weights(algo)[None, :, :] / self.n_pop
-        return weights.reshape(self.size(), algo.n_turbines)
+        return self.sizes[FC.POINT] if FC.POINT in self.sizes else None
 
-    def output_point_vars(self, algo):
+    def states_i0(self, counter=False, algo=None):
         """
-        The variables which are being modified by the model.
+        Get the state counter for first state in chunk
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
+        counter: bool
+            Return the state counter instead of the index
+        algo: foxes.core.Algorithm, optional
+            The algorithm, required for state counter
 
         Returns
         -------
-        output_vars: list of str
-            The output variable names
+        int:
+            The state counter for first state in chunk
+            or the corresponding index
 
         """
-        return self.states.output_point_vars(algo)
+        if FC.STATE not in self:
+            return None
+        elif counter:
+            if algo is None:
+                raise KeyError(f"{self.name}: Missing algo for deducing state counter")
+            return np.argwhere(algo.states.index() == self[FC.STATE][0])[0][0]
+        else:
+            return self[FC.STATE][0]
+
+    def __auto_update(self):
+        data = self
+        dims = self.dims
+
+        if (
+            FV.TXYH not in data
+            and FV.X in data
+            and FV.Y in data
+            and FV.H in data
+            and dims[FV.X] == (FC.STATE, FC.TURBINE)
+            and dims[FV.Y] == (FC.STATE, FC.TURBINE)
+            and dims[FV.H] == (FC.STATE, FC.TURBINE)
+        ):
+            self[FV.TXYH] = np.zeros(
+                (self.n_states, self.n_turbines, 3), dtype=FC.DTYPE
+            )
 
-    def calculate(self, algo, mdata, fdata, pdata):
-        """ "
-        The main model calculation.
+            self[FV.TXYH][:, :, 0] = self[FV.X]
+            self[FV.TXYH][:, :, 1] = self[FV.Y]
+            self[FV.TXYH][:, :, 2] = self[FV.H]
+
+            self[FV.X] = self[FV.TXYH][:, :, 0]
+            self[FV.Y] = self[FV.TXYH][:, :, 1]
+            self[FV.H] = self[FV.TXYH][:, :, 2]
+
+    def __run_entry_checks(self, name, data, dims):
+        # remove axes of size 1, added by dask for extra loop dimensions:
+        if dims is not None:
+            if len(dims) != len(data.shape):
+                for li, l in enumerate(self.loop_dims):
+                    if data.shape[li] == 1 and (len(dims) < li + 1 or dims[li] != l):
+                        self[name] = np.squeeze(data, axis=li)
+
+            for ci, c in enumerate(dims):
+                if c not in self.sizes:
+                    self.sizes[c] = self[name].shape[ci]
+                elif self.sizes[c] != self[name].shape[ci]:
+                    raise ValueError(
+                        f"Inconsistent size for data entry '{name}', dimension '{c}': Expecting {self.sizes[c]}, found {self[name].shape[ci]} in shape {self[name].shape}"
+                    )
 
-        This function is executed on a single chunk of data,
-        all computations should be based on numpy arrays.
+    def add(self, name, data, dims):
+        """
+        Add data entry
+
+        Parameters
+        ----------
+        name: str
+            The data name
+        data: np.ndarray
+            The data
+        dims: tuple of str
+            The dimensions
+
+        """
+        self[name] = data
+        self.dims[name] = dims
+        self.__run_entry_checks(name, data, dims)
+        self.__auto_update()
+
+    @classmethod
+    def from_points(
+        cls,
+        points,
+        data={},
+        dims={},
+        name="pdata",
+    ):
+        """
+        Create from points
 
         Parameters
         ----------
-        algo: foxes.core.Algorithm
-            The calculation algorithm
-        mdata: foxes.core.Data
-            The model data
-        fdata: foxes.core.Data
-            The farm data
-        pdata: foxes.core.Data
-            The point data
+        points: np.ndarray
+            The points, shape: (n_states, n_points, 3)
+        data: dict
+            The initial data to be stored
+        dims: dict
+            The dimensions tuples, same or subset
+            of data keys
+        name: str
+            The data container name
 
         Returns
         -------
-        results: dict
-            The resulting data, keys: output variable str.
-            Values: numpy.ndarray with shape (n_states, n_points)
+        pdata: Data
+            The data object
 
         """
-
-        hdata = {}
-        hdims = {}
-        smap = mdata[self.SMAP]
-        for dname, data in mdata.items():
-            dms = mdata.dims[dname]
-            if dname == self.SMAP or dname == self.STATE0:
-                pass
-            elif dms[0] == self.STATE0:
-                hdata[dname] = data[smap]
-                hdims[dname] = tuple([FC.STATE] + list(dms)[1:])
-            elif self.STATE0 in dms:
-                raise ValueError(
-                    f"States '{self.name}': Found states variable not at dimension 0 for mdata entry '{dname}': {dms}"
-                )
-            else:
-                hdata[dname] = data
-                hdims[dname] = dms
-        hmdata = Data(hdata, hdims, mdata.loop_dims)
-
-        return self.states.calculate(algo, hmdata, fdata, pdata)
+        if len(points.shape) != 3 or points.shape[2] != 3:
+            raise ValueError(
+                f"Expecting points shape (n_states, n_points, 3), got {points.shape}"
+            )
+        data[FC.POINTS] = points
+        dims[FC.POINTS] = (FC.STATE, FC.POINT, FC.XYH)
+        return Data(data, dims, [FC.STATE, FC.POINT], name)
```

### Comparing `foxes-0.4.0/foxes/opt/objectives/farm_vars.py` & `foxes-0.4.1/foxes/opt/objectives/farm_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import xarray as xr
 
 from foxes.opt.core.farm_objective import FarmObjective
 from foxes import variables as FV
 import foxes.constants as FC
 
+
 class FarmVarObjective(FarmObjective):
     """
     Objectives based on farm variables.
 
     Attributes
     ----------
     variable: str
@@ -38,15 +39,15 @@
         minimize,
         deps=None,
         scale=1.0,
         **kwargs,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
             The underlying optimization problem
         name: str
             The name of the objective function
         variable: str
@@ -258,15 +259,15 @@
     ----------
     problem: foxes.opt.FarmOptProblem
         The underlying optimization problem
     name: str
         The name of the objective function
     kwargs: dict, optional
         Additional parameters for `FarmVarObjective`
-    
+
     :group: opt.objectives
 
     """
 
     def __init__(self, problem, name="maximize_power", **kwargs):
         if "scale" in kwargs:
             scale = kwargs.pop("scale")
@@ -299,15 +300,15 @@
     ----------
     problem: foxes.opt.FarmOptProblem
         The underlying optimization problem
     name: str
         The name of the objective function
     kwargs: dict, optional
         Additional parameters for `FarmVarObjective`
-    
+
     :group: opt.objectives
 
     """
 
     def __init__(self, problem, name="minimize_TI", **kwargs):
         scale = kwargs.pop("scale") if "scale" in kwargs else 1.0
         super().__init__(
```

### Comparing `foxes-0.4.0/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.4.1/foxes/opt/objectives/max_n_turbines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 
 from foxes.opt.core.farm_objective import FarmObjective
 import foxes.constants as FC
 
+
 class MaxNTurbines(FarmObjective):
     """
     Maximizes the number of turrbines.
 
     Attributes
     ----------
     check_valid: bool
@@ -21,15 +22,15 @@
         problem,
         name="max_n_turbines",
         check_valid=True,
         **kwargs,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
             The underlying optimization problem
         name: str
             The name of the objective function
         check_valid: bool
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.4.1/foxes/opt/problems/layout/farm_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class FarmLayoutOptProblem(FarmVarsProblem):
     """
     The turbine positioning optimization problem
 
     :group: opt.problems.layout
-    
+
     """
 
     def var_names_float(self):
         """
         The names of float variables.
 
         Returns
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 class Valid(Constraint):
     """
     Validity constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(self, problem, name="valid", **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         name: str
             The constraint name
         kwargs: dict, optional
             Additioal parameters for the base class
 
         """
@@ -103,22 +104,23 @@
 class Boundary(Constraint):
     """
     Boundary constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(self, problem, n_turbines=None, D=None, name="boundary", **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         n_turbines: int, optional
             The number of turbines
         D: float, optional
             The rotor diameter
         name: str
             The constraint name
@@ -221,24 +223,25 @@
 class MinDist(Constraint):
     """
     Minimal distance constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(
         self, problem, min_dist=None, n_turbines=None, name="min_dist", **kwargs
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         min_dist: float, optional
             The minimal distance between turbines
         n_turbines: int, optional
             The number of turbines
         name: str
             The constraint name
@@ -359,14 +362,15 @@
 class CMinN(Constraint):
     """
     Minimal number of turbines constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(self, problem, N, name="cminN", **kwargs):
         super().__init__(
             problem,
             name,
             vnames_int=problem.var_names_int(),
             vnames_float=problem.var_names_float(),
             **kwargs,
@@ -457,22 +461,23 @@
 class CMaxN(Constraint):
     """
     Maximal number of turbines constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(self, problem, N, name="cmaxN", **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         N: int
             The maximal number of turbines
         name: str
             The constraint name
         kwargs: dict, optional
             Additioal parameters for the base class
@@ -555,22 +560,23 @@
 class CFixN(Constraint):
     """
     Fixed number of turbines constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(self, problem, N, name="cfixN", **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         N: int
             The number of turbines
         name: str
             The constraint name
         kwargs: dict, optional
             Additioal parameters for the base class
@@ -656,22 +662,23 @@
 class CMinDensity(Constraint):
     """
     Minimal turbine density constraint for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.constraints
 
     """
+
     def __init__(self, problem, min_value, dfactor=1, name="min_density"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         min_value: float
             The minimal turbine density
         dfactor: float
             Delta factor for grid spacing
         name: str
             The constraint name
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,30 +22,30 @@
         The number of turbines in the layout
     min_dist: float
         The minimal distance between points
     D: float
         The diameter of circle fully within boundary
     calc_valid: bool
         Evaluate validity
-    
+
     :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         n_turbines,
         min_dist=None,
         D=None,
         calc_valid=None,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         boundary: foxes.utils.geom2d.AreaGeometry
             The boundary geometry
         n_turbines: int
             The number of turbines in the layout
         min_dist: float, optional
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,30 +23,30 @@
         The number of turbines in the layout
     grid_spacing: float
         The background grid spacing
     min_dist: float
         The minimal distance between points
     D: float
         The diameter of circle fully within boundary
-    
+
     :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         n_turbines,
         grid_spacing,
         min_dist=None,
         D=None,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         boundary: foxes.utils.geom2d.AreaGeometry
             The boundary geometry
         n_turbines: int
             The number of turbines in the layout
         grid_spacing: float
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,30 +21,30 @@
         The number of turbines in the layout
     min_dist: float
         The minimal distance between points
     max_dist: float
         The maximal distance between points
     D: float
         The diameter of circle fully within boundary
-    
+
     :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
         n_turbines,
         min_dist,
         max_dist=None,
         D=None,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         boundary: foxes.utils.geom2d.AreaGeometry
             The boundary geometry
         n_turbines: int
             The number of turbines in the layout
         min_dist: float
@@ -281,15 +281,15 @@
                 vld[pi] = np.ones(self.n_turbines, dtype=bool)
             else:
                 qts[pi] = np.append(
                     pts[pi, valid[pi]],
                     pts[pi, ~valid[pi]][: (self.n_turbines - nvl[pi])],
                     axis=0,
                 )
-                vld[pi,: nvl[pi]] = True
+                vld[pi, : nvl[pi]] = True
 
         return qts, vld
 
     def get_fig(
         self, xy=None, valid=None, ax=None, title=None, true_circle=True, **bargs
     ):
         """
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         The maximal number of points
     n_row_max: int
         The maximal number of points in a row
     max_dist: float
         The maximal distance between points
     D: float
         The diameter of circle fully within boundary
-    
+
     :group: opt.problems.layout.geom_layouts
 
     """
 
     def __init__(
         self,
         boundary,
@@ -42,15 +42,15 @@
         n_max=None,
         n_row_max=None,
         max_dist=None,
         D=None,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         boundary: foxes.utils.geom2d.AreaGeometry
             The boundary geometry
         min_dist: float
             The minimal distance between points
         n_grids: int
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.4.1/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,23 @@
     """
     Maximal number of turbines objective
     for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.objectives
 
     """
+
     def __init__(self, problem, name="maxN"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         name: str
             The constraint name
 
         """
         super().__init__(
             problem,
@@ -115,22 +116,23 @@
     """
     Minimal number of turbines objective
     for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.objectives
 
     """
+
     def __init__(self, problem, name="ominN"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         name: str
             The constraint name
 
         """
         super().__init__(problem, name)
 
@@ -142,22 +144,23 @@
     """
     Fixed number of turbines objective
     for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.objectives
 
     """
+
     def __init__(self, problem, N, name="ofixN"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         N: int
             The number of turbines
         name: str
             The constraint name
 
         """
@@ -253,22 +256,23 @@
     """
     Maximal grid spacing objective
     for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.objectives
 
     """
+
     def __init__(self, problem, name="max_dxdy"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         name: str
             The constraint name
 
         """
         super().__init__(
             problem,
@@ -362,22 +366,23 @@
     """
     Maximal turbine density objective
     for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.objectives
 
     """
+
     def __init__(self, problem, dfactor=1, min_dist=None, name="max_density"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         dfactor: float
             Delta factor for grid spacing
         min_dist: float, optional
             The minimal distance
         name: str
             The constraint name
@@ -516,22 +521,23 @@
     """
     Mean-min-max distance objective
     for purely geometrical layouts problems.
 
     :group: opt.problems.layout.geom_layouts.objectives
 
     """
+
     def __init__(self, problem, scale=500.0, c1=1, c2=1, c3=1, name="MiMaMean"):
         """
         Constructor.
-        
+
         Parameters
         ----------
         problem: foxes.opt.FarmOptProblem
-            The underlying geometrical layout 
+            The underlying geometrical layout
             optimization problem
         scale: float
             The distance scale
         c1: float
             Parameter for mean weighting
         c2: float
             Parameter for max diff weighting
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.4.1/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     min_spacing: float
         The minimal turbine spacing
     n_grids: int
         The number of grids
     max_n_row: int
         The maximal number of turbines per
         grid and row
-    
+
     :group: opt.problems.layout
 
     """
 
     def __init__(
         self,
         name,
@@ -39,15 +39,15 @@
         n_row_max=None,
         max_dist=None,
         runner=None,
         **kwargs,
     ):
         """
         Constraints.
-        
+
         Parameters
         ----------
         name: str
             The problem's name
         algo: foxes.core.Algorithm
             The algorithm
         min_dist: float
```

### Comparing `foxes-0.4.0/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.4.1/foxes/opt/problems/layout/regular_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         name,
         algo,
         min_spacing,
         **kwargs,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         name: str
             The problem's name
         algo: foxes.core.Algorithm
             The algorithm
         min_spacing: float
```

### Comparing `foxes-0.4.0/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.4.1/foxes/opt/problems/opt_farm_vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     :group: opt.problems
 
     """
 
     def __init__(self, *args, **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         args: tuple, optional
             Arguments for `FarmVarsProblem`
         kwargs: dict, optional
             Keyword arguments for `FarmVarsProblem`
 
@@ -480,15 +480,15 @@
 
         farm_vars = {}
         grps = self._vars.groupby(["type", "var", "level"])
         for (typ, var, level), g in grps:
             src = vars_int if typ == "int" else vars_float
             i0 = g.index[0]
             i1 = g.index[-1]
-            data = src[np.s_[i0: i1 + 1]]
+            data = src[np.s_[i0 : i1 + 1]]
 
             if level == "uniform":
                 farm_vars[var] = np.full((n_states, n_sturb), data[0], dtype=FC.DTYPE)
 
             elif level == "state":
                 farm_vars[var] = np.full((n_states, n_sturb), np.nan, dtype=FC.DTYPE)
                 if np.all(g["state"] == np.arange(n_states)):
@@ -542,15 +542,15 @@
 
         farm_vars = {}
         grps = self._vars.groupby(["type", "var", "level"])
         for (typ, var, level), g in grps:
             src = vars_int if typ == "int" else vars_float
             i0 = g.index[0]
             i1 = g.index[-1]
-            data = src[:, np.s_[i0: i1 + 1]]
+            data = src[:, np.s_[i0 : i1 + 1]]
 
             if level == "uniform":
                 farm_vars[var] = np.full(
                     (n_pop, n_states, n_sturb), np.nan, dtype=FC.DTYPE
                 )
                 farm_vars[var][:] = data[:, 0, None, None]
```

### Comparing `foxes-0.4.0/foxes/output/farm_layout.py` & `foxes-0.4.1/foxes/output/farm_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
     def __init__(
         self, farm, farm_results=None, from_results=False, results_state=None, D=None
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         farm: foxes.WindFarm
             The wind farm
         farm_results: xarray.Dataset, optional
             The wind farm calculation results
         from_results: bool, optional
```

### Comparing `foxes-0.4.0/foxes/output/farm_results_eval.py` & `foxes-0.4.1/foxes/output/farm_results_eval.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     :group: output
 
     """
 
     def __init__(self, farm_results):
         """
         Constructor.
-        
+
         Parameters
         ----------
         farm_results: xarray.Dataset
             The farm results
 
         """
         self.results = farm_results
```

### Comparing `foxes-0.4.0/foxes/output/flow_plots_2d.py` & `foxes-0.4.1/foxes/output/flow_plots_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,33 +14,38 @@
 
     Attributes
     ----------
     algo: foxes.Algorithm
         The algorithm for point calculation
     farm_results: xarray.Dataset
         The farm results
+    runner: foxes.utils.runners.Runner, optional
+        The runner
 
     :group: output
 
     """
 
-    def __init__(self, algo, farm_results):
+    def __init__(self, algo, farm_results, runner=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         algo: foxes.Algorithm
             The algorithm for point calculation
         farm_results: xarray.Dataset
             The farm results
+        runner: foxes.utils.runners.Runner, optional
+            The runner
 
         """
         self.algo = algo
         self.fres = farm_results
+        self.runner = runner
 
     def _get_fig(
         self,
         var,
         fig,
         figsize,
         ax,
@@ -61,14 +66,15 @@
         title,
         add_bar,
         vlabel,
         ret_state,
         ret_im,
         quiv=None,
         invert_axis=None,
+        animated=False,
     ):
         """
         Helper function for image creation
         """
         # create plot:
         if fig is None:
             hfig = plt.figure(figsize=figsize)
@@ -83,35 +89,70 @@
         zz = data[si].reshape([N_x, N_y]).T
         if normalize_var is not None:
             zz /= normalize_var
 
         # raw data image:
         if levels is None:
             im = hax.pcolormesh(
-                x_pos, y_pos, zz, vmin=vmin, vmax=vmax, shading="auto", cmap=cmap
+                x_pos,
+                y_pos,
+                zz,
+                vmin=vmin,
+                vmax=vmax,
+                shading="auto",
+                cmap=cmap,
+                animated=animated,
             )
 
         # contour plot:
         else:
-            im = hax.contourf(x_pos, y_pos, zz, levels, vmax=vmax, vmin=vmin, cmap=cmap)
+            im = hax.contourf(
+                x_pos,
+                y_pos,
+                zz,
+                levels,
+                vmax=vmax,
+                vmin=vmin,
+                cmap=cmap,
+                animated=animated,
+            )
 
+        qv = None
         if quiv is not None and quiv[0] is not None:
             n, pars, wd, ws = quiv
             uv = wd2uv(wd[si], ws[si])
             u = uv[:, 0].reshape([N_x, N_y]).T[::n, ::n]
             v = uv[:, 1].reshape([N_x, N_y]).T[::n, ::n]
-            hax.quiver(x_pos[::n], y_pos[::n], u, v, **pars)
+            qv = hax.quiver(x_pos[::n], y_pos[::n], u, v, animated=animated, **pars)
             del n, pars, u, v, uv
 
         hax.autoscale_view()
         hax.set_xlabel(xlabel)
         hax.set_ylabel(ylabel)
-        hax.set_title(title if title is not None else f"State {s}")
         hax.set_aspect("equal", adjustable="box")
 
+        ttl = None
+        if animated and title is None:
+            if hasattr(s, "dtype") and np.issubdtype(s.dtype, np.datetime64):
+                t = np.datetime_as_string(s, unit="m").replace("T", " ")
+            else:
+                t = s
+            ttl = hax.text(
+                0.5,
+                1.02,
+                f"State {t}",
+                backgroundcolor="w",
+                transform=hax.transAxes,
+                ha="center",
+                animated=True,
+                clip_on=False,
+            )
+        else:
+            hax.set_title(title if title is not None else f"State {s}")
+
         if invert_axis == "x":
             hax.invert_xaxis()
         elif invert_axis == "y":
             hax.invert_yaxis()
 
         if add_bar:
             divider = make_axes_locatable(hax)
@@ -123,20 +164,37 @@
             out = fig
 
         if ret_state or ret_im:
             out = [out]
         if ret_state:
             out.append(si)
         if ret_im:
-            out.append(im)
+            out.append([i for i in [im, qv, ttl] if i is not None])
         if ret_state or ret_im:
             out = tuple(out)
 
         return out
 
+    def _calc_point_results(self, verbosity, g_pts, **kwargs):
+        """Helper function for point data calculation"""
+        averb = None if verbosity == self.algo.verbosity else self.algo.verbosity
+        if averb is not None:
+            self.algo.verbosity = verbosity
+        if self.runner is None:
+            point_results = self.algo.calc_points(self.fres, points=g_pts, **kwargs)
+        else:
+            kwargs["points"] = g_pts
+            point_results = self.runner.run(
+                self.algo.calc_points, args=(self.fres,), kwargs=kwargs
+            )
+        if averb is not None:
+            self.algo.verbosity = averb
+
+        return point_results
+
     def get_mean_fig_xy(
         self,
         var,
         resolution,
         xmin=None,
         ymin=None,
         xmax=None,
@@ -158,14 +216,15 @@
         ax=None,
         add_bar=True,
         cmap=None,
         weight_turbine=0,
         verbosity=0,
         ret_state=False,
         ret_im=False,
+        animated=False,
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a horizontal xy-plane.
 
         Parameters
         ----------
@@ -219,26 +278,29 @@
             Index of the turbine from which to take the weight
         verbosity: int, optional
             The verbosity level
         ret_state: bool, optional
             Flag for state index return
         ret_im: bool, optional
             Flag for image return
+        animated: bool
+            Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
-        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
-            The image object
+        im: tuple, optional
+            The image objects, atplotlib.collections.QuadMesh
+            or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
 
         # get base rectangle:
@@ -280,22 +342,15 @@
             print("Max XYZ  =", x_max, y_max, z_max)
             print("Pos Z    =", z_pos)
             print("Res XY   =", x_res, y_res)
             print("Dim XY   =", N_x, N_y)
             print("Grid pts =", n_pts)
 
         # calculate point results:
-        averb = None if verbosity == self.algo.verbosity else self.algo.verbosity
-        if averb is not None:
-            self.algo.verbosity = verbosity
-        point_results = self.algo.calc_points(self.fres, points=g_pts, **kwargs)
-        if averb is not None:
-            self.algo.verbosity = averb
-        data = point_results[var].to_numpy()
-        del point_results
+        data = self._calc_point_results(verbosity, g_pts, **kwargs)[var].to_numpy()
 
         # take mean over states:
         weights = self.fres[FV.WEIGHT][:, weight_turbine].to_numpy()
         data = np.einsum("s,sp->p", weights, data)
 
         # find data min max:
         vmin = var_min if var_min is not None else np.min(data)
@@ -333,14 +388,15 @@
             xlabel,
             ylabel,
             title,
             add_bar,
             vlabel,
             ret_state,
             ret_im,
+            animated=animated,
         )
 
         return out
 
     def get_mean_fig_xz(
         self,
         var,
@@ -368,14 +424,15 @@
         ax=None,
         add_bar=True,
         cmap=None,
         weight_turbine=0,
         verbosity=0,
         ret_state=False,
         ret_im=False,
+        animated=False,
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a vertical xz-plane.
 
         Parameters
         ----------
@@ -433,26 +490,29 @@
             Index of the turbine from which to take the weight
         verbosity: int, optional
             The verbosity level
         ret_state: bool, optional
             Flag for state index return
         ret_im: bool, optional
             Flag for image return
+        animated: bool
+            Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
-        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
-            The image object
+        im: tuple, optional
+            The image objects, atplotlib.collections.QuadMesh
+            or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
         n_x = np.append(wd2uv(x_direction), [0.0], axis=0)
@@ -509,22 +569,15 @@
             print("Max XYZ  =", x_max, y_max, z_max)
             print("Pos Y    =", y_pos)
             print("Res XZ   =", x_res, z_res)
             print("Dim XZ   =", N_x, N_z)
             print("Grid pts =", n_pts)
 
         # calculate point results:
-        averb = None if verbosity == self.algo.verbosity else self.algo.verbosity
-        if averb is not None:
-            self.algo.verbosity = verbosity
-        point_results = self.algo.calc_points(self.fres, points=g_pts, **kwargs)
-        if averb is not None:
-            self.algo.verbosity = averb
-        data = point_results[var].to_numpy()
-        del point_results
+        data = self._calc_point_results(verbosity, g_pts, **kwargs)[var].to_numpy()
 
         # take mean over states:
         weights = self.fres[FV.WEIGHT][:, weight_turbine].to_numpy()
         data = np.einsum("s,sp->p", weights, data)
 
         # find data min max:
         vmin = var_min if var_min is not None else np.min(data)
@@ -563,14 +616,15 @@
             xlabel,
             zlabel,
             title,
             add_bar,
             vlabel,
             ret_state,
             ret_im,
+            animated=animated,
         )
 
         return out
 
     def get_mean_fig_yz(
         self,
         var,
@@ -598,14 +652,15 @@
         ax=None,
         add_bar=True,
         cmap=None,
         weight_turbine=0,
         verbosity=1,
         ret_state=False,
         ret_im=False,
+        animated=False,
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a vertical yz-plane.
 
         Parameters
         ----------
@@ -663,26 +718,29 @@
             Index of the turbine from which to take the weight
         verbosity: int, optional
             The verbosity level
         ret_state: bool, optional
             Flag for state index return
         ret_im: bool, optional
             Flag for image return
+        animated: bool
+            Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
-        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
-            The image object
+        im: tuple, optional
+            The image objects, atplotlib.collections.QuadMesh
+            or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
         n_x = np.append(wd2uv(x_direction), [0.0], axis=0)
@@ -739,19 +797,15 @@
             print("Max XYZ  =", x_max, y_max, z_max)
             print("Pos X    =", x_pos)
             print("Res YZ   =", y_res, z_res)
             print("Dim YZ   =", N_y, N_z)
             print("Grid pts =", n_pts)
 
         # calculate point results:
-        point_results = self.algo.calc_points(
-            self.fres, points=g_pts, verbosity=verbosity, **kwargs
-        )
-        data = point_results[var].to_numpy()
-        del point_results
+        data = self._calc_point_results(verbosity, g_pts, **kwargs)[var].to_numpy()
 
         # take mean over states:
         weights = self.fres[FV.WEIGHT][:, weight_turbine].to_numpy()
         data = np.einsum("s,sp->p", weights, data)
 
         # find data min max:
         vmin = var_min if var_min is not None else np.min(data)
@@ -791,14 +845,15 @@
             zlabel,
             title,
             add_bar,
             vlabel,
             ret_state,
             ret_im,
             invert_axis="x",
+            animated=animated,
         )
 
         return out
 
     def gen_states_fig_xy(
         self,
         var,
@@ -825,14 +880,15 @@
         add_bar=True,
         cmap=None,
         quiver_n=None,
         quiver_pars={},
         verbosity=0,
         ret_state=False,
         ret_im=False,
+        animated=False,
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a horizontal xy-plane.
 
         Parameters
         ----------
@@ -888,26 +944,29 @@
             Parameters for plt.quiver
         verbosity: int, optional
             The verbosity level
         ret_state: bool, optional
             Flag for state index return
         ret_im: bool, optional
             Flag for image return
+        animated: bool
+            Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
-        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
-            The image object
+        im: tuple, optional
+            The image objects, atplotlib.collections.QuadMesh
+            or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
 
         # get base rectangle:
@@ -949,21 +1008,16 @@
             print("Max XYZ  =", x_max, y_max, z_max)
             print("Pos Z    =", z_pos)
             print("Res XY   =", x_res, y_res)
             print("Dim XY   =", N_x, N_y)
             print("Grid pts =", n_pts)
 
         # calculate point results:
-        averb = None if verbosity == self.algo.verbosity else self.algo.verbosity
-        if averb is not None:
-            self.algo.verbosity = verbosity
-        point_results = self.algo.calc_points(self.fres, points=g_pts, **kwargs)
-        if averb is not None:
-            self.algo.verbosity = averb
-        data = point_results[var].values
+        point_results = self._calc_point_results(verbosity, g_pts, **kwargs)
+        data = point_results[var].to_numpy()
         quiv = (
             None
             if quiver_n is None
             else (
                 quiver_n,
                 quiver_pars,
                 point_results[FV.WD].values,
@@ -982,16 +1036,19 @@
         # normalize x and y:
         if normalize_xy is not None:
             x_pos /= normalize_xy
             y_pos /= normalize_xy
 
         # loop over states:
         for si, s in enumerate(self.fres[FC.STATE].to_numpy()):
-            ttl = f"State {s}" if title is None else title
-            ttl += f", z =  {int(np.round(z_pos))} m"
+            if not animated and title is None:
+                ttl = f"State {s}"
+                ttl += f", z =  {int(np.round(z_pos))} m"
+            else:
+                ttl = title
 
             out = self._get_fig(
                 var,
                 fig,
                 figsize,
                 ax,
                 data,
@@ -1010,14 +1067,15 @@
                 ylabel,
                 ttl,
                 add_bar,
                 vlabel,
                 ret_state,
                 ret_im,
                 quiv,
+                animated=animated,
             )
 
             yield out
 
     def gen_states_fig_xz(
         self,
         var,
@@ -1046,14 +1104,15 @@
         add_bar=True,
         cmap=None,
         quiver_n=None,
         quiver_pars={},
         verbosity=0,
         ret_state=False,
         ret_im=False,
+        animated=False,
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a vertical xz-plane.
 
         Parameters
         ----------
@@ -1113,26 +1172,29 @@
             Parameters for plt.quiver
         verbosity: int, optional
             The verbosity level
         ret_state: bool, optional
             Flag for state index return
         ret_im: bool, optional
             Flag for image return
+        animated: bool
+            Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
-        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
-            The image object
+        im: tuple, optional
+            The image objects, atplotlib.collections.QuadMesh
+            or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
         n_x = np.append(wd2uv(x_direction), [0.0], axis=0)
@@ -1189,21 +1251,16 @@
             print("Max XYZ  =", x_max, y_max, z_max)
             print("Pos Y    =", y_pos)
             print("Res XZ   =", x_res, z_res)
             print("Dim XZ   =", N_x, N_z)
             print("Grid pts =", n_pts)
 
         # calculate point results:
-        averb = None if verbosity == self.algo.verbosity else self.algo.verbosity
-        if averb is not None:
-            self.algo.verbosity = verbosity
-        point_results = self.algo.calc_points(self.fres, points=g_pts, **kwargs)
-        if averb is not None:
-            self.algo.verbosity = averb
-        data = point_results[var].values
+        point_results = self._calc_point_results(verbosity, g_pts, **kwargs)
+        data = point_results[var].to_numpy()
         quiv = (
             None
             if quiver_n is None
             else (
                 quiver_n,
                 quiver_pars,
                 point_results[FV.WD].values,
@@ -1223,17 +1280,20 @@
         if normalize_x is not None:
             x_pos /= normalize_x
         if normalize_z is not None:
             z_pos /= normalize_z
 
         # loop over states:
         for si, s in enumerate(self.fres[FC.STATE].to_numpy()):
-            ttl = f"State {s}" if title is None else title
-            ttl += f", x direction = {x_direction}°"
-            ttl += f", y =  {int(np.round(y_pos))} m"
+            if not animated and title is None:
+                ttl = f"State {s}"
+                ttl += f", x direction = {x_direction}°"
+                ttl += f", y =  {int(np.round(y_pos))} m"
+            else:
+                ttl = title
 
             out = self._get_fig(
                 var,
                 fig,
                 figsize,
                 ax,
                 data,
@@ -1252,14 +1312,15 @@
                 zlabel,
                 ttl,
                 add_bar,
                 vlabel,
                 ret_state,
                 ret_im,
                 quiv,
+                animated=animated,
             )
 
             yield out
 
     def gen_states_fig_yz(
         self,
         var,
@@ -1288,14 +1349,15 @@
         add_bar=True,
         cmap=None,
         quiver_n=None,
         quiver_pars={},
         verbosity=1,
         ret_state=False,
         ret_im=False,
+        animated=False,
         **kwargs,
     ):
         """
         Generates 2D farm flow figure in a plane.
 
         Parameters
         ----------
@@ -1355,26 +1417,29 @@
             Parameters for plt.quiver
         verbosity: int, optional
             The verbosity level
         ret_state: bool, optional
             Flag for state index return
         ret_im: bool, optional
             Flag for image return
+        animated: bool
+            Switch for usage for an animation
         kwargs: dict, optional
             Parameters forwarded to the algorithm's calc_points
             function.
 
         Yields
         ------
         fig: matplotlib.Figure
             The figure object
         si: int, optional
             The state index
-        im: matplotlib.collections.QuadMesh or matplotlib.QuadContourSet, optional
-            The image object
+        im: tuple, optional
+            The image objects, atplotlib.collections.QuadMesh
+            or matplotlib.QuadContourSet
 
         """
 
         # prepare:
         n_states = self.algo.n_states
         n_turbines = self.algo.n_turbines
         n_x = np.append(wd2uv(x_direction), [0.0], axis=0)  ## -180 to get [1,0,0]
@@ -1430,21 +1495,17 @@
             print("Min XYZ  =", x_min, y_min, z_min)
             print("Max XYZ  =", x_max, y_max, z_max)
             print("Pos X    =", x_pos)
             print("Res YZ   =", y_res, z_res)
             print("Dim YZ   =", N_y, N_z)
             print("Grid pts =", n_pts)
 
-        averb = None if verbosity == self.algo.verbosity else self.algo.verbosity
-        if averb is not None:
-            self.algo.verbosity = verbosity
-        point_results = self.algo.calc_points(self.fres, points=g_pts, **kwargs)
-        if averb is not None:
-            self.algo.verbosity = averb
-        data = point_results[var].values
+        # calculate point results:
+        point_results = self._calc_point_results(verbosity, g_pts, **kwargs)
+        data = point_results[var].to_numpy()
         quiv = (
             None
             if quiver_n is None
             else (
                 quiver_n,
                 quiver_pars,
                 point_results[FV.WD].values,
@@ -1494,10 +1555,11 @@
                 ttl,
                 add_bar,
                 vlabel,
                 ret_state,
                 ret_im,
                 quiv=quiv,
                 invert_axis="x",
+                animated=animated,
             )
 
             yield out
```

### Comparing `foxes-0.4.0/foxes/output/output.py` & `foxes-0.4.1/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/output/results_writer.py` & `foxes-0.4.1/foxes/output/results_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :group: output
 
     """
 
     def __init__(self, farm_results=None, data=None):
         """
         Constructor.
-        
+
         Parameters
         ----------
         farm_results: xarray.Dataset, optional
             The farm results, if data is None
         data: pandas.DataFrame, optional
             The data, if farm_results is None
```

### Comparing `foxes-0.4.0/foxes/output/rose_plot.py` & `foxes-0.4.1/foxes/output/rose_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     :group: output
 
     """
 
     def __init__(self, results):
         """
         Constructor.
-        
+
         Parameters
         ----------
         results: xarray.Dataset
             The calculation results (farm or points)
 
         """
         dims = list(results.dims.keys())
```

### Comparing `foxes-0.4.0/foxes/output/state_turbine_map.py` & `foxes-0.4.1/foxes/output/state_turbine_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Creates heat maps with turbines on the one
     and states on the other axis.
 
     Attributes
     ----------
     results: xarray.Dataset
         The farm results
-    
+
     :group: output
 
     """
 
     def __init__(self, farm_results):
         """
         Constructor.
```

### Comparing `foxes-0.4.0/foxes/output/turbine_type_curves.py` & `foxes-0.4.1/foxes/output/turbine_type_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     Creates power and ct curves for turbine
     types, optionally including derating/boost.
 
     Attributes
     ----------
     mbook: foxes.models.ModelBook
         The model book
-    
+
     :group: output
 
     """
 
     def __init__(self, mbook):
         """
         Constructor.
-        
+
         Parameters
         ----------
         mbook: foxes.models.ModelBook
             The model book
 
         """
         self.mbook = mbook
```

### Comparing `foxes-0.4.0/foxes/utils/abl/neutral.py` & `foxes-0.4.1/foxes/utils/abl/neutral.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     z0: float
         The roughness length
 
     Returns
     -------
     lz: float
         The log factor
-    
+
     :group: utils.abl.neutral
 
     """
     h = np.maximum(height, z0)
     return np.log(h / z0)
 
 
@@ -41,15 +41,15 @@
     kappa: float
         The van-Karman constant
 
     Returns
     -------
     ustar: float
         The friction velocity
-    
+
     :group: utils.abl.neutral
 
     """
     lz = logz(h_ref, z0)
     return ws_ref * kappa / lz
 
 
@@ -68,12 +68,12 @@
     kappa: float
         The van-Karman constant
 
     Returns
     -------
     ws: float
         The wind speed
-    
+
     :group: utils.abl.neutral
 
     """
     return ustar / kappa * logz(height, z0)
```

### Comparing `foxes-0.4.0/foxes/utils/abl/stable.py` & `foxes-0.4.1/foxes/utils/abl/stable.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     z0: float
         The roughness length
 
     Returns
     -------
     lz: float
         The log factor
-    
+
     :group: utils.abl.stable
 
     """
     return lgz(height, z0)
 
 
 def psi(height, mol):
```

### Comparing `foxes-0.4.0/foxes/utils/abl/unstable.py` & `foxes-0.4.1/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/utils/cubic_roots.py` & `foxes-0.4.1/foxes/utils/cubic_roots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/utils/data_book.py` & `foxes-0.4.1/foxes/utils/data_book.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         A data book to start from
 
     Attributes
     ----------
     dbase: dict
         The data base. Key: context str,
         value: dict (file name str to pathlib.Path)
-    
+
     :group: utils
 
     """
 
     def __init__(self, data_book=None):
         """
         Constructor.
```

### Comparing `foxes-0.4.0/foxes/utils/dict.py` & `foxes-0.4.1/foxes/utils/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
     """
     A slightly enhanced dictionary.
 
     Attributes
     ----------
     name: str
         The dictionary name
-    
+
     :group: utils
 
     """
 
     def __init__(self, *args, name=None, **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         *args: tuple, optional
             Arguments passed to `dict`
         name: str, optional
             The dictionary name
         **kwargs: dict, optional
```

### Comparing `foxes-0.4.0/foxes/utils/geom2d/area_geometry.py` & `foxes-0.4.1/foxes/utils/geom2d/area_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,23 +218,23 @@
         else:
             return AreaIntersection([self, g.inverse()])
 
 
 class InvertedAreaGeometry(AreaGeometry):
     """
     Base class for inverted geometries.
-    
+
     :group: utils.geom2d
 
     """
 
     def __init__(self, geometry):
         """
         Constructor.
-        
+
         Parameters
         ----------
         geometry: geom2d.AreaGeometry
             The original geometry
 
         """
         self._geometry = geometry
@@ -384,23 +384,23 @@
     """
     The union of area geometries.
 
     Attributes
     ----------
     geometries: list of geom2d.AreaGeometry
         The geometries
-    
+
     :group: utils.geom2d
 
     """
 
     def __init__(self, geometries):
         """
         Constructor.
-        
+
         Parameters
         ----------
         geometries: list of geom2d.AreaGeometry
             The geometries
 
         """
         self.geometries = geometries
@@ -596,18 +596,19 @@
 class InvertedAreaUnion(InvertedAreaGeometry):
     """
     Inversion of a union of areas
 
     :group: utils.geom2d
 
     """
+
     def __init__(self, union):
         """
         Constructor.
-        
+
         Parameters
         ----------
         union: geom2d.AreaUnion
             The original area union geometry
 
         """
         super().__init__(union)
@@ -676,15 +677,15 @@
     :group: utils.geom2d
 
     """
 
     def __new__(cls, geometries):
         """
         Constructor.
-        
+
         Parameters
         ----------
         geometries: list of geom2d.AreaGeometry
             The geometries
 
         """
         return AreaUnion([g.inverse() for g in geometries]).inverse()
```

### Comparing `foxes-0.4.0/foxes/utils/geom2d/circle.py` & `foxes-0.4.1/foxes/utils/geom2d/circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :group: utils.geom2d
 
     """
 
     def __init__(self, centre, radius):
         """
         Cobnstructor.
-        
+
         Parameters
         ----------
         centre: numpy.ndarray
             The centre point, shape: (2,)
         radius: float
             The radius
```

### Comparing `foxes-0.4.0/foxes/utils/geom2d/example_intersection.py` & `foxes-0.4.1/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/utils/geom2d/example_union.py` & `foxes-0.4.1/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.4.0/foxes/utils/geom2d/half_plane.py` & `foxes-0.4.1/foxes/utils/geom2d/half_plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     :group: utils.geom2d
 
     """
 
     def __init__(self, centre, n):
         """
         Constructor.
-        
+
         Parameters
         ----------
         centre: numpy.ndarray
             The centre point, shape: (2,)
         n: numpy.ndarray
             The direction vector to the inside, shape: (2,)
```

### Comparing `foxes-0.4.0/foxes/utils/geom2d/polygon.py` & `foxes-0.4.1/foxes/utils/geom2d/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     :group: utils.geom2d
 
     """
 
     def __init__(self, points):
         """
         Constructor.
-        
+
         Parameters
         ----------
         points: numpy.ndarray
             The polygon points, shape: (n_points, 2)
 
         """
         self.points = points
```

### Comparing `foxes-0.4.0/foxes/utils/geopandas_helpers.py` & `foxes-0.4.1/foxes/utils/geopandas_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     kwargs: dict, optional
         Additional parameters for geopandas.read_file()
 
     Returns
     -------
     data: geopandas.GeoDataFrame
         The data frame in WSG84
-    
+
     :group: utils
 
     """
     check_import_gpd()
     gpdf = gpd.read_file(fname, **kwargs)
     return gpdf.to_crs("EPSG:4326")  # Convert to WGS84
 
@@ -84,15 +84,15 @@
         Path to the output .csv file
     in_kwargs: dict
         Additional parameters for geopandas.read_file()
     out_kwargs: dict
         Additional parameters for geopandas to_csv()
     verbosity: int
         The verbosity level, 0 = silent
-    
+
     :group: utils
 
     """
     if verbosity > 0:
         print("Reading file", ifile)
 
     gpdf = read_shp(ifile, **in_kwargs)
@@ -163,15 +163,15 @@
         Dict with list of array of points. Key: area name,
         Value: list:np.ndarray, shape of latter: (n_points, 2)
     point_dict_interior: dict
         Dict with list of array of points. Key: area name,
         Value: list:np.ndarray, shape of latter: (n_points, 2)
     utm_zone_str: str, optional
         The utem zone plus letter as str, e.g. "32U"
-    
+
     :group: utils
 
     """
 
     pdf = read_shp(fname, **kwargs)
     pnames = list(pdf[name_col])
 
@@ -240,17 +240,17 @@
 
     Returns
     -------
     geom: foxes.tools.geom2D.AreaGeometry
         The geometry object
     utm_zone_str: str, optional
         The utem zone plus letter as str, e.g. "32U"
-    
+
     :group: utils
-    
+
     """
 
     exint = read_shp_polygons(*args, ret_utm_zone=ret_utm_zone, **kwargs)
 
     def _create_geom(data):
         if not len(data):
             return None
```

### Comparing `foxes-0.4.0/foxes/utils/pandas_helpers.py` & `foxes-0.4.1/foxes/utils/pandas_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     DEFAULT_WRITING_PARAMETERS: dict
         Default parameters for file writing
         for the supported file formats
     DATA_FILE_FORMAT: list:str
         The supported file formats for data export
     DEFAULT_FORMAT_DICT: dict
         Default column formatting
-    
+
     :group: utils
 
     """
 
     DEFAULT_READING_PARAMETERS = {
         "csv": {},
         "csv.gz": {},
```

### Comparing `foxes-0.4.0/foxes/utils/runners/runners.py` & `foxes-0.4.1/foxes/utils/runners/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dask
 from abc import abstractmethod, ABCMeta
 from copy import deepcopy
 from dask.distributed import Client, LocalCluster
 from dask.distributed import get_client
 from dask.diagnostics import ProgressBar
 
+
 class Runner(metaclass=ABCMeta):
     """
     Abstract base class for runners.
 
     :group: utils.runners
 
     """
@@ -131,15 +132,15 @@
         cluster_args=None,
         client_args={},
         progress_bar=True,
         verbosity=1,
     ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         scheduler: str, optional
             The dask scheduler choice
         n_workers: int, optional
             The number of workers for parallel run
         threads_per_worker: int, optional
@@ -190,32 +191,30 @@
             return False
 
     def initialize(self):
         """
         Initialize the runner
         """
         if self.scheduler == "distributed":
-
             self.print("Launching local dask cluster..")
 
             self._cluster = LocalCluster(**self.cluster_args)
             self._client = Client(self._cluster, **self.client_args)
 
             self.print(self._cluster)
             self.print(f"Dashboard: {self._client.dashboard_link}\n")
 
         elif self.scheduler == "slurm":
-
             from dask_jobqueue import SLURMCluster
 
             self.print("Launching dask cluster on HPC using SLURM..")
 
             cargs = deepcopy(self.cluster_args)
             nodes = cargs.pop("nodes", 1)
-            
+
             self._cluster = SLURMCluster(**cargs)
             self._cluster.scale(jobs=nodes)
             self._client = Client(self._cluster, **self.client_args)
 
             self.print(self._cluster)
             self.print(f"Dashboard: {self._client.dashboard_link}\n")
```

### Comparing `foxes-0.4.0/foxes/utils/two_circles.py` & `foxes-0.4.1/foxes/utils/two_circles.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         The distance between the centre points
         of the two circles
 
     Returns
     -------
     area: float or numpy.ndarray
         The intersectional area
-    
+
     :group: utils.two_circles
 
     """
     d1 = (r1**2 - r2**2 + d**2) / (2 * d)
     d2 = d - d1
 
     a = np.maximum(np.minimum(d1 / r1, 1.0), -1)
@@ -72,15 +72,15 @@
         The distance between the centre points
         of the two circles
 
     Returns
     -------
     area: numpy.ndarray
         The intersectional area
-    
+
     :group: utils.two_circles
 
     """
 
     # prepare:
     out = np.zeros_like(d)
```

### Comparing `foxes-0.4.0/foxes/utils/wind_dir.py` & `foxes-0.4.1/foxes/utils/wind_dir.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         Location where to insert the (x, y) dimension
         into the shape of wd
 
     Returns
     -------
     wdvec: numpy.ndarray
         The wind direction vectors
-    
+
     :group: utils
 
     """
 
     wdr = wd * np.pi / 180.0
     n = np.stack([np.sin(wdr), np.cos(wdr)], axis=axis)
```

### Comparing `foxes-0.4.0/foxes.egg-info/PKG-INFO` & `foxes-0.4.1/foxes.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.4.0
+Version: 0.4.1
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
 Keywords: Wind farm,Wake modelling,Wind farm optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: scripts
 License-File: LICENSE
 
@@ -43,14 +43,38 @@
 
 Source code: [https://github.com/FraunhoferIWES/foxes](https://github.com/FraunhoferIWES/foxes)
 
 PyPi reference: [https://pypi.org/project/foxes/](https://pypi.org/project/foxes/)
 
 Anaconda reference: [https://anaconda.org/conda-forge/foxes](https://anaconda.org/conda-forge/foxes)
 
+## Citation
+
+Please cite the JOSS paper `"FOXES: Farm Optimization and eXtended yield
+Evaluation Software"` 
+
+ [![DOI](https://joss.theoj.org/papers/10.21105/joss.05464/status.svg)](https://doi.org/10.21105/joss.05464)
+
+ Bibtex:
+ ```
+@article{
+    Schmidt2023, 
+    author = {Jonas Schmidt and Lukas Vollmer and Martin Dörenkämper and Bernhard Stoevesandt}, 
+    title = {FOXES: Farm Optimization and eXtended yield Evaluation Software}, 
+    doi = {10.21105/joss.05464}, 
+    url = {https://doi.org/10.21105/joss.05464}, 
+    year = {2023}, 
+    publisher = {The Open Journal}, 
+    volume = {8}, 
+    number = {86}, 
+    pages = {5464}, 
+    journal = {Journal of Open Source Software} 
+}
+ ```
+
 ## Requirements
 
 The supported Python versions are: 
 
 - `Python 3.7`
 - `Python 3.8`
 - `Python 3.9`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foxes-0.4.0/foxes.egg-info/SOURCES.txt` & `foxes-0.4.1/foxes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 foxes/algorithms/downwind/models/set_amb_farm_results.py
 foxes/algorithms/downwind/models/set_amb_point_results.py
 foxes/algorithms/iterative/__init__.py
 foxes/algorithms/iterative/iterative.py
 foxes/algorithms/iterative/models/__init__.py
 foxes/algorithms/iterative/models/convergence.py
 foxes/algorithms/iterative/models/farm_wakes_calc.py
-foxes/algorithms/iterative/models/loop_runner.py
 foxes/core/__init__.py
 foxes/core/algorithm.py
 foxes/core/data.py
 foxes/core/data_calc_model.py
 foxes/core/farm_controller.py
 foxes/core/farm_data_model.py
 foxes/core/farm_model.py
@@ -59,14 +58,15 @@
 foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
 foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
 foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
 foxes/data/power_ct_curves/__init__.py
 foxes/data/states/WRF-Timeseries-4464.csv.gz
 foxes/data/states/__init__.py
 foxes/data/states/abl_states_6000.csv.gz
+foxes/data/states/timeseries_100.csv.gz
 foxes/data/states/timeseries_3000.csv.gz
 foxes/data/states/timeseries_8000.csv.gz
 foxes/data/states/wind_rose_bremen.csv
 foxes/data/states/wind_rotation.nc
 foxes/input/__init__.py
 foxes/input/farm_layout/__init__.py
 foxes/input/farm_layout/from_csv.py
@@ -132,14 +132,15 @@
 foxes/models/vertical_profiles/abl_log_ws.py
 foxes/models/vertical_profiles/sheared_ws.py
 foxes/models/vertical_profiles/uniform.py
 foxes/models/wake_frames/__init__.py
 foxes/models/wake_frames/farm_order.py
 foxes/models/wake_frames/rotor_wd.py
 foxes/models/wake_frames/streamlines.py
+foxes/models/wake_frames/timelines.py
 foxes/models/wake_frames/yawed_wakes.py
 foxes/models/wake_models/__init__.py
 foxes/models/wake_models/axisymmetric.py
 foxes/models/wake_models/dist_sliced.py
 foxes/models/wake_models/gaussian.py
 foxes/models/wake_models/top_hat.py
 foxes/models/wake_models/ti/__init__.py
```

### Comparing `foxes-0.4.0/setup.cfg` & `foxes-0.4.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	Source Code = https://github.com/FraunhoferIWES/foxes
 	Bug Tracker = https://github.com/FraunhoferIWES/foxes/issues
 	Documentation = https://fraunhoferiwes.github.io/foxes.docs/index.html
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 
 [options]
 zip_safe = True
 include_package_data = True
 package_dir = 
 packages = find:
 python_requires = 
@@ -32,14 +32,15 @@
 	dask[distributed]
 	scipy
 	netcdf4
 	plotly
 	kaleido
 	iwopy>=0.1.4
 	pymoo>=0.6
+	tqdm
 
 [options.extras_require]
 test = 
 	flake8
 	pytest
 doc = 
 	sphinx
```


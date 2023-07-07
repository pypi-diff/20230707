# Comparing `tmp/power-grid-model-1.5.0rc9205913270508.tar.gz` & `tmp/power-grid-model-1.5.0rc9207011180609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9205913270508.tar", last modified: Fri Jul  7 08:05:35 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9207011180609.tar", last modified: Fri Jul  7 13:11:08 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9205913270508.tar` & `power-grid-model-1.5.0rc9207011180609.tar`

### file list

```diff
@@ -1,622 +1,622 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.974006 power-grid-model-1.5.0rc9205913270508/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-07 08:05:35.974006 power-grid-model-1.5.0rc9205913270508/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 08:04:55.000000 power-grid-model-1.5.0rc9205913270508/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.886005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.886005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.866005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.886005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.886005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.890005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    68269 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.890005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.890005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.890005 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/include/
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
--rw-r--r--   0 runner    (1001) docker     (123)    15757 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:05:35.974006 power-grid-model-1.5.0rc9205913270508/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.866005 power-grid-model-1.5.0rc9205913270508/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.894005 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.894005 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.894005 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.894005 power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-07 08:05:35.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-07-07 08:05:35.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:05:35.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 08:05:35.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 08:05:35.000000 power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.886005 power-grid-model-1.5.0rc9205913270508/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.882005 power-grid-model-1.5.0rc9205913270508/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.878005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.894005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.898005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.898005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.902005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.902005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.902005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.902005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.906005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.906005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.906005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.910005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.910005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.878005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.874005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.874005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.910005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.914005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.914005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.914005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.914005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.918005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.918005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.918005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.918005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.878005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.918005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.922005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.922005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.922005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.922005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.926005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.926005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.926005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.926005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.878005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.878005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.930005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.930005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.878005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.930005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.930005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.934005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.934005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.938005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.942005 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.882005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.942005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.946005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.950005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.954005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.954005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.954005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.958005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.958005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.958005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.958005 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.882005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.958005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.962005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.962005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.962005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.962005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.966005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.970005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.970005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.970005 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.970005 power-grid-model-1.5.0rc9205913270508/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:05:35.974006 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-07-07 08:04:49.000000 power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.854103 power-grid-model-1.5.0rc9207011180609/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-07 13:11:08.854103 power-grid-model-1.5.0rc9207011180609/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 13:10:18.000000 power-grid-model-1.5.0rc9207011180609/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.730103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.730103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.718103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.730103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.734103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17079 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.738103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68269 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.738103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30819 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.738103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.738103 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15757 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:11:08.854103 power-grid-model-1.5.0rc9207011180609/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.718103 power-grid-model-1.5.0rc9207011180609/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.742103 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.746103 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.746103 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34661 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29948 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.742103 power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-07 13:11:08.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-07-07 13:11:08.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:11:08.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 13:11:08.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 13:11:08.000000 power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.746103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.746103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.750103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.750103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.754103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.762103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.762103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.762103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.766103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.766103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.770103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.770103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.722103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.722103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.722103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.770103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.774103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.774103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.778103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.782103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.786103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.790103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.790103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.794103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.722103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.794103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.798103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.798103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.802103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.802103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.802103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.806103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.806103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.810103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.722103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.810103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.810103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.814103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.814103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.818103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.818103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.818103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.822103 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.822103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.826103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.826103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.830103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.830103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.830103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.834103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.834103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:04.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.834103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.838103 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.726103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.838103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.842103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.842103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.846103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.846103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.846103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.850103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.850103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.850103 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.850103 power-grid-model-1.5.0rc9207011180609/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:11:08.854103 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29354 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-07 13:10:05.000000 power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9205913270508/LICENSE` & `power-grid-model-1.5.0rc9207011180609/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/PKG-INFO` & `power-grid-model-1.5.0rc9207011180609/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9205913270508
+Version: 1.5.0rc9207011180609
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9205913270508/README.md` & `power-grid-model-1.5.0rc9207011180609/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,25 @@
 };
 
 enum class FaultType : IntS {
     three_phase = 0,
     single_phase_to_ground = 1,
     two_phase = 2,
     two_phase_to_ground = 3,
-    default_value = na_IntS
+    nan = na_IntS
 };
 
-enum class FaultPhase : IntS { abc = 0, a = 1, b = 2, c = 3, ab = 4, ac = 5, bc = 6, default_value = na_IntS };
+enum class FaultPhase : IntS {
+    abc = 0,
+    a = 1,
+    b = 2,
+    c = 3,
+    ab = 4,
+    ac = 5,
+    bc = 6,
+    default_value = -1,
+    nan = na_IntS
+};
 
 }  // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,18 @@
     explicit UnknownAttributeName(std::string const &attr_name) {
         append_msg("Unknown attribute name!" + attr_name + "\n");
     }
 };
 
 class InvalidShortCircuitType : public PowerGridError {
    public:
+    explicit InvalidShortCircuitType(FaultType short_circuit_type) {
+        append_msg("The short circuit type (" + std::to_string(static_cast<IntS>(short_circuit_type)) +
+                   ") is invalid!\n");
+    }
     InvalidShortCircuitType(bool sym, FaultType short_circuit_type) {
         append_msg("The short circuit type (" + std::to_string(static_cast<IntS>(short_circuit_type)) +
                    ") does not match the calculation type (symmetric=" + std::to_string(sym) + ")\n");
     }
 };
 
 class InvalidShortCircuitPhases : public PowerGridError {
```

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/short_circuit_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp` & `power-grid-model-1.5.0rc9207011180609/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/pyproject.toml` & `power-grid-model-1.5.0rc9207011180609/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/setup.py` & `power-grid-model-1.5.0rc9207011180609/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/__init__.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/data_handling.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/data_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 class FaultType(IntEnum):
     """The type of fault represented by a fault component"""
 
     three_phase = 0
     single_phase_to_ground = 1
     two_phase = 2
     two_phase_to_ground = 3
-    default_value = -128
+    nan = -128
     """
-    Unspecified fault phase. Like np.nan. Needs to be overloaded at the latest in the update_data
+    Unspecified fault type. Needs to be overloaded at the latest in the update_data
     """
 
 
 class FaultPhase(IntEnum):
     """The faulty phase(s) affected by the provided fault type"""
 
     abc = 0
@@ -150,13 +150,17 @@
     """
     ac = 5
     """
     The first and third phase are faulty in a two-phase or two-phase-to-ground fault
     """
     bc = 6
     """
-    The first and second phase are faulty in a two-phase or two-phase-to-ground fault
+    The second and third phase are faulty in a two-phase or two-phase-to-ground fault
+    """
+    default_value = -1
+    """
+    Use the default fault phase. Depends on the fault_type.
     """
-    default_value = -128
+    nan = -128
     """
-    Unspecified fault phase. Like np.nan. Needs to be overloaded at the latest in the update_data
+    Unspecified fault phase. Needs to be overloaded at the latest in the update_data
     """
```

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 Error classes
 """
 import re
 from abc import ABC
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
 
 
 class ValidationError(ABC):
     """
     The Validation Error is an abstract base class which should be extended by all validation errors. It supplies
     three public member variables: component, field and ids; storing information about the origin of the validation
     error. Error classes can extend the public members. For example:
@@ -188,14 +188,32 @@
         return "/".join(self.component)
 
     @property
     def field_str(self) -> str:
         return " and ".join(f"{component}.{field}" for component, field in self.field)
 
 
+class NotIdenticalError(SingleFieldValidationError):
+    """
+    The value is not unique within a single column in a dataset
+    E.g. When two nodes share the same id.
+    """
+
+    _message = "Field {field} is not unique for {n} {objects}: {num_unique} different values."
+    values: List[Any]
+    unique: Set[Any]
+    num_unique: int
+
+    def __init__(self, component: str, field: str, ids: List[int], values: List[Any]):
+        super().__init__(component, field, ids)
+        self.values = values
+        self.unique = set(self.values)
+        self.num_unique = len(self.unique)
+
+
 class NotUniqueError(SingleFieldValidationError):
     """
     The value is not unique within a single column in a dataset
     E.g. When two nodes share the same id.
     """
 
     _message = "Field {field} is not unique for {n} {objects}."
@@ -424,15 +442,23 @@
     """
 
     _message = "Field {field} is infinite for {n} {objects}."
 
 
 class TransformerClockError(MultiFieldValidationError):
     """
-    The value of a field is infinite.
+    Invalid clock number.
     """
 
     _message = (
         "Invalid clock number for {n} {objects}. "
         "If one side has wye winding and the other side has not, the clock number should be odd. "
         "If either both or none of the sides have wye winding, the clock number should be even."
     )
+
+
+class FaultPhaseError(MultiFieldValidationError):
+    """
+    The fault phase does not match the fault type.
+    """
+
+    _message = "The fault phase is not applicable to the corresponding fault type for {n} {objects}."
```

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,28 +36,30 @@
 """
 from enum import Enum
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 
 from power_grid_model.data_types import SingleDataset
-from power_grid_model.enum import WindingType
+from power_grid_model.enum import FaultPhase, FaultType, WindingType
 from power_grid_model.validation.errors import (
     ComparisonError,
+    FaultPhaseError,
     IdNotInDatasetError,
     InfinityError,
     InvalidEnumValueError,
     InvalidIdError,
     MissingValueError,
     MultiComponentNotUniqueError,
     NotBetweenError,
     NotBetweenOrAtError,
     NotBooleanError,
     NotGreaterOrEqualError,
     NotGreaterThanError,
+    NotIdenticalError,
     NotLessOrEqualError,
     NotLessThanError,
     NotUniqueError,
     SameValueError,
     TransformerClockError,
     TwoValuesZeroError,
     ValidationError,
@@ -351,14 +353,65 @@
         if matches.ndim > 1:
             matches = matches.any(axis=1)
         ids = component_data["id"][matches].flatten().tolist()
         return [error(component, field, ids, ref_value)]
     return []
 
 
+def all_identical(data: SingleDataset, component: str, field: str) -> List[NotIdenticalError]:
+    """
+    Check that for all records of a particular type of component, the values in the 'field' column are identical.
+
+    Args:
+        data: The input/update data set for all components
+        component: The component of interest
+        field: The field of interest
+
+    Returns:
+        A list containing zero or one NotIdenticalError, listing all ids of that component if the value in the field
+        of interest was not identical across all components, all values for those ids, the set of unique values in
+        that field and the number of unique values in that field.
+    """
+    field_data = data[component][field]
+    if len(field_data) > 0:
+        first = field_data[0]
+        if np.any(field_data != first):
+            return [NotIdenticalError(component, field, data[component]["id"], list(field_data))]
+
+    return []
+
+
+def all_enabled_identical(
+    data: SingleDataset, component: str, field: str, status_field: str
+) -> List[NotIdenticalError]:
+    """
+    Check that for all records of a particular type of component, the values in the 'field' column are identical.
+    Only entries are checked where the 'status' field is not 0.
+
+    Args:
+        data: The input/update data set for all components
+        component: The component of interest
+        field: The field of interest
+        status_field: The status field based on which to decide whether a component is enabled
+
+    Returns:
+        A list containing zero or one NotIdenticalError, listing:
+            - all ids of enabled components if the value in the field of interest was not identical across all enabled
+              components
+            - all values of the 'field' column for enabled components (including duplications)
+            - the set of unique such values
+            - the amount of unique such values.
+    """
+    return all_identical(
+        {key: (value if key is not component else value[value[status_field] != 0]) for key, value in data.items()},
+        component,
+        field,
+    )
+
+
 def all_unique(data: SingleDataset, component: str, field: str) -> List[NotUniqueError]:
     """
     Check that for all records of a particular type of component, the values in the 'field' column are unique within
     the 'field' column of that component.
 
     Args:
         data: The input/update data set for all components
@@ -366,22 +419,18 @@
         field: The field of interest
 
     Returns:
         A list containing zero or one NotUniqueError, listing all ids where the value in the field of interest was
         not unique. If the field name was 'id' (a very common check), the id is added as many times as it occurred in
         the 'id' column, to maintain object counts.
     """
-    _, index, counts = np.unique(data[component][field], return_index=True, return_counts=True)
+    field_data = data[component][field]
+    _, inverse, counts = np.unique(field_data, return_inverse=True, return_counts=True)
     if any(counts != 1):
-        ids = data[component]["id"][index[counts != 1]].flatten().tolist()
-        if field == "id":  # Add ids multiple times
-            counts = counts[counts != 1]
-            for obj_id, count in zip(ids, counts):
-                ids += [obj_id] * (count - 1)
-            ids = sorted(ids)
+        ids = data[component]["id"][(counts != 1)[inverse]].flatten().tolist()
         return [NotUniqueError(component, field, ids)]
     return []
 
 
 def all_cross_unique(
     data: SingleDataset, fields: List[Tuple[str, str]], cross_only=True
 ) -> List[MultiComponentNotUniqueError]:
@@ -671,7 +720,61 @@
             TransformerClockError(
                 component=component,
                 fields=[clock_field, winding_from_field, winding_to_field],
                 ids=data[component]["id"][err].flatten().tolist(),
             )
         ]
     return []
+
+
+def all_valid_fault_phases(
+    data: SingleDataset, component: str, fault_type_field: str, fault_phase_field: str
+) -> List[FaultPhaseError]:
+    """
+    Custom validation rule: Only a subset of fault_phases is supported for each fault type.
+
+    Args:
+        data: The input/update data set for all components
+        component: The component of interest
+        fault_type_field: The fault type field
+        fault_phase_field: The fault phase field
+
+    Returns:
+        A list containing zero or more FaultPhaseErrors; listing all the ids of faults where the fault phase was
+        invalid, given the fault phase.
+    """
+    fault_types = data[component][fault_type_field]
+    fault_phases = data[component][fault_phase_field]
+
+    supported_combinations: Dict[FaultType, List[FaultPhase]] = {
+        FaultType.three_phase: [FaultPhase.abc, FaultPhase.default_value, FaultPhase.nan],
+        FaultType.single_phase_to_ground: [
+            FaultPhase.a,
+            FaultPhase.b,
+            FaultPhase.c,
+            FaultPhase.default_value,
+            FaultPhase.nan,
+        ],
+        FaultType.two_phase: [FaultPhase.ab, FaultPhase.ac, FaultPhase.bc, FaultPhase.default_value, FaultPhase.nan],
+        FaultType.two_phase_to_ground: [
+            FaultPhase.ab,
+            FaultPhase.ac,
+            FaultPhase.bc,
+            FaultPhase.default_value,
+            FaultPhase.nan,
+        ],
+        FaultType.nan: [],
+    }
+
+    def _fault_phase_supported(fault_type: FaultType, fault_phase: FaultPhase):
+        return fault_phase not in supported_combinations.get(fault_type, [])
+
+    err = np.vectorize(_fault_phase_supported)(fault_type=fault_types, fault_phase=fault_phases)
+    if err.any():
+        return [
+            FaultPhaseError(
+                component=component,
+                fields=[fault_type_field, fault_phase_field],
+                ids=data[component]["id"][err].flatten().tolist(),
+            )
+        ]
+    return []
```

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model/validation/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from power_grid_model import power_grid_meta_data
 from power_grid_model.data_types import BatchDataset, Dataset, SingleDataset
 from power_grid_model.enum import (
     Branch3Side,
     BranchSide,
     CalculationType,
+    FaultPhase,
+    FaultType,
     LoadGenType,
     MeasuredTerminalType,
     WindingType,
 )
 from power_grid_model.utils import convert_batch_dataset_to_batch_list
 from power_grid_model.validation.errors import (
     IdNotInDatasetError,
@@ -32,25 +34,27 @@
     ValidationError,
 )
 from power_grid_model.validation.rules import (
     all_between,
     all_between_or_at,
     all_boolean,
     all_cross_unique,
+    all_enabled_identical,
     all_finite,
     all_greater_or_equal,
     all_greater_than_or_equal_to_zero,
     all_greater_than_zero,
     all_ids_exist_in_data_set,
     all_less_than,
     all_not_two_values_equal,
     all_not_two_values_zero,
     all_unique,
     all_valid_clocks,
     all_valid_enum_values,
+    all_valid_fault_phases,
     all_valid_ids,
     none_missing,
 )
 from power_grid_model.validation.utils import update_input_data
 
 
 def validate_input_data(
@@ -305,15 +309,26 @@
         required["voltage_sensor"] += ["u_sigma", "u_measured"]
         required["power_sensor"] += ["power_sigma", "p_measured", "q_measured"]
     required["sym_voltage_sensor"] = required["voltage_sensor"].copy()
     required["asym_voltage_sensor"] = required["voltage_sensor"].copy()
     required["sym_power_sensor"] = required["power_sensor"].copy()
     required["asym_power_sensor"] = required["power_sensor"].copy()
 
-    if not symmetric:
+    # Faults
+    required["fault"] = required["base"] + ["fault_object"]
+    asym_sc = False
+    if calculation_type is None or calculation_type == CalculationType.short_circuit:
+        required["fault"] += ["status", "fault_type"]
+        if "fault" in data:
+            for elem in data["fault"]["fault_type"]:
+                if elem not in (FaultType.three_phase, FaultType.nan):
+                    asym_sc = True
+                    break
+
+    if not symmetric or asym_sc:
         required["line"] += ["r0", "x0", "c0", "tan0"]
         required["shunt"] += ["g0", "b0"]
 
     return list(chain(*(none_missing(data, component, required.get(component, [])) for component in data)))
 
 
 def validate_values(data: SingleDataset) -> List[ValidationError]:  # pylint: disable=too-many-branches
@@ -353,14 +368,16 @@
         errors += validate_generic_voltage_sensor(data, "sym_voltage_sensor")
     if "asym_voltage_sensor" in data:
         errors += validate_generic_voltage_sensor(data, "asym_voltage_sensor")
     if "sym_power_sensor" in data:
         errors += validate_generic_power_sensor(data, "sym_power_sensor")
     if "asym_power_sensor" in data:
         errors += validate_generic_power_sensor(data, "asym_power_sensor")
+    if "fault" in data:
+        errors += validate_fault(data)
     return errors
 
 
 # pylint: disable=missing-function-docstring
 
 
 def validate_base(data: SingleDataset, component: str) -> List[ValidationError]:
@@ -668,7 +685,20 @@
         component,
         field="measured_object",
         ref_components="node",
         measured_terminal_type=MeasuredTerminalType.node,
     )
 
     return errors
+
+
+def validate_fault(data: SingleDataset) -> List[ValidationError]:
+    errors = validate_base(data, "fault")
+    errors += all_boolean(data, "fault", "status")
+    errors += all_valid_enum_values(data, "fault", "fault_type", FaultType)
+    errors += all_valid_enum_values(data, "fault", "fault_phase", FaultPhase)
+    errors += all_valid_fault_phases(data, "fault", "fault_type", "fault_phase")
+    errors += all_valid_ids(data, "fault", field="fault_object", ref_components="node")
+    errors += all_greater_than_or_equal_to_zero(data, "fault", "r_f")
+    errors += all_enabled_identical(data, "fault", "fault_type", "status")
+    errors += all_enabled_identical(data, "fault", "fault_phase", "status")
+    return errors
```

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9205913270508
+Version: 1.5.0rc9207011180609
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9205913270508/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9207011180609/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9207011180609/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/three_phase_abc/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/three_phase_abc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9207011180609/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/utils.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_input_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 
 from typing import Dict
 
 import numpy as np
 import pytest
 
 from power_grid_model import Branch3Side, BranchSide, LoadGenType, MeasuredTerminalType, WindingType, initialize_array
+from power_grid_model.enum import CalculationType, FaultPhase, FaultType
 from power_grid_model.validation import validate_input_data
 from power_grid_model.validation.errors import (
+    FaultPhaseError,
     InvalidEnumValueError,
     InvalidIdError,
     MultiComponentNotUniqueError,
     NotBetweenError,
     NotBetweenOrAtError,
     NotBooleanError,
     NotGreaterOrEqualError,
     NotGreaterThanError,
+    NotIdenticalError,
     NotLessThanError,
     NotUniqueError,
     TwoValuesZeroError,
 )
 from power_grid_model.validation.utils import nan_type
 
 
@@ -216,14 +219,23 @@
 
     asym_power_sensor = initialize_array("input", "asym_power_sensor", 4)
     asym_power_sensor["id"] = [7, 8, 9, 10]
     asym_power_sensor["measured_object"] = [12, 3, 13, 200]
     asym_power_sensor["power_sigma"] = [1.0, np.nan, 0.0, -1.0]
     asym_power_sensor["measured_terminal_type"] = [1, 1, 10, 1]
 
+    fault = initialize_array("input", "fault", 20)
+    fault["id"] = [1] + list(range(32, 51))
+    fault["status"] = [0, -1, 2] + 17 * [1]
+    fault["fault_type"] = 6 * [0] + 4 * [1] + 4 * [2] + 4 * [3] + [nan_type("fault", "fault_type"), 4]
+    fault["fault_phase"] = list(range(1, 7)) + [0, 4, 5, 6] + 2 * list(range(4)) + [nan_type("fault", "fault_phase"), 7]
+    fault["fault_object"] = [200, 3] + list(range(10, 28, 2)) + 9 * [0]
+    fault["r_f"] = [-1.0, 0.0, 1.0] + 17 * [nan_type("fault", "r_f")]
+    fault["x_f"] = [-1.0, 0.0, 1.0] + 17 * [nan_type("fault", "x_f")]
+
     data = {
         "node": node,
         "line": line,
         "link": link,
         "transformer": transformer,
         "three_winding_transformer": three_winding_transformer,
         "source": source,
@@ -232,14 +244,15 @@
         "sym_gen": sym_gen,
         "asym_load": asym_load,
         "asym_gen": asym_gen,
         "sym_voltage_sensor": sym_voltage_sensor,
         "asym_voltage_sensor": asym_voltage_sensor,
         "sym_power_sensor": sym_power_sensor,
         "asym_power_sensor": asym_power_sensor,
+        "fault": fault,
     }
     return data
 
 
 def test_validate_input_data_sym_calculation(input_data):
     validation_errors = validate_input_data(input_data, symmetric=True)
 
@@ -255,14 +268,15 @@
                 ("source", "id"),
                 ("sym_gen", "id"),
                 ("sym_load", "id"),
                 ("sym_power_sensor", "id"),
                 ("sym_voltage_sensor", "id"),
                 ("transformer", "id"),
                 ("three_winding_transformer", "id"),
+                ("fault", "id"),
             ],
             [
                 ("asym_gen", 1),
                 ("asym_load", 1),
                 ("asym_power_sensor", 7),
                 ("asym_power_sensor", 8),
                 ("asym_power_sensor", 9),
@@ -282,14 +296,15 @@
                 ("sym_power_sensor", 10),
                 ("sym_voltage_sensor", 7),
                 ("sym_voltage_sensor", 8),
                 ("sym_voltage_sensor", 9),
                 ("sym_voltage_sensor", 10),
                 ("transformer", 1),
                 ("three_winding_transformer", 1),
+                ("fault", 1),
             ],
         )
         in validation_errors
     )
 
     assert NotGreaterThanError("node", "u_rated", [1], 0) in validation_errors
     assert NotUniqueError("node", "id", [2, 2]) in validation_errors
@@ -439,14 +454,17 @@
     assert (
         InvalidEnumValueError("asym_power_sensor", "measured_terminal_type", [9], MeasuredTerminalType)
         in validation_errors
     )
 
     assert NotGreaterOrEqualError("transformer", "uk_max", [15], "uk_min") not in validation_errors
 
+    assert NotBooleanError("fault", "status", [32, 33]) in validation_errors
+    assert InvalidIdError("fault", "fault_object", [1] + list(range(32, 42)), ["node"]) in validation_errors
+
 
 def test_validate_three_winding_transformer(input_data):
     validation_errors = validate_input_data(input_data, symmetric=True)
     assert NotBooleanError("three_winding_transformer", "status_1", [28]) in validation_errors
     assert NotBooleanError("three_winding_transformer", "status_2", [1]) in validation_errors
     assert NotBooleanError("three_winding_transformer", "status_3", [29]) in validation_errors
     assert InvalidIdError("three_winding_transformer", "node_1", [29], "node") in validation_errors
@@ -528,14 +546,40 @@
     assert NotGreaterOrEqualError("three_winding_transformer", "pk_13_min", [1], 0) in validation_errors
     assert NotGreaterOrEqualError("three_winding_transformer", "pk_23_min", [1], 0) in validation_errors
     assert NotGreaterOrEqualError("three_winding_transformer", "pk_12_max", [1], 0) in validation_errors
     assert NotGreaterOrEqualError("three_winding_transformer", "pk_13_max", [1], 0) in validation_errors
     assert NotGreaterOrEqualError("three_winding_transformer", "pk_23_max", [1], 0) in validation_errors
 
 
+def test_fault(input_data):
+    validation_errors = validate_input_data(input_data, calculation_type=CalculationType.short_circuit)
+    assert InvalidEnumValueError("fault", "fault_type", [50], FaultType) in validation_errors
+    assert InvalidEnumValueError("fault", "fault_phase", [50], FaultPhase) in validation_errors
+    assert FaultPhaseError("fault", ("fault_type", "fault_phase"), [1] + list(range(32, 51)))
+    assert NotGreaterOrEqualError("fault", "r_f", [1], 0) in validation_errors
+    assert (
+        NotIdenticalError(
+            "fault",
+            "fault_type",
+            list(range(32, 51)),
+            5 * [0] + 4 * [1] + 4 * [2] + 4 * [3] + [nan_type("fault", "fault_type"), 4],
+        )
+        in validation_errors
+    )
+    assert (
+        NotIdenticalError(
+            "fault",
+            "fault_phase",
+            list(range(32, 51)),
+            list(range(2, 7)) + [0, 4, 5, 6] + 2 * list(range(4)) + [nan_type("fault", "fault_phase"), 7],
+        )
+        in validation_errors
+    )
+
+
 def test_validate_input_data_asym_calculation(input_data):
     validation_errors = validate_input_data(input_data, symmetric=False)
     assert NotGreaterThanError("node", "u_rated", [1], 0) in validation_errors
     assert NotUniqueError("node", "id", [2, 2]) in validation_errors
     assert NotBooleanError("line", "from_status", [5]) in validation_errors
     assert NotBooleanError("line", "to_status", [4]) in validation_errors
     assert InvalidIdError("line", "from_node", [4], "node") in validation_errors
```

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9205913270508/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9207011180609/tests/unit/validation/test_validation_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # SPDX-FileCopyrightText: 2022 Contributors to the Power Grid Model project <dynamic.grid.calculation@alliander.com>
 #
 # SPDX-License-Identifier: MPL-2.0
 
+from itertools import product
 from typing import List, Union
 from unittest.mock import ANY, MagicMock, patch
 
 import numpy as np
 import pytest
 
 from power_grid_model import MeasuredTerminalType, initialize_array, power_grid_meta_data
-from power_grid_model.enum import CalculationType
+from power_grid_model.enum import CalculationType, FaultPhase, FaultType
 from power_grid_model.validation.errors import IdNotInDatasetError, MissingValueError, MultiComponentNotUniqueError
 from power_grid_model.validation.validation import (
     assert_valid_data_structure,
     validate_generic_power_sensor,
     validate_ids_exist,
     validate_required_values,
     validate_unique_ids_across_components,
@@ -130,14 +131,15 @@
 
 @pytest.mark.parametrize(
     "calculation_type",
     [
         pytest.param(None, id="no calculation type specified"),
         pytest.param(CalculationType.power_flow, id="power_flow"),
         pytest.param(CalculationType.state_estimation, id="state_estimation"),
+        pytest.param(CalculationType.short_circuit, id="short_circuit"),
     ],
 )
 @pytest.mark.parametrize("symmetric", [pytest.param(True, id="symmetric"), pytest.param(False, id="asymmetric")])
 def test_validate_required_values_sym_calculation(calculation_type, symmetric):
     node = initialize_array("input", "node", 1)
     line = initialize_array("input", "line", 1)
     link = initialize_array("input", "link", 1)
@@ -156,14 +158,16 @@
 
     sym_power_sensor = initialize_array("input", "sym_power_sensor", 1)
 
     asym_power_sensor = initialize_array("input", "asym_power_sensor", 1)
     asym_power_sensor["p_measured"] = [[np.nan, 2.0, 1.0]]
     asym_power_sensor["q_measured"] = [[2.0, 1.0, np.nan]]
 
+    fault = initialize_array("input", "fault", 1)
+
     data = {
         "node": node,
         "line": line,
         "link": link,
         "transformer": transformer,
         "three_winding_transformer": three_winding_transformer,
         "source": source,
@@ -172,19 +176,21 @@
         "sym_gen": sym_gen,
         "asym_load": asym_load,
         "asym_gen": asym_gen,
         "sym_voltage_sensor": sym_voltage_sensor,
         "asym_voltage_sensor": asym_voltage_sensor,
         "sym_power_sensor": sym_power_sensor,
         "asym_power_sensor": asym_power_sensor,
+        "fault": fault,
     }
     required_values_errors = validate_required_values(data=data, calculation_type=calculation_type, symmetric=symmetric)
 
     pf_dependent = calculation_type == CalculationType.power_flow or calculation_type is None
     se_dependent = calculation_type == CalculationType.state_estimation or calculation_type is None
+    sc_dependent = calculation_type == CalculationType.short_circuit or calculation_type is None
     asym_dependent = not symmetric
 
     assert MissingValueError("node", "id", [NaN]) in required_values_errors
     assert MissingValueError("node", "u_rated", [NaN]) in required_values_errors
 
     assert MissingValueError("line", "id", [NaN]) in required_values_errors
     assert MissingValueError("line", "from_node", [NaN]) in required_values_errors
@@ -323,14 +329,18 @@
     assert MissingValueError("asym_power_sensor", "id", [NaN]) in required_values_errors
     assert MissingValueError("asym_power_sensor", "measured_object", [NaN]) in required_values_errors
     assert MissingValueError("asym_power_sensor", "measured_terminal_type", [NaN]) in required_values_errors
     assert (MissingValueError("asym_power_sensor", "power_sigma", [NaN]) in required_values_errors) == se_dependent
     assert (MissingValueError("asym_power_sensor", "p_measured", [NaN]) in required_values_errors) == se_dependent
     assert (MissingValueError("asym_power_sensor", "q_measured", [NaN]) in required_values_errors) == se_dependent
 
+    assert MissingValueError("fault", "id", [NaN]) in required_values_errors
+    assert (MissingValueError("fault", "status", [NaN]) in required_values_errors) == sc_dependent
+    assert (MissingValueError("fault", "fault_type", [NaN]) in required_values_errors) == sc_dependent
+
 
 def test_validate_required_values_asym_calculation():
     line = initialize_array("input", "line", 1)
     shunt = initialize_array("input", "shunt", 1)
 
     data = {"line": line, "shunt": shunt}
     required_values_errors = validate_required_values(data=data, symmetric=False)
@@ -340,14 +350,37 @@
     assert MissingValueError("line", "c0", [NaN]) in required_values_errors
     assert MissingValueError("line", "tan0", [NaN]) in required_values_errors
 
     assert MissingValueError("shunt", "g0", [NaN]) in required_values_errors
     assert MissingValueError("shunt", "b0", [NaN]) in required_values_errors
 
 
+@pytest.mark.parametrize("fault_types", product(list(FaultType), list(FaultType)))
+def test_validate_fault_sc_calculation(fault_types):
+    line = initialize_array("input", "line", 1)
+    shunt = initialize_array("input", "shunt", 1)
+    fault = initialize_array("input", "fault", 2)
+    fault["fault_type"] = fault_types
+
+    data = {"line": line, "shunt": shunt, "fault": fault}
+    required_values_errors = validate_required_values(data=data, calculation_type=CalculationType.short_circuit)
+
+    asym_sc_calculation = np.any(
+        list(fault_type not in (FaultType.three_phase, FaultType.nan) for fault_type in fault_types)
+    )
+
+    assert (MissingValueError("line", "r0", [NaN]) in required_values_errors) == asym_sc_calculation
+    assert (MissingValueError("line", "x0", [NaN]) in required_values_errors) == asym_sc_calculation
+    assert (MissingValueError("line", "c0", [NaN]) in required_values_errors) == asym_sc_calculation
+    assert (MissingValueError("line", "tan0", [NaN]) in required_values_errors) == asym_sc_calculation
+
+    assert (MissingValueError("shunt", "g0", [NaN]) in required_values_errors) == asym_sc_calculation
+    assert (MissingValueError("shunt", "b0", [NaN]) in required_values_errors) == asym_sc_calculation
+
+
 def test_validate_values():
     # Create invalid nodes and lines
     node = initialize_array("input", "node", 3)
     line = initialize_array("input", "line", 3)
 
     # Validate nodes and lines individually
     node_errors = validate_values({"node": node})
```


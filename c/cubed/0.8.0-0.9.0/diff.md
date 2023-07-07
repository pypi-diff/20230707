# Comparing `tmp/cubed-0.8.0.tar.gz` & `tmp/cubed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubed-0.8.0.tar", last modified: Fri Jun 16 11:03:06 2023, max compression
+gzip compressed data, was "cubed-0.9.0.tar", last modified: Fri Jul  7 13:20:05 2023, max compression
```

## Comparing `cubed-0.8.0.tar` & `cubed-0.9.0.tar`

### file list

```diff
@@ -1,111 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 11:02:53.000000 cubed-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 11:03:06.533476 cubed-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-16 11:02:53.000000 cubed-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.517476 cubed-0.8.0/cubed/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.521476 cubed-0.8.0/cubed/array_api/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/array_object.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/creation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/data_type_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/elementwise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/indexing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/linear_algebra_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/manipulation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/searching_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/statistical_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/array_api/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.521476 cubed-0.8.0/cubed/core/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/gufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/core/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/extensions/tqdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/blockwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/rechunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/primitive/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/runtime/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/beam.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/lithops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/modal_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/executors/python_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.525476 cubed-0.8.0/cubed/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/storage/zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.529476 cubed-0.8.0/cubed/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.529476 cubed-0.8.0/cubed/tests/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/primitive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/primitive/test_blockwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/primitive/test_rechunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.529476 cubed-0.8.0/cubed/tests/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_lithops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_modal_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/test_python_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/storage/test_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_array_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_gufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_mem_utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/dask/array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/gufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/array/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/blockwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/dask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/rechunker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.533476 cubed-0.8.0/cubed/vendor/rechunker/executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/executors/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-16 11:02:53.000000 cubed-0.8.0/cubed/vendor/rechunker/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:03:06.517476 cubed-0.8.0/cubed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 11:03:06.000000 cubed-0.8.0/cubed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-16 11:02:53.000000 cubed-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-16 11:03:06.537476 cubed-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 11:02:53.000000 cubed-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.815186 cubed-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-07 13:19:45.000000 cubed-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-07 13:20:05.815186 cubed-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-07 13:19:45.000000 cubed-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.799184 cubed-0.9.0/cubed/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.803185 cubed-0.9.0/cubed/array_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/array_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/creation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/data_type_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/elementwise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/indexing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/linear_algebra_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/manipulation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/searching_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/statistical_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/array_api/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.803185 cubed-0.9.0/cubed/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16524 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/core/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/core/gufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27022 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/core/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/core/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.803185 cubed-0.9.0/cubed/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/extensions/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/extensions/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/extensions/tqdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.803185 cubed-0.9.0/cubed/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/primitive/blockwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/primitive/rechunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/primitive/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.807185 cubed-0.9.0/cubed/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.807185 cubed-0.9.0/cubed/runtime/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/beam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/lithops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/lithops_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/modal_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/executors/python_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.807185 cubed-0.9.0/cubed/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/storage/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/storage/zarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.811185 cubed-0.9.0/cubed/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.811185 cubed-0.9.0/cubed/tests/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/primitive/test_blockwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/primitive/test_rechunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.811185 cubed-0.9.0/cubed/tests/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/test_lithops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/test_lithops_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/test_modal_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/test_python_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.811185 cubed-0.9.0/cubed/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/storage/test_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16740 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_array_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17318 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_gufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_mem_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.811185 cubed-0.9.0/cubed/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.815186 cubed-0.9.0/cubed/vendor/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.815186 cubed-0.9.0/cubed/vendor/dask/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/array/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/array/gufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/array/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/array/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/array/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14901 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/blockwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.815186 cubed-0.9.0/cubed/vendor/dask/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/dask/widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.815186 cubed-0.9.0/cubed/vendor/rechunker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.815186 cubed-0.9.0/cubed/vendor/rechunker/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/executors/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-07 13:19:45.000000 cubed-0.9.0/cubed/vendor/rechunker/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:20:05.799184 cubed-0.9.0/cubed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-07 13:20:05.000000 cubed-0.9.0/cubed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-07 13:20:05.000000 cubed-0.9.0/cubed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:20:05.000000 cubed-0.9.0/cubed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-07 13:20:05.000000 cubed-0.9.0/cubed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 13:20:05.000000 cubed-0.9.0/cubed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-07 13:19:45.000000 cubed-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-07 13:20:05.815186 cubed-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-07 13:19:45.000000 cubed-0.9.0/setup.py
```

### Comparing `cubed-0.8.0/LICENSE` & `cubed-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/PKG-INFO` & `cubed-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.8.0
+Version: 0.9.0
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
@@ -32,9 +32,10 @@
 Cubed is a distributed N-dimensional array library implemented in Python using bounded-memory serverless processing and Zarr for storage.
 
 - Implements the [Python Array API standard](https://data-apis.org/array-api/latest/) (see [coverage status](./api_status.md))
 - Guaranteed maximum memory usage for standard array functions
 - Follows [Dask Array](https://docs.dask.org/en/stable/array.html)'s chunked array API (`map_blocks`, `rechunk`, `apply_gufunc`, etc)
 - [Zarr](https://zarr.readthedocs.io/en/stable/) for persistent and intermediate storage
 - Multiple serverless runtimes: Python (in-process), [Lithops](https://lithops-cloud.github.io/), [Modal](https://modal.com/), [Apache Beam](https://beam.apache.org/)
+- Integration with [Xarray](https://xarray.dev/) via [cubed-xarray](https://github.com/xarray-contrib/cubed-xarray)
 
 [Documentation](https://tomwhite.github.io/cubed)
```

### Comparing `cubed-0.8.0/cubed/__init__.py` & `cubed-0.9.0/cubed/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/array_api/__init__.py` & `cubed-0.9.0/cubed/array_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/array_api/array_object.py` & `cubed-0.9.0/cubed/array_api/array_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import operator
 
 import numpy as np
 
 from cubed.array_api.creation_functions import asarray
 from cubed.array_api.data_type_functions import result_type
 from cubed.array_api.dtypes import (
@@ -10,14 +11,20 @@
     _floating_dtypes,
     _integer_or_boolean_dtypes,
     _numeric_dtypes,
 )
 from cubed.array_api.linear_algebra_functions import matmul
 from cubed.core.array import CoreArray
 from cubed.core.ops import elemwise
+from cubed.utils import memory_repr
+from cubed.vendor.dask.widgets import get_template
+
+ARRAY_SVG_SIZE = (
+    120  # cubed doesn't have a config module like dask does so hard-code this for now
+)
 
 
 class Array(CoreArray):
     def __init__(self, name, zarray, spec, plan):
         super().__init__(name, zarray, spec, plan)
 
     def __array__(self, dtype=None) -> np.ndarray:
@@ -27,14 +34,63 @@
         if not isinstance(x, np.ndarray):
             x = np.array(x)
         return x
 
     def __repr__(self):
         return f"cubed.Array<{self.name}, shape={self.shape}, dtype={self.dtype}, chunks={self.chunks}>"
 
+    def _repr_html_(self):
+        try:
+            grid = self.to_svg(size=ARRAY_SVG_SIZE)
+        except NotImplementedError:
+            grid = ""
+
+        if not math.isnan(self.nbytes):
+            nbytes = memory_repr(self.nbytes)
+            cbytes = memory_repr(math.prod(self.chunksize) * self.dtype.itemsize)
+        else:
+            nbytes = "unknown"
+            cbytes = "unknown"
+
+        return get_template("array.html.j2").render(
+            array=self,
+            grid=grid,
+            nbytes=nbytes,
+            cbytes=cbytes,
+            arrs_in_plan=f"{self.plan.num_arrays()} arrays in Plan",
+            arrtype="np.ndarray",
+        )
+
+    def to_svg(self, size=500):
+        """Convert chunks from Cubed Array into an SVG Image
+
+        Parameters
+        ----------
+        chunks: tuple
+        size: int
+            Rough size of the image
+
+        Examples
+        --------
+        >>> x.to_svg(size=500)  # doctest: +SKIP
+
+        Returns
+        -------
+        text: An svg string depicting the array as a grid of chunks
+        """
+        from cubed.vendor.dask.array.svg import svg
+
+        return svg(self.chunks, size=size)
+
+    def _repr_inline_(self, max_width):
+        """
+        Format to a single line with at most max_width characters. Used by xarray.
+        """
+        return f"cubed.Array<chunksize={self.chunksize}>"
+
     # Attributes
 
     @property
     def device(self):
         return "cpu"
 
     @property
```

### Comparing `cubed-0.8.0/cubed/array_api/creation_functions.py` & `cubed-0.9.0/cubed/array_api/creation_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 from zarr.util import normalize_shape
 
 from cubed.core import Plan, gensym, map_blocks
 from cubed.core.ops import map_direct
 from cubed.core.plan import new_temp_path
+from cubed.storage.virtual import virtual_offsets
 from cubed.storage.zarr import lazy_from_array, lazy_full
 from cubed.utils import to_chunksize
 from cubed.vendor.dask.array.core import normalize_chunks
 
 if TYPE_CHECKING:
     from .array_object import Array
 
@@ -149,14 +150,24 @@
 
     from .array_object import Array
 
     plan = Plan._new(name, "full", target)
     return Array(name, target, spec, plan)
 
 
+def offsets_array(shape, spec=None) -> "Array":
+    name = gensym()
+    target = virtual_offsets(shape)
+
+    from .array_object import Array
+
+    plan = Plan._new(name, "block_ids", target)
+    return Array(name, target, spec, plan)
+
+
 def full_like(
     x, /, fill_value, *, dtype=None, device=None, chunks=None, spec=None
 ) -> "Array":
     return full(fill_value=fill_value, **_like_args(x, dtype, device, chunks, spec))
 
 
 def linspace(
```

### Comparing `cubed-0.8.0/cubed/array_api/data_type_functions.py` & `cubed-0.9.0/cubed/array_api/data_type_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/array_api/elementwise_functions.py` & `cubed-0.9.0/cubed/array_api/elementwise_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/array_api/linear_algebra_functions.py` & `cubed-0.9.0/cubed/array_api/linear_algebra_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 
 
 def outer(x1, x2, /):
     return blockwise(np.outer, "ij", x1, "i", x2, "j", dtype=x1.dtype)
 
 
 def tensordot(x1, x2, /, *, axes=2):
-
     from cubed.array_api.statistical_functions import sum
 
     if x1.dtype not in _numeric_dtypes or x2.dtype not in _numeric_dtypes:
         raise TypeError("Only numeric dtypes are allowed in tensordot")
 
     # based on dask
```

### Comparing `cubed-0.8.0/cubed/array_api/manipulation_functions.py` & `cubed-0.9.0/cubed/array_api/manipulation_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/array_api/searching_functions.py` & `cubed-0.9.0/cubed/array_api/searching_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/array_api/statistical_functions.py` & `cubed-0.9.0/cubed/array_api/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/core/array.py` & `cubed-0.9.0/cubed/core/array.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,24 @@
         return self._shape
 
     @property
     def size(self):
         """Number of elements in the array."""
         return reduce(mul, self.shape, 1)
 
+    @property
+    def nbytes(self) -> int:
+        """Number of bytes in array"""
+        return self.size * self.dtype.itemsize
+
+    @property
+    def itemsize(self) -> int:
+        """Length of one array element in bytes"""
+        return self.dtype.itemsize
+
     def _read_stored(self):
         # Only works if the array has been computed
         if self.size > 0:
             # read back from zarr
             return self.zarray[...]
         else:
             # this case fails for zarr, so just return an empty array of the correct shape
@@ -240,25 +250,25 @@
                 "`max_mem` is deprecated, please use `allowed_mem` instead",
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         self._work_dir = work_dir
 
-        self._reserved_mem = convert_to_bytes(reserved_mem)
+        self._reserved_mem = convert_to_bytes(reserved_mem or 0)
         if allowed_mem is None:
             self._allowed_mem = (max_mem or 0) + self.reserved_mem
         else:
             self._allowed_mem = convert_to_bytes(allowed_mem)
 
         self._executor = executor
         self._storage_options = storage_options
 
     @property
-    def work_dir(self) -> str:
+    def work_dir(self) -> Optional[str]:
         """The directory path (specified as an fsspec URL) used for storing intermediate data."""
         return self._work_dir
 
     @property
     def allowed_mem(self) -> int:
         """
         The total memory available to a worker for running a task, in bytes.
@@ -275,20 +285,20 @@
         See Also
         --------
         cubed.measure_reserved_mem
         """
         return self._reserved_mem
 
     @property
-    def executor(self) -> Executor:
+    def executor(self) -> Optional[Executor]:
         """The default executor for running computations."""
         return self._executor
 
     @property
-    def storage_options(self) -> dict:
+    def storage_options(self) -> Optional[dict]:
         """Storage options to be passed to fsspec."""
         return self._storage_options
 
     def __repr__(self) -> str:
         return (
             f"cubed.Spec(work_dir={self._work_dir}, allowed_mem={self._allowed_mem}, "
             f"reserved_mem={self._reserved_mem}, executor={self._executor}, storage_options={self._storage_options})"
```

### Comparing `cubed-0.8.0/cubed/core/gufunc.py` & `cubed-0.9.0/cubed/core/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/core/ops.py` & `cubed-0.9.0/cubed/core/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,28 +419,24 @@
 
 
 def map_blocks(
     func, *args: "Array", dtype=None, chunks=None, drop_axis=[], new_axis=None, **kwargs
 ) -> "Array":
     """Apply a function to corresponding blocks from multiple input arrays."""
     if has_keyword(func, "block_id"):
-        from cubed.array_api import asarray
+        from cubed.array_api.creation_functions import offsets_array
 
         # Create an array of index offsets with the same chunk structure as the args,
         # which we convert to block ids (chunk coordinates) later.
         a = args[0]
-        _offsets = np.arange(a.npartitions, dtype=np.int32).reshape(a.numblocks)
-        offsets = asarray(_offsets, spec=a.spec)
-        # rechunk in a separate operation to avoid potentially writing lots of zarr chunks from the client
-        offsets_chunks = (1,) * len(a.numblocks)
-        offsets = rechunk(offsets, offsets_chunks)
+        offsets = offsets_array(a.numblocks, a.spec)
         new_args = args + (offsets,)
 
         def offset_to_block_id(offset):
-            return list(np.ndindex(*(a.numblocks)))[offset]
+            return np.unravel_index(offset, a.numblocks)
 
         def func_with_block_id(func):
             def wrap(*a, **kw):
                 block_id = offset_to_block_id(a[-1].item())
                 return func(*a[:-1], block_id=block_id, **kw)
 
             return wrap
@@ -586,24 +582,27 @@
         extra_source_arrays=args,
         extra_projected_mem=extra_projected_mem,
         **kwargs,
     )
 
 
 def rechunk(x, chunks, target_store=None):
-    if x.chunks == normalize_chunks(chunks, x.shape, dtype=x.dtype):
+    normalized_chunks = normalize_chunks(chunks, x.shape, dtype=x.dtype)
+    if x.chunks == normalized_chunks:
         return x
+    # normalizing takes care of dict args for chunks
+    target_chunks = to_chunksize(normalized_chunks)
     name = gensym()
     spec = x.spec
     if target_store is None:
         target_store = new_temp_path(name=name, spec=spec)
     temp_store = new_temp_path(name=f"{name}-intermediate", spec=spec)
     pipeline = primitive_rechunk(
         x.zarray_maybe_lazy,
-        target_chunks=chunks,
+        target_chunks=target_chunks,
         allowed_mem=spec.allowed_mem,
         reserved_mem=spec.reserved_mem,
         target_store=target_store,
         temp_store=temp_store,
     )
     plan = Plan._new(
         name,
```

### Comparing `cubed-0.8.0/cubed/core/plan.py` & `cubed-0.9.0/cubed/core/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,32 +133,37 @@
 
         return Plan(dag)
 
     def create_lazy_zarr_arrays(self, dag):
         # find all lazy zarr arrays in dag
         all_array_nodes = []
         lazy_zarr_arrays = []
+        reserved_mem_values = []
         for n, d in dag.nodes(data=True):
+            if "reserved_mem" in d and d["reserved_mem"] is not None:
+                reserved_mem_values.append(d["reserved_mem"])
             if isinstance(d["target"], LazyZarrArray):
                 all_array_nodes.append(n)
                 lazy_zarr_arrays.append(d["target"])
 
+        reserved_mem = max(reserved_mem_values, default=0)
+
         if len(lazy_zarr_arrays) > 0:
             # add new node and edges
             name = "create-arrays"
             op_name = name
-            pipeline = create_zarr_arrays(lazy_zarr_arrays)
+            pipeline = create_zarr_arrays(lazy_zarr_arrays, reserved_mem)
             dag.add_node(
                 name,
                 name=name,
                 op_name=op_name,
                 target=None,
                 pipeline=pipeline,
                 projected_mem=pipeline.projected_mem,
-                reserved_mem=0,  # TODO: get from Spec
+                reserved_mem=reserved_mem,
                 num_tasks=pipeline.num_tasks,
             )
             # make create arrays node a dependency of all lazy array nodes
             for n in all_array_nodes:
                 dag.add_edge(name, n)
 
         return dag
@@ -212,21 +217,22 @@
     def num_tasks(self, optimize_graph=True, resume=None):
         """Return the number of tasks needed to execute this plan."""
         dag = self.optimize().dag if optimize_graph else self.dag.copy()
         dag = self.create_lazy_zarr_arrays(dag)
         tasks = 0
         for _, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
-            for stage in pipeline.stages:
-                if stage.mappable is not None:
-                    tasks += len(list(stage.mappable))
-                else:
-                    tasks += 1
+            tasks += pipeline.num_tasks
         return tasks
 
+    def num_arrays(self, optimize_graph: bool = True) -> int:
+        """Return the number of arrays in this plan."""
+        dag = self.optimize().dag if optimize_graph else self.dag
+        return dag.number_of_nodes()
+
     def max_projected_mem(self, optimize_graph=True, resume=None):
         """Return the maximum projected memory across all tasks to execute this plan."""
         dag = self.optimize().dag if optimize_graph else self.dag.copy()
         dag = self.create_lazy_zarr_arrays(dag)
         projected_mem_values = [
             node["pipeline"].projected_mem
             for _, node in visit_nodes(dag, resume=resume)
@@ -257,15 +263,15 @@
             "labeljust": "left",
             "fontsize": "10",
         }
         dag.graph["node"] = {"fontname": "helvetica", "shape": "box", "fontsize": "10"}
 
         # do an initial pass to extract array variable names from stack summaries
         array_display_names = {}
-        for (n, d) in dag.nodes(data=True):
+        for n, d in dag.nodes(data=True):
             if "stack_summaries" in d:
                 stack_summaries = d["stack_summaries"]
                 first_cubed_i = min(
                     i for i, s in enumerate(stack_summaries) if s.is_cubed()
                 )
                 caller_summary = stack_summaries[first_cubed_i - 1]
                 array_display_names.update(caller_summary.array_names_to_variable_names)
@@ -273,15 +279,15 @@
         frame = inspect.currentframe().f_back  # go back one in the stack
         stack_summaries = extract_stack_summaries(frame, limit=10)
         first_cubed_i = min(i for i, s in enumerate(stack_summaries) if s.is_cubed())
         caller_summary = stack_summaries[first_cubed_i - 1]
         array_display_names.update(caller_summary.array_names_to_variable_names)
 
         # now set node attributes with visualization info
-        for (n, d) in dag.nodes(data=True):
+        for n, d in dag.nodes(data=True):
             if d["op_name"] == "blockwise":
                 d["style"] = "filled"
                 d["fillcolor"] = "#dcbeff"
                 op_name_summary = "(bw)"
             elif d["op_name"] == "rechunk":
                 d["style"] = "filled"
                 d["fillcolor"] = "#aaffc3"
@@ -404,27 +410,32 @@
 
 
 def create_zarr_array(lazy_zarr_array, *, config=None):
     """Stage function for create."""
     lazy_zarr_array.create(mode="a")
 
 
-def create_zarr_arrays(lazy_zarr_arrays):
+def create_zarr_arrays(lazy_zarr_arrays, reserved_mem):
     stages = [
         Stage(
             create_zarr_array,
             "create_zarr_array",
             mappable=lazy_zarr_arrays,
         )
     ]
 
-    # projected memory is size of largest initial values, or 0 if there aren't any
-    projected_mem = max(
-        [
-            lza.initial_values.nbytes if lza.initial_values is not None else 0
-            for lza in lazy_zarr_arrays
-        ],
-        default=0,
+    # projected memory is size of largest initial values, or dtype size if there aren't any
+    projected_mem = (
+        max(
+            [
+                lza.initial_values.nbytes
+                if lza.initial_values is not None
+                else lza.dtype.itemsize
+                for lza in lazy_zarr_arrays
+            ],
+            default=0,
+        )
+        + reserved_mem
     )
     num_tasks = len(lazy_zarr_arrays)
 
     return CubedPipeline(stages, None, None, None, projected_mem, num_tasks)
```

### Comparing `cubed-0.8.0/cubed/extensions/history.py` & `cubed-0.9.0/cubed/extensions/history.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/extensions/timeline.py` & `cubed-0.9.0/cubed/extensions/timeline.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/extensions/tqdm.py` & `cubed-0.9.0/cubed/extensions/tqdm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/primitive/blockwise.py` & `cubed-0.9.0/cubed/primitive/blockwise.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import itertools
+import math
 from dataclasses import dataclass
 from functools import partial
-from typing import Callable, Dict
+from typing import Any, Callable, Dict, Iterator, List, Optional, Sequence, Tuple, Union
 
 import toolz
 import zarr
 from toolz import map
 
-from cubed.storage.zarr import lazy_empty
+from cubed.storage.zarr import T_ZarrArray, lazy_empty
+from cubed.types import T_Chunks, T_DType, T_Shape, T_Store
 from cubed.utils import chunk_memory, get_item, to_chunksize
 from cubed.vendor.dask.array.core import normalize_chunks
 from cubed.vendor.dask.blockwise import _get_coord_mapping, _make_dims, lol_product
 from cubed.vendor.dask.core import flatten
 from cubed.vendor.rechunker.types import Stage
 
 from .types import CubedArrayProxy, CubedPipeline
 
 sym_counter = 0
 
 
-def gensym(name):
+def gensym(name: str) -> str:
     global sym_counter
     sym_counter += 1
     return f"{name}-{sym_counter:03}"
 
 
 @dataclass(frozen=True)
 class BlockwiseSpec:
@@ -39,27 +41,29 @@
         A function that maps input chunks to an output chunk.
     reads_map : Dict[str, CubedArrayProxy]
         Read proxy dictionary keyed by array name.
     write : CubedArrayProxy
         Write proxy with an ``array`` attribute that supports ``__setitem__``.
     """
 
-    block_function: Callable
-    function: Callable
+    block_function: Callable[..., Any]
+    function: Callable[..., Any]
     reads_map: Dict[str, CubedArrayProxy]
     write: CubedArrayProxy
 
 
-def apply_blockwise(out_key, *, config=BlockwiseSpec):
+def apply_blockwise(out_key: List[int], *, config: BlockwiseSpec) -> None:
     """Stage function for blockwise."""
     # lithops needs params to be lists not tuples, so convert back
-    out_key = tuple(out_key)
-    out_chunk_key = key_to_slices(out_key, config.write.array, config.write.chunks)
+    out_key_tuple = tuple(out_key)
+    out_chunk_key = key_to_slices(
+        out_key_tuple, config.write.array, config.write.chunks
+    )
     args = []
-    name_chunk_inds = config.block_function(("out",) + out_key)
+    name_chunk_inds = config.block_function(("out",) + out_key_tuple)
     for name_chunk_ind in name_chunk_inds:
         name = name_chunk_ind[0]
         chunk_ind = name_chunk_ind[1:]
         arr = config.reads_map[name].open()
         chunk_key = key_to_slices(chunk_ind, arr)
         arg = arr[chunk_key]
         args.append(arg)
@@ -68,33 +72,35 @@
     if isinstance(result, dict):  # structured array with named fields
         for k, v in result.items():
             config.write.open().set_basic_selection(out_chunk_key, v, fields=k)
     else:
         config.write.open()[out_chunk_key] = result
 
 
-def key_to_slices(key, arr, chunks=None):
+def key_to_slices(
+    key: Tuple[int, ...], arr: T_ZarrArray, chunks: Optional[T_Chunks] = None
+) -> Tuple[slice, ...]:
     """Convert a chunk index key to a tuple of slices"""
     chunks = normalize_chunks(chunks or arr.chunks, shape=arr.shape, dtype=arr.dtype)
     return get_item(chunks, key)
 
 
 def blockwise(
-    func,
-    out_ind,
-    *args,
-    allowed_mem,
-    reserved_mem,
-    target_store,
-    shape,
-    dtype,
-    chunks,
-    new_axes=None,
-    in_names=None,
-    out_name=None,
+    func: Callable[..., Any],
+    out_ind: Sequence[Union[str, int]],
+    *args: Any,
+    allowed_mem: int,
+    reserved_mem: int,
+    target_store: T_Store,
+    shape: T_Shape,
+    dtype: T_DType,
+    chunks: T_Chunks,
+    new_axes: Optional[Dict[int, int]] = None,
+    in_names: Optional[List[str]] = None,
+    out_name: Optional[str] = None,
     **kwargs,
 ):
     """Apply a function across blocks from multiple source Zarr arrays.
 
     Parameters
     ----------
     func : callable
@@ -122,28 +128,28 @@
 
     Returns
     -------
     CubedPipeline to run the operation
     """
 
     # Use dask's make_blockwise_graph
-    arrays = args[::2]
+    arrays: Sequence[T_ZarrArray] = args[::2]
     array_names = in_names or [f"in_{i}" for i in range(len(arrays))]
     array_map = {name: array for name, array in zip(array_names, arrays)}
 
-    inds = args[1::2]
+    inds: Sequence[Union[str, int]] = args[1::2]
 
-    numblocks = {}
+    numblocks: Dict[str, Tuple[int, ...]] = {}
     for name, array in zip(array_names, arrays):
         input_chunks = normalize_chunks(
             array.chunks, shape=array.shape, dtype=array.dtype
         )
         numblocks[name] = tuple(map(len, input_chunks))
 
-    argindsstr = []
+    argindsstr: List[Any] = []
     for name, ind in zip(array_names, inds):
         argindsstr.extend((name, ind))
 
     # TODO: check output shape and chunks are consistent with inputs
     chunks = normalize_chunks(chunks, shape=shape, dtype=dtype)
 
     # block func
@@ -153,15 +159,26 @@
         out_name or "out",
         out_ind,
         *argindsstr,
         numblocks=numblocks,
         new_axes=new_axes,
     )
 
-    output_blocks = get_output_blocks(
+    output_blocks_generator_fn = partial(
+        get_output_blocks,
+        func,
+        out_name or "out",
+        out_ind,
+        *argindsstr,
+        numblocks=numblocks,
+        new_axes=new_axes,
+    )
+    output_blocks = IterableFromGenerator(output_blocks_generator_fn)
+
+    num_tasks = num_output_blocks(
         func,
         out_name or "out",
         out_ind,
         *argindsstr,
         numblocks=numblocks,
         new_axes=new_axes,
     )
@@ -207,37 +224,35 @@
     projected_mem += chunk_memory(dtype, chunksize) * 2
 
     if projected_mem > allowed_mem:
         raise ValueError(
             f"Projected blockwise memory ({projected_mem}) exceeds allowed_mem ({allowed_mem}), including reserved_mem ({reserved_mem})"
         )
 
-    num_tasks = len(output_blocks)
-
     return CubedPipeline(stages, spec, target_array, None, projected_mem, num_tasks)
 
 
 # Code for fusing pipelines
 
 
-def is_fuse_candidate(pipeline):
+def is_fuse_candidate(pipeline: CubedPipeline) -> bool:
     """
     Return True if a pipeline is a candidate for blockwise fusion.
     """
     stages = pipeline.stages
     return len(stages) == 1 and stages[0].function == apply_blockwise
 
 
-def can_fuse_pipelines(pipeline1, pipeline2):
+def can_fuse_pipelines(pipeline1: CubedPipeline, pipeline2: CubedPipeline) -> bool:
     if is_fuse_candidate(pipeline1) and is_fuse_candidate(pipeline2):
         return pipeline1.num_tasks == pipeline2.num_tasks
     return False
 
 
-def fuse(pipeline1, pipeline2):
+def fuse(pipeline1: CubedPipeline, pipeline2: CubedPipeline) -> CubedPipeline:
     """
     Fuse two blockwise pipelines into a single pipeline, avoiding writing to (or reading from) the target of the first pipeline.
     """
 
     assert pipeline1.num_tasks == pipeline2.num_tasks
 
     mappable = pipeline2.stages[0].mappable
@@ -269,16 +284,21 @@
     return CubedPipeline(stages, spec, target_array, None, projected_mem, num_tasks)
 
 
 # blockwise functions
 
 
 def make_blockwise_function(
-    func, output, out_indices, *arrind_pairs, numblocks=None, new_axes=None
-):
+    func: Callable[..., Any],
+    output: str,
+    out_indices: Sequence[Union[str, int]],
+    *arrind_pairs: Any,
+    numblocks: Optional[Dict[str, Tuple[int, ...]]] = None,
+    new_axes: Optional[Dict[int, int]] = None,
+) -> Callable[[List[int]], Any]:
     """Make a function that is the equivalent of make_blockwise_graph."""
 
     if numblocks is None:
         raise ValueError("Missing required numblocks argument.")
     new_axes = new_axes or {}
     argpairs = list(toolz.partition(2, arrind_pairs))
 
@@ -322,16 +342,21 @@
 
         return val
 
     return blockwise_fn
 
 
 def make_blockwise_function_flattened(
-    func, output, out_indices, *arrind_pairs, numblocks=None, new_axes=None
-):
+    func: Callable[..., Any],
+    output: str,
+    out_indices: Sequence[Union[str, int]],
+    *arrind_pairs: Any,
+    numblocks: Optional[Dict[str, Tuple[int, ...]]] = None,
+    new_axes: Optional[Dict[int, int]] = None,
+) -> Callable[[List[int]], Any]:
     # TODO: make this a part of make_blockwise_function?
     blockwise_fn = make_blockwise_function(
         func, output, out_indices, *arrind_pairs, numblocks=numblocks, new_axes=new_axes
     )
 
     def blockwise_fn_flattened(out_key):
         name_chunk_inds = blockwise_fn(out_key)[1:]  # drop function in position 0
@@ -340,23 +365,51 @@
             name_chunk_inds = list(flatten(name_chunk_inds))
         return name_chunk_inds
 
     return blockwise_fn_flattened
 
 
 def get_output_blocks(
-    func, output, out_indices, *arrind_pairs, numblocks=None, new_axes=None
-):
-
+    func: Callable[..., Any],
+    output: str,
+    out_indices: Sequence[Union[str, int]],
+    *arrind_pairs: Any,
+    numblocks: Optional[Dict[str, Tuple[int, ...]]] = None,
+    new_axes: Optional[Dict[int, int]] = None,
+) -> Iterator[List[int]]:
     if numblocks is None:
         raise ValueError("Missing required numblocks argument.")
     new_axes = new_axes or {}
     argpairs = list(toolz.partition(2, arrind_pairs))
 
     # Dictionary mapping {i: 3, j: 4, ...} for i, j, ... the dimensions
     dims = _make_dims(argpairs, numblocks, new_axes)
 
     # return a list of lists, not of tuples, otherwise lithops breaks
-    output_blocks_lists = [
-        list(tup) for tup in itertools.product(*[range(dims[i]) for i in out_indices])
-    ]
-    return output_blocks_lists
+    for tup in itertools.product(*[range(dims[i]) for i in out_indices]):
+        yield list(tup)
+
+
+class IterableFromGenerator:
+    def __init__(self, generator_fn: Callable[[], Iterator[List[int]]]):
+        self.generator_fn = generator_fn
+
+    def __iter__(self):
+        return self.generator_fn()
+
+
+def num_output_blocks(
+    func: Callable[..., Any],
+    output: str,
+    out_indices: Sequence[Union[str, int]],
+    *arrind_pairs: Any,
+    numblocks: Optional[Dict[str, Tuple[int, ...]]] = None,
+    new_axes: Optional[Dict[int, int]] = None,
+) -> int:
+    if numblocks is None:
+        raise ValueError("Missing required numblocks argument.")
+    new_axes = new_axes or {}
+    argpairs = list(toolz.partition(2, arrind_pairs))
+
+    # Dictionary mapping {i: 3, j: 4, ...} for i, j, ... the dimensions
+    dims = _make_dims(argpairs, numblocks, new_axes)
+    return math.prod(dims[i] for i in out_indices)
```

### Comparing `cubed-0.8.0/cubed/primitive/rechunk.py` & `cubed-0.9.0/cubed/primitive/rechunk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from math import ceil, prod
+from typing import Any, Dict, List, Optional, Tuple
 
-import zarr
-
-import cubed
-from cubed.primitive.types import CubedArrayProxy
+from cubed.primitive.types import CubedArrayProxy, CubedCopySpec, CubedPipeline
 from cubed.runtime.pipeline import spec_to_pipeline
-from cubed.storage.zarr import lazy_empty
+from cubed.storage.zarr import T_ZarrArray, lazy_empty
+from cubed.types import T_RegularChunks, T_Shape, T_Store
 from cubed.vendor.rechunker.algorithm import rechunking_plan
-from cubed.vendor.rechunker.api import (
-    _get_dims_from_zarr_array,
-    _shape_dict_to_tuple,
-    _validate_options,
-)
-from cubed.vendor.rechunker.types import CopySpec
+from cubed.vendor.rechunker.api import _validate_options
 
 
 def rechunk(
-    source, target_chunks, allowed_mem, reserved_mem, target_store, temp_store=None
-):
+    source: T_ZarrArray,
+    target_chunks: T_RegularChunks,
+    allowed_mem: int,
+    reserved_mem: int,
+    target_store: T_Store,
+    temp_store: Optional[T_Store] = None,
+) -> CubedPipeline:
     """Rechunk a Zarr array to have target_chunks.
 
     Parameters
     ----------
     source : Zarr array
     target_chunks : tuple
         The desired chunks of the array after rechunking.
@@ -37,15 +36,15 @@
     Returns
     -------
     CubedPipeline to run the operation
     """
 
     # rechunker doesn't take account of uncompressed and compressed copies of the
     # input and output array chunk/selection, so adjust appropriately
-    rechunker_max_mem = (allowed_mem - reserved_mem) / 4
+    rechunker_max_mem = (allowed_mem - reserved_mem) // 4
 
     copy_specs, intermediate, target = _setup_rechunk(
         source=source,
         target_chunks=target_chunks,
         max_mem=rechunker_max_mem,
         target_store=target_store,
         temp_store=temp_store,
@@ -63,22 +62,22 @@
     # we assume that rechunker is going to use all the memory it is allowed to
     projected_mem = allowed_mem
     return spec_to_pipeline(copy_spec, target, projected_mem, num_tasks)
 
 
 # from rechunker, but simpler since it only has to handle Zarr arrays
 def _setup_rechunk(
-    source,
-    target_chunks,
-    max_mem,
-    target_store,
-    target_options=None,
-    temp_store=None,
-    temp_options=None,
-):
+    source: T_ZarrArray,
+    target_chunks: T_RegularChunks,
+    max_mem: int,
+    target_store: T_Store,
+    target_options: Optional[Dict[Any, Any]] = None,
+    temp_store: Optional[T_Store] = None,
+    temp_options: Optional[Dict[Any, Any]] = None,
+) -> Tuple[List[CubedCopySpec], T_ZarrArray, T_ZarrArray]:
     if temp_options is None:
         temp_options = target_options
     target_options = target_options or {}
     temp_options = temp_options or {}
 
     copy_spec = _setup_array_rechunk(
         source,
@@ -91,23 +90,23 @@
     )
     intermediate = copy_spec.intermediate.array
     target = copy_spec.write.array
     return [copy_spec], intermediate, target
 
 
 def _setup_array_rechunk(
-    source_array,
-    target_chunks,
-    max_mem,
-    target_store_or_group,
-    target_options=None,
-    temp_store_or_group=None,
-    temp_options=None,
-    name=None,
-) -> CopySpec:
+    source_array: T_ZarrArray,
+    target_chunks: T_RegularChunks,
+    max_mem: int,
+    target_store_or_group: T_Store,
+    target_options: Optional[Dict[Any, Any]] = None,
+    temp_store_or_group: Optional[T_Store] = None,
+    temp_options: Optional[Dict[Any, Any]] = None,
+    name: Optional[str] = None,
+) -> CubedCopySpec:
     _validate_options(target_options)
     _validate_options(temp_options)
     shape = source_array.shape
     # source_chunks = (
     #     source_array.chunksize
     #     if isinstance(source_array, dask.array.Array)
     #     else source_array.chunks
@@ -116,36 +115,20 @@
     dtype = source_array.dtype
     itemsize = dtype.itemsize
 
     if target_chunks is None:
         # this is just a pass-through copy
         target_chunks = source_chunks
 
-    if isinstance(target_chunks, dict):
-        array_dims = _get_dims_from_zarr_array(source_array)
-        try:
-            target_chunks = _shape_dict_to_tuple(array_dims, target_chunks)
-        except KeyError:
-            raise KeyError(
-                "You must explicitly specify each dimension size in target_chunks. "
-                f"Got array_dims {array_dims}, target_chunks {target_chunks}."
-            )
-
-    # TODO: rewrite to avoid the hard dependency on dask
-    max_mem = cubed.vendor.dask.utils.parse_bytes(max_mem)
-
-    # don't consolidate reads for Dask arrays
-    consolidate_reads = isinstance(source_array, zarr.core.Array)
     read_chunks, int_chunks, write_chunks = rechunking_plan(
         shape,
         source_chunks,
         target_chunks,
         itemsize,
         max_mem,
-        consolidate_reads=consolidate_reads,
     )
 
     # create target
     shape = tuple(int(x) for x in shape)  # ensure python ints for serialization
     target_chunks = tuple(int(x) for x in target_chunks)
     int_chunks = tuple(int(x) for x in int_chunks)
     write_chunks = tuple(int(x) for x in write_chunks)
@@ -154,19 +137,14 @@
         shape,
         dtype=dtype,
         chunks=target_chunks,
         store=target_store_or_group,
         **(target_options or {}),
     )
 
-    try:
-        target_array.attrs.update(source_array.attrs)
-    except AttributeError:
-        pass
-
     if read_chunks == write_chunks:
         int_array = None
     else:
         # do intermediate store
         if temp_store_or_group is None:
             raise ValueError(
                 "A temporary store location must be provided{}.".format(
@@ -180,13 +158,13 @@
             store=temp_store_or_group,
             **(target_options or {}),
         )
 
     read_proxy = CubedArrayProxy(source_array, read_chunks)
     int_proxy = CubedArrayProxy(int_array, int_chunks)
     write_proxy = CubedArrayProxy(target_array, write_chunks)
-    return CopySpec(read_proxy, int_proxy, write_proxy)
+    return CubedCopySpec(read_proxy, int_proxy, write_proxy)
 
 
-def total_chunks(shape, chunks):
+def total_chunks(shape: T_Shape, chunks: T_RegularChunks) -> int:
     # cf rechunker's chunk_keys
     return prod(ceil(s / c) for s, c in zip(shape, chunks))
```

### Comparing `cubed-0.8.0/cubed/primitive/types.py` & `cubed-0.9.0/cubed/primitive/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 from dataclasses import dataclass
-from typing import Any, Iterable, Optional
+from typing import Any, Optional, Sequence
 
-from cubed.storage.zarr import open_if_lazy_zarr_array
+import zarr
+
+from cubed.storage.zarr import T_ZarrArray, open_if_lazy_zarr_array
+from cubed.types import T_RegularChunks
 from cubed.vendor.rechunker.types import Config, Stage
 
 
 @dataclass(frozen=True)
 class CubedPipeline:
     """Generalisation of rechunker ``Pipeline`` with extra attributes."""
 
-    stages: Iterable[Stage]
+    stages: Sequence[Stage]
     config: Config
     target_array: Any
     intermediate_array: Optional[Any]
     projected_mem: int
     num_tasks: int
 
 
 class CubedArrayProxy:
     """Generalisation of rechunker ``ArrayProxy`` with support for ``LazyZarrArray``."""
 
-    def __init__(self, array, chunks):
+    def __init__(self, array: T_ZarrArray, chunks: T_RegularChunks):
         self.array = array
         self.chunks = chunks
 
-    def open(self):
+    def open(self) -> zarr.Array:
         return open_if_lazy_zarr_array(self.array)
+
+
+@dataclass(frozen=True)
+class CubedCopySpec:
+    """Generalisation of rechunker ``CopySpec`` with support for ``LazyZarrArray``."""
+
+    read: CubedArrayProxy
+    intermediate: CubedArrayProxy
+    write: CubedArrayProxy
```

### Comparing `cubed-0.8.0/cubed/random.py` & `cubed-0.9.0/cubed/random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/runtime/backup.py` & `cubed-0.9.0/cubed/runtime/backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/runtime/executors/beam.py` & `cubed-0.9.0/cubed/runtime/executors/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
             | beam.combiners.ToList()
             | "Validate" >> beam.Map(self.post_validate)
         )
 
 
 class BeamPipelineExecutor(PipelineExecutor[List[beam.PTransform]]):
     def pipelines_to_plan(self, pipelines: ParallelPipelines) -> List[beam.PTransform]:
-
         start = "Start" >> beam.Create([-1])
 
         pcolls = []
 
         for pipeline in pipelines:
             pcoll = start
             for step, stage in enumerate(pipeline.stages):
```

### Comparing `cubed-0.8.0/cubed/runtime/executors/lithops.py` & `cubed-0.9.0/cubed/runtime/executors/lithops.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import time
 from functools import partial
 from typing import Callable, Iterable
 
 from lithops.executors import FunctionExecutor
 from lithops.wait import ALWAYS, ANY_COMPLETED
-from six import reraise
 
 from cubed.core.plan import visit_nodes
 from cubed.runtime.backup import should_launch_backup
+from cubed.runtime.executors.lithops_retries import map_with_retries, wait_with_retries
 from cubed.runtime.types import DagExecutor
 from cubed.runtime.utils import handle_callbacks
 from cubed.vendor.rechunker.types import ParallelPipelines, PipelineExecutor
 
 logger = logging.getLogger(__name__)
 
 # Lithops represents delayed execution tasks as functions that require
@@ -91,99 +91,78 @@
     backups = {}
     pending = []
 
     # can't use functools.partial here as we get an error in lithops
     # also, lithops extra_args doesn't work for this case
     partial_map_function = lambda x: map_function(x, **kwargs)
 
-    futures = lithops_function_executor.map(
-        partial_map_function, inputs, timeout=timeout, include_modules=include_modules
+    futures = map_with_retries(
+        lithops_function_executor,
+        partial_map_function,
+        inputs,
+        timeout=timeout,
+        include_modules=include_modules,
+        retries=retries,
     )
     tasks.update({k: v for (k, v) in zip(futures, inputs)})
     start_times.update({k: time.monotonic() for k in futures})
     pending.extend(futures)
 
-    future_to_index = {f: i for i, f in enumerate(futures)}
-    failure_counts = [0] * len(inputs)
-
     while pending:
-        finished, pending = lithops_function_executor.wait(
-            pending, throw_except=False, return_when=return_when, show_progressbar=False
+        finished, pending = wait_with_retries(
+            lithops_function_executor,
+            pending,
+            throw_except=False,
+            return_when=return_when,
+            show_progressbar=False,
         )
-        failed = []
         for future in finished:
             if future.error:
-                index = future_to_index[future]
-                failure_counts[index] = failure_counts[index] + 1
-                failure_count = failure_counts[index]
-
-                if failure_count > retries:
-                    # re-raise exception
-                    # TODO: why does calling status not raise the exception?
-                    future.status(throw_except=True)
-                    reraise(*future._exception)
-                failed.append(future)
+                # if the task has a backup that is not done, or is done with no exception, then don't raise this exception
+                backup = backups.get(future, None)
+                if backup:
+                    if not backup.done or not backup.error:
+                        continue
+                future.status(throw_except=True)
+            end_times[future] = time.monotonic()
+            if return_stats:
+                yield future.result(), standardise_lithops_stats(future.stats)
             else:
-                end_times[future] = time.monotonic()
-                if return_stats:
-                    yield future.result(), standardise_lithops_stats(future.stats)
-                else:
-                    yield future.result()
+                yield future.result()
 
             # remove any backup task
             if use_backups:
                 backup = backups.get(future, None)
                 if backup:
                     if backup in pending:
                         pending.remove(backup)
                     del backups[future]
                     del backups[backup]
-
-        if failed:
-            # rerun and add to pending
-            inputs_to_rerun = []
-            input_indexes_to_rerun = []
-            for fut in failed:
-                index = future_to_index[fut]
-                inputs_to_rerun.append(inputs[index])
-                input_indexes_to_rerun.append(index)
-                del future_to_index[fut]
-            # TODO: de-duplicate code from above
-            futures = lithops_function_executor.map(
-                partial_map_function,
-                inputs_to_rerun,
-                timeout=timeout,
-                include_modules=include_modules,
-            )
-            tasks.update({k: v for (k, v) in zip(futures, inputs_to_rerun)})
-            start_times.update({k: time.monotonic() for k in futures})
-            pending.extend(futures)
-
-            future_to_index.update(
-                {f: i for i, f in zip(input_indexes_to_rerun, futures)}
-            )
+                    backup.cancel()
 
         if use_backups:
             now = time.monotonic()
             for future in copy.copy(pending):
                 if future not in backups and should_launch_backup(
                     future, now, start_times, end_times
                 ):
                     input = tasks[future]
                     logger.info("Running backup task for %s", input)
-                    futures = lithops_function_executor.map(
+                    futures = map_with_retries(
+                        lithops_function_executor,
                         partial_map_function,
                         [input],
                         timeout=timeout,
                         include_modules=include_modules,
+                        retries=0,  # don't retry backup tasks
                     )
                     tasks.update({k: v for (k, v) in zip(futures, [input])})
                     start_times.update({k: time.monotonic() for k in futures})
                     pending.extend(futures)
-                    backup = futures[0]  # TODO: launch multiple backups at once
+                    backup = futures[0]
                     backups[future] = backup
                     backups[backup] = future
             time.sleep(1)
 
 
 def execute_dag(dag, callbacks=None, array_names=None, resume=None, **kwargs):
     use_backups = kwargs.pop("use_backups", False)
@@ -191,15 +170,15 @@
         for name, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
             for stage in pipeline.stages:
                 if stage.mappable is not None:
                     for _, stats in map_unordered(
                         executor,
                         run_func,
-                        list(stage.mappable),
+                        stage.mappable,
                         func=stage.function,
                         config=pipeline.config,
                         name=name,
                         use_backups=use_backups,
                         return_stats=True,
                     ):
                         stats["array_name"] = name
@@ -225,15 +204,15 @@
     def sf(mappable):
         return stage.function(mappable, config=config)
 
     def stage_func(lithops_function_executor):
         for _, stats in map_unordered(
             lithops_function_executor,
             sf,
-            list(stage.mappable),
+            stage.mappable,
             use_backups=use_backups,
             return_stats=True,
         ):
             stats["array_name"] = name
             handle_callbacks(callbacks, stats)
 
     return stage_func
```

### Comparing `cubed-0.8.0/cubed/runtime/executors/modal.py` & `cubed-0.9.0/cubed/runtime/executors/modal.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,72 +6,124 @@
 from modal.exception import ConnectionError
 from tenacity import retry, retry_if_exception_type, stop_after_attempt
 
 from cubed.core.plan import visit_nodes
 from cubed.runtime.types import DagExecutor
 from cubed.runtime.utils import execute_with_stats, handle_callbacks
 
-stub = modal.Stub("sync-stub")
+stub = modal.Stub("cubed-stub")
 
 requirements_file = os.getenv("CUBED_MODAL_REQUIREMENTS_FILE")
 
 if requirements_file:
     image = modal.Image.debian_slim().pip_install_from_requirements(requirements_file)
+    aws_image = image
+    gcp_image = image
 else:
-    image = modal.Image.debian_slim().pip_install(
+    aws_image = modal.Image.debian_slim().pip_install(
         [
             "fsspec",
             "mypy_extensions",  # for rechunker
             "networkx",
             "pytest-mock",  # TODO: only needed for tests
             "s3fs",
             "tenacity",
             "toolz",
             "zarr",
         ]
     )
+    gcp_image = modal.Image.debian_slim().pip_install(
+        [
+            "fsspec",
+            "mypy_extensions",  # for rechunker
+            "networkx",
+            "pytest-mock",  # TODO: only needed for tests
+            "gcsfs",
+            "tenacity",
+            "toolz",
+            "zarr",
+        ]
+    )
 
 
-# Use a generator, since we want results to be returned as they finish and we don't care about order
 @stub.function(
-    image=image,
+    image=aws_image,
     secret=modal.Secret.from_name("my-aws-secret"),
     memory=2000,
     retries=2,
-    is_generator=True,
+    cloud="aws",
 )
 def run_remotely(input, func=None, config=None):
     print(f"running remotely on {input}")
     # note we can't use the execution_stat decorator since it doesn't work with modal decorators
     result, stats = execute_with_stats(func, input, config=config)
-    yield result, stats
+    return result, stats
+
+
+# For GCP we need to use a class so we can set up credentials by hooking into the container lifecycle
+@stub.cls(
+    image=gcp_image,
+    secret=modal.Secret.from_name("my-googlecloud-secret"),
+    memory=2000,
+    retries=2,
+    cloud="gcp",
+)
+class Container:
+    def __enter__(self):
+        json = os.environ["SERVICE_ACCOUNT_JSON"]
+        path = os.path.abspath("application_credentials.json")
+        with open(path, "w") as f:
+            f.write(json)
+        os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = path
+
+    @modal.method()
+    def run_remotely(self, input, func=None, config=None):
+        print(f"running remotely on {input}")
+        # note we can't use the execution_stat decorator since it doesn't work with modal decorators
+        result, stats = execute_with_stats(func, input, config=config)
+        return result, stats
 
 
 # This just retries the initial connection attempt, not the function calls
 @retry(
+    reraise=True,
     retry=retry_if_exception_type((TimeoutError, ConnectionError)),
     stop=stop_after_attempt(3),
 )
-def execute_dag(dag, callbacks=None, array_names=None, resume=None, **kwargs):
+def execute_dag(
+    dag, callbacks=None, array_names=None, resume=None, cloud=None, **kwargs
+):
     with stub.run():
+        cloud = cloud or "aws"
+        if cloud == "aws":
+            app_function = run_remotely
+        elif cloud == "gcp":
+            app_function = Container().run_remotely
+        else:
+            raise ValueError(f"Unrecognized cloud: {cloud}")
         for name, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
 
             for stage in pipeline.stages:
                 if stage.mappable is not None:
                     task_create_tstamp = time.time()
-                    for _, stats in run_remotely.map(
-                        list(stage.mappable),
+                    for _, stats in app_function.map(
+                        stage.mappable,
+                        order_outputs=False,
                         kwargs=dict(func=stage.function, config=pipeline.config),
                     ):
                         stats["array_name"] = name
                         stats["task_create_tstamp"] = task_create_tstamp
                         handle_callbacks(callbacks, stats)
                 else:
                     raise NotImplementedError()
 
 
 class ModalDagExecutor(DagExecutor):
     """An execution engine that uses Modal."""
 
+    def __init__(self, **kwargs):
+        self.kwargs = kwargs
+
     def execute_dag(self, dag, callbacks=None, array_names=None, **kwargs):
-        execute_dag(dag, callbacks=callbacks, array_names=array_names)
+        merged_kwargs = {**self.kwargs, **kwargs}
+        execute_dag(dag, callbacks=callbacks, array_names=array_names, **merged_kwargs)
```

### Comparing `cubed-0.8.0/cubed/runtime/executors/modal_async.py` & `cubed-0.9.0/cubed/runtime/executors/modal_async.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,31 @@
 import asyncio
 import copy
-import os
 import time
 from asyncio.exceptions import TimeoutError
 
-import modal
-import modal.aio
 from modal.exception import ConnectionError
 from tenacity import retry, retry_if_exception_type, stop_after_attempt
 
 from cubed.core.plan import visit_nodes
 from cubed.runtime.backup import should_launch_backup
+from cubed.runtime.executors.modal import Container, run_remotely, stub
 from cubed.runtime.types import DagExecutor
-from cubed.runtime.utils import execute_with_stats, handle_callbacks
-
-async_stub = modal.aio.AioStub("async-stub")
-
-requirements_file = os.getenv("CUBED_MODAL_REQUIREMENTS_FILE")
-
-if requirements_file:
-    image = modal.Image.debian_slim().pip_install_from_requirements(requirements_file)
-else:
-    image = modal.Image.debian_slim().pip_install(
-        [
-            "fsspec",
-            "mypy_extensions",  # for rechunker
-            "networkx",
-            "pytest-mock",  # TODO: only needed for tests
-            "s3fs",
-            "tenacity",
-            "toolz",
-            "zarr",
-        ]
-    )
-
-
-@async_stub.function(
-    image=image,
-    secret=modal.Secret.from_name("my-aws-secret"),
-    memory=2000,
-    retries=2,
-    is_generator=True,
-)
-async def async_run_remotely(input, func=None, config=None):
-    print(f"running remotely on {input}")
-    # note we can't use the execution_stat decorator since it doesn't work with modal decorators
-    result, stats = execute_with_stats(func, input, config=config)
-    yield result, stats
+from cubed.runtime.utils import handle_callbacks
 
 
 # We need map_unordered for the use_backups implementation
 async def map_unordered(
-    app_function, input, use_backups=False, return_stats=False, name=None, **kwargs
+    app_function,
+    input,
+    use_backups=False,
+    backup_function=None,
+    return_stats=False,
+    name=None,
+    **kwargs,
 ):
     """
     Apply a function to items of an input list, yielding results as they are completed
     (which may be different to the input order).
 
     :param app_function: The Modal function to map over the data.
     :param input: An iterable of input data.
@@ -63,42 +33,48 @@
     :param kwargs: Keyword arguments to pass to the function.
 
     :return: Function values (and optionally stats) as they are completed, not necessarily in the input order.
     """
     task_create_tstamp = time.time()
 
     if not use_backups:
-        async for result in app_function.map(input, kwargs=kwargs):
+        async for result in app_function.map(input, order_outputs=False, kwargs=kwargs):
             if return_stats:
                 result, stats = result
                 if name is not None:
                     stats["array_name"] = name
                 stats["task_create_tstamp"] = task_create_tstamp
                 yield result, stats
             else:
                 yield result
         return
 
-    tasks = {asyncio.ensure_future(app_function.call(i, **kwargs)): i for i in input}
+    backup_function = backup_function or app_function
+
+    tasks = {
+        asyncio.ensure_future(app_function.call.aio(i, **kwargs)): i for i in input
+    }
     pending = set(tasks.keys())
     t = time.monotonic()
     start_times = {f: t for f in pending}
     end_times = {}
     backups = {}
 
     while pending:
         finished, pending = await asyncio.wait(
             pending, return_when=asyncio.FIRST_COMPLETED, timeout=2
         )
-        # print("finished", finished)
-        # print("pending", pending)
-
         for task in finished:
             # TODO: use exception groups in Python 3.11 to handle case of multiple task exceptions
             if task.exception():
+                # if the task has a backup that is not done, or is done with no exception, then don't raise this exception
+                backup = backups.get(task, None)
+                if backup:
+                    if not backup.done() or not backup.exception():
+                        continue
                 raise task.exception()
             end_times[task] = time.monotonic()
             if return_stats:
                 result, stats = task.result()
                 if name is not None:
                     stats["array_name"] = name
                 stats["task_create_tstamp"] = task_create_tstamp
@@ -106,68 +82,85 @@
             else:
                 yield task.result()
 
             # remove any backup task
             if use_backups:
                 backup = backups.get(task, None)
                 if backup:
-                    pending.remove(backup)
+                    if backup in pending:
+                        pending.remove(backup)
                     del backups[task]
                     del backups[backup]
+                    backup.cancel()
 
         if use_backups:
             now = time.monotonic()
             for task in copy.copy(pending):
                 if task not in backups and should_launch_backup(
                     task, now, start_times, end_times
                 ):
                     # launch backup task
+                    print("Launching backup task")
                     i = tasks[task]
-                    new_task = asyncio.ensure_future(app_function.call(i, **kwargs))
+                    new_task = asyncio.ensure_future(
+                        backup_function.call.aio(i, **kwargs)
+                    )
                     tasks[new_task] = i
                     start_times[new_task] = time.monotonic()
                     pending.add(new_task)
                     backups[task] = new_task
                     backups[new_task] = task
 
 
 # This just retries the initial connection attempt, not the function calls
 @retry(
+    reraise=True,
     retry=retry_if_exception_type((TimeoutError, ConnectionError)),
     stop=stop_after_attempt(3),
 )
 async def async_execute_dag(
-    dag, callbacks=None, array_names=None, resume=None, **kwargs
+    dag, callbacks=None, array_names=None, resume=None, cloud=None, **kwargs
 ):
-    async with async_stub.run():
+    async with stub.run():
+        cloud = cloud or "aws"
+        if cloud == "aws":
+            app_function = run_remotely
+        elif cloud == "gcp":
+            app_function = Container().run_remotely
+        else:
+            raise ValueError(f"Unrecognized cloud: {cloud}")
         for name, node in visit_nodes(dag, resume=resume):
             pipeline = node["pipeline"]
 
             for stage in pipeline.stages:
                 if stage.mappable is not None:
                     async for _, stats in map_unordered(
-                        async_run_remotely,
-                        list(stage.mappable),
+                        app_function,
+                        stage.mappable,
                         return_stats=True,
                         name=name,
                         func=stage.function,
                         config=pipeline.config,
                         **kwargs,
                     ):
                         handle_callbacks(callbacks, stats)
                 else:
                     raise NotImplementedError()
 
 
 class AsyncModalDagExecutor(DagExecutor):
     """An execution engine that uses Modal's async API."""
 
+    def __init__(self, **kwargs):
+        self.kwargs = kwargs
+
     def execute_dag(self, dag, callbacks=None, array_names=None, resume=None, **kwargs):
+        merged_kwargs = {**self.kwargs, **kwargs}
         asyncio.run(
             async_execute_dag(
                 dag,
                 callbacks=callbacks,
                 array_names=array_names,
                 resume=resume,
-                **kwargs,
+                **merged_kwargs,
             )
         )
```

### Comparing `cubed-0.8.0/cubed/runtime/executors/python.py` & `cubed-0.9.0/cubed/runtime/executors/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tenacity import retry, stop_after_attempt
 
 from cubed.core.array import TaskEndEvent
 from cubed.core.plan import visit_nodes
 from cubed.runtime.types import DagExecutor
 
 
-@retry(stop=stop_after_attempt(3))
+@retry(reraise=True, stop=stop_after_attempt(3))
 def exec_stage_func(func, *args, **kwargs):
     return func(*args, **kwargs)
 
 
 class PythonDagExecutor(DagExecutor):
     """The default execution engine that runs tasks sequentially uses Python loops."""
```

### Comparing `cubed-0.8.0/cubed/runtime/executors/python_async.py` & `cubed-0.9.0/cubed/runtime/executors/python_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         raise NotImplementedError("All stages must be mappable in pipelines")
     it = stream.iterate(
         [
             partial(
                 map_unordered,
                 concurrent_executor,
                 run_func,
-                list(stage.mappable),
+                stage.mappable,
                 return_stats=True,
                 name=name,
                 func=stage.function,
                 config=pipeline.config,
                 **kwargs,
             )
             for stage in pipeline.stages
```

### Comparing `cubed-0.8.0/cubed/runtime/pipeline.py` & `cubed-0.9.0/cubed/runtime/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import itertools
 import math
 from typing import Any, Iterable, Iterator, List, Tuple
 
 import numpy as np
 
-from cubed.primitive.types import CubedPipeline
+from cubed.primitive.types import CubedCopySpec, CubedPipeline
 from cubed.storage.zarr import open_if_lazy_zarr_array
-from cubed.vendor.rechunker.types import CopySpec, Stage
+from cubed.vendor.rechunker.types import Stage
 
 from .utils import gensym
 
 
 # differs from rechunker's chunk_keys to return a list rather than a tuple, to keep lithops happy
 def chunk_keys(
     shape: Tuple[int, ...], chunks: Tuple[int, ...]
@@ -35,40 +35,40 @@
         self.shape = shape
         self.chunks = chunks
 
     def __iter__(self):
         return chunk_keys(self.shape, self.chunks)
 
 
-def copy_read_to_write(chunk_key, *, config=CopySpec):
+def copy_read_to_write(chunk_key, *, config: CubedCopySpec):
     # workaround limitation of lithops.utils.verify_args
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
     data = np.asarray(config.read.open()[chunk_key])
     config.write.open()[chunk_key] = data
 
 
-def copy_read_to_intermediate(chunk_key, *, config=CopySpec):
+def copy_read_to_intermediate(chunk_key, *, config: CubedCopySpec):
     # workaround limitation of lithops.utils.verify_args
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
     data = np.asarray(config.read.open()[chunk_key])
     config.intermediate.open()[chunk_key] = data
 
 
-def copy_intermediate_to_write(chunk_key, *, config=CopySpec):
+def copy_intermediate_to_write(chunk_key, *, config: CubedCopySpec):
     # workaround limitation of lithops.utils.verify_args
     if isinstance(chunk_key, list):
         chunk_key = tuple(chunk_key)
     data = np.asarray(config.intermediate.open()[chunk_key])
     config.write.open()[chunk_key] = data
 
 
 def spec_to_pipeline(
-    spec: CopySpec, target_array: Any, projected_mem: int, num_tasks: int
+    spec: CubedCopySpec, target_array: Any, projected_mem: int, num_tasks: int
 ) -> CubedPipeline:
     # typing won't work until we start using numpy types
     shape = spec.read.array.shape  # type: ignore
     if spec.intermediate.array is None:
         stages = [
             Stage(
                 copy_read_to_write,
```

### Comparing `cubed-0.8.0/cubed/runtime/utils.py` & `cubed-0.9.0/cubed/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/storage/zarr.py` & `cubed-0.9.0/cubed/storage/zarr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from typing import Any, Optional, Union
+
 import zarr
+from numpy import ndarray
+
+from cubed.types import T_DType, T_RegularChunks, T_Shape, T_Store
 
 
 class LazyZarrArray:
     """A Zarr array that may not have been written to storage yet.
 
     On creation, a normal Zarr array's metadata is immediately written to storage,
     and there is no way to avoid this, hence this class, which separates the creation
     of the object in memory and the creation of array metadata in storage.
     """
 
     def __init__(
         self,
-        shape,
-        dtype,
-        chunks,
-        store,
-        initial_values=None,
-        fill_value=None,
+        shape: T_Shape,
+        dtype: T_DType,
+        chunks: T_RegularChunks,
+        store: T_Store,
+        initial_values: Optional[ndarray] = None,
+        fill_value: Any = None,
         **kwargs,
     ):
         """Create a Zarr array lazily in memory."""
         # use an empty in-memory Zarr array as a template since it normalizes its properties
         template = zarr.empty(
             shape, dtype=dtype, chunks=chunks, store=zarr.storage.MemoryStore()
         )
@@ -29,67 +34,82 @@
         self.chunks = template.chunks
 
         self.store = store
         self.initial_values = initial_values
         self.fill_value = fill_value
         self.kwargs = kwargs
 
-    def create(self, mode="w-"):
+    def create(self, mode: str = "w-") -> zarr.Array:
         """Create the Zarr array in storage.
 
         The Zarr array's metadata is initialized in the backing store, and any
         initial values are set on the array.
 
         Parameters
         ----------
         mode : str
             The mode to open the Zarr array with using ``zarr.open``.
             Default is 'w-', which means create, fail it already exists.
         """
-        target = zarr.open(
+        target = zarr.open_array(
             self.store,
             mode=mode,
             shape=self.shape,
             dtype=self.dtype,
             chunks=self.chunks,
             fill_value=self.fill_value,
             **self.kwargs,
         )
         if self.initial_values is not None and self.initial_values.size > 0:
             target[...] = self.initial_values
         return target
 
-    def open(self):
+    def open(self) -> zarr.Array:
         """Open the Zarr array for reading or writing and return it.
 
         Note that the Zarr array must have been created or this method will raise an exception.
         """
         # r+ means read/write, fail if it doesn't exist
-        return zarr.open(
+        return zarr.open_array(
             self.store,
             mode="r+",
             shape=self.shape,
             dtype=self.dtype,
             chunks=self.chunks,
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"cubed.storage.zarr.LazyZarrArray<shape={self.shape}, dtype={self.dtype}, chunks={self.chunks}>"
 
 
-def lazy_empty(shape, *, dtype, chunks, store, **kwargs):
+T_ZarrArray = Union[zarr.Array, LazyZarrArray]
+
+
+def lazy_empty(
+    shape: T_Shape, *, dtype: T_DType, chunks: T_RegularChunks, store: T_Store, **kwargs
+) -> LazyZarrArray:
     return LazyZarrArray(shape, dtype, chunks, store, **kwargs)
 
 
-def lazy_from_array(array, *, dtype, chunks, store, **kwargs):
+def lazy_from_array(
+    array: ndarray, *, dtype: T_DType, chunks: T_RegularChunks, store: T_Store, **kwargs
+) -> LazyZarrArray:
     return LazyZarrArray(
         array.shape, dtype, chunks, store, initial_values=array, **kwargs
     )
 
 
-def lazy_full(shape, fill_value, *, dtype, chunks, store, **kwargs):
+def lazy_full(
+    shape: T_Shape,
+    fill_value: Any,
+    *,
+    dtype: T_DType,
+    chunks: T_RegularChunks,
+    store: T_Store,
+    **kwargs,
+) -> LazyZarrArray:
     return LazyZarrArray(shape, dtype, chunks, store, fill_value=fill_value, **kwargs)
 
 
-def open_if_lazy_zarr_array(array):
+def open_if_lazy_zarr_array(array: T_ZarrArray) -> zarr.Array:
     """If array is a LazyZarrArray then open it, leaving other arrays unchanged."""
     return array.open() if isinstance(array, LazyZarrArray) else array
```

### Comparing `cubed-0.8.0/cubed/tests/primitive/test_blockwise.py` & `cubed-0.9.0/cubed/tests/primitive/test_blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/primitive/test_rechunk.py` & `cubed-0.9.0/cubed/tests/primitive/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/runtime/test_backup.py` & `cubed-0.9.0/cubed/tests/runtime/test_backup.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/runtime/test_lithops.py` & `cubed-0.9.0/cubed/tests/runtime/test_lithops.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/runtime/test_modal_async.py` & `cubed-0.9.0/cubed/tests/runtime/test_modal_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pytest
 
 modal = pytest.importorskip("modal")
 
 import asyncio
 
 import fsspec
-import modal.aio
+import modal
 
 from cubed.runtime.executors.modal_async import map_unordered
 from cubed.tests.runtime.utils import check_invocation_counts, deterministic_failure
 
 tmp_path = "s3://cubed-unittest/map_unordered"
 
 
-stub = modal.aio.AioStub("async-test-stub")
+stub = modal.Stub("cubed-test-stub")
 
 image = modal.Image.debian_slim().pip_install(
     [
         "fsspec",
         "mypy_extensions",  # for rechunker
         "networkx",
         "pytest-mock",  # TODO: only needed for tests
```

### Comparing `cubed-0.8.0/cubed/tests/runtime/test_python_async.py` & `cubed-0.9.0/cubed/tests/runtime/test_python_async.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/runtime/utils.py` & `cubed-0.9.0/cubed/tests/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/storage/test_zarr.py` & `cubed-0.9.0/cubed/tests/storage/test_zarr.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/test_array_api.py` & `cubed-0.9.0/cubed/tests/test_array_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         b.compute(executor=executor),
         np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]),
     )
 
 
 # Elementwise functions
 
+
 # test on all executors (`any_executor`) for coverage
 def test_add(spec, any_executor):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 2), spec=spec)
     b = xp.asarray([[1, 1, 1], [1, 1, 1], [1, 1, 1]], chunks=(2, 2), spec=spec)
     c = xp.add(a, b)
     assert_array_equal(
         c.compute(executor=any_executor), np.array([[2, 3, 4], [5, 6, 7], [8, 9, 10]])
```

### Comparing `cubed-0.8.0/cubed/tests/test_core.py` & `cubed-0.9.0/cubed/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import pytest
 import zarr
 from numpy.testing import assert_array_equal
 
 import cubed
 import cubed.array_api as xp
+import cubed.random
 from cubed.extensions.history import HistoryCallback
 from cubed.extensions.timeline import TimelineVisualizationCallback
 from cubed.extensions.tqdm import TqdmProgressBar
 from cubed.primitive.blockwise import apply_blockwise
 from cubed.runtime.types import DagExecutor
 from cubed.tests.utils import MAIN_EXECUTORS, MODAL_EXECUTORS, TaskCounter, create_zarr
 
@@ -193,17 +194,18 @@
     d = xp.negative(c)
     assert_array_equal(
         d.compute(executor=executor),
         np.array([[-2, -3, -4], [-5, -6, -7], [-8, -9, -10]]),
     )
 
 
-def test_rechunk(spec, executor):
+@pytest.mark.parametrize("new_chunks", [(1, 2), {0: 1, 1: 2}])
+def test_rechunk(spec, executor, new_chunks):
     a = xp.asarray([[1, 2, 3], [4, 5, 6], [7, 8, 9]], chunks=(2, 1), spec=spec)
-    b = a.rechunk((1, 2))
+    b = a.rechunk(new_chunks)
     assert_array_equal(
         b.compute(executor=executor),
         np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]),
     )
 
 
 def test_rechunk_same_chunks(spec):
@@ -507,7 +509,24 @@
     from cubed.runtime.executors.lithops import LithopsDagExecutor
 
     if not isinstance(executor, LithopsDagExecutor):
         pytest.skip(f"{type(executor)} does not support measure_reserved_mem")
 
     reserved_memory = cubed.measure_reserved_mem(executor=executor)
     assert reserved_memory > 1_000_000  # over 1MB
+
+
+# Test we can create a plan for arrays of up to 5PB, and 100s of billions of tasks
+@pytest.mark.parametrize("factor", [10, 20, 50, 100, 200, 500, 1000, 2000, 5000])
+def test_plan_scaling(tmp_path, factor):
+    spec = cubed.Spec(tmp_path, allowed_mem="2GB")
+    chunksize = 5000
+    a = cubed.random.random(
+        (factor * chunksize, factor * chunksize), chunks=chunksize, spec=spec
+    )
+    b = cubed.random.random(
+        (factor * chunksize, factor * chunksize), chunks=chunksize, spec=spec
+    )
+    c = xp.matmul(a, b)
+
+    assert c.plan.num_tasks() > 0
+    c.visualize(filename=tmp_path / "c")
```

### Comparing `cubed-0.8.0/cubed/tests/test_gufunc.py` & `cubed-0.9.0/cubed/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/test_indexing.py` & `cubed-0.9.0/cubed/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/test_mem_utilization.py` & `cubed-0.9.0/cubed/tests/test_mem_utilization.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def spec(tmp_path, reserved_mem):
     return cubed.Spec(tmp_path, allowed_mem=2_000_000_000, reserved_mem=reserved_mem)
 
 
 @pytest.fixture(scope="module")
 def reserved_mem():
     executor = LithopsDagExecutor(config=LITHOPS_LOCAL_CONFIG)
-    res = cubed.measure_reserved_mem(executor) * 1.05  # add some wiggle room
+    res = cubed.measure_reserved_mem(executor) * 1.1  # add some wiggle room
     return round_up_to_multiple(res, 10_000_000)  # round up to nearest multiple of 10MB
 
 
 def round_up_to_multiple(x, multiple=10):
     """Round up to the nearest multiple"""
     return math.ceil(x / multiple) * multiple
```

### Comparing `cubed-0.8.0/cubed/tests/test_optimization.py` & `cubed-0.9.0/cubed/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/test_random.py` & `cubed-0.9.0/cubed/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/tests/test_utils.py` & `cubed-0.9.0/cubed/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     assert memory_repr(0) == "0 bytes"
     assert memory_repr(1) == "1 bytes"
     assert memory_repr(999) == "999 bytes"
     assert memory_repr(1_000) == "1.0 KB"
     assert memory_repr(9_999) == "10.0 KB"
     assert memory_repr(1_000_000) == "1.0 MB"
     assert memory_repr(1_000_000_000_000_000) == "1.0 PB"
+    assert memory_repr(int(1e18)) == "1.0e+18 bytes"
+    with pytest.raises(ValueError):
+        memory_repr(-1)
 
 
 @pytest.mark.skipif(platform.system() == "Windows", reason="does not run on windows")
 def test_peak_measured_mem():
     assert peak_measured_mem() > 0
```

### Comparing `cubed-0.8.0/cubed/tests/utils.py` & `cubed-0.9.0/cubed/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/utils.py` & `cubed-0.9.0/cubed/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 import sysconfig
 import traceback
 from dataclasses import dataclass
 from math import prod
 from operator import add
 from pathlib import Path
 from posixpath import join
-from typing import Union
+from typing import Tuple, Union
 from urllib.parse import quote, unquote, urlsplit, urlunsplit
 
 import numpy as np
 import tlz as toolz
 
+from cubed.types import T_DType, T_RectangularChunks, T_RegularChunks
 from cubed.vendor.dask.array.core import _check_regular_chunks
 
 PathType = Union[str, Path]
 
 
-def chunk_memory(dtype, chunksize):
+def chunk_memory(dtype: T_DType, chunksize: T_RegularChunks) -> int:
     """Calculate the amount of memory in bytes that a single chunk uses."""
     return np.dtype(dtype).itemsize * prod(chunksize)
 
 
-def get_item(chunks, idx):
+def get_item(chunks: T_RectangularChunks, idx: Tuple[int, ...]) -> Tuple[slice, ...]:
     """Convert a chunk index to a tuple of slices."""
     # could use Dask's cached_cumsum here if it improves performance
     starts = tuple(_cumsum(c, initial_zero=True) for c in chunks)
     loc = tuple((start[i], start[i + 1]) for i, start in zip(idx, starts))
     return tuple(slice(*s, None) for s in loc)
 
 
@@ -44,37 +45,41 @@
     """Combine a URL for a directory with a child path"""
     parts = urlsplit(str(dir_url))
     new_path = quote(join(unquote(parts.path), child_path))
     split_parts = (parts.scheme, parts.netloc, new_path, parts.query, parts.fragment)
     return urlunsplit(split_parts)
 
 
-def memory_repr(num):
+def memory_repr(num: int) -> str:
     """Convert bytes to a human-readable string in decimal form.
     1 KB is 1,000 bytes, 1 MB is 1,000,000 bytes, and so on.
 
     Parameters
     ----------
     num: int
         Number of bytes
 
     Returns
     -------
     str
     """
+    if num < 0:
+        raise ValueError(f"Invalid value: {num}. Expected a positive integer.")
     if num < 1000.0:
         return f"{num} bytes"
-    num /= 1000.0
+    val = num / 1000.0
     for x in ["KB", "MB", "GB", "TB", "PB"]:
-        if num < 1000.0:
-            return f"{num:3.1f} {x}"
-        num /= 1000.0
+        if val < 1000.0:
+            return f"{val:3.1f} {x}"
+        val /= 1000.0
+    # fall back to scientific notation
+    return f"{num:.1e} bytes"
 
 
-def peak_measured_mem():
+def peak_measured_mem() -> int:
     """Measures the peak memory usage in bytes.
 
     Note: this function currently doesn't work on Windows.
     """
 
     if platform.system() == "Windows":
         raise NotImplementedError("`peak_measured_mem` is not implemented on Windows")
@@ -83,29 +88,29 @@
 
     ru_maxrss = getrusage(RUSAGE_SELF).ru_maxrss
     # note that on Linux ru_maxrss is in KiB, while on Mac it is in bytes
     # see https://pythonspeed.com/articles/estimating-memory-usage/#measuring-peak-memory-usage
     return ru_maxrss * 1024 if platform.system() == "Linux" else ru_maxrss
 
 
-def to_chunksize(chunkset):
+def to_chunksize(chunkset: T_RectangularChunks) -> T_RegularChunks:
     """Convert a chunkset to a chunk size for Zarr.
 
     Parameters
     ----------
     chunkset: tuple of tuples of ints
         From the ``.chunks`` attribute of an ``Array``
 
     Returns
     -------
     Tuple of ints
     """
 
     if not _check_regular_chunks(chunkset):
-        raise ValueError("Array must have regular chunks")
+        raise ValueError(f"Array must have regular chunks, but found chunks={chunkset}")
 
     return tuple(c[0] for c in chunkset)
 
 
 @dataclass
 class StackSummary:
     """Like Python's ``FrameSummary``, but with module information."""
@@ -209,14 +214,12 @@
             value = size[:-2]
         else:
             raise ValueError(
                 f"Invalid value: {size}. Expected a string ending with an SI prefix."
             )
 
         if unit in units and value.isdigit():
-            value = int(value)
             # convert to bytes
-            return value * (1000 ** units[unit])
-    else:
-        raise ValueError(
-            f"Invalid value: {size}. Expected a positive integer or a string ending with an SI prefix."
-        )
+            return int(value) * (1000 ** units[unit])
+    raise ValueError(
+        f"Invalid value: {size}. Expected a positive integer or a string ending with an SI prefix."
+    )
```

### Comparing `cubed-0.8.0/cubed/vendor/dask/array/core.py` & `cubed-0.9.0/cubed/vendor/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/dask/array/gufunc.py` & `cubed-0.9.0/cubed/vendor/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/dask/array/reshape.py` & `cubed-0.9.0/cubed/vendor/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/dask/array/utils.py` & `cubed-0.9.0/cubed/vendor/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/dask/blockwise.py` & `cubed-0.9.0/cubed/vendor/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/dask/core.py` & `cubed-0.9.0/cubed/vendor/dask/core.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/rechunker/algorithm.py` & `cubed-0.9.0/cubed/vendor/rechunker/algorithm.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/rechunker/api.py` & `cubed-0.9.0/cubed/vendor/rechunker/api.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/rechunker/executors/python.py` & `cubed-0.9.0/cubed/vendor/rechunker/executors/python.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed/vendor/rechunker/types.py` & `cubed-0.9.0/cubed/vendor/rechunker/types.py`

 * *Files identical despite different names*

### Comparing `cubed-0.8.0/cubed.egg-info/PKG-INFO` & `cubed-0.9.0/cubed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubed
-Version: 0.8.0
+Version: 0.9.0
 Summary: Bounded-memory serverless distributed N-dimensional array processing
 Author-email: Tom White <tom.e.white@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/tomwhite/cubed
 Project-URL: documentation, https://tomwhite.github.io/cubed
 Project-URL: repository, https://github.com/tomwhite/cubed
 Classifier: Development Status :: 3 - Alpha
@@ -32,9 +32,10 @@
 Cubed is a distributed N-dimensional array library implemented in Python using bounded-memory serverless processing and Zarr for storage.
 
 - Implements the [Python Array API standard](https://data-apis.org/array-api/latest/) (see [coverage status](./api_status.md))
 - Guaranteed maximum memory usage for standard array functions
 - Follows [Dask Array](https://docs.dask.org/en/stable/array.html)'s chunked array API (`map_blocks`, `rechunk`, `apply_gufunc`, etc)
 - [Zarr](https://zarr.readthedocs.io/en/stable/) for persistent and intermediate storage
 - Multiple serverless runtimes: Python (in-process), [Lithops](https://lithops-cloud.github.io/), [Modal](https://modal.com/), [Apache Beam](https://beam.apache.org/)
+- Integration with [Xarray](https://xarray.dev/) via [cubed-xarray](https://github.com/xarray-contrib/cubed-xarray)
 
 [Documentation](https://tomwhite.github.io/cubed)
```

### Comparing `cubed-0.8.0/cubed.egg-info/SOURCES.txt` & `cubed-0.9.0/cubed.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 cubed/__init__.py
 cubed/random.py
+cubed/types.py
 cubed/utils.py
 cubed.egg-info/PKG-INFO
 cubed.egg-info/SOURCES.txt
 cubed.egg-info/dependency_links.txt
 cubed.egg-info/requires.txt
 cubed.egg-info/top_level.txt
 cubed/array_api/__init__.py
@@ -41,51 +42,58 @@
 cubed/runtime/backup.py
 cubed/runtime/pipeline.py
 cubed/runtime/types.py
 cubed/runtime/utils.py
 cubed/runtime/executors/__init__.py
 cubed/runtime/executors/beam.py
 cubed/runtime/executors/lithops.py
+cubed/runtime/executors/lithops_retries.py
 cubed/runtime/executors/modal.py
 cubed/runtime/executors/modal_async.py
 cubed/runtime/executors/python.py
 cubed/runtime/executors/python_async.py
 cubed/storage/__init__.py
+cubed/storage/virtual.py
 cubed/storage/zarr.py
 cubed/tests/__init__.py
 cubed/tests/test_array_api.py
 cubed/tests/test_core.py
 cubed/tests/test_gufunc.py
+cubed/tests/test_html.py
 cubed/tests/test_indexing.py
 cubed/tests/test_mem_utilization.py
 cubed/tests/test_optimization.py
 cubed/tests/test_random.py
 cubed/tests/test_utils.py
 cubed/tests/utils.py
 cubed/tests/primitive/__init__.py
 cubed/tests/primitive/test_blockwise.py
 cubed/tests/primitive/test_rechunk.py
 cubed/tests/runtime/__init__.py
 cubed/tests/runtime/test_backup.py
 cubed/tests/runtime/test_lithops.py
+cubed/tests/runtime/test_lithops_retries.py
 cubed/tests/runtime/test_modal_async.py
 cubed/tests/runtime/test_python_async.py
 cubed/tests/runtime/utils.py
 cubed/tests/storage/__init__.py
 cubed/tests/storage/test_zarr.py
 cubed/vendor/__init__.py
 cubed/vendor/dask/__init__.py
 cubed/vendor/dask/blockwise.py
 cubed/vendor/dask/core.py
 cubed/vendor/dask/utils.py
 cubed/vendor/dask/array/__init__.py
 cubed/vendor/dask/array/core.py
 cubed/vendor/dask/array/gufunc.py
 cubed/vendor/dask/array/reshape.py
+cubed/vendor/dask/array/svg.py
 cubed/vendor/dask/array/utils.py
+cubed/vendor/dask/widgets/__init__.py
+cubed/vendor/dask/widgets/widgets.py
 cubed/vendor/rechunker/__init__.py
 cubed/vendor/rechunker/algorithm.py
 cubed/vendor/rechunker/api.py
 cubed/vendor/rechunker/compat.py
 cubed/vendor/rechunker/types.py
 cubed/vendor/rechunker/executors/__init__.py
 cubed/vendor/rechunker/executors/python.py
```

### Comparing `cubed-0.8.0/pyproject.toml` & `cubed-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cubed"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
     {name = "Tom White", email = "tom.e.white@gmail.com"},
 ]
 license = {text = "Apache License 2.0"}
 description = "Bounded-memory serverless distributed N-dimensional array processing"
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
@@ -31,14 +31,15 @@
     "zarr",
 ]
 
 [project.optional-dependencies]
 diagnostics = [
     "tqdm",
     "graphviz",
+    "jinja2",
     "pydot",
     "pandas",
     "matplotlib",
     "seaborn",
 ]
 beam = ["apache-beam", "gcsfs"]
 lithops = ["lithops[aws] >= 2.7.0"]
```

### Comparing `cubed-0.8.0/setup.cfg` & `cubed-0.9.0/setup.cfg`

 * *Files identical despite different names*


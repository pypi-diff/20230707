# Comparing `tmp/unidist-0.3.0.tar.gz` & `tmp/unidist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidist-0.3.0.tar", last modified: Wed Mar 22 16:18:16 2023, max compression
+gzip compressed data, was "unidist-0.4.0.tar", last modified: Fri Jul  7 15:55:14 2023, max compression
```

## Comparing `unidist-0.3.0.tar` & `unidist-0.4.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.859020 unidist-0.3.0/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      687 2023-03-22 16:09:14.000000 unidist-0.3.0/AUTHORS
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11357 2023-03-22 16:09:14.000000 unidist-0.3.0/LICENSE
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       50 2023-03-22 16:09:14.000000 unidist-0.3.0/MANIFEST.in
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5398 2023-03-22 16:18:16.859020 unidist-0.3.0/PKG-INFO
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5045 2023-03-22 16:09:14.000000 unidist-0.3.0/README.md
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      354 2023-03-22 16:18:16.859020 unidist-0.3.0/setup.cfg
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1117 2023-03-22 16:09:14.000000 unidist-0.3.0/setup.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.869020 unidist-0.3.0/unidist/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      559 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      497 2023-03-22 16:18:16.869020 unidist-0.3.0/unidist/_version.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6912 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/api.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/config/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      839 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/config/backends/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      172 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/config/backends/common/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      232 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/common/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2336 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/common/envvars.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/config/backends/dask/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      323 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/dask/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      758 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/dask/envvars.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/config/backends/mpi/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      312 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/mpi/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      756 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/mpi/envvars.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/config/backends/ray/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      434 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/ray/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1131 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/backends/ray/envvars.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6336 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/config/parameter.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      107 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/__init__.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/common/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      122 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/common/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      909 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/common/data_id.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1121 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/common/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/dask/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      115 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/dask/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6692 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/dask/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5526 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/dask/backend.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3460 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/dask/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1078 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/dask/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/mpi/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5692 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4668 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/backend.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/mpi/core/
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)      408 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1997 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/async_operations.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     8445 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/common.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)    20459 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/communication.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/mpi/core/controller/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      533 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/controller/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6091 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/controller/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    12275 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/controller/api.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7885 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/controller/common.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5566 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/controller/garbage_collector.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7903 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/controller/object_store.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     2511 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/monitor.py
--rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     8654 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/serialization.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/mpi/core/worker/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      142 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/worker/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7059 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/worker/loop.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6340 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/worker/object_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    10732 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/worker/request_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    14351 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/core/worker/task_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3153 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      275 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/mpi/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/pymp/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      133 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4336 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4815 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/backend.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/pymp/core/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      305 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/core/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4701 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/core/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4067 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/core/api.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4268 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/core/object_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6900 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/core/process_manager.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3004 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      506 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pymp/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist/core/backends/pyseq/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      128 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4225 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4609 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/backend.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.859020 unidist-0.3.0/unidist/core/backends/pyseq/core/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      252 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/core/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3060 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/core/api.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2313 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/core/object_store.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2905 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      382 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/pyseq/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.859020 unidist-0.3.0/unidist/core/backends/ray/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/ray/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5544 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/ray/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4616 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/ray/backend.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2742 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/ray/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4778 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/backends/ray/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.859020 unidist-0.3.0/unidist/core/base/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      112 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6620 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    10573 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/backend.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1255 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/common.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      384 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/object_ref.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3105 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/remote_function.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3330 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/core/base/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.859020 unidist-0.3.0/unidist/test/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/test/__init__.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4174 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/test/test_actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6039 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/test/test_async_actor.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2172 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/test/test_general.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2668 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/test/test_task.py
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2276 2023-03-22 16:09:14.000000 unidist-0.3.0/unidist/test/utils.py
-drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-03-22 16:18:16.849020 unidist-0.3.0/unidist.egg-info/
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5398 2023-03-22 16:18:16.000000 unidist-0.3.0/unidist.egg-info/PKG-INFO
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3428 2023-03-22 16:18:16.000000 unidist-0.3.0/unidist.egg-info/SOURCES.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        1 2023-03-22 16:18:16.000000 unidist-0.3.0/unidist.egg-info/dependency_links.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      235 2023-03-22 16:18:16.000000 unidist-0.3.0/unidist.egg-info/requires.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        8 2023-03-22 16:18:16.000000 unidist-0.3.0/unidist.egg-info/top_level.txt
--rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    80049 2023-03-22 16:09:14.000000 unidist-0.3.0/versioneer.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      687 2023-07-07 15:47:13.000000 unidist-0.4.0/AUTHORS
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11357 2023-07-07 15:47:13.000000 unidist-0.4.0/LICENSE
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       50 2023-07-07 15:47:13.000000 unidist-0.4.0/MANIFEST.in
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6682 2023-07-07 15:55:14.834100 unidist-0.4.0/PKG-INFO
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6329 2023-07-07 15:47:13.000000 unidist-0.4.0/README.md
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      354 2023-07-07 15:55:14.834100 unidist-0.4.0/setup.cfg
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1185 2023-07-07 15:47:13.000000 unidist-0.4.0/setup.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      559 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      497 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/_version.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6912 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/api.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      916 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      172 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/common/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      232 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/common/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2337 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/common/envvars.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/dask/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      323 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/dask/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      758 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/dask/envvars.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/mpi/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      379 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/mpi/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1331 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/mpi/envvars.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/config/backends/ray/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      434 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/ray/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1131 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/backends/ray/envvars.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6612 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/config/parameter.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist/core/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      107 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/__init__.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/common/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      122 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/common/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      909 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/common/data_id.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1121 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/common/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/dask/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      115 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6692 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5526 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/backend.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3460 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1078 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/dask/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5692 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4668 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/backend.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/core/
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)      408 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1965 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/async_operations.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     9383 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/common.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)    26560 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/communication.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/core/controller/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      533 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6091 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    16962 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/api.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7885 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/common.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5563 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/garbage_collector.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     7918 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/controller/object_store.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     7224 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/monitor.py
+-rwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)     8921 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/serialization.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/mpi/core/worker/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      142 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     9329 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/loop.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6340 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/object_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    11488 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/request_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    15638 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/core/worker/task_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3153 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      275 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/mpi/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pymp/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      133 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4336 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4815 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/backend.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pymp/core/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      305 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4701 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4067 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/api.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4268 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/object_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6900 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/core/process_manager.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3004 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      506 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pymp/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pyseq/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      128 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4225 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4609 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/backend.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/pyseq/core/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      252 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/core/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3060 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/core/api.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2313 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/core/object_store.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2905 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      382 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/pyseq/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/backends/ray/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      114 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     5544 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4616 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/backend.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2742 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4778 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/backends/ray/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/core/base/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      112 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6620 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    10573 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/backend.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     1255 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/common.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      384 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/object_ref.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3105 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/remote_function.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3330 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/core/base/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.834100 unidist-0.4.0/unidist/test/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)       80 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/__init__.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     4174 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6039 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_async_actor.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2172 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_general.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2668 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/test_task.py
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     2276 2023-07-07 15:47:13.000000 unidist-0.4.0/unidist/test/utils.py
+drwxr-xr-x   0 yigoshev  (1000) yigoshev  (1000)        0 2023-07-07 15:55:14.824100 unidist-0.4.0/unidist.egg-info/
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     6682 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/PKG-INFO
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)     3428 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/SOURCES.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        1 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/dependency_links.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)      257 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/requires.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)        8 2023-07-07 15:55:14.000000 unidist-0.4.0/unidist.egg-info/top_level.txt
+-rw-r--r--   0 yigoshev  (1000) yigoshev  (1000)    80049 2023-07-07 15:47:13.000000 unidist-0.4.0/versioneer.py
```

### Comparing `unidist-0.3.0/AUTHORS` & `unidist-0.4.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/LICENSE` & `unidist-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/PKG-INFO` & `unidist-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: unidist
-Version: 0.3.0
-Summary: Unified Distributed Execution
-Home-page: https://github.com/modin-project/unidist
-License: Apache-2.0
-Requires-Python: >=3.7.1
-Description-Content-Type: text/markdown
-Provides-Extra: ray
-Provides-Extra: dask
-Provides-Extra: mpi
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS
-
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
 <a href="https://github.com/modin-project/unidist/actions"><img src="https://github.com/modin-project/unidist/workflows/master/badge.svg" align="center"></a>
@@ -24,102 +9,114 @@
 <a href="https://pypi.org/project/unidist/"><img src="https://badge.fury.io/py/unidist.svg" alt="PyPI version" align="center"></a>
 </p>
 
 ### What is unidist?
 
 unidist is a framework that is intended to provide the unified API for distributed execution by supporting various performant execution backends. At the moment the following backends are supported under the hood:
 
-* [Ray](https://docs.ray.io/en/master/index.html)
 * [MPI](https://www.mpi-forum.org/)
 * [Dask Distributed](https://distributed.dask.org/en/latest/)
+* [Ray](https://docs.ray.io/en/master/index.html)
 * [Python Multiprocessing](https://docs.python.org/3/library/multiprocessing.html)
 
 unidist is designed to work in a [task-based parallel](https://en.wikipedia.org/wiki/Task_parallelism) model.
 
-Also, the framework provides a sequential ``Python`` backend, that can be used for debugging.
+Also, the framework provides a Python Sequential backend (`pyseq`), that can be used for debugging.
 
 ### Installation
 
-#### From PyPI
+#### Using pip
 
 unidist can be installed with `pip` on Linux, Windows and MacOS:
 
 ```bash
 pip install unidist # Install unidist with dependencies for Python Multiprocessing and Python Sequential backends
 ```
 
-unidist can also be used with Dask, MPI or Ray execution backend.
-If you don't have Dask, MPI or Ray installed, you will need to install unidist with one of the targets:
+unidist can also be used with MPI, Dask or Ray execution backend.
+If you don't have MPI, Dask or Ray installed, you will need to install unidist with one of the targets:
 
 ```bash
 pip install unidist[all] # Install unidist with dependencies for all the backends
-pip install unidist[dask] # Install unidist with dependencies for Dask backend
 pip install unidist[mpi] # Install unidist with dependencies for MPI backend
+pip install unidist[dask] # Install unidist with dependencies for Dask backend
 pip install unidist[ray] # Install unidist with dependencies for Ray backend
 ```
 
 unidist automatically detects which execution backends are installed and uses that for scheduling computation.
 
-#### From conda-forge
+**Note:** There are different MPI implementations, each of which can be used as a backend in unidist.
+By default, mapping `unidist[mpi]` installs MPICH on Linux and MacOS and MSMPI on Windows. If you want to use
+a specific version of MPI, you can install the core dependencies of unidist as `pip install unidist` and then
+install the specific version of MPI using pip as shown in the [installation](https://mpi4py.readthedocs.io/en/latest/install.html)
+section of mpi4py documentation.
+
+#### Using conda
 
-For installing unidist with dependencies for Dask and MPI execution backends into a conda environment
+For installing unidist with dependencies for MPI and Dask execution backends into a conda environment
 the following command should be used:
 
 ```bash
-conda install unidist-dask unidist-mpi -c conda-forge
+conda install unidist-mpi unidist-dask -c conda-forge
 ```
 
 All set of backends could be available in a conda environment by specifying:
 
 ```bash
 conda install unidist-all -c conda-forge
 ```
 
 or explicitly:
 
 ```bash
-conda install unidist-dask unidist-mpi unidist-ray -c conda-forge
+conda install unidist-mpi unidist-dask unidist-ray -c conda-forge
 ```
 
+**Note:** There are different MPI implementations, each of which can be used as a backend in unidist.
+By default, mapping `unidist-mpi` installs MPICH on Linux and MacOS and MSMPI on Windows. If you want to use
+a specific version of MPI, you can install the core dependencies of unidist as `conda install unidist` and then
+install the specific version of MPI using conda as shown in the [installation](https://mpi4py.readthedocs.io/en/latest/install.html)
+section of mpi4py documentation. That said, it is highly encouraged to use your own MPI binaries as stated in the
+[Using External MPI Libraries](https://conda-forge.org/docs/user/tipsandtricks.html#using-external-message-passing-interface-mpi-libraries)
+section of the conda-forge documentation in order to get ultimate performance.
+
 For more information refer to [Installation](https://unidist.readthedocs.io/en/latest/installation.html) section.
 
 #### Choosing an execution backend
 
 If you want to choose a specific execution backend to run on,
 you can set the environment variable `UNIDIST_BACKEND` and unidist will do computation with that backend:
 
 ```bash
-export UNIDIST_BACKEND=ray  # unidist will use Ray
 export UNIDIST_BACKEND=mpi  # unidist will use MPI
 export UNIDIST_BACKEND=dask  # unidist will use Dask
+export UNIDIST_BACKEND=ray  # unidist will use Ray
 ```
 
 This can also be done within a notebook/interpreter before you initialize unidist:
 
 ```python
 from unidist.config import Backend
 
-Backend.put("ray")  # unidist will use Ray
 Backend.put("mpi")  # unidist will use MPI
 Backend.put("dask")  # unidist will use Dask
+Backend.put("ray")  # unidist will use Ray
 ```
 
-If you have installed all the execution backends and haven't specified any of the execution backends, Ray is used by default.
-
-Since some of the execution backends, particularly, MPI, have some specifics regarding running python programs, please
-refer to [Using Unidist](https://unidist.readthedocs.io/en/latest/using_unidist/index.html) section to get more information on
-setting the execution backend to run on.
+If you have installed all the execution backends and haven't specified any of the execution backends, MPI is used by default.
+Currently, almost all MPI implementations require ``mpiexec`` command to be used when running an MPI program.
+If you use a backend other than MPI, you run a program as a regular python script (see below).
 
 #### Usage
 
 ```python
 # script.py
 
 import unidist
-unidist.init() # Ray backend is used by default
+unidist.init() # MPI backend is used by default
 
 @unidist.remote
 def foo(x):
     return x * x
 
 # This will run `foo` on a pool of workers in parallel;
 # `refs` will contain object references to actual data
@@ -127,16 +124,17 @@
 # To get the data call `unidist.get(...)`
 print(unidist.get(refs))
 ```
 
 Run the `script.py` with:
 
 ```bash
-$ python script.py
-[0, 1, 4, 9, 16] # output
+$ mpiexec -n 1 python script.py  # for MPI backend
+# $ python script.py  # for any other supported backend
+[0, 1, 4, 9, 16]  # output
 ```
 
 For more examples refer to [Getting Started](https://unidist.readthedocs.io/en/latest/getting_started.html) section
 in our documentation.
 
 ### Powered by unidist
```

### Comparing `unidist-0.3.0/README.md` & `unidist-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: unidist
+Version: 0.4.0
+Summary: Unified Distributed Execution
+Home-page: https://github.com/modin-project/unidist
+License: Apache-2.0
+Requires-Python: >=3.7.1
+Description-Content-Type: text/markdown
+Provides-Extra: ray
+Provides-Extra: dask
+Provides-Extra: mpi
+Provides-Extra: all
+License-File: LICENSE
+License-File: AUTHORS
+
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
 <a href="https://github.com/modin-project/unidist/actions"><img src="https://github.com/modin-project/unidist/workflows/master/badge.svg" align="center"></a>
@@ -9,102 +24,114 @@
 <a href="https://pypi.org/project/unidist/"><img src="https://badge.fury.io/py/unidist.svg" alt="PyPI version" align="center"></a>
 </p>
 
 ### What is unidist?
 
 unidist is a framework that is intended to provide the unified API for distributed execution by supporting various performant execution backends. At the moment the following backends are supported under the hood:
 
-* [Ray](https://docs.ray.io/en/master/index.html)
 * [MPI](https://www.mpi-forum.org/)
 * [Dask Distributed](https://distributed.dask.org/en/latest/)
+* [Ray](https://docs.ray.io/en/master/index.html)
 * [Python Multiprocessing](https://docs.python.org/3/library/multiprocessing.html)
 
 unidist is designed to work in a [task-based parallel](https://en.wikipedia.org/wiki/Task_parallelism) model.
 
-Also, the framework provides a sequential ``Python`` backend, that can be used for debugging.
+Also, the framework provides a Python Sequential backend (`pyseq`), that can be used for debugging.
 
 ### Installation
 
-#### From PyPI
+#### Using pip
 
 unidist can be installed with `pip` on Linux, Windows and MacOS:
 
 ```bash
 pip install unidist # Install unidist with dependencies for Python Multiprocessing and Python Sequential backends
 ```
 
-unidist can also be used with Dask, MPI or Ray execution backend.
-If you don't have Dask, MPI or Ray installed, you will need to install unidist with one of the targets:
+unidist can also be used with MPI, Dask or Ray execution backend.
+If you don't have MPI, Dask or Ray installed, you will need to install unidist with one of the targets:
 
 ```bash
 pip install unidist[all] # Install unidist with dependencies for all the backends
-pip install unidist[dask] # Install unidist with dependencies for Dask backend
 pip install unidist[mpi] # Install unidist with dependencies for MPI backend
+pip install unidist[dask] # Install unidist with dependencies for Dask backend
 pip install unidist[ray] # Install unidist with dependencies for Ray backend
 ```
 
 unidist automatically detects which execution backends are installed and uses that for scheduling computation.
 
-#### From conda-forge
+**Note:** There are different MPI implementations, each of which can be used as a backend in unidist.
+By default, mapping `unidist[mpi]` installs MPICH on Linux and MacOS and MSMPI on Windows. If you want to use
+a specific version of MPI, you can install the core dependencies of unidist as `pip install unidist` and then
+install the specific version of MPI using pip as shown in the [installation](https://mpi4py.readthedocs.io/en/latest/install.html)
+section of mpi4py documentation.
+
+#### Using conda
 
-For installing unidist with dependencies for Dask and MPI execution backends into a conda environment
+For installing unidist with dependencies for MPI and Dask execution backends into a conda environment
 the following command should be used:
 
 ```bash
-conda install unidist-dask unidist-mpi -c conda-forge
+conda install unidist-mpi unidist-dask -c conda-forge
 ```
 
 All set of backends could be available in a conda environment by specifying:
 
 ```bash
 conda install unidist-all -c conda-forge
 ```
 
 or explicitly:
 
 ```bash
-conda install unidist-dask unidist-mpi unidist-ray -c conda-forge
+conda install unidist-mpi unidist-dask unidist-ray -c conda-forge
 ```
 
+**Note:** There are different MPI implementations, each of which can be used as a backend in unidist.
+By default, mapping `unidist-mpi` installs MPICH on Linux and MacOS and MSMPI on Windows. If you want to use
+a specific version of MPI, you can install the core dependencies of unidist as `conda install unidist` and then
+install the specific version of MPI using conda as shown in the [installation](https://mpi4py.readthedocs.io/en/latest/install.html)
+section of mpi4py documentation. That said, it is highly encouraged to use your own MPI binaries as stated in the
+[Using External MPI Libraries](https://conda-forge.org/docs/user/tipsandtricks.html#using-external-message-passing-interface-mpi-libraries)
+section of the conda-forge documentation in order to get ultimate performance.
+
 For more information refer to [Installation](https://unidist.readthedocs.io/en/latest/installation.html) section.
 
 #### Choosing an execution backend
 
 If you want to choose a specific execution backend to run on,
 you can set the environment variable `UNIDIST_BACKEND` and unidist will do computation with that backend:
 
 ```bash
-export UNIDIST_BACKEND=ray  # unidist will use Ray
 export UNIDIST_BACKEND=mpi  # unidist will use MPI
 export UNIDIST_BACKEND=dask  # unidist will use Dask
+export UNIDIST_BACKEND=ray  # unidist will use Ray
 ```
 
 This can also be done within a notebook/interpreter before you initialize unidist:
 
 ```python
 from unidist.config import Backend
 
-Backend.put("ray")  # unidist will use Ray
 Backend.put("mpi")  # unidist will use MPI
 Backend.put("dask")  # unidist will use Dask
+Backend.put("ray")  # unidist will use Ray
 ```
 
-If you have installed all the execution backends and haven't specified any of the execution backends, Ray is used by default.
-
-Since some of the execution backends, particularly, MPI, have some specifics regarding running python programs, please
-refer to [Using Unidist](https://unidist.readthedocs.io/en/latest/using_unidist/index.html) section to get more information on
-setting the execution backend to run on.
+If you have installed all the execution backends and haven't specified any of the execution backends, MPI is used by default.
+Currently, almost all MPI implementations require ``mpiexec`` command to be used when running an MPI program.
+If you use a backend other than MPI, you run a program as a regular python script (see below).
 
 #### Usage
 
 ```python
 # script.py
 
 import unidist
-unidist.init() # Ray backend is used by default
+unidist.init() # MPI backend is used by default
 
 @unidist.remote
 def foo(x):
     return x * x
 
 # This will run `foo` on a pool of workers in parallel;
 # `refs` will contain object references to actual data
@@ -112,16 +139,17 @@
 # To get the data call `unidist.get(...)`
 print(unidist.get(refs))
 ```
 
 Run the `script.py` with:
 
 ```bash
-$ python script.py
-[0, 1, 4, 9, 16] # output
+$ mpiexec -n 1 python script.py  # for MPI backend
+# $ python script.py  # for any other supported backend
+[0, 1, 4, 9, 16]  # output
 ```
 
 For more examples refer to [Getting Started](https://unidist.readthedocs.io/en/latest/getting_started.html) section
 in our documentation.
 
 ### Powered by unidist
```

### Comparing `unidist-0.3.0/setup.py` & `unidist-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pathlib
 from setuptools import setup, find_packages
 import sys
 import versioneer
 
-ray_deps = ["ray[default]>=1.13.0"]
+# https://github.com/modin-project/unidist/issues/324
+ray_deps = ["ray[default]>=1.13.0", "pydantic<2"]
 dask_deps = ["dask[complete]>=2.22.0", "distributed>=2.22.0"]
 mpi_deps = ["mpi4py-mpich", "msgpack>=1.0.0"]
 if sys.version_info[1] < 8:
     mpi_deps += "pickle5"
 all_deps = ray_deps + dask_deps + mpi_deps
 
 here = pathlib.Path(__file__).parent.resolve()
```

### Comparing `unidist-0.3.0/unidist/__init__.py` & `unidist-0.4.0/unidist/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/api.py` & `unidist-0.4.0/unidist/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     """
     Initialize an execution backend.
 
     Notes
     -----
     The concrete execution backend can be set via
     `UNIDIST_BACKEND` environment variable or ``Backend`` config value.
-    Ray backend is used by default.
+    MPI backend is used by default.
     """
     init_backend()
 
 
 def is_initialized():
     """
     Check if a unidist backend has already been initialized.
```

### Comparing `unidist-0.3.0/unidist/config/__init__.py` & `unidist-0.4.0/unidist/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,21 @@
     RayGpuCount,
     IsRayCluster,
     RayRedisAddress,
     RayRedisPassword,
     RayObjectStoreMemory,
 )
 from .backends.dask import DaskMemoryLimit, IsDaskCluster, DaskSchedulerAddress
-from .backends.mpi import IsMpiSpawnWorkers, MpiHosts, MpiPickleThreshold
+from .backends.mpi import (
+    IsMpiSpawnWorkers,
+    MpiHosts,
+    MpiPickleThreshold,
+    MpiBackoff,
+    MpiLog,
+)
 from .parameter import ValueSource
 
 __all__ = [
     "Backend",
     "CpuCount",
     "RayGpuCount",
     "IsRayCluster",
@@ -27,8 +33,10 @@
     "DaskMemoryLimit",
     "IsDaskCluster",
     "DaskSchedulerAddress",
     "IsMpiSpawnWorkers",
     "MpiHosts",
     "ValueSource",
     "MpiPickleThreshold",
+    "MpiBackoff",
+    "MpiLog",
 ]
```

### Comparing `unidist-0.3.0/unidist/config/backends/common/envvars.py` & `unidist-0.4.0/unidist/config/backends/common/envvars.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,24 @@
         Get default value of the config.
 
         Returns
         -------
         str
         """
         try:
+            import mpi4py
+        except ImportError:
+            pass
+        else:
+            if version.parse(mpi4py.__version__) < version.parse("3.0.3"):
+                raise ImportError(
+                    "Please `pip install unidist[mpi]` to install compatible MPI version."
+                )
+            return BackendName.MPI
+        try:
             import ray
 
         except ImportError:
             pass
         else:
             if version.parse(ray.__version__) < version.parse("1.4.0"):
                 raise ImportError(
@@ -52,24 +62,15 @@
             if version.parse(dask.__version__) < version.parse(
                 "2.22.0"
             ) or version.parse(distributed.__version__) < version.parse("2.22.0"):
                 raise ImportError(
                     "Please `pip install unidist[dask]` to install compatible Dask version."
                 )
             return BackendName.DASK
-        try:
-            import mpi4py
-        except ImportError:
-            pass
-        else:
-            if version.parse(mpi4py.__version__) < version.parse("3.0.3"):
-                raise ImportError(
-                    "Please `pip install unidist[mpi]` to install compatible MPI version."
-                )
-            return BackendName.MPI
+
         return BackendName.PYMP
 
 
 class CpuCount(EnvironmentVariable, type=int):
     """How many CPU cores to use during initialization of the unidist backend."""
 
     varname = "UNIDIST_CPUS"
```

### Comparing `unidist-0.3.0/unidist/config/backends/dask/envvars.py` & `unidist-0.4.0/unidist/config/backends/dask/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/config/backends/ray/envvars.py` & `unidist-0.4.0/unidist/config/backends/ray/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/config/parameter.py` & `unidist-0.4.0/unidist/config/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,21 @@
     int: TypeDescriptor(
         decode=lambda value: int(value.strip()),
         normalize=int,
         verify=lambda value: isinstance(value, int)
         or (isinstance(value, str) and value.strip().isdigit()),
         help="an integer value",
     ),
+    float: TypeDescriptor(
+        decode=lambda value: float(value.strip()),
+        normalize=float,
+        verify=lambda value: isinstance(value, float)
+        or (isinstance(value, str) and value.strip().replace(".", "").isdigit()),
+        help="a float value",
+    ),
 }
 
 # Special marker to distinguish unset value from ``None`` value
 # as someone may want to use ``None`` as a real value for a parameter
 _UNSET = object()
```

### Comparing `unidist-0.3.0/unidist/core/backends/common/data_id.py` & `unidist-0.4.0/unidist/core/backends/common/data_id.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/common/utils.py` & `unidist-0.4.0/unidist/core/backends/common/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/dask/actor.py` & `unidist-0.4.0/unidist/core/backends/dask/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/dask/backend.py` & `unidist-0.4.0/unidist/core/backends/dask/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/dask/remote_function.py` & `unidist-0.4.0/unidist/core/backends/dask/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/dask/utils.py` & `unidist-0.4.0/unidist/core/backends/dask/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/actor.py` & `unidist-0.4.0/unidist/core/backends/mpi/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/backend.py` & `unidist-0.4.0/unidist/core/backends/mpi/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/async_operations.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/async_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,13 +57,12 @@
 
         # tup[0] - mpi async send handler object
         self._send_async_handlers[:] = [
             tup for tup in self._send_async_handlers if not is_ready(tup[0])
         ]
 
     def finish(self):
-        """Cancel all MPI async send requests."""
-        for handler, data in self._send_async_handlers:
+        """Finish all MPI async send requests."""
+        for handler, _ in self._send_async_handlers:
             logger.debug("WAIT ASYNC HANDLER {}".format(handler))
-            handler.Cancel()
             handler.Wait()
         self._send_async_handlers.clear()
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/common.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 """Common classes and utilities."""
 
 import logging
 import inspect
 
 from unidist.core.backends.common.data_id import DataID, is_data_id
+from unidist.config import MpiLog
 
 
 class Operation:
     """
     Class that describes supported operations.
 
     Attributes
     ----------
     EXECUTE : int, default 1
-        Execute remote task.
+        Execute a remote task.
     GET : int, default 2
         Return local data to a requester.
     PUT_DATA : int, default 3
         Save the data to a local storage.
     PUT_OWNER : int, default 4
         Save the data location to a local storage.
     WAIT : int, default 5
@@ -31,17 +32,22 @@
     ACTOR_EXECUTE : int, default 7
         Execute method of a local actor instance.
     CLEANUP : int, default 8
         Cleanup local object storage for out-of-scope IDs.
     TASK_DONE : int, default 9
         Increment global task counter.
     GET_TASK_COUNT : int, default 10
-        Exit event loop.
-    CANCEL : int, default 11
         Return global task counter to a requester.
+    CANCEL : int, default 11
+        Send a message to a worker to exit the event loop.
+    READY_TO_SHUTDOWN : int, default 12
+        Send a message to monitor from a worker,
+        which is ready to shutdown.
+    SHUTDOWN : int, default 13
+        Send a message from monitor to a worker to shutdown.
     """
 
     ### --- Master/worker operations --- ###
     EXECUTE = 1
     GET = 2
     PUT_DATA = 3
     PUT_OWNER = 4
@@ -50,14 +56,35 @@
     ACTOR_EXECUTE = 7
     CLEANUP = 8
     ### --- Monitor operations --- ###
     TASK_DONE = 9
     GET_TASK_COUNT = 10
     ### --- Common operations --- ###
     CANCEL = 11
+    READY_TO_SHUTDOWN = 12
+    SHUTDOWN = 13
+
+
+class MPITag:
+    """
+    Class that describes tags that are used internally for communications.
+
+    Attributes
+    ----------
+    OPERATION : int, default: 111
+        The tag for send/recv of an operation type.
+    OBJECT : int, default: 112
+        The tag for send/recv of a regular Python object.
+    BUFFER : int, default: 113
+        The tag for send/recv of a buffer-like object.
+    """
+
+    OPERATION = 111
+    OBJECT = 112
+    BUFFER = 113
 
 
 default_class_properties = dir(type("dummy", (object,), {}))
 # Mapping between operations and their names (e.g., Operation.EXECUTE: "EXECUTE")
 operations_dict = dict(
     (value, name)
     for name, value in inspect.getmembers(Operation)
@@ -129,39 +156,42 @@
         -------
         unidist.core.backends.common.data_id.DataID
             Base ``DataID`` class object without garbage collector reference.
         """
         return DataID(self._id)
 
 
-def get_logger(logger_name, file_name, activate=False):
+def get_logger(logger_name, file_name, activate=None):
     """
     Configure logger and get it's instance.
 
     Parameters
     ----------
     logger_name : str
         Name of a logger.
     file_name : str
         File name.
-    activate : bool
-        Write logs or not.
+    activate : optional, default: None
+        Whether to enable logging or not.
+        If ``None``, the value is superseded with ``MpiLog``.
 
     Returns
     -------
     object
         A Python logger object.
     """
     logger = logging.getLogger(logger_name)
     if not logger.hasHandlers():
         f_format = logging.Formatter("%(message)s")
         f_handler = logging.FileHandler(file_name, delay=True)
         f_handler.setFormatter(f_format)
         logger.addHandler(f_handler)
 
+    if activate is None:
+        activate = MpiLog.get()
     if activate:
         logger.setLevel(logging.DEBUG)
     else:
         logger.setLevel(logging.NOTSET)
 
     return logger
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/controller/__init__.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/controller/actor.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/controller/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/controller/api.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/controller/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2021-2023 Modin authors
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """High-level API of MPI backend."""
 
+import os
 import sys
 import atexit
 import signal
 import asyncio
 from collections import defaultdict
 
 try:
@@ -31,28 +32,84 @@
 from unidist.core.backends.mpi.core.async_operations import AsyncOperations
 from unidist.config import (
     CpuCount,
     IsMpiSpawnWorkers,
     MpiHosts,
     ValueSource,
     MpiPickleThreshold,
+    MpiBackoff,
+    MpiLog,
 )
 
 
 # TODO: Find a way to move this after all imports
 mpi4py.rc(recv_mprobe=False, initialize=False)
 from mpi4py import MPI  # noqa: E402
 
 
 logger = common.get_logger("api", "api.log")
 
 # The topology of MPI cluster gets available when MPI initialization in `init`
 topology = dict()
 # The global variable is responsible for if MPI backend has already been initialized
 is_mpi_initialized = False
+# The global variable is responsible for if MPI backend has already been shutdown
+is_mpi_shutdown = False
+
+# This should be in line with https://docs.python.org/3/library/sys.html#sys.flags
+_PY_FLAGS_MAP = {
+    "debug": "d",
+    "inspect": "i",
+    "interactive": "i",
+    "isolated": "I",
+    "optimize": "O",
+    "dont_write_bytecode": "B",
+    "no_user_site": "s",
+    "no_site": "S",
+    "ignore_environment": "E",
+    "verbose": "v",
+    "bytes_warning": "b",
+    "quiet": "q",
+    "hash_randomization": "R",
+    "safe_path": "P",
+    # The flags below are handled separately using sys._xoptions.
+    # See more in https://docs.python.org/3/library/sys.html#sys._xoptions
+    # 'dev_mode': 'Xdev',
+    # 'utf8_mode': 'Xutf8',
+    # 'int_max_str_digits': 'Xint_max_str_digits',
+}
+
+
+def _get_py_flags():
+    """
+    Get a list of the flags passed in to python.
+
+    Returns
+    -------
+    list
+
+    Notes
+    -----
+    This function is used to get the python flags
+    in order to pass them to the workers initialization.
+    """
+    args = []
+    for flag, opt in _PY_FLAGS_MAP.items():
+        val = getattr(sys.flags, flag, 0)
+        # We do not want workers to get into interactive mode
+        # so the value should be 0
+        val = val if opt[0] != "i" else 0
+        if val > 0:
+            args.append("-" + opt * val)
+    for opt in sys.warnoptions:
+        args.append("-W" + opt)
+    sys_xoptions = getattr(sys, "_xoptions", {})
+    for opt, val in sys_xoptions.items():
+        args.append("-X" + opt if val is True else "-X" + opt + "=" + val)
+    return args
 
 
 def init():
     """
     Initialize MPI processes.
 
     Notes
@@ -80,36 +137,64 @@
 
     parent_comm = MPI.Comm.Get_parent()
 
     # path to dynamically spawn MPI processes
     if rank == 0 and parent_comm == MPI.COMM_NULL:
         if IsMpiSpawnWorkers.get():
             nprocs_to_spawn = CpuCount.get() + 1  # +1 for monitor process
-            args = ["-c"]
+            args = _get_py_flags()
+            args += ["-c"]
             py_str = [
                 "import unidist",
                 "import unidist.config as cfg",
                 "cfg.Backend.put('mpi')",
             ]
             if IsMpiSpawnWorkers.get_value_source() != ValueSource.DEFAULT:
                 py_str += [f"cfg.IsMpiSpawnWorkers.put({IsMpiSpawnWorkers.get()})"]
             if MpiHosts.get_value_source() != ValueSource.DEFAULT:
                 py_str += [f"cfg.MpiHosts.put('{MpiHosts.get()}')"]
             if CpuCount.get_value_source() != ValueSource.DEFAULT:
                 py_str += [f"cfg.CpuCount.put({CpuCount.get()})"]
             if MpiPickleThreshold.get_value_source() != ValueSource.DEFAULT:
                 py_str += [f"cfg.MpiPickleThreshold.put({MpiPickleThreshold.get()})"]
+            if MpiBackoff.get_value_source() != ValueSource.DEFAULT:
+                py_str += [f"cfg.MpiBackoff.put({MpiBackoff.get()})"]
+            if MpiLog.get_value_source() != ValueSource.DEFAULT:
+                py_str += [f"cfg.MpiLog.put({MpiLog.get()})"]
             py_str += ["unidist.init()"]
             py_str = "; ".join(py_str)
             args += [py_str]
 
             hosts = MpiHosts.get()
             info = MPI.Info.Create()
+            lib_version = MPI.Get_library_version()
+            if "Intel" in lib_version:
+                # To make dynamic spawn of MPI processes work properly
+                # we should set this environment variable.
+                # See more about Intel MPI environment variables in
+                # https://www.intel.com/content/www/us/en/docs/mpi-library/developer-reference-linux/2021-8/other-environment-variables.html.
+                os.environ["I_MPI_SPAWN"] = "1"
+
             if hosts:
-                info.Set("hosts", hosts)
+                if "Open MPI" in lib_version:
+                    host_list = str(hosts).split(",")
+                    workers_per_host = [
+                        int(nprocs_to_spawn / len(host_list))
+                        + (1 if i < nprocs_to_spawn % len(host_list) else 0)
+                        for i in range(len(host_list))
+                    ]
+                    hosts = ",".join(
+                        [
+                            f"{host}:{workers_per_host[i]}"
+                            for i, host in enumerate(host_list)
+                        ]
+                    )
+                    info.Set("add-host", hosts)
+                else:
+                    info.Set("hosts", hosts)
 
             intercomm = MPI.COMM_SELF.Spawn(
                 sys.executable,
                 args,
                 maxprocs=nprocs_to_spawn,
                 info=info,
                 root=rank,
@@ -141,23 +226,33 @@
         signal.signal(signal.SIGINT, _termination_handler)
         return
 
     if mpi_state.rank == communication.MPIRank.MONITOR:
         from unidist.core.backends.mpi.core.monitor import monitor_loop
 
         monitor_loop()
+        # If the user executes a program in SPMD mode,
+        # we do not want workers to continue the flow after `unidist.init()`
+        # so just killing them.
+        if not IsMpiSpawnWorkers.get():
+            sys.exit()
         return
 
     if mpi_state.rank not in (
         communication.MPIRank.ROOT,
         communication.MPIRank.MONITOR,
     ):
         from unidist.core.backends.mpi.core.worker.loop import worker_loop
 
         asyncio.run(worker_loop())
+        # If the user executes a program in SPMD mode,
+        # we do not want workers to continue the flow after `unidist.init()`
+        # so just killing them.
+        if not IsMpiSpawnWorkers.get():
+            sys.exit()
         return
 
 
 def is_initialized():
     """
     Check if MPI backend has already been initialized.
 
@@ -175,25 +270,40 @@
     """
     Shutdown all MPI processes.
 
     Notes
     -----
     Sends cancelation operation to all workers and monitor processes.
     """
-    mpi_state = communication.MPIState.get_instance()
-    # Send shutdown commands to all ranks
-    for rank_id in range(communication.MPIRank.MONITOR, mpi_state.world_size):
-        # We use a blocking send here because we have to wait for
-        # completion of the communication, which is necessary for the pipeline to continue.
-        communication.mpi_send_object(mpi_state.comm, common.Operation.CANCEL, rank_id)
-        logger.debug("Shutdown rank {}".format(rank_id))
-    async_operations = AsyncOperations.get_instance()
-    async_operations.finish()
-    if not MPI.Is_finalized():
-        MPI.Finalize()
+    global is_mpi_shutdown
+    if not is_mpi_shutdown:
+        async_operations = AsyncOperations.get_instance()
+        async_operations.finish()
+        mpi_state = communication.MPIState.get_instance()
+        # Send shutdown commands to all ranks
+        for rank_id in range(communication.MPIRank.FIRST_WORKER, mpi_state.world_size):
+            # We use a blocking send here because we have to wait for
+            # completion of the communication, which is necessary for the pipeline to continue.
+            communication.mpi_send_operation(
+                mpi_state.comm,
+                common.Operation.CANCEL,
+                rank_id,
+            )
+            logger.debug("Shutdown rank {}".format(rank_id))
+        # Make sure that monitor has sent the shutdown signal to all workers.
+        op_type = communication.mpi_recv_object(
+            mpi_state.comm,
+            communication.MPIRank.MONITOR,
+        )
+        if op_type != common.Operation.SHUTDOWN:
+            raise ValueError(f"Got wrong operation type {op_type}.")
+        if not MPI.Is_finalized():
+            MPI.Finalize()
+        logger.debug("Shutdown root")
+        is_mpi_shutdown = True
 
 
 def cluster_resources():
     """
     Get resources of MPI cluster.
 
     Returns
@@ -292,49 +402,58 @@
         The number of ``DataID``-s that should be returned as ready.
 
     Returns
     -------
     tuple
         List of data IDs that are ready and list of the remaining data IDs.
     """
-    mpi_state = communication.MPIState.get_instance()
-
-    def wait_impl(data_id):
-        if object_store.contains(data_id):
-            return
-
-        owner_rank = object_store.get_data_owner(data_id)
-
-        operation_type = common.Operation.WAIT
-        operation_data = {"id": data_id.base_data_id()}
-        # We use a blocking send here because we have to wait for
-        # completion of the communication, which is necessary for the pipeline to continue.
-        communication.send_simple_operation(
-            mpi_state.comm,
-            operation_type,
-            operation_data,
-            owner_rank,
-        )
-
-        logger.debug("WAIT {} id from {} rank".format(data_id._id, owner_rank))
-
-        communication.mpi_busy_wait_recv(mpi_state.comm, owner_rank)
-
-    logger.debug("WAIT {} ids".format(common.unwrapped_data_ids_list(data_ids)))
-
     if not isinstance(data_ids, list):
         data_ids = [data_ids]
-
-    ready = []
+    # Since the controller should operate MasterDataID(s),
+    # we use this map to retrieve and return them
+    # instead of DataID(s) received from workers.
+    data_id_map = dict(zip(data_ids, data_ids))
     not_ready = data_ids
+    pending_returns = num_returns
+    ready = []
 
-    while len(ready) != num_returns:
-        first = not_ready.pop(0)
-        wait_impl(first)
-        ready.append(first)
+    logger.debug("WAIT {} ids".format(common.unwrapped_data_ids_list(data_ids)))
+    for data_id in not_ready:
+        if object_store.contains(data_id):
+            ready.append(data_id)
+            not_ready.remove(data_id)
+            pending_returns -= 1
+            if len(ready) == num_returns:
+                return ready, not_ready
+
+    operation_type = common.Operation.WAIT
+    not_ready = [common.unwrap_data_ids(arg) for arg in not_ready]
+    operation_data = {
+        "data_ids": not_ready,
+        "num_returns": pending_returns,
+    }
+    mpi_state = communication.MPIState.get_instance()
+    # We use a blocking send and recv here because we have to wait for
+    # completion of the communication, which is necessary for the pipeline to continue.
+    communication.send_simple_operation(
+        mpi_state.comm,
+        operation_type,
+        operation_data,
+        communication.MPIRank.MONITOR,
+    )
+    data = communication.mpi_recv_object(
+        mpi_state.comm,
+        communication.MPIRank.MONITOR,
+    )
+    ready.extend(data["ready"])
+    not_ready = data["not_ready"]
+    # We have to retrieve and return MasterDataID(s)
+    # in order for the controller to operate them in further operations.
+    ready = [data_id_map[data_id] for data_id in ready]
+    not_ready = [data_id_map[data_id] for data_id in not_ready]
 
     # Initiate reference count based cleaup
     # if all the tasks were completed
     garbage_collector.regular_cleanup()
 
     return ready, not_ready
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/controller/common.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/controller/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/controller/garbage_collector.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/controller/garbage_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,20 +118,20 @@
                 if (timestamp_snapshot - self._timestamp) > self._time_threshold:
                     logger.debug("Cleanup counter {}".format(self._cleanup_counter))
 
                     mpi_state = communication.MPIState.get_instance()
                     # Compare submitted and executed tasks
                     # We use a blocking send here because we have to wait for
                     # completion of the communication, which is necessary for the pipeline to continue.
-                    communication.mpi_send_object(
+                    communication.mpi_send_operation(
                         mpi_state.comm,
                         common.Operation.GET_TASK_COUNT,
                         communication.MPIRank.MONITOR,
                     )
-                    executed_task_counter = communication.recv_simple_operation(
+                    executed_task_counter = communication.mpi_recv_object(
                         mpi_state.comm,
                         communication.MPIRank.MONITOR,
                     )
 
                     logger.debug(
                         "Submitted task count {} vs executed task count {}".format(
                             self._task_counter, executed_task_counter
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/controller/object_store.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/controller/object_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,18 +192,18 @@
         """
         if num_returns == 1:
             output_ids = self.generate_data_id(gc)
             self.put_data_owner(output_ids, dest_rank)
         elif num_returns == 0:
             output_ids = None
         else:
-            output_ids = []
-            for _ in range(num_returns):
+            output_ids = [None] * num_returns
+            for i in range(num_returns):
                 output_id = self.generate_data_id(gc)
-                output_ids.append(output_id)
+                output_ids[i] = output_id
                 self.put_data_owner(output_id, dest_rank)
         return output_ids
 
     def cache_send_info(self, data_id, rank):
         """
         Save communication event for this `data_id` and rank.
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/serialization.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 
 """Serialization interface"""
 
 import importlib
 import inspect
 import sys
 from collections.abc import KeysView
-from mpi4py.MPI import memory
+
+try:
+    import mpi4py
+except ImportError:
+    raise ImportError(
+        "Missing dependency 'mpi4py'. Use pip or conda to install it."
+    ) from None
 
 # Serialization libraries
 if sys.version_info[1] < 8:  # check the minor Python version
     try:
         import pickle5 as pkl
     except ImportError:
         raise ImportError(
@@ -22,14 +28,19 @@
     import pickle as pkl
 import cloudpickle as cpkl
 import msgpack
 import gc  # msgpack optimization
 
 from unidist.config import MpiPickleThreshold
 
+# TODO: Find a way to move this after all imports
+mpi4py.rc(recv_mprobe=False, initialize=False)
+from mpi4py.MPI import memory  # noqa: E402
+
+
 # Pickle 5 protocol compatible types check
 compatible_modules = ("pandas", "numpy")
 available_modules = []
 for module_name in compatible_modules:
     try:
         available_modules.append(importlib.import_module(module_name))
     except ModuleNotFoundError:
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/worker/object_store.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/worker/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/worker/request_store.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/worker/request_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Copyright (C) 2021-2023 Modin authors
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from collections import defaultdict
 
 import unidist.core.backends.mpi.core.common as common
 import unidist.core.backends.mpi.core.communication as communication
 from unidist.core.backends.mpi.core.async_operations import AsyncOperations
 from unidist.core.backends.mpi.core.worker.object_store import ObjectStore
 
@@ -15,34 +19,43 @@
 logger = common.get_logger(logger_name, log_file)
 
 
 class RequestStore:
     """
     Class that stores data requests that couldn't be satisfied now.
 
+    Attributes
+    ----------
+    GET : int, default 0
+        `Get` request from other worker to be executed.
+    WAIT : int, default 1
+        `Wait` request from other worker to be executed.
+    DATA : int, default 2
+        Data request to other worker.
+
     Notes
     -----
-    Supports GET and WAIT requests.
+    Supports `GET` and `WAIT` requests.
     """
 
     __instance = None
 
-    REQ_DATA = 0
-    REQ_WAIT = 1
-    REQ_DATA_CACHE = 2
+    GET = 0
+    WAIT = 1
+    DATA = 2
 
     def __init__(self):
-        # Data requests {DataId : [ Set of Ranks ]}
-        self._data_request = defaultdict(set)
-        # Blocking data requests {DataId : [ Set of Ranks ]}
-        self._blocking_data_request = defaultdict(set)
-        # Wait requests {DataId : Rank}
-        self._wait_request = {}
-        # Cache for already requested ids
-        self._data_request_cache = set()
+        # Non-blocking get requests {DataId : [ Set of Ranks ]}
+        self._nonblocking_get_requests = defaultdict(set)
+        # Blocking get requests {DataId : [ Set of Ranks ]}
+        self._blocking_get_requests = defaultdict(set)
+        # Blocking wait requests {DataId : Rank}
+        self._blocking_wait_requests = {}
+        # Data requests
+        self._data_requests = set()
 
     @classmethod
     def get_instance(cls):
         """
         Get instance of ``RequestStore``.
 
         Returns
@@ -66,52 +79,61 @@
         request_type : int
             Type of request.
         is_blocking_op : bool
             Whether the get request should be blocking or not.
             If ``True``, the request should be processed immediatly
             even for a worker since it can get into controller mode.
         """
-        if request_type == self.REQ_DATA:
+        if request_type == self.GET:
             if is_blocking_op:
-                self._blocking_data_request[data_id].add(rank)
+                self._blocking_get_requests[data_id].add(rank)
             else:
-                self._data_request[data_id].add(rank)
-        elif request_type == self.REQ_WAIT:
-            self._wait_request[data_id] = rank
-        elif request_type == self.REQ_DATA_CACHE:
-            self._data_request_cache.add(data_id)
+                self._nonblocking_get_requests[data_id].add(rank)
+        elif request_type == self.WAIT:
+            self._blocking_wait_requests[data_id] = rank
+        elif request_type == self.DATA:
+            self._data_requests.add(data_id)
         else:
             raise ValueError("Unsupported request type option!")
 
-    def is_already_requested(self, data_id):
+    def is_data_already_requested(self, data_id):
         """
-        Check if particular `data_id` was already requested from another MPI process.
+        Check if data by particular `data_id` was already requested from another MPI process.
 
         Parameters
         ----------
         data_id : unidist.core.backends.common.data_id.DataID
             An ID to data.
 
         Returns
         -------
         bool
             ``True`` if communnication request was happened for this ID.
         """
-        return data_id in self._data_request_cache
+        return data_id in self._data_requests
 
-    def clear_cache(self, data_id):
+    def discard_data_request(self, data_id):
         """
-        Clear internal cache for happened communication requests.
+        Discard data request by `data_id` because the data has become available.
 
         Parameters
         ----------
         data_id : unidist.core.backends.common.data_id.DataID
             An ID to data.
         """
-        self._data_request_cache.discard(data_id)
+        self._data_requests.discard(data_id)
+
+    def clear_get_requests(self):
+        """Clear blocking and non-blocking get requests."""
+        self._blocking_get_requests.clear()
+        self._nonblocking_get_requests.clear()
+
+    def clear_wait_requests(self):
+        """Clear blocking wait requests requests."""
+        self._blocking_wait_requests.clear()
 
     def check_pending_get_requests(self, data_ids):
         """
         Check if `GET` event on this `data_ids` is waiting to be processed.
 
         Process the request if data ID available in local object store.
 
@@ -119,27 +141,27 @@
         ----------
         data_id : iterable or unidist.core.backends.common.data_id.DataID
             An ID or list of IDs to data.
         """
 
         def check_request(data_id):
             # Check non-blocking data requests for one of the workers
-            if data_id in self._data_request:
-                ranks_with_get_request = self._data_request[data_id]
+            if data_id in self._nonblocking_get_requests:
+                ranks_with_get_request = self._nonblocking_get_requests[data_id]
                 for rank_num in ranks_with_get_request:
                     # Data is already in DataMap, so not problem here
                     self.process_get_request(rank_num, data_id, is_blocking_op=False)
-                del self._data_request[data_id]
+                del self._nonblocking_get_requests[data_id]
             # Check blocking data requests for other of the workers
-            if data_id in self._blocking_data_request:
-                ranks_with_get_request = self._blocking_data_request[data_id]
+            if data_id in self._blocking_get_requests:
+                ranks_with_get_request = self._blocking_get_requests[data_id]
                 for rank_num in ranks_with_get_request:
                     # Data is already in DataMap, so not problem here
                     self.process_get_request(rank_num, data_id, is_blocking_op=True)
-                del self._blocking_data_request[data_id]
+                del self._blocking_get_requests[data_id]
 
         if isinstance(data_ids, (list, tuple)):
             for data_id in data_ids:
                 check_request(data_id)
         else:
             check_request(data_ids)
 
@@ -153,32 +175,32 @@
         Parameters
         ----------
         data_id : iterable or unidist.core.backends.common.data_id.DataID
             An ID or list of IDs to data.
         """
         if isinstance(data_ids, (list, tuple)):
             for data_id in data_ids:
-                if data_id in self._wait_request:
+                if data_id in self._blocking_wait_requests:
                     # Data is already in DataMap, so not problem here.
                     # We use a blocking send here because the receiver is waiting for the result.
                     communication.mpi_send_object(
                         communication.MPIState.get_instance().comm,
                         data_id,
                         communication.MPIRank.ROOT,
                     )
-                    del self._wait_request[data_id]
+                    del self._blocking_wait_requests[data_id]
         else:
-            if data_ids in self._wait_request:
+            if data_ids in self._blocking_wait_requests:
                 # We use a blocking send here because the receiver is waiting for the result.
                 communication.mpi_send_object(
                     communication.MPIState.get_instance().comm,
                     data_ids,
                     communication.MPIRank.ROOT,
                 )
-                del self._wait_request[data_ids]
+                del self._blocking_wait_requests[data_ids]
 
     def process_wait_request(self, data_id):
         """
         Satisfy WAIT operation request from another process.
 
         Save request for later processing if `data_id` is not available currently.
 
@@ -197,15 +219,15 @@
             communication.mpi_send_object(
                 communication.MPIState.get_instance().comm,
                 data_id,
                 communication.MPIRank.ROOT,
             )
             logger.debug("Wait data {} id is ready".format(data_id._id))
         else:
-            self.put(data_id, communication.MPIRank.ROOT, self.REQ_WAIT)
+            self.put(data_id, communication.MPIRank.ROOT, self.WAIT)
             logger.debug("Pending wait request {} id".format(data_id._id))
 
     def process_get_request(self, source_rank, data_id, is_blocking_op=False):
         """
         Satisfy GET operation request from another process.
 
         Save request for later processing if `data_id` is not available currently.
@@ -272,8 +294,8 @@
                     data_id._id, source_rank
                 )
             )
         else:
             logger.debug(
                 "Pending request {} id to {} rank".format(data_id._id, source_rank)
             )
-            self.put(data_id, source_rank, self.REQ_DATA, is_blocking_op=is_blocking_op)
+            self.put(data_id, source_rank, self.GET, is_blocking_op=is_blocking_op)
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/core/worker/task_store.py` & `unidist-0.4.0/unidist/core/backends/mpi/core/worker/task_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -89,14 +89,22 @@
             updated_list = []
             for request in self._pending_tasks_list:
                 pending_request = self.process_task_request(request)
                 if pending_request:
                     updated_list.append(pending_request)
             self._pending_tasks_list = updated_list
 
+    def clear_pending_tasks(self):
+        """
+        Clear a list of pending task execution requests.
+        """
+        w_logger.debug("Clear pending tasks")
+
+        self._pending_tasks_list.clear()
+
     def check_pending_actor_tasks(self):
         """
         Check a list of pending actor task execution requests and process all ready tasks.
 
         Task is ready if all data dependencies are resolved.
         """
         w_logger.debug("Check pending actor tasks")
@@ -105,14 +113,22 @@
             updated_list = []
             for request in self._pending_actor_tasks_list:
                 pending_request = self.process_task_request(request)
                 if pending_request:
                     updated_list.append(pending_request)
             self._pending_actor_tasks_list = updated_list
 
+    def clear_pending_actor_tasks(self):
+        """
+        Clear a list of pending actor task execution requests.
+        """
+        w_logger.debug("Clear pending actor tasks")
+
+        self._pending_actor_tasks_list.clear()
+
     def request_worker_data(self, dest_rank, data_id):
         """
         Send GET operation with data request to destination worker.
 
         Parameters
         ----------
         dest_rank : int
@@ -140,15 +156,15 @@
             operation_type,
             operation_data,
             dest_rank,
         )
         async_operations.extend(h_list)
 
         # Save request in order to prevent massive communication during pending task checks
-        RequestStore.get_instance().put(data_id, dest_rank, RequestStore.REQ_DATA_CACHE)
+        RequestStore.get_instance().put(data_id, dest_rank, RequestStore.DATA)
 
     def unwrap_local_data_id(self, arg):
         """
         Inspect argument and get the ID associated data from the local object store if available.
 
         If the object store is missing this data ID, request the data from another worker.
 
@@ -171,15 +187,15 @@
             object_store = ObjectStore.get_instance()
             arg = object_store.get_unique_data_id(arg)
             if object_store.contains(arg):
                 value = ObjectStore.get_instance().get(arg)
                 # Data is already local or was pushed from master
                 return value, False
             elif object_store.contains_data_owner(arg):
-                if not RequestStore.get_instance().is_already_requested(arg):
+                if not RequestStore.get_instance().is_data_already_requested(arg):
                     # Request the data from an owner worker
                     owner_rank = object_store.get_data_owner(arg)
                     if owner_rank != communication.MPIState.get_instance().rank:
                         self.request_worker_data(owner_rank, arg)
                 return arg, True
             else:
                 raise ValueError("DataID is missing!")
@@ -202,14 +218,15 @@
             Keyword arguments to be passed in the `task`.
 
         Notes
         -----
         Exceptions are stored in output data IDs as value.
         """
         object_store = ObjectStore.get_instance()
+        completed_data_ids = []
         if inspect.iscoroutinefunction(task):
 
             async def execute():
                 try:
                     w_logger.debug("- Start task execution -")
 
                     for arg in args:
@@ -245,30 +262,34 @@
                         object_store.put(data_id, e)
                 else:
                     if output_data_ids is not None:
                         if (
                             isinstance(output_data_ids, (list, tuple))
                             and len(output_data_ids) > 1
                         ):
-                            for output_id, value in zip(output_data_ids, output_values):
+                            completed_data_ids = [None] * len(output_data_ids)
+                            for idx, (output_id, value) in enumerate(
+                                zip(output_data_ids, output_values)
+                            ):
                                 data_id = object_store.get_unique_data_id(output_id)
                                 object_store.put(data_id, value)
+                                completed_data_ids[idx] = data_id
                         else:
                             data_id = object_store.get_unique_data_id(output_data_ids)
                             object_store.put(data_id, output_values)
+                            completed_data_ids = [data_id]
 
-                        RequestStore.get_instance().check_pending_get_requests(
-                            output_data_ids
-                        )
+                RequestStore.get_instance().check_pending_get_requests(output_data_ids)
                 # Monitor the task execution
                 # We use a blocking send here because we have to wait for
                 # completion of the communication, which is necessary for the pipeline to continue.
-                communication.mpi_send_object(
+                communication.send_simple_operation(
                     communication.MPIState.get_instance().comm,
                     common.Operation.TASK_DONE,
+                    completed_data_ids,
                     communication.MPIRank.MONITOR,
                 )
 
             async_task = asyncio.create_task(execute())
             # Add task to the set. This creates a strong reference.
             self.background_tasks.add(async_task)
             # To prevent keeping references to finished tasks forever,
@@ -311,26 +332,33 @@
                     object_store.put(data_id, e)
             else:
                 if output_data_ids is not None:
                     if (
                         isinstance(output_data_ids, (list, tuple))
                         and len(output_data_ids) > 1
                     ):
-                        for output_id, value in zip(output_data_ids, output_values):
+                        completed_data_ids = [None] * len(output_data_ids)
+                        for idx, (output_id, value) in enumerate(
+                            zip(output_data_ids, output_values)
+                        ):
                             data_id = object_store.get_unique_data_id(output_id)
                             object_store.put(data_id, value)
+                            completed_data_ids[idx] = data_id
                     else:
                         data_id = object_store.get_unique_data_id(output_data_ids)
                         object_store.put(data_id, output_values)
+                        completed_data_ids = [data_id]
+            RequestStore.get_instance().check_pending_get_requests(output_data_ids)
             # Monitor the task execution.
             # We use a blocking send here because we have to wait for
             # completion of the communication, which is necessary for the pipeline to continue.
-            communication.mpi_send_object(
+            communication.send_simple_operation(
                 communication.MPIState.get_instance().comm,
                 common.Operation.TASK_DONE,
+                completed_data_ids,
                 communication.MPIRank.MONITOR,
             )
 
     def process_task_request(self, request):
         """
         Parse request data and execute the task if possible.
 
@@ -348,16 +376,20 @@
         """
         # Parse request
         task = request["task"]
         args = request["args"]
         kwargs = request["kwargs"]
         output_ids = request["output"]
 
+        w_logger.debug("REMOTE task: {}".format(task))
         w_logger.debug("REMOTE args: {}".format(common.unwrapped_data_ids_list(args)))
         w_logger.debug(
+            "REMOTE kwargs: {}".format(common.unwrapped_data_ids_list(kwargs))
+        )
+        w_logger.debug(
             "REMOTE outputs: {}".format(common.unwrapped_data_ids_list(output_ids))
         )
 
         # DataID -> real data
         args, is_pending = common.materialize_data_ids(args, self.unwrap_local_data_id)
         kwargs, is_kw_pending = common.materialize_data_ids(
             kwargs, self.unwrap_local_data_id
```

### Comparing `unidist-0.3.0/unidist/core/backends/mpi/remote_function.py` & `unidist-0.4.0/unidist/core/backends/mpi/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/actor.py` & `unidist-0.4.0/unidist/core/backends/pymp/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/backend.py` & `unidist-0.4.0/unidist/core/backends/pymp/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/core/actor.py` & `unidist-0.4.0/unidist/core/backends/pymp/core/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/core/api.py` & `unidist-0.4.0/unidist/core/backends/pymp/core/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/core/object_store.py` & `unidist-0.4.0/unidist/core/backends/pymp/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/core/process_manager.py` & `unidist-0.4.0/unidist/core/backends/pymp/core/process_manager.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pymp/remote_function.py` & `unidist-0.4.0/unidist/core/backends/pymp/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pyseq/actor.py` & `unidist-0.4.0/unidist/core/backends/pyseq/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pyseq/backend.py` & `unidist-0.4.0/unidist/core/backends/pyseq/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pyseq/core/api.py` & `unidist-0.4.0/unidist/core/backends/pyseq/core/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pyseq/core/object_store.py` & `unidist-0.4.0/unidist/core/backends/pyseq/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/pyseq/remote_function.py` & `unidist-0.4.0/unidist/core/backends/pyseq/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/ray/actor.py` & `unidist-0.4.0/unidist/core/backends/ray/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/ray/backend.py` & `unidist-0.4.0/unidist/core/backends/ray/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/ray/remote_function.py` & `unidist-0.4.0/unidist/core/backends/ray/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/backends/ray/utils.py` & `unidist-0.4.0/unidist/core/backends/ray/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/base/actor.py` & `unidist-0.4.0/unidist/core/base/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/base/backend.py` & `unidist-0.4.0/unidist/core/base/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/base/common.py` & `unidist-0.4.0/unidist/core/base/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/base/remote_function.py` & `unidist-0.4.0/unidist/core/base/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/core/base/utils.py` & `unidist-0.4.0/unidist/core/base/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,39 +13,39 @@
     """
     Initialize an execution backend.
 
     Notes
     -----
     The concrete execution backend can be set via
     `UNIDIST_BACKEND` environment variable or ``Backend`` config value.
-    Ray backend is used by default.
+    MPI backend is used by default.
     """
     backend_name = Backend.get()
 
-    if backend_name == BackendName.RAY:
-        from unidist.core.backends.ray.backend import RayBackend
-        from unidist.core.backends.ray.utils import initialize_ray
+    if backend_name == BackendName.MPI:
+        from unidist.core.backends.mpi.backend import MPIBackend
+        from unidist.core.backends.mpi.utils import initialize_mpi
 
-        initialize_ray()
-        backend_cls = RayBackend()
+        initialize_mpi()
+        backend_cls = MPIBackend()
     elif backend_name == BackendName.DASK:
         import threading
 
         if threading.current_thread() is threading.main_thread():
             from unidist.core.backends.dask.backend import DaskBackend
             from unidist.core.backends.dask.utils import initialize_dask
 
             initialize_dask()
             backend_cls = DaskBackend()
-    elif backend_name == BackendName.MPI:
-        from unidist.core.backends.mpi.backend import MPIBackend
-        from unidist.core.backends.mpi.utils import initialize_mpi
+    elif backend_name == BackendName.RAY:
+        from unidist.core.backends.ray.backend import RayBackend
+        from unidist.core.backends.ray.utils import initialize_ray
 
-        initialize_mpi()
-        backend_cls = MPIBackend()
+        initialize_ray()
+        backend_cls = RayBackend()
     elif backend_name == BackendName.PYMP:
         from unidist.core.backends.pymp.backend import PyMpBackend
         from unidist.core.backends.pymp.utils import (
             initialize_pymp,
         )
 
         initialize_pymp()
@@ -71,26 +71,26 @@
     Backend
         The ``Backend`` instance that is considered as the proxy object.
     """
     backend = BackendProxy.get_instance()
 
     if backend is None:
         backend_name = Backend.get()
-        if backend_name == BackendName.RAY:
-            from unidist.core.backends.ray.backend import RayBackend
+        if backend_name == BackendName.MPI:
+            from unidist.core.backends.mpi.backend import MPIBackend
 
-            backend_cls = RayBackend()
+            backend_cls = MPIBackend()
         elif backend_name == BackendName.DASK:
             from unidist.core.backends.dask.backend import DaskBackend
 
             backend_cls = DaskBackend()
-        elif backend_name == BackendName.MPI:
-            from unidist.core.backends.mpi.backend import MPIBackend
+        elif backend_name == BackendName.RAY:
+            from unidist.core.backends.ray.backend import RayBackend
 
-            backend_cls = MPIBackend()
+            backend_cls = RayBackend()
         elif backend_name == BackendName.PYMP:
             from unidist.core.backends.pymp.backend import (
                 PyMpBackend,
             )
 
             backend_cls = PyMpBackend()
         elif backend_name == BackendName.PYSEQ:
```

### Comparing `unidist-0.3.0/unidist/test/test_actor.py` & `unidist-0.4.0/unidist/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/test/test_async_actor.py` & `unidist-0.4.0/unidist/test/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/test/test_general.py` & `unidist-0.4.0/unidist/test/test_general.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/test/test_task.py` & `unidist-0.4.0/unidist/test/test_task.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist/test/utils.py` & `unidist-0.4.0/unidist/test/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/unidist.egg-info/PKG-INFO` & `unidist-0.4.0/unidist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidist
-Version: 0.3.0
+Version: 0.4.0
 Summary: Unified Distributed Execution
 Home-page: https://github.com/modin-project/unidist
 License: Apache-2.0
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 Provides-Extra: dask
@@ -24,102 +24,114 @@
 <a href="https://pypi.org/project/unidist/"><img src="https://badge.fury.io/py/unidist.svg" alt="PyPI version" align="center"></a>
 </p>
 
 ### What is unidist?
 
 unidist is a framework that is intended to provide the unified API for distributed execution by supporting various performant execution backends. At the moment the following backends are supported under the hood:
 
-* [Ray](https://docs.ray.io/en/master/index.html)
 * [MPI](https://www.mpi-forum.org/)
 * [Dask Distributed](https://distributed.dask.org/en/latest/)
+* [Ray](https://docs.ray.io/en/master/index.html)
 * [Python Multiprocessing](https://docs.python.org/3/library/multiprocessing.html)
 
 unidist is designed to work in a [task-based parallel](https://en.wikipedia.org/wiki/Task_parallelism) model.
 
-Also, the framework provides a sequential ``Python`` backend, that can be used for debugging.
+Also, the framework provides a Python Sequential backend (`pyseq`), that can be used for debugging.
 
 ### Installation
 
-#### From PyPI
+#### Using pip
 
 unidist can be installed with `pip` on Linux, Windows and MacOS:
 
 ```bash
 pip install unidist # Install unidist with dependencies for Python Multiprocessing and Python Sequential backends
 ```
 
-unidist can also be used with Dask, MPI or Ray execution backend.
-If you don't have Dask, MPI or Ray installed, you will need to install unidist with one of the targets:
+unidist can also be used with MPI, Dask or Ray execution backend.
+If you don't have MPI, Dask or Ray installed, you will need to install unidist with one of the targets:
 
 ```bash
 pip install unidist[all] # Install unidist with dependencies for all the backends
-pip install unidist[dask] # Install unidist with dependencies for Dask backend
 pip install unidist[mpi] # Install unidist with dependencies for MPI backend
+pip install unidist[dask] # Install unidist with dependencies for Dask backend
 pip install unidist[ray] # Install unidist with dependencies for Ray backend
 ```
 
 unidist automatically detects which execution backends are installed and uses that for scheduling computation.
 
-#### From conda-forge
+**Note:** There are different MPI implementations, each of which can be used as a backend in unidist.
+By default, mapping `unidist[mpi]` installs MPICH on Linux and MacOS and MSMPI on Windows. If you want to use
+a specific version of MPI, you can install the core dependencies of unidist as `pip install unidist` and then
+install the specific version of MPI using pip as shown in the [installation](https://mpi4py.readthedocs.io/en/latest/install.html)
+section of mpi4py documentation.
+
+#### Using conda
 
-For installing unidist with dependencies for Dask and MPI execution backends into a conda environment
+For installing unidist with dependencies for MPI and Dask execution backends into a conda environment
 the following command should be used:
 
 ```bash
-conda install unidist-dask unidist-mpi -c conda-forge
+conda install unidist-mpi unidist-dask -c conda-forge
 ```
 
 All set of backends could be available in a conda environment by specifying:
 
 ```bash
 conda install unidist-all -c conda-forge
 ```
 
 or explicitly:
 
 ```bash
-conda install unidist-dask unidist-mpi unidist-ray -c conda-forge
+conda install unidist-mpi unidist-dask unidist-ray -c conda-forge
 ```
 
+**Note:** There are different MPI implementations, each of which can be used as a backend in unidist.
+By default, mapping `unidist-mpi` installs MPICH on Linux and MacOS and MSMPI on Windows. If you want to use
+a specific version of MPI, you can install the core dependencies of unidist as `conda install unidist` and then
+install the specific version of MPI using conda as shown in the [installation](https://mpi4py.readthedocs.io/en/latest/install.html)
+section of mpi4py documentation. That said, it is highly encouraged to use your own MPI binaries as stated in the
+[Using External MPI Libraries](https://conda-forge.org/docs/user/tipsandtricks.html#using-external-message-passing-interface-mpi-libraries)
+section of the conda-forge documentation in order to get ultimate performance.
+
 For more information refer to [Installation](https://unidist.readthedocs.io/en/latest/installation.html) section.
 
 #### Choosing an execution backend
 
 If you want to choose a specific execution backend to run on,
 you can set the environment variable `UNIDIST_BACKEND` and unidist will do computation with that backend:
 
 ```bash
-export UNIDIST_BACKEND=ray  # unidist will use Ray
 export UNIDIST_BACKEND=mpi  # unidist will use MPI
 export UNIDIST_BACKEND=dask  # unidist will use Dask
+export UNIDIST_BACKEND=ray  # unidist will use Ray
 ```
 
 This can also be done within a notebook/interpreter before you initialize unidist:
 
 ```python
 from unidist.config import Backend
 
-Backend.put("ray")  # unidist will use Ray
 Backend.put("mpi")  # unidist will use MPI
 Backend.put("dask")  # unidist will use Dask
+Backend.put("ray")  # unidist will use Ray
 ```
 
-If you have installed all the execution backends and haven't specified any of the execution backends, Ray is used by default.
-
-Since some of the execution backends, particularly, MPI, have some specifics regarding running python programs, please
-refer to [Using Unidist](https://unidist.readthedocs.io/en/latest/using_unidist/index.html) section to get more information on
-setting the execution backend to run on.
+If you have installed all the execution backends and haven't specified any of the execution backends, MPI is used by default.
+Currently, almost all MPI implementations require ``mpiexec`` command to be used when running an MPI program.
+If you use a backend other than MPI, you run a program as a regular python script (see below).
 
 #### Usage
 
 ```python
 # script.py
 
 import unidist
-unidist.init() # Ray backend is used by default
+unidist.init() # MPI backend is used by default
 
 @unidist.remote
 def foo(x):
     return x * x
 
 # This will run `foo` on a pool of workers in parallel;
 # `refs` will contain object references to actual data
@@ -127,16 +139,17 @@
 # To get the data call `unidist.get(...)`
 print(unidist.get(refs))
 ```
 
 Run the `script.py` with:
 
 ```bash
-$ python script.py
-[0, 1, 4, 9, 16] # output
+$ mpiexec -n 1 python script.py  # for MPI backend
+# $ python script.py  # for any other supported backend
+[0, 1, 4, 9, 16]  # output
 ```
 
 For more examples refer to [Getting Started](https://unidist.readthedocs.io/en/latest/getting_started.html) section
 in our documentation.
 
 ### Powered by unidist
```

### Comparing `unidist-0.3.0/unidist.egg-info/SOURCES.txt` & `unidist-0.4.0/unidist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unidist-0.3.0/versioneer.py` & `unidist-0.4.0/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/xoscar-0.0.7.tar.gz` & `tmp/xoscar-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoscar-0.0.7.tar", last modified: Thu Jun  8 10:20:48 2023, max compression
+gzip compressed data, was "xoscar-0.0.8.tar", last modified: Fri Jul  7 08:47:40 2023, max compression
```

## Comparing `xoscar-0.0.7.tar` & `xoscar-0.0.8.tar`

### file list

```diff
@@ -1,91 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-08 10:20:22.000000 xoscar-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-08 10:20:48.125736 xoscar-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-08 10:20:22.000000 xoscar-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-08 10:20:48.125736 xoscar-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-08 10:20:22.000000 xoscar-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-08 10:20:22.000000 xoscar-0.0.7/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.121736 xoscar-0.0.7/xoscar/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    23719 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.121736 xoscar-0.0.7/xoscar/aio/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/aio/_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/aio/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/aio/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/aio/lru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/aio/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.121736 xoscar-0.0.7/xoscar/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/allocate_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/backends/communication/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/ucx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/backends/indigen/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/indigen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/indigen/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/indigen/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/indigen/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/message.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    55798 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/backends/test/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/test/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/backends/test/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/context.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/context.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/core.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/core.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/libcpp.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/metrics/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/metrics/backends/console/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/backends/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/backends/console/console_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/backends/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/metrics/backends/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/backends/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/metrics/backends/prometheus/prometheus_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/nvutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.125736 xoscar-0.0.7/xoscar/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/core.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/core.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/serialization/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-06-08 10:20:22.000000 xoscar-0.0.7/xoscar/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:20:48.121736 xoscar-0.0.7/xoscar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-08 10:20:48.000000 xoscar-0.0.7/xoscar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 10:20:48.000000 xoscar-0.0.7/xoscar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:20:48.000000 xoscar-0.0.7/xoscar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:20:47.000000 xoscar-0.0.7/xoscar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 10:20:48.000000 xoscar-0.0.7/xoscar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 10:20:48.000000 xoscar-0.0.7/xoscar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 08:47:06.000000 xoscar-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-07 08:47:40.385716 xoscar-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-07 08:47:06.000000 xoscar-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-07 08:47:40.389716 xoscar-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-07 08:47:06.000000 xoscar-0.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-07 08:47:06.000000 xoscar-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.373715 xoscar-0.0.8/xoscar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    23719 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.377715 xoscar-0.0.8/xoscar/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/aio/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.377715 xoscar-0.0.8/xoscar/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/allocate_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/backends/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/backends/indigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/indigen/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/message.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    57991 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/backends/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/test/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/backends/test/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/collective/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/collective/rendezvous/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/rendezvous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/collective/rendezvous/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/rendezvous/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/collective/rendezvous/test/test_tcp_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/libcpp.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.381716 xoscar-0.0.8/xoscar/metrics/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/xoscar/metrics/backends/console/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/console/console_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/xoscar/metrics/backends/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/metrics/backends/prometheus/prometheus_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20412 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/nvutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.385716 xoscar-0.0.8/xoscar/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    29468 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/serialization/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-07-07 08:47:06.000000 xoscar-0.0.8/xoscar/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:47:40.373715 xoscar-0.0.8/xoscar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:47:39.000000 xoscar-0.0.8/xoscar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 08:47:40.000000 xoscar-0.0.8/xoscar.egg-info/top_level.txt
```

### Comparing `xoscar-0.0.7/PKG-INFO` & `xoscar-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xoscar
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python actor framework for heterogeneous computing.
-Home-page: http://github.com/xprobe-inc/xoscar
+Home-page: http://github.com/xorbitsai/xoscar
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -26,17 +26,17 @@
 
 <div align="center">
   <img width="77%" alt="" src="https://raw.githubusercontent.com/xprobe-inc/xoscar/main/doc/source/_static/Xoscar.svg"><br>
 </div>
 
 # Python actor framework for heterogeneous computing.
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xoscar.svg?style=for-the-badge)](https://pypi.org/project/xoscar/)
-[![Coverage](https://img.shields.io/codecov/c/github/xprobe-inc/xoscar?style=for-the-badge)](https://codecov.io/gh/xprobe-inc/xoscar)
-[![Build Status](https://img.shields.io/github/actions/workflow/status/xprobe-inc/xoscar/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xprobe-inc/xoscar/goto?ref=main)
-[![License](https://img.shields.io/pypi/l/xoscar.svg?style=for-the-badge)](https://github.com/xprobe-inc/xoscar/blob/main/LICENSE)
+[![Coverage](https://img.shields.io/codecov/c/github/xorbitsai/xoscar?style=for-the-badge)](https://codecov.io/gh/xorbitsai/xoscar)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/xoscar/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/xoscar/goto?ref=main)
+[![License](https://img.shields.io/pypi/l/xoscar.svg?style=for-the-badge)](https://github.com/xorbitsai/xoscar/blob/main/LICENSE)
 
 ## What is actor
 Writing parallel and distributed programs is often challenging and requires a lot of time to deal with concurrency
 issues. Actor model provides a high-level, scalable and robust abstraction for building distributed applications. 
 It provides several benefits:
 - Scalability: Actors easily scale across nodes. The asynchronous, non-blocking nature of actors allows them to handle huge volumes of concurrent tasks efficiently.
 - Concurrency: The actor model abstracts over concurrency, allowing developers to avoid raw threads and locks.
@@ -65,15 +65,15 @@
 appropriate pool based on the specified policy.
 
 When actors communicate, Xoscar will choose the optimal communication mechanism based on which pools the actors 
 belong to. This allows Xoscar to optimize communication in heterogeneous environments with multiple processing 
 units and accelerators.
 
 ## Where to get it
-The source code is currently hosted on GitHub at: https://github.com/xprobe-inc/xoscar
+The source code is currently hosted on GitHub at: https://github.com/xorbitsai/xoscar
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/xoscar).
 
 ```shell
 # PyPI
 pip install xoscar
```

### Comparing `xoscar-0.0.7/pyproject.toml` & `xoscar-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/setup.cfg` & `xoscar-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = xoscar
 description = Python actor framework for heterogeneous computing.
 author = Qin Xuye
 author_email = qinxuye@xprobe.io
 maintainer = Qin Xuye
 maintainer_email = qinxuye@xprobe.io
 license = Apache License 2.0
-url = http://github.com/xprobe-inc/xoscar
+url = http://github.com/xorbitsai/xoscar
 python_requires = >=3.8
 classifier = 
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `xoscar-0.0.7/versioneer.py` & `xoscar-0.0.8/versioneer.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/__init__.py` & `xoscar-0.0.8/xoscar/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from . import debug
 from .api import (
     actor_ref,
     create_actor,
     has_actor,
     destroy_actor,
     kill_actor,
+    buffer_ref,
+    file_object_ref,
+    copy_to,
     Actor,
     StatelessActor,
     create_actor_pool,
     setup_cluster,
     wait_actor_pool_recovered,
     get_pool_config,
 )
```

### Comparing `xoscar-0.0.7/xoscar/_utils.pxd` & `xoscar-0.0.8/xoscar/_utils.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/_utils.pyx` & `xoscar-0.0.8/xoscar/_utils.pyx`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/_version.py` & `xoscar-0.0.8/xoscar/_version.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/aio/__init__.py` & `xoscar-0.0.8/xoscar/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/aio/_threads.py` & `xoscar-0.0.8/xoscar/aio/_threads.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/aio/base.py` & `xoscar-0.0.8/xoscar/aio/base.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/aio/file.py` & `xoscar-0.0.8/xoscar/aio/file.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/aio/lru.py` & `xoscar-0.0.8/xoscar/aio/lru.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/aio/parallelism.py` & `xoscar-0.0.8/xoscar/aio/parallelism.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/api.py` & `xoscar-0.0.8/xoscar/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections import defaultdict
 from numbers import Number
-from typing import TYPE_CHECKING, Any, Dict, Tuple, Type
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, Union
 from urllib.parse import urlparse
 
+from .aio import AioFileObject
 from .backend import get_backend
 from .context import get_context
-from .core import ActorRef, _Actor, _StatelessActor
+from .core import ActorRef, BufferRef, FileObjectRef, _Actor, _StatelessActor
 
 if TYPE_CHECKING:
     from .backends.config import ActorPoolConfig
     from .backends.pool import MainActorPoolType
 
 
 async def create_actor(
@@ -101,15 +102,15 @@
     ActorRef
     """
     # TODO: refine the argument list for better user experience.
     ctx = get_context()
     return await ctx.actor_ref(*args, **kwargs)
 
 
-async def kill_actor(actor_ref):
+async def kill_actor(actor_ref: ActorRef):
     # TODO: explain the meaning of 'kill'
     """
     Forcefully kill an actor.
 
     It's important to note that this operation is potentially
     dangerous as it may result in the termination of other
     associated actors. Only proceed if you understand the
@@ -157,14 +158,73 @@
         scheme = urlparse(address).scheme or None
 
     return await get_backend(scheme).create_actor_pool(
         address, n_process=n_process, **kwargs
     )
 
 
+def buffer_ref(address: str, buffer: Any) -> BufferRef:
+    """
+    Init buffer ref according address and buffer.
+
+    Parameters
+    ----------
+    address
+        The address of the buffer.
+    buffer
+        CPU / GPU buffer. Need to support for slicing and retrieving the length.
+
+    Returns
+    ----------
+    BufferRef obj.
+    """
+    ctx = get_context()
+    return ctx.buffer_ref(address, buffer)
+
+
+def file_object_ref(address: str, fileobj: AioFileObject) -> FileObjectRef:
+    """
+    Init file object ref according to address and aio file obj.
+
+    Parameters
+    ----------
+    address
+        The address of the file obj.
+    fileobj
+        Aio file object.
+
+    Returns
+    ----------
+    FileObjectRef obj.
+    """
+    ctx = get_context()
+    return ctx.file_object_ref(address, fileobj)
+
+
+async def copy_to(
+    local_buffers_or_fileobjs: list,
+    remote_refs: List[Union[BufferRef, FileObjectRef]],
+    block_size: Optional[int] = None,
+):
+    """
+    Copy data from local buffers to remote buffers or copy local file objects to remote file objects.
+
+    Parameters
+    ----------
+    local_buffers_or_fileobjs
+        Local buffers or file objects.
+    remote_refs
+        Remote buffer refs or file object refs.
+    block_size
+        Transfer block size when non-ucx
+    """
+    ctx = get_context()
+    return await ctx.copy_to(local_buffers_or_fileobjs, remote_refs, block_size)
+
+
 async def wait_actor_pool_recovered(address: str, main_pool_address: str | None = None):
     """
     Wait until the specified actor pool has recovered from failure.
 
     Parameters
     ----------
     address: str
```

### Comparing `xoscar-0.0.7/xoscar/backend.py` & `xoscar-0.0.8/xoscar/backend.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/__init__.py` & `xoscar-0.0.8/xoscar/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/allocate_strategy.py` & `xoscar-0.0.8/xoscar/backends/allocate_strategy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/__init__.py` & `xoscar-0.0.8/xoscar/backends/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/base.py` & `xoscar-0.0.8/xoscar/backends/communication/base.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/core.py` & `xoscar-0.0.8/xoscar/backends/communication/core.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/dummy.py` & `xoscar-0.0.8/xoscar/backends/communication/dummy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/errors.py` & `xoscar-0.0.8/xoscar/backends/communication/errors.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/socket.py` & `xoscar-0.0.8/xoscar/backends/communication/socket.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/communication/ucx.py` & `xoscar-0.0.8/xoscar/backends/communication/ucx.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 
 import asyncio
 import concurrent.futures as futures
 import functools
 import logging
 import os
 import weakref
-from typing import Any, Callable, Coroutine, Dict, List, Tuple, Type
+from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple, Type
 
 import cloudpickle
 import numpy as np
 
 from ...nvutils import get_cuda_context, get_index_and_uuid
 from ...serialization import deserialize
 from ...serialization.aio import BUFFER_SIZES_NAME, AioSerializer, get_header_length
-from ...utils import classproperty, implements, lazy_import
+from ...utils import classproperty, implements, is_cuda_buffer, lazy_import
+from ..message import _MessageBase
 from .base import Channel, ChannelType, Client, Server
 from .core import register_client, register_server
 from .errors import ChannelClosed
 
 ucp = lazy_import("ucp")
 numba_cuda = lazy_import("numba.cuda")
 rmm = lazy_import("rmm")
@@ -172,17 +173,15 @@
                 )
 
         original_environ = os.environ
         new_environ = os.environ.copy()
         new_environ.update(envs)
         os.environ = new_environ  # type: ignore
         try:
-            ucp.init(
-                options=options, env_takes_precedence=True, blocking_progress_mode=False
-            )
+            ucp.init(options=options, env_takes_precedence=True)
         finally:
             os.environ = original_environ
 
         UCXInitializer._inited = True
 
     @staticmethod
     def reset():
@@ -233,44 +232,31 @@
 
     @staticmethod
     def _close_channel(channel_ref: weakref.ReferenceType):
         channel = channel_ref()
         if channel is not None:
             channel._closed = True
 
+    async def _serialize(self, message: Any) -> List[bytes]:
+        compress = self.compression or 0
+        serializer = AioSerializer(message, compress=compress)
+        return await serializer.run()
+
     @property
     @implements(Channel.type)
     def type(self) -> int:
         return ChannelType.remote
 
     @implements(Channel.send)
     async def send(self, message: Any):
         if self.closed:
             raise ChannelClosed("UCX Endpoint is closed, unable to send message")
 
-        compress = self.compression or 0
-        serializer = AioSerializer(message, compress=compress)
-        buffers = await serializer.run()
-        try:
-            # It is necessary to first synchronize the default stream before start
-            # sending We synchronize the default stream because UCX is not
-            # stream-ordered and syncing the default stream will wait for other
-            # non-blocking CUDA streams. Note this is only sufficient if the memory
-            # being sent is not currently in use on non-blocking CUDA streams.
-            if any(hasattr(buf, "__cuda_array_interface__") for buf in buffers):
-                # has GPU buffer
-                synchronize_stream(0)
-
-            async with self._send_lock:
-                for buffer in buffers:
-                    if buffer.nbytes if hasattr(buffer, "nbytes") else len(buffer) > 0:
-                        await self.ucp_endpoint.send(buffer)
-        except ucp.exceptions.UCXBaseException:  # pragma: no cover
-            self.abort()
-            raise ChannelClosed("While writing, the connection was closed")
+        buffers = await self._serialize(message)
+        return await self.send_buffers(buffers)
 
     @implements(Channel.recv)
     async def recv(self):
         async with self._recv_lock:
             try:
                 info_buffer = np.empty(11, dtype="u1").data
                 await self.ucp_endpoint.recv(info_buffer)
@@ -302,14 +288,56 @@
                     raise ChannelClosed(
                         f"Connection closed by writer.\nInner exception: {e!r}"
                     ) from e
                 else:
                     raise EOFError("Server closed already")
         return deserialize(header, buffers)
 
+    async def send_buffers(self, buffers: list, meta: Optional[_MessageBase] = None):
+        try:
+            # It is necessary to first synchronize the default stream before start
+            # sending We synchronize the default stream because UCX is not
+            # stream-ordered and syncing the default stream will wait for other
+            # non-blocking CUDA streams. Note this is only sufficient if the memory
+            # being sent is not currently in use on non-blocking CUDA streams.
+            if any(is_cuda_buffer(buf) for buf in buffers):
+                # has GPU buffer
+                synchronize_stream(0)
+
+            meta_buffers = None
+            if meta:
+                meta_buffers = await self._serialize(meta)
+
+            async with self._send_lock:
+                if meta_buffers:
+                    for buf in meta_buffers:
+                        await self.ucp_endpoint.send(buf)
+                for buffer in buffers:
+                    if buffer.nbytes if hasattr(buffer, "nbytes") else len(buffer) > 0:
+                        await self.ucp_endpoint.send(buffer)
+        except ucp.exceptions.UCXBaseException:  # pragma: no cover
+            self.abort()
+            raise ChannelClosed("While writing, the connection was closed")
+
+    async def recv_buffers(self, buffers: list):
+        async with self._recv_lock:
+            try:
+                for buffer in buffers:
+                    await self.ucp_endpoint.recv(buffer)
+            except BaseException as e:  # pragma: no cover
+                if not self._closed:
+                    # In addition to UCX exceptions, may be CancelledError or another
+                    # "low-level" exception. The only safe thing to do is to abort.
+                    self.abort()
+                    raise ChannelClosed(
+                        f"Connection closed by writer.\nInner exception: {e!r}"
+                    ) from e
+                else:
+                    raise EOFError("Server closed already")
+
     def abort(self):
         self._closed = True
         if self.ucp_endpoint is not None:
             self.ucp_endpoint.abort()
             self.ucp_endpoint = None
 
     @implements(Channel.close)
@@ -386,15 +414,15 @@
 
         async def serve_forever(client_ucp_endpoint: "ucp.Endpoint"):  # type: ignore
             try:
                 await server.on_connected(
                     client_ucp_endpoint, local_address=server.address
                 )
             except ChannelClosed:  # pragma: no cover
-                logger.debug("Connection closed before handshake completed")
+                logger.exception("Connection closed before handshake completed")
                 return
 
         ucp_listener = ucp.create_listener(serve_forever, port=port)
 
         # get port of the ucp listener if not specified
         if not port:
             port = ucp_listener.port
@@ -438,28 +466,30 @@
     @implements(Server.stop)
     async def stop(self):
         self._ucp_listener.close()
         # close all channels
         await asyncio.gather(
             *(channel.close() for channel in self._channels if not channel.closed)
         )
+        self._channels = []
         self._ucp_listener = None
         self._closed.set()
 
     @property
     @implements(Server.stopped)
     def stopped(self) -> bool:
         return self._ucp_listener is None
 
 
 @register_client
 class UCXClient(Client):
     __slots__ = ()
 
     scheme = UCXServer.scheme
+    channel: UCXChannel
 
     @classmethod
     def parse_config(cls, config: dict) -> dict:
         return config
 
     @staticmethod
     @implements(Client.connect)
@@ -473,13 +503,19 @@
         port = int(port_str)
         kwargs = kwargs.copy()
         ucx_config = kwargs.pop("config", dict()).get("ucx", dict())
         UCXInitializer.init(ucx_config)
 
         try:
             ucp_endpoint = await ucp.create_endpoint(host, port)
-        except ucp.exceptions.UCXBaseException:  # pragma: no cover
-            raise ChannelClosed("Connection closed before handshake completed")
+        except ucp.exceptions.UCXBaseException as e:  # pragma: no cover
+            raise ChannelClosed(
+                f"Connection closed before handshake completed, "
+                f"local address: {local_address}, dest address: {dest_address}"
+            ) from e
         channel = UCXChannel(
             ucp_endpoint, local_address=local_address, dest_address=dest_address
         )
         return UCXClient(local_address, dest_address, channel)
+
+    async def send_buffers(self, buffers: list, meta: _MessageBase):
+        return await self.channel.send_buffers(buffers, meta)
```

### Comparing `xoscar-0.0.7/xoscar/backends/communication/utils.py` & `xoscar-0.0.8/xoscar/backends/communication/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     is_cuda_buffers = header[0].get("is_cuda_buffers")
     buffer_sizes = header[0].pop(BUFFER_SIZES_NAME)
 
     buffers = []
     for is_cuda_buffer, buf_size in zip(is_cuda_buffers, buffer_sizes):
         if is_cuda_buffer:  # pragma: no cover
             if buf_size == 0:
-                content = await reader.readexactly(buf_size)
-                buffers.append(content)
+                # uniformly use rmm.DeviceBuffer for cuda's deserialization
+                buffers.append(rmm.DeviceBuffer(size=buf_size))
             else:
                 buffer = rmm.DeviceBuffer(size=buf_size)
                 arr = _convert_to_cupy_ndarray(buffer)
                 offset = 0
                 chunk_size = CUDA_CHUNK_SIZE
                 while offset < buf_size:
                     read_size = (
```

### Comparing `xoscar-0.0.7/xoscar/backends/config.py` & `xoscar-0.0.8/xoscar/backends/config.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/core.py` & `xoscar-0.0.8/xoscar/backends/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import asyncio
 import copy
 import logging
-from typing import Union
+from typing import Type, Union
 
 from .._utils import Timer
 from ..errors import ServerClosed
 from ..profiling import get_profiling_data
-from .communication import Client
+from .communication import Client, UCXClient
 from .message import DeserializeMessageFailed, ErrorMessage, ResultMessage, _MessageBase
 from .router import Router
 
 ResultMessageType = Union[ResultMessage, ErrorMessage]
 logger = logging.getLogger(__name__)
 
 
@@ -38,27 +38,39 @@
     _clients: dict[Client, asyncio.Task]
 
     def __init__(self):
         self._client_to_message_futures = dict()
         self._clients = dict()
         self._profiling_data = get_profiling_data()
 
-    async def get_client(self, router: Router, dest_address: str) -> Client:
-        client = await router.get_client(dest_address, from_who=self)
+    def _listen_client(self, client: Client):
         if client not in self._clients:
             self._clients[client] = asyncio.create_task(self._listen(client))
             self._client_to_message_futures[client] = dict()
             client_count = len(self._clients)
             if client_count >= 100:  # pragma: no cover
                 if (client_count - 100) % 10 == 0:  # pragma: no cover
                     logger.warning(
                         "Actor caller has created too many clients (%s >= 100), "
                         "the global router may not be set.",
                         client_count,
                     )
+
+    async def get_client_via_type(
+        self, router: Router, dest_address: str, client_type: Type[Client]
+    ) -> Client:
+        client = await router.get_client_via_type(
+            dest_address, client_type, from_who=self
+        )
+        self._listen_client(client)
+        return client
+
+    async def get_client(self, router: Router, dest_address: str) -> Client:
+        client = await router.get_client(dest_address, from_who=self)
+        self._listen_client(client)
         return client
 
     async def _listen(self, client: Client):
         while not client.closed:
             try:
                 try:
                     message: _MessageBase = await client.recv()
@@ -98,22 +110,17 @@
 
         message_futures = self._client_to_message_futures[client]
         self._client_to_message_futures[client] = dict()
         error = ServerClosed(f"Remote server {client.dest_address} closed")
         for future in message_futures.values():
             future.set_exception(copy.copy(error))
 
-    async def call(
-        self,
-        router: Router,
-        dest_address: str,
-        message: _MessageBase,
-        wait: bool = True,
+    async def call_with_client(
+        self, client: Client, message: _MessageBase, wait: bool = True
     ) -> ResultMessage | ErrorMessage | asyncio.Future:
-        client = await self.get_client(router, dest_address)
         loop = asyncio.get_running_loop()
         wait_response = loop.create_future()
         self._client_to_message_futures[client][message.message_id] = wait_response
 
         with Timer() as timer:
             try:
                 await client.send(message)
@@ -129,14 +136,54 @@
                 r = wait_response
             else:
                 r = await wait_response
 
         self._profiling_data.collect_actor_call(message, timer.duration)
         return r
 
+    async def call_send_buffers(
+        self,
+        client: UCXClient,
+        local_buffers: list,
+        meta_message: _MessageBase,
+        wait: bool = True,
+    ) -> ResultMessage | ErrorMessage | asyncio.Future:
+        loop = asyncio.get_running_loop()
+        wait_response = loop.create_future()
+        self._client_to_message_futures[client][meta_message.message_id] = wait_response
+
+        with Timer() as timer:
+            try:
+                await client.send_buffers(local_buffers, meta_message)
+            except ConnectionError:  # pragma: no cover
+                try:
+                    await client.close()
+                except ConnectionError:
+                    # close failed, ignore it
+                    pass
+                raise ServerClosed(f"Remote server {client.dest_address} closed")
+
+            if not wait:  # pragma: no cover
+                r = wait_response
+            else:
+                r = await wait_response
+
+        self._profiling_data.collect_actor_call(meta_message, timer.duration)
+        return r
+
+    async def call(
+        self,
+        router: Router,
+        dest_address: str,
+        message: _MessageBase,
+        wait: bool = True,
+    ) -> ResultMessage | ErrorMessage | asyncio.Future:
+        client = await self.get_client(router, dest_address)
+        return await self.call_with_client(client, message, wait)
+
     async def stop(self):
         try:
             await asyncio.gather(*[client.close() for client in self._clients])
         except (ConnectionError, ServerClosed):
             pass
         self.cancel_tasks()
```

### Comparing `xoscar-0.0.7/xoscar/backends/indigen/__init__.py` & `xoscar-0.0.8/xoscar/backends/indigen/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/indigen/backend.py` & `xoscar-0.0.8/xoscar/backends/indigen/backend.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/indigen/driver.py` & `xoscar-0.0.8/xoscar/backends/indigen/driver.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/indigen/pool.py` & `xoscar-0.0.8/xoscar/backends/indigen/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import random
 import signal
 import sys
 import threading
 import uuid
 from dataclasses import dataclass
 from types import TracebackType
-from typing import List
+from typing import List, Optional
 
 from ..._utils import reset_id_random_seed
 from ...utils import dataslots, ensure_coverage
 from ..config import ActorPoolConfig
 from ..message import CreateActorMessage
 from ..pool import MainActorPoolBase, SubActorPoolBase, _register_message_handler
 
@@ -118,15 +118,15 @@
 class MainActorPool(MainActorPoolBase):
     @classmethod
     def get_external_addresses(
         cls,
         address: str,
         n_process: int | None = None,
         ports: list[int] | None = None,
-        schemes: list[str] | None = None,
+        schemes: list[Optional[str]] | None = None,
     ):
         """Get external address for every process"""
         assert n_process is not None
         if ":" in address:
             host, port_str = address.split(":", 1)
             port = int(port_str)
             if ports:
@@ -305,15 +305,15 @@
         process.kill()
         await asyncio.to_thread(process.join, 5)
 
     async def is_sub_pool_alive(self, process: multiprocessing.Process):
         try:
             return await asyncio.to_thread(process.is_alive)
         except RuntimeError as ex:  # pragma: no cover
-            if "cannot schedule new futures after interpreter shutdown" not in str(ex):
+            if "cannot schedule new futures" not in str(ex):
                 # when atexit is triggered, the default pool might be shutdown
                 # and to_thread will fail
                 raise
             return process.is_alive()
 
     async def recover_sub_pool(self, address: str):
         process_index = self._config.get_process_index(address)
```

### Comparing `xoscar-0.0.7/xoscar/backends/message.pyx` & `xoscar-0.0.8/xoscar/backends/message.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from enum import Enum
 from types import TracebackType
 from typing import Any, Type
 
 from tblib import pickling_support
 
-from ..core cimport ActorRef
+from ..core cimport ActorRef, BufferRef
 from ..serialization.core cimport Serializer
 from ..utils import wrap_exception
 from .._utils cimport new_random_id
 
 # make sure traceback can be pickled
 pickling_support.install()
 
@@ -38,23 +38,27 @@
     create_actor = 3
     destroy_actor = 4
     has_actor = 5
     actor_ref = 6
     send = 7
     tell = 8
     cancel = 9
+    copy_to_buffers = 10
+    copy_to_fileobjs = 11
 
 
 class ControlMessageType(Enum):
     stop = 0
     restart = 1
     sync_config = 2
     get_config = 3
     wait_pool_recovered = 4
     add_sub_pool_actor = 5
+    # the new channel created is for data transfer only
+    switch_to_copy_to = 6
 
 
 cdef class _MessageSerialItem:
     cdef:
         tuple serialized
         list subs
 
@@ -482,25 +486,62 @@
 
     cdef deserial_members(self, tuple serialized, list subs):
         _MessageBase.deserial_members(self, serialized, subs)
         self.address = serialized[-2]
         self.cancel_message_id = serialized[-1]
 
 
+cdef class CopyToBuffersMessage(_MessageBase):
+    message_type = MessageType.copy_to_buffers
+
+    cdef:
+        public object content
+
+    def __init__(
+        self,
+        bytes message_id = None,
+        object content = None,
+        int protocol = _DEFAULT_PROTOCOL,
+        list message_trace = None,
+    ):
+        _MessageBase.__init__(
+            self,
+            message_id,
+            protocol=protocol,
+            message_trace=message_trace
+        )
+        self.content = content
+
+    cdef _MessageSerialItem serial(self):
+        cdef _MessageSerialItem item = _MessageBase.serial(self)
+        item.subs = [self.content]
+        return item
+
+    cdef deserial_members(self, tuple serialized, list subs):
+        _MessageBase.deserial_members(self, serialized, subs)
+        self.content = subs[0]
+
+
+cdef class CopyToFileObjectsMessage(CopyToBuffersMessage):
+    message_type = MessageType.copy_to_fileobjs
+
+
 cdef dict _message_type_to_message_cls = {
     MessageType.control.value: ControlMessage,
     MessageType.result.value: ResultMessage,
     MessageType.error.value: ErrorMessage,
     MessageType.create_actor.value: CreateActorMessage,
     MessageType.destroy_actor.value: DestroyActorMessage,
     MessageType.has_actor.value: HasActorMessage,
     MessageType.actor_ref.value: ActorRefMessage,
     MessageType.send.value: SendMessage,
     MessageType.tell.value: TellMessage,
     MessageType.cancel.value: CancelMessage,
+    MessageType.copy_to_buffers.value: CopyToBuffersMessage,
+    MessageType.copy_to_fileobjs.value: CopyToFileObjectsMessage
 }
 
 
 class DeserializeMessageFailed(RuntimeError):
     def __init__(self, message_id):
         self.message_id = message_id
```

### Comparing `xoscar-0.0.7/xoscar/backends/pool.py` & `xoscar-0.0.8/xoscar/backends/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,34 @@
 import threading
 import traceback
 from abc import ABC, ABCMeta, abstractmethod
 from typing import Any, Callable, Coroutine, Optional, Type, TypeVar
 
 from .._utils import TypeDispatcher, create_actor_ref, to_binary
 from ..api import Actor
-from ..core import ActorRef, register_local_pool
+from ..core import ActorRef, BufferRef, FileObjectRef, register_local_pool
 from ..debug import debug_async_timeout, record_message_trace
 from ..entrypoints import init_extension_entrypoints
 from ..errors import (
     ActorAlreadyExist,
     ActorNotExist,
     CannotCancelTask,
     SendMessageFailed,
     ServerClosed,
 )
 from ..metrics import init_metrics
 from ..utils import implements, register_asyncio_task_timeout_detector
 from .allocate_strategy import AddressSpecified, allocated_type
-from .communication import Channel, Server, gen_local_address, get_server_type
+from .communication import (
+    Channel,
+    Server,
+    UCXChannel,
+    gen_local_address,
+    get_server_type,
+)
 from .communication.errors import ChannelClosed
 from .config import ActorPoolConfig
 from .core import ActorCaller, ResultMessageType
 from .message import (
     DEFAULT_PROTOCOL,
     ActorRefMessage,
     CancelMessage,
@@ -113,14 +119,16 @@
         (MessageType.destroy_actor, pool_type.destroy_actor),
         (MessageType.has_actor, pool_type.has_actor),
         (MessageType.actor_ref, pool_type.actor_ref),
         (MessageType.send, pool_type.send),
         (MessageType.tell, pool_type.tell),
         (MessageType.cancel, pool_type.cancel),
         (MessageType.control, pool_type.handle_control_command),
+        (MessageType.copy_to_buffers, pool_type.handle_copy_to_buffers_message),
+        (MessageType.copy_to_fileobjs, pool_type.handle_copy_to_fileobjs_message),
     ]:
         pool_type._message_handler[message_type] = handler  # type: ignore
     return pool_type
 
 
 class AbstractActorPool(ABC):
     __slots__ = (
@@ -489,30 +497,75 @@
 
             self._servers = []
             if self._asyncio_task_timeout_detector_task:  # pragma: no cover
                 self._asyncio_task_timeout_detector_task.cancel()
         finally:
             self._stopped.set()
 
+    async def handle_copy_to_buffers_message(self, message) -> ResultMessage:
+        for addr, uid, start, _len, data in message.content:
+            buffer = BufferRef.get_buffer(BufferRef(addr, uid))
+            buffer[start : start + _len] = data
+        return ResultMessage(message_id=message.message_id, result=True)
+
+    async def handle_copy_to_fileobjs_message(self, message) -> ResultMessage:
+        for addr, uid, data in message.content:
+            file_obj = FileObjectRef.get_local_file_object(FileObjectRef(addr, uid))
+            await file_obj.write(data)
+        return ResultMessage(message_id=message.message_id, result=True)
+
     @property
     def stopped(self) -> bool:
         return self._stopped.is_set()
 
+    async def _handle_ucx_meta_message(
+        self, message: _MessageBase, channel: Channel
+    ) -> bool:
+        if (
+            isinstance(message, ControlMessage)
+            and message.message_type == MessageType.control
+            and message.control_message_type == ControlMessageType.switch_to_copy_to
+            and isinstance(channel, UCXChannel)
+        ):
+            with _ErrorProcessor(
+                self.external_address, message.message_id, message.protocol
+            ) as processor:
+                # use `%.500` to avoid print too long messages
+                with debug_async_timeout(
+                    "process_message_timeout",
+                    "Process message %.500s of channel %s timeout.",
+                    message,
+                    channel,
+                ):
+                    buffers = [
+                        BufferRef.get_buffer(BufferRef(addr, uid))
+                        for addr, uid in message.content
+                    ]
+                    await channel.recv_buffers(buffers)
+                    processor.result = ResultMessage(
+                        message_id=message.message_id, result=True
+                    )
+            asyncio.create_task(self._send_channel(processor.result, channel))
+            return True
+        return False
+
     async def on_new_channel(self, channel: Channel):
         while not self._stopped.is_set():
             try:
                 message = await channel.recv()
             except EOFError:
                 # no data to read, check channel
                 try:
                     await channel.close()
                 except (ConnectionError, EOFError):
                     # close failed, ignore
                     pass
                 return
+            if await self._handle_ucx_meta_message(message, channel):
+                continue
             asyncio.create_task(self.process_message(message, channel))
             # delete to release the reference of message
             del message
             await asyncio.sleep(0)
 
     async def __aenter__(self):
         await self.start()
@@ -1351,18 +1404,15 @@
                                     self._on_process_recover(self, address)
                         if recover_events_discovered:
                             event = self._recover_events.pop(address)
                             event.set()
                     except asyncio.CancelledError:
                         raise
                     except RuntimeError as ex:  # pragma: no cover
-                        if (
-                            "cannot schedule new futures after interpreter shutdown"
-                            not in str(ex)
-                        ):
+                        if "cannot schedule new futures" not in str(ex):
                             # to silence log when process exit, otherwise it
                             # will raise "RuntimeError: cannot schedule new futures
                             # after interpreter shutdown".
                             logger.exception("Monitor sub pool %s failed", address)
                     except Exception:
                         # log the exception instead of stop monitoring the
                         # sub pool silently.
@@ -1377,15 +1427,15 @@
     @classmethod
     @abstractmethod
     def get_external_addresses(
         cls,
         address: str,
         n_process: int | None = None,
         ports: list[int] | None = None,
-        schemes: list[str] | None = None,
+        schemes: list[Optional[str]] | None = None,
     ):
         """Returns external addresses for n pool processes"""
 
     @classmethod
     @abstractmethod
     def gen_internal_address(
         cls, process_index: int, external_address: str | None = None
@@ -1397,15 +1447,15 @@
     address: str,
     *,
     pool_cls: Type[MainActorPoolType] | None = None,
     n_process: int | None = None,
     labels: list[str] | None = None,
     ports: list[int] | None = None,
     envs: list[dict] | None = None,
-    external_address_schemes: list[str] | None = None,
+    external_address_schemes: list[Optional[str]] | None = None,
     enable_internal_addresses: list[bool] | None = None,
     subprocess_start_method: str | None = None,
     auto_recover: str | bool = "actor",
     modules: list[str] | None = None,
     suspend_sigint: bool | None = None,
     use_uvloop: str | bool = "auto",
     logging_conf: dict | None = None,
```

### Comparing `xoscar-0.0.7/xoscar/backends/router.py` & `xoscar-0.0.8/xoscar/backends/router.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import asyncio
 import threading
-from typing import Any, Optional, Type
+from typing import Any, Dict, List, Optional, Type
 
 from .communication import Client, get_client_type
 
 
 class Router:
     """
     Router provides mapping from external address to internal address.
@@ -63,21 +64,29 @@
         if mapping is None:
             mapping = dict()
         self._mapping = mapping
         self._comm_config = comm_config or dict()
         self._cache_local = threading.local()
 
     @property
-    def _cache(self) -> dict[tuple[str, Any], Client]:
+    def _cache(self) -> dict[tuple[str, Any, Optional[Type[Client]]], Client]:
         try:
             return self._cache_local.cache
         except AttributeError:
             cache = self._cache_local.cache = dict()
             return cache
 
+    @property
+    def _lock(self) -> asyncio.Lock:
+        try:
+            return self._cache_local.lock
+        except AttributeError:
+            lock = self._cache_local.lock = asyncio.Lock()
+            return lock
+
     def set_mapping(self, mapping: dict[str, str]):
         self._mapping = mapping
         self._cache_local = threading.local()
 
     def add_router(self, router: "Router"):
         self._curr_external_addresses.extend(router._curr_external_addresses)
         self._local_mapping.update(router._local_mapping)
@@ -99,39 +108,100 @@
 
     @property
     def external_address(self):
         if self._curr_external_addresses:
             return self._curr_external_addresses[0]
 
     def get_internal_address(self, external_address: str) -> str | None:
-        if external_address in self._curr_external_addresses:
+        try:
             # local address, use dummy address
-            return self._local_mapping.get(external_address)
-        # try to lookup inner address from address mapping
-        return self._mapping.get(external_address)
+            return self._local_mapping[external_address]
+        except KeyError:
+            # try to lookup inner address from address mapping
+            return self._mapping.get(external_address)
 
     async def get_client(
-        self, external_address: str, from_who: Any = None, cached: bool = True, **kw
+        self,
+        external_address: str,
+        from_who: Any = None,
+        cached: bool = True,
+        **kw,
+    ) -> Client:
+        async with self._lock:
+            if cached and (external_address, from_who, None) in self._cache:
+                cached_client = self._cache[external_address, from_who, None]
+                if cached_client.closed:
+                    # closed before, ignore it
+                    del self._cache[external_address, from_who, None]
+                else:
+                    return cached_client
+
+            address = self.get_internal_address(external_address)
+            if address is None:
+                # no inner address, just use external address
+                address = external_address
+            client_type: Type[Client] = get_client_type(address)
+            client = await self._create_client(client_type, address, **kw)
+            if cached:
+                self._cache[external_address, from_who, None] = client
+            return client
+
+    async def _create_client(
+        self, client_type: Type[Client], address: str, **kw
     ) -> Client:
-        if cached and (external_address, from_who) in self._cache:
-            cached_client = self._cache[external_address, from_who]
-            if cached_client.closed:
-                # closed before, ignore it
-                del self._cache[external_address, from_who]
-            else:
-                return cached_client
-
-        address = self.get_internal_address(external_address)
-        if address is None:
-            # no inner address, just use external address
-            address = external_address
-        client_type: Type[Client] = get_client_type(address)
-        local_address = (
-            self._curr_external_addresses[0] if self._curr_external_addresses else None
-        )
         config = client_type.parse_config(self._comm_config)
         if config:
             kw["config"] = config
-        client = await client_type.connect(address, local_address=local_address, **kw)
-        if cached:
-            self._cache[external_address, from_who] = client
-        return client
+        local_address = (
+            self._curr_external_addresses[0] if self._curr_external_addresses else None
+        )
+        return await client_type.connect(address, local_address=local_address, **kw)
+
+    def _get_client_type_to_addresses(
+        self, external_address: str
+    ) -> Dict[Type[Client], str]:
+        client_type_to_addresses = dict()
+        client_type_to_addresses[get_client_type(external_address)] = external_address
+        if external_address in self._curr_external_addresses:  # pragma: no cover
+            # local address, use dummy address
+            addr = self._local_mapping.get(external_address)
+            client_type = get_client_type(addr)  # type: ignore
+            client_type_to_addresses[client_type] = addr  # type: ignore
+        if external_address in self._mapping:
+            # try to lookup inner address from address mapping
+            addr = self._mapping.get(external_address)
+            client_type = get_client_type(addr)  # type: ignore
+            client_type_to_addresses[client_type] = addr  # type: ignore
+        return client_type_to_addresses
+
+    def get_all_client_types(self, external_address: str) -> List[Type[Client]]:
+        return list(self._get_client_type_to_addresses(external_address))
+
+    async def get_client_via_type(
+        self,
+        external_address: str,
+        client_type: Type[Client],
+        from_who: Any = None,
+        cached: bool = True,
+        **kw,
+    ) -> Client:
+        async with self._lock:
+            if cached and (external_address, from_who, client_type) in self._cache:
+                cached_client = self._cache[external_address, from_who, client_type]
+                if cached_client.closed:  # pragma: no cover
+                    # closed before, ignore it
+                    del self._cache[external_address, from_who, client_type]
+                else:
+                    return cached_client
+
+            client_type_to_addresses = self._get_client_type_to_addresses(
+                external_address
+            )
+            if client_type not in client_type_to_addresses:  # pragma: no cover
+                raise ValueError(
+                    f"Client type({client_type}) is not supported for {external_address}"
+                )
+            address = client_type_to_addresses[client_type]
+            client = await self._create_client(client_type, address, **kw)
+            if cached:
+                self._cache[external_address, from_who, client_type] = client
+            return client
```

### Comparing `xoscar-0.0.7/xoscar/backends/test/__init__.py` & `xoscar-0.0.8/xoscar/backends/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/test/backend.py` & `xoscar-0.0.8/xoscar/backends/test/backend.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/backends/test/pool.py` & `xoscar-0.0.8/xoscar/backends/test/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import asyncio
 import multiprocessing
-from typing import Any
+from typing import Any, Optional
 
 from ..communication import DummyServer, gen_local_address
 from ..config import ActorPoolConfig
 from ..indigen.pool import MainActorPool, SubActorPool, SubpoolStatus
 from ..pool import ActorPoolType
 
 
 class TestMainActorPool(MainActorPool):
     @classmethod
     def get_external_addresses(
         cls,
         address: str,
         n_process: int | None = None,
         ports: list[int] | None = None,
-        schemes: list[str] | None = None,
+        schemes: list[Optional[str]] | None = None,
     ):
         if "://" in address:
             address = address.split("://", 1)[1]
         return super().get_external_addresses(address, n_process=n_process, ports=ports)
 
     @classmethod
     def gen_internal_address(
```

### Comparing `xoscar-0.0.7/xoscar/batch.py` & `xoscar-0.0.8/xoscar/batch.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/constants.py` & `xoscar-0.0.8/xoscar/constants.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/context.pxd` & `xoscar-0.0.8/xoscar/context.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/core.pxd` & `xoscar-0.0.8/xoscar/core.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 
 
 cdef class LocalActorRef(ActorRef):
     cdef object _actor_weakref
     cdef _weakref_local_actor(self)
 
 
+cdef class BufferRef:
+    cdef public str address
+    cdef public bytes uid
+
+
+cdef class FileObjectRef:
+    cdef public str address
+    cdef public bytes uid
+
+
 cdef class _BaseActor:
     cdef object __weakref__
     cdef str _address
     cdef object _lock
     cdef object _uid
 
     cpdef ActorRef ref(self)
```

### Comparing `xoscar-0.0.7/xoscar/core.pyx` & `xoscar-0.0.8/xoscar/core.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,23 @@
 # limitations under the License.
 
 import asyncio
 import inspect
 import logging
 import sys
 import weakref
-from typing import AsyncGenerator
+from typing import Any, AsyncGenerator
 
 cimport cython
 
+from .aio import AioFileObject
 from .context cimport get_context
+
 from .errors import ActorNotExist, Return
+
 from ._utils cimport is_async_generator
 
 CALL_METHOD_DEFAULT = 0
 CALL_METHOD_BATCH = 1
 
 logger = logging.getLogger(__name__)
 
@@ -542,7 +545,83 @@
 
 # The @cython.binding(True) is for ray getting members.
 # The value is True by default after cython >= 3.0.0
 @cython.binding(True)
 cdef class _StatelessActor(_BaseActor):
     def _create_lock(self):
         return _FakeLock()
+
+
+cdef class BufferRef:
+    """
+    Reference of a buffer
+    """
+    _ref_to_buffers = weakref.WeakValueDictionary()
+
+    def __init__(self, str address, bytes uid):
+        self.uid = uid
+        self.address = address
+
+    @classmethod
+    def create(cls, buffer: Any, address: str, uid: bytes) -> "BufferRef":
+        ref = BufferRef(address, uid)
+        cls._ref_to_buffers[ref] = buffer
+        return ref
+
+    @classmethod
+    def get_buffer(cls, ref: "BufferRef"):
+        return cls._ref_to_buffers[ref]
+
+    def __getstate__(self):
+        return self.uid, self.address
+
+    def __setstate__(self, state):
+        self.uid, self.address = state
+
+    def __hash__(self):
+        return hash((self.address, self.uid))
+
+    def __eq__(self, other):
+        if type(other) != BufferRef:
+            return False
+        return self.address == other.address and self.uid == other.uid
+
+    def __repr__(self):
+        return f'BufferRef(uid={self.uid.hex()}, address={self.address})'
+
+
+cdef class FileObjectRef:
+    """
+    Reference of a file obj
+    """
+    _ref_to_fileobjs = weakref.WeakValueDictionary()
+
+    def __init__(self, str address, bytes uid):
+        self.uid = uid
+        self.address = address
+
+    @classmethod
+    def create(cls, fileobj: AioFileObject, address: str, uid: bytes) -> "FileObjectRef":
+        ref = FileObjectRef(address, uid)
+        cls._ref_to_fileobjs[ref] = fileobj
+        return ref
+
+    @classmethod
+    def get_local_file_object(cls, ref: "FileObjectRef") -> AioFileObject:
+        return cls._ref_to_fileobjs[ref]
+
+    def __getstate__(self):
+        return self.uid, self.address
+
+    def __setstate__(self, state):
+        self.uid, self.address = state
+
+    def __hash__(self):
+        return hash((self.address, self.uid))
+
+    def __eq__(self, other):
+        if type(other) != FileObjectRef:
+            return False
+        return self.address == other.address and self.uid == other.uid
+
+    def __repr__(self):
+        return f'FileObjectRef(uid={self.uid.hex()}, address={self.address})'
```

### Comparing `xoscar-0.0.7/xoscar/debug.py` & `xoscar-0.0.8/xoscar/debug.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/driver.py` & `xoscar-0.0.8/xoscar/driver.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/entrypoints.py` & `xoscar-0.0.8/xoscar/entrypoints.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/errors.py` & `xoscar-0.0.8/xoscar/errors.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/libcpp.pxd` & `xoscar-0.0.8/xoscar/libcpp.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/__init__.py` & `xoscar-0.0.8/xoscar/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/api.py` & `xoscar-0.0.8/xoscar/metrics/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,23 +66,23 @@
                 "Failed to start prometheus http server because there is no prometheus_client"
             )
     _init = True
     for m in _metrics_to_be_initialized:
         cls = getattr(_backends_cls[_metric_backend], m.type)
         metric = cls(m.name, m.description, m.tag_keys)
         m.set_metric(metric)
-    logger.info("Finished initialize the metrics of backend: %s.", _metric_backend)
+    logger.debug("Finished initialize the metrics of backend: %s.", _metric_backend)
 
 
 def shutdown_metrics():
     global _metric_backend
     _metric_backend = "console"
     global _init
     _init = False
-    logger.info("Shutdown metrics of backend: %s.", _metric_backend)
+    logger.debug("Shutdown metrics of backend: %s.", _metric_backend)
 
 
 class _MetricWrapper(AbstractMetric):
     _metric: AbstractMetric | None
     _log_not_init_error: bool
 
     def __init__(
```

### Comparing `xoscar-0.0.7/xoscar/metrics/backends/__init__.py` & `xoscar-0.0.8/xoscar/collective/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/backends/console/__init__.py` & `xoscar-0.0.8/xoscar/collective/rendezvous/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/backends/console/console_metric.py` & `xoscar-0.0.8/xoscar/metrics/backends/console/console_metric.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/backends/metric.py` & `xoscar-0.0.8/xoscar/metrics/backends/metric.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/backends/prometheus/__init__.py` & `xoscar-0.0.8/xoscar/collective/rendezvous/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/metrics/backends/prometheus/prometheus_metric.py` & `xoscar-0.0.8/xoscar/metrics/backends/prometheus/prometheus_metric.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/nvutils.py` & `xoscar-0.0.8/xoscar/nvutils.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/profiling.py` & `xoscar-0.0.8/xoscar/profiling.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/__init__.py` & `xoscar-0.0.8/xoscar/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/aio.py` & `xoscar-0.0.8/xoscar/serialization/aio.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/arrow.py` & `xoscar-0.0.8/xoscar/serialization/arrow.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/core.pxd` & `xoscar-0.0.8/xoscar/serialization/core.pxd`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/core.pyx` & `xoscar-0.0.8/xoscar/serialization/core.pyx`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/cuda.py` & `xoscar-0.0.8/xoscar/serialization/cuda.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/exception.py` & `xoscar-0.0.8/xoscar/serialization/exception.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/numpy.py` & `xoscar-0.0.8/xoscar/serialization/numpy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/serialization/scipy.py` & `xoscar-0.0.8/xoscar/serialization/scipy.py`

 * *Files identical despite different names*

### Comparing `xoscar-0.0.7/xoscar/utils.py` & `xoscar-0.0.8/xoscar/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import random
 import socket
 import sys
 import time
 import uuid
 from abc import ABC
 from types import TracebackType
-from typing import Callable, Type
+from typing import Callable, Type, Union
 
 from ._utils import (  # noqa: F401 # pylint: disable=unused-import
     NamedType,
     Timer,
     TypeDispatcher,
     to_binary,
     to_str,
@@ -442,7 +442,19 @@
                 except ex_type as e:
                     ex = e
                     time.sleep(wait_interval)
             assert ex is not None
             raise ex  # pylint: disable-msg=E0702
 
     return retry_call
+
+
+_cupy = lazy_import("cupy")
+_rmm = lazy_import("rmm")
+
+
+def is_cuda_buffer(cuda_buffer: Union["_cupy.ndarray", "_rmm.DeviceBuffer"]) -> bool:  # type: ignore
+    return hasattr(cuda_buffer, "__cuda_array_interface__")
+
+
+def is_windows():
+    return sys.platform.startswith("win")
```

### Comparing `xoscar-0.0.7/xoscar.egg-info/PKG-INFO` & `xoscar-0.0.8/xoscar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xoscar
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python actor framework for heterogeneous computing.
-Home-page: http://github.com/xprobe-inc/xoscar
+Home-page: http://github.com/xorbitsai/xoscar
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -26,17 +26,17 @@
 
 <div align="center">
   <img width="77%" alt="" src="https://raw.githubusercontent.com/xprobe-inc/xoscar/main/doc/source/_static/Xoscar.svg"><br>
 </div>
 
 # Python actor framework for heterogeneous computing.
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xoscar.svg?style=for-the-badge)](https://pypi.org/project/xoscar/)
-[![Coverage](https://img.shields.io/codecov/c/github/xprobe-inc/xoscar?style=for-the-badge)](https://codecov.io/gh/xprobe-inc/xoscar)
-[![Build Status](https://img.shields.io/github/actions/workflow/status/xprobe-inc/xoscar/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xprobe-inc/xoscar/goto?ref=main)
-[![License](https://img.shields.io/pypi/l/xoscar.svg?style=for-the-badge)](https://github.com/xprobe-inc/xoscar/blob/main/LICENSE)
+[![Coverage](https://img.shields.io/codecov/c/github/xorbitsai/xoscar?style=for-the-badge)](https://codecov.io/gh/xorbitsai/xoscar)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/xoscar/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/xoscar/goto?ref=main)
+[![License](https://img.shields.io/pypi/l/xoscar.svg?style=for-the-badge)](https://github.com/xorbitsai/xoscar/blob/main/LICENSE)
 
 ## What is actor
 Writing parallel and distributed programs is often challenging and requires a lot of time to deal with concurrency
 issues. Actor model provides a high-level, scalable and robust abstraction for building distributed applications. 
 It provides several benefits:
 - Scalability: Actors easily scale across nodes. The asynchronous, non-blocking nature of actors allows them to handle huge volumes of concurrent tasks efficiently.
 - Concurrency: The actor model abstracts over concurrency, allowing developers to avoid raw threads and locks.
@@ -65,15 +65,15 @@
 appropriate pool based on the specified policy.
 
 When actors communicate, Xoscar will choose the optimal communication mechanism based on which pools the actors 
 belong to. This allows Xoscar to optimize communication in heterogeneous environments with multiple processing 
 units and accelerators.
 
 ## Where to get it
-The source code is currently hosted on GitHub at: https://github.com/xprobe-inc/xoscar
+The source code is currently hosted on GitHub at: https://github.com/xorbitsai/xoscar
 
 Binary installers for the latest released version are available at the [Python
 Package Index (PyPI)](https://pypi.org/project/xoscar).
 
 ```shell
 # PyPI
 pip install xoscar
```

### Comparing `xoscar-0.0.7/xoscar.egg-info/SOURCES.txt` & `xoscar-0.0.8/xoscar.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 xoscar/backends/indigen/__init__.py
 xoscar/backends/indigen/backend.py
 xoscar/backends/indigen/driver.py
 xoscar/backends/indigen/pool.py
 xoscar/backends/test/__init__.py
 xoscar/backends/test/backend.py
 xoscar/backends/test/pool.py
+xoscar/collective/__init__.py
+xoscar/collective/rendezvous/__init__.py
+xoscar/collective/rendezvous/test/__init__.py
+xoscar/collective/rendezvous/test/test_tcp_store.py
 xoscar/metrics/__init__.py
 xoscar/metrics/api.py
 xoscar/metrics/backends/__init__.py
 xoscar/metrics/backends/metric.py
 xoscar/metrics/backends/console/__init__.py
 xoscar/metrics/backends/console/console_metric.py
 xoscar/metrics/backends/prometheus/__init__.py
```

### Comparing `xoscar-0.0.7/xoscar.egg-info/requires.txt` & `xoscar-0.0.8/xoscar.egg-info/requires.txt`

 * *Files identical despite different names*


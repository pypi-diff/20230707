# Comparing `tmp/frites-0.4.3.tar.gz` & `tmp/frites-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frites-0.4.3.tar", last modified: Thu Nov  3 19:28:10 2022, max compression
+gzip compressed data, was "frites-0.4.4.tar", last modified: Fri Jul  7 08:18:18 2023, max compression
```

## Comparing `frites-0.4.3.tar` & `frites-0.4.4.tar`

### file list

```diff
@@ -1,83 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.258026 frites-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-03 19:27:53.000000 frites-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-03 19:27:53.000000 frites-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-11-03 19:28:10.258026 frites-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-11-03 19:27:53.000000 frites-0.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.250026 frites-0.4.3/frites/
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-11-03 19:27:53.000000 frites-0.4.3/frites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-11-03 19:27:53.000000 frites-0.4.3/frites/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.250026 frites-0.4.3/frites/conn/
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5357 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_ccf.py
--rw-r--r--   0 runner    (1001) docker     (121)    18135 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_covgc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5529 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_dfc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_fcd_corr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5644 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_sliding_windows.py
--rw-r--r--   0 runner    (1001) docker     (121)    13360 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_te.py
--rw-r--r--   0 runner    (1001) docker     (121)     7310 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_tf.py
--rw-r--r--   0 runner    (1001) docker     (121)    25930 2022-11-03 19:27:53.000000 frites-0.4.3/frites/conn/conn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/core/
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-11-03 19:27:53.000000 frites-0.4.3/frites/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-11-03 19:27:53.000000 frites-0.4.3/frites/core/copnorm.py
--rw-r--r--   0 runner    (1001) docker     (121)    19832 2022-11-03 19:27:53.000000 frites-0.4.3/frites/core/gcmi_1d.py
--rw-r--r--   0 runner    (1001) docker     (121)    26893 2022-11-03 19:27:53.000000 frites-0.4.3/frites/core/gcmi_nd.py
--rw-r--r--   0 runner    (1001) docker     (121)     7296 2022-11-03 19:27:53.000000 frites-0.4.3/frites/core/mi_bin_ephy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-03 19:27:53.000000 frites-0.4.3/frites/data/frites.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/dataset/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-11-03 19:27:53.000000 frites-0.4.3/frites/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18082 2022-11-03 19:27:53.000000 frites-0.4.3/frites/dataset/ds_ephy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2855 2022-11-03 19:27:53.000000 frites-0.4.3/frites/dataset/ds_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10427 2022-11-03 19:27:53.000000 frites-0.4.3/frites/dataset/suj_ephy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/estimator/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8420 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_bin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9873 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_corr.py
--rw-r--r--   0 runner    (1001) docker     (121)     8358 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_custom.py
--rw-r--r--   0 runner    (1001) docker     (121)     7561 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_dcorr.py
--rw-r--r--   0 runner    (1001) docker     (121)     9254 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_gcmi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_mi_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-11-03 19:27:53.000000 frites-0.4.3/frites/estimator/est_resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/io/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-03 19:27:53.000000 frites-0.4.3/frites/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3017 2022-11-03 19:27:53.000000 frites-0.4.3/frites/io/io_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-11-03 19:27:53.000000 frites-0.4.3/frites/io/io_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7029 2022-11-03 19:27:53.000000 frites-0.4.3/frites/io/io_syslog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-03 19:27:53.000000 frites-0.4.3/frites/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26143 2022-11-03 19:27:53.000000 frites-0.4.3/frites/plot/plot_conn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/simulations/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-03 19:27:53.000000 frites-0.4.3/frites/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23889 2022-11-03 19:27:53.000000 frites-0.4.3/frites/simulations/sim_ar.py
--rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-11-03 19:27:53.000000 frites-0.4.3/frites/simulations/sim_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    21094 2022-11-03 19:27:53.000000 frites-0.4.3/frites/simulations/sim_local_mi.py
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-11-03 19:27:53.000000 frites-0.4.3/frites/simulations/sim_mi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/stats/
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-11-03 19:27:53.000000 frites-0.4.3/frites/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10543 2022-11-03 19:27:53.000000 frites-0.4.3/frites/stats/stats_mcp.py
--rw-r--r--   0 runner    (1001) docker     (121)    12951 2022-11-03 19:27:53.000000 frites-0.4.3/frites/stats/stats_nonparam.py
--rw-r--r--   0 runner    (1001) docker     (121)     5411 2022-11-03 19:27:53.000000 frites-0.4.3/frites/stats/stats_param.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.254026 frites-0.4.3/frites/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-03 19:27:53.000000 frites-0.4.3/frites/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-11-03 19:27:53.000000 frites-0.4.3/frites/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-03 19:27:53.000000 frites-0.4.3/frites/utils/perf.py
--rw-r--r--   0 runner    (1001) docker     (121)    11812 2022-11-03 19:27:53.000000 frites-0.4.3/frites/utils/preproc.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-03 19:27:53.000000 frites-0.4.3/frites/utils/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.258026 frites-0.4.3/frites/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-11-03 19:27:53.000000 frites-0.4.3/frites/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-11-03 19:27:53.000000 frites-0.4.3/frites/workflow/wf_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    12587 2022-11-03 19:27:53.000000 frites-0.4.3/frites/workflow/wf_conn_comod.py
--rw-r--r--   0 runner    (1001) docker     (121)    30229 2022-11-03 19:27:53.000000 frites-0.4.3/frites/workflow/wf_mi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-11-03 19:27:53.000000 frites-0.4.3/frites/workflow/wf_mi_combine.py
--rw-r--r--   0 runner    (1001) docker     (121)     9002 2022-11-03 19:27:53.000000 frites-0.4.3/frites/workflow/wf_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 19:28:10.250026 frites-0.4.3/frites.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-11-03 19:28:10.000000 frites-0.4.3/frites.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-11-03 19:28:10.000000 frites-0.4.3/frites.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 19:28:10.000000 frites-0.4.3/frites.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-11-03 19:28:10.000000 frites-0.4.3/frites.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-03 19:28:10.000000 frites-0.4.3/frites.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-03 19:27:53.000000 frites-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-03 19:28:10.258026 frites-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-11-03 19:27:53.000000 frites-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-07 08:18:02.000000 frites-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-07 08:18:02.000000 frites-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-07 08:18:18.345443 frites-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-07 08:18:02.000000 frites-0.4.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.341443 frites-0.4.4/frites/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-07 08:18:02.000000 frites-0.4.4/frites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-07 08:18:02.000000 frites-0.4.4/frites/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.341443 frites-0.4.4/frites/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_ccf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_covgc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_dfc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_fcd_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_ii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_sliding_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_te.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28339 2023-07-07 08:18:02.000000 frites-0.4.4/frites/conn/conn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.341443 frites-0.4.4/frites/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:02.000000 frites-0.4.4/frites/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 08:18:02.000000 frites-0.4.4/frites/core/copnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-07-07 08:18:02.000000 frites-0.4.4/frites/core/gcmi_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29154 2023-07-07 08:18:02.000000 frites-0.4.4/frites/core/gcmi_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-07-07 08:18:02.000000 frites-0.4.4/frites/core/mi_bin_ephy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.341443 frites-0.4.4/frites/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 08:18:02.000000 frites-0.4.4/frites/data/frites.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.341443 frites-0.4.4/frites/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 08:18:02.000000 frites-0.4.4/frites/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18082 2023-07-07 08:18:02.000000 frites-0.4.4/frites/dataset/ds_ephy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-07 08:18:02.000000 frites-0.4.4/frites/dataset/ds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-07-07 08:18:02.000000 frites-0.4.4/frites/dataset/suj_ephy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_dcorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_gcmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_mi_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-07 08:18:02.000000 frites-0.4.4/frites/estimator/est_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 08:18:02.000000 frites-0.4.4/frites/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-07 08:18:02.000000 frites-0.4.4/frites/io/io_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 08:18:02.000000 frites-0.4.4/frites/io/io_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-07 08:18:02.000000 frites-0.4.4/frites/io/io_syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-07 08:18:02.000000 frites-0.4.4/frites/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26143 2023-07-07 08:18:02.000000 frites-0.4.4/frites/plot/plot_conn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-07 08:18:02.000000 frites-0.4.4/frites/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23889 2023-07-07 08:18:02.000000 frites-0.4.4/frites/simulations/sim_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-07 08:18:02.000000 frites-0.4.4/frites/simulations/sim_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-07-07 08:18:02.000000 frites-0.4.4/frites/simulations/sim_local_mi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-07 08:18:02.000000 frites-0.4.4/frites/simulations/sim_mi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-07 08:18:02.000000 frites-0.4.4/frites/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-07 08:18:02.000000 frites-0.4.4/frites/stats/stats_mcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-07 08:18:02.000000 frites-0.4.4/frites/stats/stats_nonparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-07 08:18:02.000000 frites-0.4.4/frites/stats/stats_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 08:18:02.000000 frites-0.4.4/frites/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-07 08:18:02.000000 frites-0.4.4/frites/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-07 08:18:02.000000 frites-0.4.4/frites/utils/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-07-07 08:18:02.000000 frites-0.4.4/frites/utils/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-07 08:18:02.000000 frites-0.4.4/frites/utils/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.345443 frites-0.4.4/frites/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-07 08:18:02.000000 frites-0.4.4/frites/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-07 08:18:02.000000 frites-0.4.4/frites/workflow/wf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-07 08:18:02.000000 frites-0.4.4/frites/workflow/wf_conn_comod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-07 08:18:02.000000 frites-0.4.4/frites/workflow/wf_mi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-07 08:18:02.000000 frites-0.4.4/frites/workflow/wf_mi_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-07 08:18:02.000000 frites-0.4.4/frites/workflow/wf_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:18.341443 frites-0.4.4/frites.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-07 08:18:18.000000 frites-0.4.4/frites.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-07 08:18:18.000000 frites-0.4.4/frites.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:18:18.000000 frites-0.4.4/frites.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-07 08:18:18.000000 frites-0.4.4/frites.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 08:18:18.000000 frites-0.4.4/frites.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 08:18:02.000000 frites-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-07 08:18:18.345443 frites-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-07 08:18:02.000000 frites-0.4.4/setup.py
```

### Comparing `frites-0.4.3/LICENSE` & `frites-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/PKG-INFO` & `frites-0.4.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: frites
-Version: 0.4.3
+Version: 0.4.4
 Summary: Framework of Information Theory for Electrophysiological data and Statistics
 Home-page: https://github.com/brainets/frites
-Download-URL: https://github.com/brainets/frites/archive/v0.4.3.tar.gz
+Download-URL: https://github.com/brainets/frites/archive/v0.4.4.tar.gz
 Author: BraiNets
 Author-email: e.combrisson@gmail.com
 Maintainer: Etienne Combrisson
 License: BSD 3-Clause License
 Keywords: information-theory statistics
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: flake
 Provides-Extra: full
 License-File: LICENSE
 
+.. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/logo_desc.png
+    :align:  center
+
+
+Frites
+======
+
 .. image:: https://github.com/brainets/frites/actions/workflows/test_doc.yml/badge.svg
     :target: https://github.com/brainets/frites/actions/workflows/test_doc.yml
 
 .. image:: https://github.com/brainets/frites/actions/workflows/flake.yml/badge.svg
     :target: https://github.com/brainets/frites/actions/workflows/flake.yml
 
 .. image:: https://travis-ci.org/brainets/frites.svg?branch=master
@@ -37,36 +46,50 @@
 
 .. image:: https://badge.fury.io/py/frites.svg
     :target: https://badge.fury.io/py/frites
 
 .. image:: https://pepy.tech/badge/frites
     :target: https://pepy.tech/project/frites
 
-.. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/logo_desc.png
-    :align:  center
+.. image:: https://zenodo.org/badge/213869364.svg
+    :target: https://zenodo.org/badge/latestdoi/213869364
+
+.. image:: https://joss.theoj.org/papers/437a7362501b2ea984e1d4fed4646076/status.svg
+    :target: https://joss.theoj.org/papers/437a7362501b2ea984e1d4fed4646076
+
+
+.. _Documentation: https://brainets.github.io/frites/
+.. |Documentation| replace:: **Documentation**
+
+.. _Installation: https://brainets.github.io/frites/install.html
+.. |Installation| replace:: **Installation**
+
+.. _Usage: https://brainets.github.io/frites/auto_examples/index.html
+.. |Usage| replace:: **Usage example**
+
+.. _API: https://brainets.github.io/frites/api/index.html
+.. |API| replace:: **List of functions**
+
+.. _Cite: https://brainets.github.io/frites/overview/ovw_cite.html
+.. |Cite| replace:: **Cite Frites**
+
+|Documentation|_ | |Installation|_ | |Usage|_ | |API|_ | |Cite|_
 
-======
-Frites
-======
 
 Description
------------
+===========
 
-`Frites <https://brainets.github.io/frites/>`_ is a Python toolbox for assessing information-theorical measures on human and animal neurophysiological data (M/EEG, Intracranial). The aim of Frites is to extract task-related cognitive brain networks (i.e modulated by the task). The toolbox also includes directed and undirected connectivity metrics such as group-level statistics.
+`Frites <https://brainets.github.io/frites/>`_ is a Python toolbox for assessing information-theorical measures on human and animal neurophysiological data (M/EEG, Intracranial). The aim of Frites is to extract task-related cognitive brain networks (i.e modulated by the task). The toolbox also includes directed and undirected connectivity metrics such as group-level statistics. Frites documentation is available online at https://brainets.github.io/frites/
 
 .. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/network_framework.png
     :align:  center
 
-Documentation
--------------
-
-Frites documentation is available online at https://brainets.github.io/frites/
 
 Installation
-------------
+============
 
 Run the following command into your terminal to get the latest stable version :
 
 .. code-block:: shell
 
     pip install -U frites
 
@@ -102,10 +125,10 @@
 
 * `Numba <http://numba.pydata.org/>`_ : speed up the computations of some functions
 * `Dcor <https://dcor.readthedocs.io/en/latest/>`_ for fast implementation of distance correlation
 * `Matplotlib <https://matplotlib.org/>`_, `Seaborn <https://seaborn.pydata.org/>`_ and `Networkx <https://networkx.github.io/>`_ for plotting the examples
 * Some example are using `scikit learn <https://scikit-learn.org/stable/index.html>`_ estimators
 
 Acknowledgments
----------------
+===============
 
 See `acknowledgments <https://brainets.github.io/frites/overview/ovw_acknowledgments.html>`_
```

### Comparing `frites-0.4.3/README.rst` & `frites-0.4.4/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+.. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/logo_desc.png
+    :align:  center
+
+
+Frites
+======
+
 .. image:: https://github.com/brainets/frites/actions/workflows/test_doc.yml/badge.svg
     :target: https://github.com/brainets/frites/actions/workflows/test_doc.yml
 
 .. image:: https://github.com/brainets/frites/actions/workflows/flake.yml/badge.svg
     :target: https://github.com/brainets/frites/actions/workflows/flake.yml
 
 .. image:: https://travis-ci.org/brainets/frites.svg?branch=master
@@ -12,36 +19,50 @@
 
 .. image:: https://badge.fury.io/py/frites.svg
     :target: https://badge.fury.io/py/frites
 
 .. image:: https://pepy.tech/badge/frites
     :target: https://pepy.tech/project/frites
 
-.. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/logo_desc.png
-    :align:  center
+.. image:: https://zenodo.org/badge/213869364.svg
+    :target: https://zenodo.org/badge/latestdoi/213869364
+
+.. image:: https://joss.theoj.org/papers/437a7362501b2ea984e1d4fed4646076/status.svg
+    :target: https://joss.theoj.org/papers/437a7362501b2ea984e1d4fed4646076
+
+
+.. _Documentation: https://brainets.github.io/frites/
+.. |Documentation| replace:: **Documentation**
+
+.. _Installation: https://brainets.github.io/frites/install.html
+.. |Installation| replace:: **Installation**
+
+.. _Usage: https://brainets.github.io/frites/auto_examples/index.html
+.. |Usage| replace:: **Usage example**
+
+.. _API: https://brainets.github.io/frites/api/index.html
+.. |API| replace:: **List of functions**
+
+.. _Cite: https://brainets.github.io/frites/overview/ovw_cite.html
+.. |Cite| replace:: **Cite Frites**
+
+|Documentation|_ | |Installation|_ | |Usage|_ | |API|_ | |Cite|_
 
-======
-Frites
-======
 
 Description
------------
+===========
 
-`Frites <https://brainets.github.io/frites/>`_ is a Python toolbox for assessing information-theorical measures on human and animal neurophysiological data (M/EEG, Intracranial). The aim of Frites is to extract task-related cognitive brain networks (i.e modulated by the task). The toolbox also includes directed and undirected connectivity metrics such as group-level statistics.
+`Frites <https://brainets.github.io/frites/>`_ is a Python toolbox for assessing information-theorical measures on human and animal neurophysiological data (M/EEG, Intracranial). The aim of Frites is to extract task-related cognitive brain networks (i.e modulated by the task). The toolbox also includes directed and undirected connectivity metrics such as group-level statistics. Frites documentation is available online at https://brainets.github.io/frites/
 
 .. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/network_framework.png
     :align:  center
 
-Documentation
--------------
-
-Frites documentation is available online at https://brainets.github.io/frites/
 
 Installation
-------------
+============
 
 Run the following command into your terminal to get the latest stable version :
 
 .. code-block:: shell
 
     pip install -U frites
 
@@ -77,10 +98,10 @@
 
 * `Numba <http://numba.pydata.org/>`_ : speed up the computations of some functions
 * `Dcor <https://dcor.readthedocs.io/en/latest/>`_ for fast implementation of distance correlation
 * `Matplotlib <https://matplotlib.org/>`_, `Seaborn <https://seaborn.pydata.org/>`_ and `Networkx <https://networkx.github.io/>`_ for plotting the examples
 * Some example are using `scikit learn <https://scikit-learn.org/stable/index.html>`_ estimators
 
 Acknowledgments
----------------
+===============
 
 See `acknowledgments <https://brainets.github.io/frites/overview/ovw_acknowledgments.html>`_
```

### Comparing `frites-0.4.3/frites/__init__.py` & `frites-0.4.4/frites/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Frites
 ======
 
-Framework of Information Theory for Electrophysiological data and Statistics
+Framework for Information Theoretical analyses of Electrophysiological data and Statistics
 """
 import logging
 
 from frites import (
     io, core, conn, plot, stats, utils, workflow, simulations,  estimator  # noqa
 )
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 # -----------------------------------------------------------------------------
 # Set 'info' as the default logging level
 logger = logging.getLogger('frites')
 io.set_log_level('info')
 
 # -----------------------------------------------------------------------------
```

### Comparing `frites-0.4.3/frites/config.py` & `frites-0.4.4/frites/config.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/__init__.py` & `frites-0.4.4/frites/conn/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,23 @@
    connectivity arrays to `frites.workflow.WfMi`
 2. **Connectivity related utility functions :** small utility functions that
    work on connectivity arrays
 """
 # connectivity input conversion
 from .conn_io import conn_io  # noqa
 
+# connectivity utility functions
+from .conn_fcd_corr import conn_fcd_corr  # noqa
+from .conn_sliding_windows import define_windows, plot_windows  # noqa
+from .conn_utils import (conn_get_pairs, conn_links, conn_reshape_undirected,  # noqa
+                         conn_reshape_directed, conn_ravel_directed, conn_net,
+                         _conn_mi)
+
 # connectivity metrics
 from .conn_ccf import conn_ccf  # noqa
 from .conn_covgc import conn_covgc  # noqa
 from .conn_dfc import conn_dfc  # noqa
 from .conn_spec import conn_spec  # noqa
 from .conn_te import conn_te
-
-# connectivity utility functions
-from .conn_fcd_corr import conn_fcd_corr  # noqa
-from .conn_sliding_windows import define_windows, plot_windows  # noqa
-from .conn_utils import (conn_get_pairs, conn_links, conn_reshape_undirected,  # noqa
-                         conn_reshape_directed, conn_ravel_directed, conn_net)
+from .conn_ii import conn_ii  # noqa
+from .conn_pid import conn_pid  # noqa
+from .conn_fit import conn_fit
```

### Comparing `frites-0.4.3/frites/conn/conn_ccf.py` & `frites-0.4.4/frites/conn/conn_ccf.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_covgc.py` & `frites-0.4.4/frites/conn/conn_covgc.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_dfc.py` & `frites-0.4.4/frites/conn/conn_dfc.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,11 +123,11 @@
     dfc = xr.DataArray(dfc, dims=('trials', 'roi', 'times'),
                        coords=(trials, roi_p, win_times),
                        name=f'DFC ({estimator.name})')
 
     # add the windows used in the attributes
     cfg = dict(
         win_sample=np.r_[tuple(win_sample)], win_times=np.r_[tuple(win_times)],
-        agg_ch=agg_ch, type='dfc', estimator=estimator.name)
+        agg_ch=agg_ch, type='dfc', estimator=estimator.name, unit='Bits')
     dfc.attrs = check_attrs({**cfg, **attrs})
 
     return dfc
```

### Comparing `frites-0.4.3/frites/conn/conn_fcd_corr.py` & `frites-0.4.4/frites/conn/conn_fcd_corr.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_io.py` & `frites-0.4.4/frites/conn/conn_io.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_sliding_windows.py` & `frites-0.4.4/frites/conn/conn_sliding_windows.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_spec.py` & `frites-0.4.4/frites/conn/conn_spec.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_te.py` & `frites-0.4.4/frites/conn/conn_te.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_tf.py` & `frites-0.4.4/frites/conn/conn_tf.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/conn/conn_utils.py` & `frites-0.4.4/frites/conn/conn_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utility functions for connectivity."""
 import numpy as np
 import xarray as xr
 import pandas as pd
 
 from frites.utils import nonsorted_unique
 from frites.io import set_log_level, logger
+from frites.core import ent_nd_g, mi_nd_gg, mi_model_nd_gd
 
 
 ###############################################################################
 ###############################################################################
 #                                 CONN PAIRS
 ###############################################################################
 ###############################################################################
@@ -338,32 +339,37 @@
 ###############################################################################
 ###############################################################################
 #                              CONN RESHAPING
 ###############################################################################
 ###############################################################################
 
 
-def conn_reshape_undirected(da, sep='-', order=None, rm_missing=False,
-                            fill_value=np.nan, fill_diagonal=None,
-                            to_dataframe=False, inplace=False, verbose=None):
+def conn_reshape_undirected(
+        da, sep='-', order=None, axis='roi', rm_missing=False,
+        fill_value=np.nan, fill_diagonal=None, to_dataframe=False,
+        inplace=False, verbose=None):
     """Reshape a raveled undirected array of connectivity.
 
-    This function takes a DataArray of shape (n_pairs,) or (n_pairs, n_times)
-    where n_pairs reflects pairs of roi (e.g 'roi_1-roi_2') and reshape it to
-    be a symmetric DataArray of shape (n_roi, n_roi, n_times).
+    This function reshapes a DataArray of connectivity values into a symmetric
+    matrix. For example, a DataArray of shape (n_pairs,) where n_pairs reflects
+    pairs of roi (e.g 'roi_1-roi_2') is going to be reshaped into a symmetric
+    DataArray of shape (n_roi, n_roi). Similarly, a DataArray of shape
+    (n_pairs, n_times) is going to be reshaped into a symmetric DataArray of
+    shape (n_roi, n_roi, n_times).
 
     Parameters
     ----------
     da : xarray.DataArray
-        Xarray DataArray of shape (n_pairs, n_times) where actually the roi
-        dimension contains the pairs (roi_1-roi_2, roi_1-roi_3 etc.)
+        Flatten DataArray of connectivity values to be reshaped
     sep : string | '-'
         Separator used to separate the pairs of roi names.
     order : list | None
         List of roi names to reorder the output.
+    axis : string | 'roi'
+        Name of the spatial dimension to use for reshaping
     rm_missing : bool | False
         When reordering the connectivity array, choose if you prefer to reindex
         even if there's missing regions (rm_missing=False) or if missing
         regions should be removed (rm_missing=True)
     fill_value : float | np.nan
         Value to use for filling missing pairs
     fill_diagonal : float | None
@@ -382,59 +388,62 @@
     --------
     conn_dfc
     """
     set_log_level(verbose)
     assert isinstance(da, xr.DataArray)
     if not inplace:
         da = da.copy()
-    assert 'roi' in list(da.dims)
-    if 'times' not in list(da.dims):
-        da = da.expand_dims("times")
+    assert axis in list(da.dims)
 
     # get sources, targets names and sorted full list
-    sources, targets, roi_tot = _untangle_roi(da, sep)
+    sources, targets, roi_tot = _get_roi_names(da, sep, axis)
 
     # duplicates to make it symmetrical
-    da = xr.concat((da, da), 'roi')
+    da = xr.concat((da, da), axis)
     s_, t_ = sources + targets, targets + sources
+
     # build the multiindex and unstack it
-    da, order = _dataarray_unstack(da, s_, t_, roi_tot, fill_value,
-                                   order, rm_missing, fill_diagonal)
+    da, order = _dataarray_unstack(
+        da, s_, t_, roi_tot, fill_value, order, rm_missing, fill_diagonal, axis
+    )
 
     # dataframe conversion
     if to_dataframe:
         da = _dataframe_conversion(da, order, rm_missing)
 
     return da
 
 
-def conn_reshape_directed(da, net=False, sep='-', order=None, rm_missing=False,
-                          fill_value=np.nan, fill_diagonal=None,
-                          to_dataframe=False, inplace=False, verbose=None):
+def conn_reshape_directed(
+        da, net=False, sep='-', order=None, axis='roi', rm_missing=False,
+        fill_value=np.nan, fill_diagonal=None, to_dataframe=False,
+        inplace=False, verbose=None):
     """Reshape a raveled directed array of connectivity.
 
     This function takes a DataArray of shape (n_pairs, n_directions) or
-    (n_pairs, n_times, n_direction) where n_pairs reflects pairs of roi
-    (e.g 'roi_1-roi_2') and n_direction usually contains bidirected 'x->y' and
-    'y->x'. At the end, this function reshape the input array so that rows
-    contains the sources and columns the targets leading to a non-symmetric
-    DataArray of shape (n_roi, n_roi, n_times). A typical use case for this
-    function would be after computing the covariance based granger causality.
+    where n_pairs reflects pairs of roi (e.g 'roi_1-roi_2') and n_direction
+    usually contains bidirected 'x->y' and 'y->x'. At the end, this function
+    reshape the input array so that rows contains the sources and columns the
+    targets leading to a non-symmetric DataArray of shape (n_roi, n_roi). A
+    typical use case for this function would be after computing the covariance
+    based granger causality.
 
     Parameters
     ----------
     da : xarray.DataArray
-        Xarray DataArray of shape (n_pairs, n_times, n_directions) where
+        Xarray DataArray of shape (n_pairs, n_directions) where
         actually the roi dimension contains the pairs (roi_1-roi_2, roi_1-roi_3
         etc.). The dimension n_directions should contains the dimensions 'x->y'
         and 'y->x'
     sep : string | '-'
         Separator used to separate the pairs of roi names.
     order : list | None
         List of roi names to reorder the output.
+    axis : string | 'roi'
+        Name of the spatial dimension to use for reshaping
     rm_missing : bool | False
         When reordering the connectivity array, choose if you prefer to reindex
         even if there's missing regions (rm_missing=False) or if missing
         regions should be removed (rm_missing=True)
     fill_value : float | np.nan
         Value to use for filling missing pairs (e.g diagonal)
     fill_diagonal : float | None
@@ -443,85 +452,91 @@
     to_dataframe : bool | False
         Dataframe conversion. Only possible if the da input does not contains
         a time axis.
 
     Returns
     -------
     da_out : xarray.DataArray
-        DataArray of shape (n_roi, n_roi, n_times)
+        DataArray of shape (n_roi, n_roi)
 
     See also
     --------
     conn_covgc
     """
     set_log_level(verbose)
     assert isinstance(da, xr.DataArray)
     if not inplace:
         da = da.copy()
-    assert 'roi' in list(da.dims)
-    if 'times' not in list(da.dims):
-        da = da.expand_dims("times")
+    assert axis in list(da.dims)
 
     # get sources, targets names and sorted full list
-    sources, targets, roi_tot = _untangle_roi(da, sep)
+    sources, targets, roi_tot = _get_roi_names(da, sep, axis)
 
     # transpose, reindex and reorder (if needed)
     if 'direction' in list(da.dims):
         da_xy, da_yx = da.sel(direction='x->y'), da.sel(direction='y->x')
         if net:
-            da = xr.concat((da_xy - da_yx, da_xy - da_yx), 'roi')
+            da = xr.concat((da_xy - da_yx, da_xy - da_yx), axis)
         else:
-            da = xr.concat((da_xy, da_yx), 'roi')
+            da = xr.concat((da_xy, da_yx), axis)
         s_, t_ = sources + targets, targets + sources
     else:
         s_, t_ = sources, targets
-    da, order = _dataarray_unstack(da, s_, t_, roi_tot, fill_value,
-                                   order, rm_missing, fill_diagonal)
+    da, order = _dataarray_unstack(
+        da, s_, t_, roi_tot, fill_value, order, rm_missing, fill_diagonal, axis
+    )
 
     # dataframe conversion
     if to_dataframe:
         da = _dataframe_conversion(da, order, rm_missing)
 
     return da
 
 
-def _untangle_roi(da, sep):
-    """Get details about the roi."""
+def _get_roi_names(da, sep, axis):
+    """Get the roi names from a DataArray."""
     # start by extrating sources / targets names
     sources, targets = [], []
-    for k in da['roi'].data:
+    for k in da[axis].data:
         sources += [k.split(sep)[0]]
         targets += [k.split(sep)[1]]
 
     # merge sources and targets to force square matrix
     roi_tot = nonsorted_unique(sources + targets)
 
     return sources, targets, roi_tot
 
 
-def _dataarray_unstack(da, sources, targets, roi_tot, fill_value, order,
-                       rm_missing, fill_diagonal):
+def _dataarray_unstack(
+        da, sources, targets, roi_tot, fill_value, order, rm_missing,
+        fill_diagonal, axis):
     """Unstack a 1d to 2d DataArray."""
-    import pandas as pd
+    # replace axis by sources and targets
+    dim_names = list(da.dims)
+    cut_at = dim_names.index(axis)
+    dim_names = dim_names[:cut_at] + ['sources', 'targets'] + dim_names[
+        cut_at + 1:]
 
     # build the multi-index
-    da['roi'] = pd.MultiIndex.from_arrays(
+    da[axis] = pd.MultiIndex.from_arrays(
         [sources, targets], names=['sources', 'targets'])
+
     # test for duplicated entries
     st_names = pd.Series([f"{s}-{t}" for s, t in zip(sources, targets)])
     duplicates = np.array(list(st_names.duplicated(keep='first')))
     if duplicates.any():
         logger.warning(f"Duplicated entries found and removed : "
-                       f"{da['roi'].data[duplicates]}")
+                       f"{da[axis].data[duplicates]}")
         da = da.sel(roi=~duplicates)
+
     # unstack to be 2D/3D
     da = da.unstack(fill_value=fill_value)
 
     # transpose, reindex and reorder (if needed)
-    da = da.transpose('sources', 'targets', 'times')
+    da = da.transpose(*tuple(dim_names))
     da = da.reindex(dict(sources=roi_tot, targets=roi_tot),
                     fill_value=fill_value)
 
     # change order
     if isinstance(order, (list, np.ndarray)):
         if rm_missing:
             order = [k for k in order.copy() if k in roi_tot.tolist()]
@@ -537,15 +552,15 @@
 
 def _dataframe_conversion(da, order, rm_missing):
     """Convert a DataArray to a DataFrame and be sure its sorted correctly."""
     assert da.data.squeeze().ndim == 2, (
         "Dataframe conversion only possible for connectivity arrays when "
         "time dimension is missing")
     da = da.squeeze().to_dataframe('mi').reset_index()
-    da = da.pivot('sources', 'targets', 'mi')
+    da = da.pivot(index='sources', columns='targets', values='mi')
     if isinstance(order, (list, np.ndarray)):
         da = da.reindex(order, axis='index').reindex(order, axis='columns')
     # drop empty lines
     if rm_missing:
         da = da.dropna(axis=0, how='all').dropna(axis=1, how='all')
 
     return da
@@ -679,7 +694,68 @@
 
     # update attributes to track operations
     out.attrs['net_source'] = p_s
     out.attrs['net_target'] = p_t
     out.name = da.name + '_net' if da.name else 'Net conn'
 
     return out
+
+
+###############################################################################
+###############################################################################
+#                         CONN MUTUAL INFORMATION
+###############################################################################
+###############################################################################
+
+
+def _conn_mi(x, y, mi_type, minorm=False, **kw_mi):
+    """Compute the mutual information for connectivity-related functions.
+
+    This function compute the mutual information I(x, y) between a continuous x
+    and a continuous or discret y variable. In addition, we assume here that
+    the two last axes are multivariate and trials.
+
+    Parameters
+    ----------
+    x : array_like
+        Array of shape (n_vars, n_mvaxis, n_trials)
+    y : array_like
+        Array of shape (n_trials) or (n_vars, n_mvaxis, n_trials)
+    mi_type : {'cc', 'cd'}
+        Mutual information type
+    minorm : bool | False
+        Normalize the mutual information
+    kw_mi : dict
+        Additional arguments are sent to the MI function
+
+    Returns
+    -------
+    mi : array_like
+        Array of mutual information of shape (n_vars,)
+    """
+    assert isinstance(x, np.ndarray) and isinstance(y, np.ndarray)
+    assert (x.ndim == 3) and (1 <= y.ndim <= 3)
+    assert mi_type in ['cc', 'cd']
+    kw_mi['traxis'] = -1
+    kw_mi['mvaxis'] = -2
+    kw_mi['shape_checking'] = False
+
+    # compute mutual information
+    if mi_type == 'cc':
+        # reshape y, only if needed
+        if y.ndim in (1, 2):
+            y = np.atleast_2d(y)[np.newaxis, ...]
+            y = np.tile(y, (x.shape[0], 1, 1))
+        _mi = mi_nd_gg(x, y, **kw_mi)
+    elif mi_type == 'cd':
+        _mi = mi_model_nd_gd(x, y, **kw_mi)
+
+    # normalize the mi
+    if minorm:
+        kw_ent = dict(mvaxis=-2, traxis=-1, biascorrect=kw_mi["biascorrect"],
+                      shape_checking=False)
+        _ent_x = ent_nd_g(x, **kw_ent)
+        _ent_y = ent_nd_g(np.atleast_2d(y).astype(float), **kw_ent)
+        _ent_xy = np.minimum(_ent_x, _ent_y)
+        _mi /= _ent_xy
+
+    return _mi
```

### Comparing `frites-0.4.3/frites/core/__init__.py` & `frites-0.4.4/frites/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 """
 from .copnorm import (copnorm_1d, copnorm_cat_1d, copnorm_nd, copnorm_cat_nd)  # noqa
 from .gcmi_1d import (ent_1d_g, mi_1d_gg, gcmi_1d_cc, mi_model_1d_gd,  # noqa
                       gcmi_model_1d_cd, mi_mixture_1d_gd, gcmi_mixture_1d_cd,
                       cmi_1d_ggg, gccmi_1d_ccc, gccmi_1d_ccd, cmi_1d_ggd)
 from .gcmi_nd import (mi_nd_gg, mi_model_nd_gd, cmi_nd_ggg, gcmi_nd_cc,  # noqa
                       gcmi_model_nd_cd, gccmi_nd_ccnd, gccmi_model_nd_cdnd,
-                      gccmi_nd_ccc, cmi_nd_ggd)
+                      gccmi_nd_ccc, cmi_nd_ggd, ent_nd_g)
```

### Comparing `frites-0.4.3/frites/core/copnorm.py` & `frites-0.4.4/frites/core/copnorm.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/core/gcmi_1d.py` & `frites-0.4.4/frites/core/gcmi_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,39 +11,44 @@
 """
 import numpy as np
 import scipy as sp
 
 from frites.core import copnorm_nd, copnorm_cat_nd
 
 
-def ent_1d_g(x, biascorrect=True):
+def ent_1d_g(x, biascorrect=True, demeaned=False):
     """Entropy of a Gaussian variable in bits.
 
     H = ent_g(x) returns the entropy of a (possibly multidimensional) Gaussian
     variable x with bias correction.
 
     Parameters
     ----------
     x : array_like
         Array of data of shape (n_epochs,)
     biascorrect : bool | True
         Specifies whether bias correction should be applied to the estimated MI
+    demeaned : bool | False
+        Specifies whether the input data already has zero mean (true if it has
+        been copula-normalized)
 
     Returns
     -------
     hx : float
         Entropy of the gaussian variable (in bits)
     """
     x = np.atleast_2d(x)
     if x.ndim > 2:
         raise ValueError("x must be at most 2d")  # noqa
     nvarx, ntrl = x.shape
 
     # demean data
-    x = x - x.mean(axis=1)[:, np.newaxis]
+    if not demeaned:
+        x = x - x.mean(axis=1)[:, np.newaxis]
+
     # covariance
     c = np.dot(x, x.T) / float(ntrl - 1)
     chc = np.linalg.cholesky(c)
 
     # entropy in nats
     hx = np.sum(np.log(np.diagonal(chc))) + .5 * nvarx * (
         np.log(2 * np.pi) + 1.)
```

### Comparing `frites-0.4.3/frites/core/gcmi_nd.py` & `frites-0.4.4/frites/core/gcmi_nd.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,79 @@
     assert x.ndim == y.ndim
     dims = np.delete(np.arange(x.ndim), -2)
     assert all([x.shape[k] == y.shape[k] for k in dims])
 
 
 ###############################################################################
 ###############################################################################
+#                                  ENTROPY
+###############################################################################
+###############################################################################
+
+
+def ent_nd_g(x, mvaxis=None, traxis=-1, biascorrect=True, demeaned=False,
+             shape_checking=True):
+    """Entropy of a continuous variable.
+
+    Parameters
+    ----------
+    x : array_like
+        Array to consider for computing the entropy.
+    mvaxis : int | None
+        Spatial location of the axis to consider if multi-variate analysis
+        is needed
+    traxis : int | -1
+        Spatial location of the trial axis. By default the last axis is
+        considered
+    biascorrect : bool | True
+        Specifies whether bias correction should be applied to the estimated MI
+    demeaned : bool | False
+        Specifies whether the input data already has zero mean (true if it has
+        been copula-normalized)
+    shape_checking : bool | True
+        Perform a reshape and check that x and y shapes are consistents. For
+        high performances and to avoid extensive memory usage, it's better to
+        already have x and y with a shape of (..., mvaxis, traxis) and to set
+        this parameter to False
+
+    Returns
+    -------
+    mi : array_like
+        The mutual information with the same shape as x and y, without the
+        mvaxis and traxis
+    """
+    if shape_checking:
+        x = nd_reshape(x, mvaxis=mvaxis, traxis=traxis)
+    nvarx, ntrl = x.shape[-2], x.shape[-1]
+
+    # demean data
+    if not demeaned:
+        x -= x.mean(axis=-1, keepdims=True)
+
+    # covariance
+    c = np.einsum('...ij, ...kj->...ik', x, x)
+    c /= float(ntrl - 1.)
+    chc = np.linalg.cholesky(c)
+
+    # entropy in nats
+    hx = np.log(np.einsum('...ii->...i', chc)).sum(-1) + 0.5 * nvarx * (
+        np.log(2 * np.pi) + 1.0)
+
+    ln2 = np.log(2)
+    if biascorrect:
+        psiterms = psi((ntrl - np.arange(1, nvarx + 1).astype(
+            float)) / 2.) / 2.
+        dterm = (ln2 - np.log(ntrl - 1.)) / 2.
+        hx = hx - nvarx * dterm - psiterms.sum()
+
+    return hx / ln2
+
+
+###############################################################################
+###############################################################################
 #                          MUTUAL INFORMATION
 ###############################################################################
 ###############################################################################
 
 
 def mi_nd_gg(x, y, mvaxis=None, traxis=-1, biascorrect=True, demeaned=False,
              shape_checking=True):
```

### Comparing `frites-0.4.3/frites/core/mi_bin_ephy.py` & `frites-0.4.4/frites/core/mi_bin_ephy.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/data/frites.mplstyle` & `frites-0.4.4/frites/data/frites.mplstyle`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/dataset/ds_ephy.py` & `frites-0.4.4/frites/dataset/ds_ephy.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/dataset/ds_utils.py` & `frites-0.4.4/frites/dataset/ds_utils.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/dataset/suj_ephy.py` & `frites-0.4.4/frites/dataset/suj_ephy.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_bin.py` & `frites-0.4.4/frites/estimator/est_bin.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_corr.py` & `frites-0.4.4/frites/estimator/est_corr.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_custom.py` & `frites-0.4.4/frites/estimator/est_custom.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_dcorr.py` & `frites-0.4.4/frites/estimator/est_dcorr.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_gcmi.py` & `frites-0.4.4/frites/estimator/est_gcmi.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_mi_base.py` & `frites-0.4.4/frites/estimator/est_mi_base.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/estimator/est_resampling.py` & `frites-0.4.4/frites/estimator/est_resampling.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/io/io_attributes.py` & `frites-0.4.4/frites/io/io_attributes.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/io/io_syslog.py` & `frites-0.4.4/frites/io/io_syslog.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/plot/plot_conn.py` & `frites-0.4.4/frites/plot/plot_conn.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/simulations/__init__.py` & `frites-0.4.4/frites/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/simulations/sim_ar.py` & `frites-0.4.4/frites/simulations/sim_ar.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/simulations/sim_generate_data.py` & `frites-0.4.4/frites/simulations/sim_generate_data.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/simulations/sim_local_mi.py` & `frites-0.4.4/frites/simulations/sim_local_mi.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/simulations/sim_mi.py` & `frites-0.4.4/frites/simulations/sim_mi.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/stats/__init__.py` & `frites-0.4.4/frites/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/stats/stats_mcp.py` & `frites-0.4.4/frites/stats/stats_mcp.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/stats/stats_nonparam.py` & `frites-0.4.4/frites/stats/stats_nonparam.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/stats/stats_param.py` & `frites-0.4.4/frites/stats/stats_param.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/utils/parallel.py` & `frites-0.4.4/frites/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/utils/perf.py` & `frites-0.4.4/frites/utils/perf.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/utils/preproc.py` & `frites-0.4.4/frites/utils/preproc.py`

 * *Files 18% similar despite different names*

```diff
@@ -377,7 +377,111 @@
         x_n = x
 
     # add normalizatoin information to xarray
     if isinstance(x_n, (xr.DataArray, xr.Dataset)):
         x_n.attrs['to_min'], x_n.attrs['to_max'] = to_min, to_max
 
     return x_n
+
+
+def split_group(x, names=None, axis='roi', new_axis='subjects', average=False):
+    """Split data group.
+
+    This function can be used to reorganize a list of matrices. For example,
+    if you have a list storing the data of n_subjects :
+
+    .. math::
+
+        data = [(roi_{1}, times), (roi_{2}, times), (roi_{3}, times)]
+
+    the data can be reorganized to become a list of brain regions with
+
+    .. math::
+
+        reshaped = [(suj_{1}, times), (suj_{2}, times), (suj_{3}, times)]
+
+    Parameters
+    ----------
+    x : list
+        List of xarray.DataArray, potentially multidimensional
+    names : list | None
+        List of names associated to each element of the list. Should have the
+        same length as x.
+    axis : str | 'roi'
+        Axis name along which data should be splitted. By default, the function
+        performs a spatial split over the 'roi' dimension
+    new_axis : str | 'subjects'
+        New name replacing axis. By default, the function is going to
+        concatenate over a new axis called 'subjects'
+    average : bool | False
+        If repeated coordinates are present for each element of the list (e.g.
+        repeated brain region names for a single subject), allow to take the
+        average over repeated coordinates.
+
+    Returns
+    -------
+    reshaped : list
+        List of reshaped xarray.DataArray
+    u_names : list
+        List of unique names describing each element of the reshaped data
+    """
+    assert isinstance(x, (list, tuple))
+    assert all([isinstance(k, xr.DataArray) and axis in k.dims for k in x])
+
+    # define element names
+    if names is None:
+        names = np.arange(len(x))
+    names = np.asarray(names)
+    assert len(names) == len(x)
+
+    # get list of non-sorted unique roi
+    all_roi = [r[axis].data for r in x]
+    u_roi = nonsorted_unique(np.concatenate(all_roi))
+
+    # split the data
+    x_split = []
+    for r in u_roi:
+        x_roi, suj_roi = [], []
+        for n_s, s in zip(names, x):
+            # skip if roi is absent (ieeg)
+            if r not in s[axis]:
+                continue
+
+            # boolean selection
+            _x = s.isel(**{axis: np.where(s[axis].data == r)[0]})
+
+            # average (if required)
+            if average and (len(_x[axis]) > 1):
+                _x = _x.mean(axis, keepdims=True)
+
+            x_roi.append(_x)
+            suj_roi += [n_s] * len(_x[axis])
+
+        # merge over a new subject dimension
+        x_roi = xr.concat(x_roi, axis).rename({axis: new_axis})
+        x_roi[new_axis] = suj_roi
+        x_split.append(x_roi)
+
+    return x_split, u_roi
+
+
+if __name__ == '__main__':
+    n_suj = 4
+    n_times = 100
+    times = np.linspace(-.5, 1.5, n_times)
+
+    x = []
+    for i in range(n_suj):
+        _x = np.random.rand(np.random.randint(1, 10, (1,))[0], n_times)
+
+        # turn it into an xarray
+        roi = np.array([f"roi_{r}" for r in range(_x.shape[0])])
+        if len(roi) > 1:
+            roi[1] = roi[0]
+        _x = xr.DataArray(
+            _x, dims=['space', 'times'], coords=(roi, times)
+        )
+        x.append(_x)
+
+    x_split, u_roi = split_group(x, axis='space')
+    x_back, u_suj = split_group(x_split, names=u_roi, axis='subjects',
+                                new_axis='roi')
```

### Comparing `frites-0.4.3/frites/utils/wrapper.py` & `frites-0.4.4/frites/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/workflow/__init__.py` & `frites-0.4.4/frites/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/workflow/wf_base.py` & `frites-0.4.4/frites/workflow/wf_base.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/workflow/wf_conn_comod.py` & `frites-0.4.4/frites/workflow/wf_conn_comod.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/workflow/wf_mi.py` & `frites-0.4.4/frites/workflow/wf_mi.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/workflow/wf_mi_combine.py` & `frites-0.4.4/frites/workflow/wf_mi_combine.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites/workflow/wf_stats.py` & `frites-0.4.4/frites/workflow/wf_stats.py`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/frites.egg-info/PKG-INFO` & `frites-0.4.4/frites.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: frites
-Version: 0.4.3
+Version: 0.4.4
 Summary: Framework of Information Theory for Electrophysiological data and Statistics
 Home-page: https://github.com/brainets/frites
-Download-URL: https://github.com/brainets/frites/archive/v0.4.3.tar.gz
+Download-URL: https://github.com/brainets/frites/archive/v0.4.4.tar.gz
 Author: BraiNets
 Author-email: e.combrisson@gmail.com
 Maintainer: Etienne Combrisson
 License: BSD 3-Clause License
 Keywords: information-theory statistics
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: flake
 Provides-Extra: full
 License-File: LICENSE
 
+.. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/logo_desc.png
+    :align:  center
+
+
+Frites
+======
+
 .. image:: https://github.com/brainets/frites/actions/workflows/test_doc.yml/badge.svg
     :target: https://github.com/brainets/frites/actions/workflows/test_doc.yml
 
 .. image:: https://github.com/brainets/frites/actions/workflows/flake.yml/badge.svg
     :target: https://github.com/brainets/frites/actions/workflows/flake.yml
 
 .. image:: https://travis-ci.org/brainets/frites.svg?branch=master
@@ -37,36 +46,50 @@
 
 .. image:: https://badge.fury.io/py/frites.svg
     :target: https://badge.fury.io/py/frites
 
 .. image:: https://pepy.tech/badge/frites
     :target: https://pepy.tech/project/frites
 
-.. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/logo_desc.png
-    :align:  center
+.. image:: https://zenodo.org/badge/213869364.svg
+    :target: https://zenodo.org/badge/latestdoi/213869364
+
+.. image:: https://joss.theoj.org/papers/437a7362501b2ea984e1d4fed4646076/status.svg
+    :target: https://joss.theoj.org/papers/437a7362501b2ea984e1d4fed4646076
+
+
+.. _Documentation: https://brainets.github.io/frites/
+.. |Documentation| replace:: **Documentation**
+
+.. _Installation: https://brainets.github.io/frites/install.html
+.. |Installation| replace:: **Installation**
+
+.. _Usage: https://brainets.github.io/frites/auto_examples/index.html
+.. |Usage| replace:: **Usage example**
+
+.. _API: https://brainets.github.io/frites/api/index.html
+.. |API| replace:: **List of functions**
+
+.. _Cite: https://brainets.github.io/frites/overview/ovw_cite.html
+.. |Cite| replace:: **Cite Frites**
+
+|Documentation|_ | |Installation|_ | |Usage|_ | |API|_ | |Cite|_
 
-======
-Frites
-======
 
 Description
------------
+===========
 
-`Frites <https://brainets.github.io/frites/>`_ is a Python toolbox for assessing information-theorical measures on human and animal neurophysiological data (M/EEG, Intracranial). The aim of Frites is to extract task-related cognitive brain networks (i.e modulated by the task). The toolbox also includes directed and undirected connectivity metrics such as group-level statistics.
+`Frites <https://brainets.github.io/frites/>`_ is a Python toolbox for assessing information-theorical measures on human and animal neurophysiological data (M/EEG, Intracranial). The aim of Frites is to extract task-related cognitive brain networks (i.e modulated by the task). The toolbox also includes directed and undirected connectivity metrics such as group-level statistics. Frites documentation is available online at https://brainets.github.io/frites/
 
 .. figure::  https://github.com/brainets/frites/blob/master/docs/source/_static/network_framework.png
     :align:  center
 
-Documentation
--------------
-
-Frites documentation is available online at https://brainets.github.io/frites/
 
 Installation
-------------
+============
 
 Run the following command into your terminal to get the latest stable version :
 
 .. code-block:: shell
 
     pip install -U frites
 
@@ -102,10 +125,10 @@
 
 * `Numba <http://numba.pydata.org/>`_ : speed up the computations of some functions
 * `Dcor <https://dcor.readthedocs.io/en/latest/>`_ for fast implementation of distance correlation
 * `Matplotlib <https://matplotlib.org/>`_, `Seaborn <https://seaborn.pydata.org/>`_ and `Networkx <https://networkx.github.io/>`_ for plotting the examples
 * Some example are using `scikit learn <https://scikit-learn.org/stable/index.html>`_ estimators
 
 Acknowledgments
----------------
+===============
 
 See `acknowledgments <https://brainets.github.io/frites/overview/ovw_acknowledgments.html>`_
```

### Comparing `frites-0.4.3/frites.egg-info/SOURCES.txt` & `frites-0.4.4/frites.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 frites.egg-info/requires.txt
 frites.egg-info/top_level.txt
 frites/conn/__init__.py
 frites/conn/conn_ccf.py
 frites/conn/conn_covgc.py
 frites/conn/conn_dfc.py
 frites/conn/conn_fcd_corr.py
+frites/conn/conn_fit.py
+frites/conn/conn_ii.py
 frites/conn/conn_io.py
+frites/conn/conn_pid.py
 frites/conn/conn_sliding_windows.py
 frites/conn/conn_spec.py
 frites/conn/conn_te.py
 frites/conn/conn_tf.py
 frites/conn/conn_utils.py
 frites/core/__init__.py
 frites/core/copnorm.py
```

### Comparing `frites-0.4.3/frites.egg-info/requires.txt` & `frites-0.4.4/frites.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `frites-0.4.3/setup.py` & `frites-0.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # License: 3-clause BSD
 import os
 from setuptools import setup, find_packages
 
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 NAME = 'frites'
 AUTHOR = "BraiNets"
 MAINTAINER = "Etienne Combrisson"
 EMAIL = 'e.combrisson@gmail.com'
 KEYWORDS = "information-theory statistics"
 DESCRIPTION = ("Framework of Information Theory for Electrophysiological data "
                "and Statistics")
@@ -63,10 +63,12 @@
     download_url=DOWNLOAD_URL,
     license="BSD 3-Clause License",
     keywords=KEYWORDS,
     classifiers=["Development Status :: 5 - Production/Stable",
                  'Intended Audience :: Science/Research',
                  'Intended Audience :: Education',
                  'Intended Audience :: Developers',
-                 "Programming Language :: Python :: 3.7",
-                 "Programming Language :: Python :: 3.8"
+                 "Programming Language :: Python :: 3.8",
+                 "Programming Language :: Python :: 3.9",
+                 "Programming Language :: Python :: 3.10",
+                 "Programming Language :: Python :: 3.11",
                  ])
```


# Comparing `tmp/configurun-0.2.2.tar.gz` & `tmp/configurun-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configurun-0.2.2.tar", last modified: Thu Jul  6 16:11:10 2023, max compression
+gzip compressed data, was "configurun-0.2.3.tar", last modified: Thu Jul  6 21:55:44 2023, max compression
```

## Comparing `configurun-0.2.2.tar` & `configurun-0.2.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.681369 configurun-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-07-06 16:11:01.000000 configurun-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 16:11:01.000000 configurun-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-06 16:11:10.681369 configurun-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-06 16:11:01.000000 configurun-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/create_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45915 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/models/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/models/run_queue_console_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/models/run_queue_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/network_main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/network_login_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/run_queue_widget_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/views/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/views/run_queue_tree_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/widgets/network_login_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/widgets/run_queue_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/method_call_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    54072 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/argparse_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/configuration_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_configuration_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/examples/example_options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_options/example_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_options/example_sklearn_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_target_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1155777 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/res/app_resources_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/server/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/server/create_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:11:10.681369 configurun-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 16:11:01.000000 configurun-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.629800 configurun-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-07-06 21:55:33.000000 configurun-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 21:55:33.000000 configurun-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-06 21:55:44.629800 configurun-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-06 21:55:33.000000 configurun-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/create_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45915 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun/app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/models/run_queue_console_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/models/run_queue_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/network_main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun/app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/ui/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/ui/network_login_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/ui/run_queue_widget_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun/app/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/views/run_queue_tree_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun/app/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/widgets/network_login_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/app/widgets/run_queue_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.625800 configurun-0.2.3/configurun/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/classes/method_call_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54201 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/classes/run_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/classes/run_queue_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/classes/run_queue_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/classes/run_queue_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.625800 configurun-0.2.3/configurun/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/configuration/argparse_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/configuration/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/configuration/configuration_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.625800 configurun-0.2.3/configurun/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_configuration_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.625800 configurun-0.2.3/configurun/examples/example_options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_options/example_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_options/example_sklearn_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/examples/example_target_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.625800 configurun-0.2.3/configurun/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1155777 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/res/app_resources_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.629800 configurun-0.2.3/configurun/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-06 21:55:33.000000 configurun-0.2.3/configurun/server/create_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:55:44.621800 configurun-0.2.3/configurun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-06 21:55:44.000000 configurun-0.2.3/configurun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 21:55:44.000000 configurun-0.2.3/configurun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:55:44.000000 configurun-0.2.3/configurun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 21:55:44.000000 configurun-0.2.3/configurun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 21:55:44.000000 configurun-0.2.3/configurun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:55:44.629800 configurun-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 21:55:33.000000 configurun-0.2.3/setup.py
```

### Comparing `configurun-0.2.2/LICENSE` & `configurun-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/PKG-INFO` & `configurun-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configurun
-Version: 0.2.2
+Version: 0.2.3
 Summary: Cross-platform user-interface tools to create and manage (machine learning) configurations and run them automatically and remotely.
 Home-page: https://github.com/Woutah/configurun
 Author: Wouter Stokman
 License: LGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `configurun-0.2.2/README.md` & `configurun-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/create_run.py` & `configurun-0.2.3/configurun/app/create_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 	handler = logging.StreamHandler()
 	handler.setFormatter(formatter)
 	logging.basicConfig(
 		handlers=[handler],
 		level=log_level) #Without time
 	root_logger = logging.getLogger()
 	root_logger.setLevel(log_level)
+	root_logger.handlers=[handler]
 
 
 	if config_model_kwargs is None:
 		config_model_kwargs = {}
 
 	app = QtWidgets.QApplication(sys.argv)
```

### Comparing `configurun-0.2.2/configurun/app/main_window.py` & `configurun-0.2.3/configurun/app/main_window.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/models/run_queue_console_model.py` & `configurun-0.2.3/configurun/app/models/run_queue_console_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,18 +96,32 @@
 
 	def on_commandline_output(self,
 			   					item_id : int,
 								name : str,
 								output_path : str,
 								edit_dt : datetime.datetime,
 								filepos : int,
-								msg : str
+								msg : str,
+								emit_datachanged : bool = True 
 							): # pylint: disable=unused-argument
 		"""Called when new command line output is received, inserts the new text into the buffer and emits 
-		the currentTextChanged signal if the buffer changed"""
+		the currentTextChanged signal if the buffer changed
+		
+		Args:
+			item_id (int): The id of the item for which the output is received
+			name (str): The name of the item
+			output_path (str): The path of the item
+			edit_dt (datetime.datetime): The last (known) change to the output file
+			filepos (int): The start-position where the new text should be inserted
+			msg (str): The new text message
+			emit_datachanged (bool, optional): Whether to emit the dataChanged signal if metadata changed. 
+				Defaults to True. Set to false when using this function when resetting a model that uses this item
+				to avoid emitting the dataChanged signal before the data of the model is fully reset.
+		
+		"""
 		if item_id != self._id: #Skip if not the correct id
 			return
 		if name != self._name:
 			raise ValueError(f"Name mismatch: {name} != {self._name} but id is the same - should not happen")
 
 		data_changed = False #Whether the node-data itself changed (e.g. name (namechange not implemented) or edit_dt
 
@@ -158,15 +172,15 @@
 				self._current_text + ("X" * (filepos - len(self._current_text)))
 			new_text += msg
 			self._current_text = new_text +(self._current_text[filepos + len(msg):] \
 				if len(self._current_text) > filepos else "")
 
 
 		self.currentTextChanged.emit(self._current_text)
-		if data_changed: #If the metadata changed, emit the dataChanged signal
+		if data_changed and emit_datachanged: #If the metadata changed, emit the dataChanged signal
 			self.dataChanged.emit()
 			# if filepos + len(msg) > len(self._current_text):
 
 	def get_current_text(self) -> str:
 		return self._current_text
 
 	def data(self, role : QtCore.Qt.ItemDataRole, column : int = 0):
@@ -197,26 +211,43 @@
 
 
 class RunQueueConsoleModel(QtCore.QAbstractItemModel):
 	"""
 	A RunQueue model that synchronizes with text-output from running items in the runqueue by requesting all text-data
 	from the runqueue upon connection, and then subscribing to any changes to the text-output of the items
 	running in the runqueue.
+
+	On reset, will try to fetch the history of the consoles using the runqueue fetch methods.
 	"""
 
 
-	def __init__(self, parent: QtWidgets.QWidget | None = None) -> None:
+	def __init__(self, 
+	    		parent: QtWidgets.QWidget | None = None,
+				max_initial_console_history : int = 200_000
+			) -> None:
+		"""Initializes the runqueueconsolemodel
+
+		Args:
+			parent (QtWidgets.QWidget | None, optional): The parent. Defaults to None.
+			max_initial_console_history (int, optional): Limits the max amount of characters that the model will 
+				fetch on-reset (per item) this makes sure that the initial load times on model-reset do not become 
+				too outrageous by only loading part of the data. Especially useful useful when working over network 
+				connections. NOTE: this limit is not enforced when gradually loading data from the runqueue as 
+				we assume that it's not feasible to load too much text-data in a single session.
+				Defaults to 200_000. -1 for no limit.
+		"""
+
 		super().__init__(parent)
 		self._run_queue = None
 		self._id_item_map_mutex = threading.Lock()
 		self._id_item_map : typing.OrderedDict[int, RunQueueConsoleItem] = OrderedDict({}) #Maps run queue id to item
 			# Note: we use an ordered dict to keep a consistent item-order for the UI
-		self._id_order : typing.List[int] = [] #The order of the ids in the model
 		self._ignored_ids : typing.Set[int] = set() #Ids that are ignored/not tracked
 
+		self._max_initial_console_history = max_initial_console_history
 
 		self._new_cmd_text_signal : QtCore.SignalInstance | None= None
 		self._active_ids_signal : QtCore.SignalInstance | None = None
 		self._queue_reset_signal : QtCore.SignalInstance | None = None
 
 	def set_run_queue(self, run_queue : RunQueue):
 		"""Set the runqueue to synchronize with
@@ -253,25 +284,34 @@
 		if self._run_queue is not None:
 			cur_queue = self._run_queue.get_command_line_info_list()
 			if cur_queue:
 				for cur_id, (name, path, file_size, running) in cur_queue.items():
 					if cur_id in self._ignored_ids:
 						continue
 					item = RunQueueConsoleItem(cur_id, name, path, running)
-					self.append_row(item)
+					self._append_row(item)
 
-					all_txt, last_edit_dt = self._run_queue.get_command_line_output(cur_id, -1, file_size)
+					if self._max_initial_console_history > 0 and file_size > self._max_initial_console_history: #if limit to initial console history
+						all_txt, last_edit_dt = self._run_queue.get_command_line_output(
+							cur_id, -1, self._max_initial_console_history) #TODO: this probably goes wrong if we resume
+							# logging on an existing logfile, as we will "start again" at filepos 0
+							# while the actual filepos = file_size-self._max_initial_console_history.
+							# probably best to put a start_pos inside run_queue_item 
+					else: #Fetch all data NOTE: this can be very costly, especially over network connections
+						all_txt, last_edit_dt = self._run_queue.get_command_line_output(cur_id, -1, file_size)
 					item.on_commandline_output( #Append all text to the item #TODO: do this before reading file to avoid
 							# missing any of the data that was added during reading
 						item_id=cur_id,
 						name=name,
 						output_path=path,
 						edit_dt=last_edit_dt,
 						filepos=0,
-						msg=all_txt
+						msg=all_txt,
+						emit_datachanged=False #Don't emit changes, otherwise we will try to update items that are not
+							# yet known to the model
 					) #TODO: maybe only import active items?
 
 
 
 		self.endResetModel()
 		log.info("Done resetting RunQueueConsoleModel")
 
@@ -370,34 +410,46 @@
 	# 				continue
 	# 			item = RunQueueConsoleItem(id, name, path)
 	# 			with self._id_item_map_mutex:
 	# 				self._id_item_map[id] = item
 	# 			self.appendRow(item)
 	# 	self.endResetModel()
 
-	def append_row(self, item : RunQueueConsoleItem):
-		"""Append a row to the model - consisting of a single ConsoleStandardItem
+	def _append_row(self, item : RunQueueConsoleItem):
+		"""Append a row to the model - consisting of a single ConsoleStandardItem.
+		NOTE: this is the same as appendRow, but without the begin/endInsertRows calls, better to be used during model
+		reset to avoid emitting dataChanged/rowInserted signals for new items as this might cause issues when 
+		begin/endresetModel is called during a reset
+		
 		Args:
 			item (ConsoleStandardItem): The item to append (each row corresponds to 1 item)
 		"""
-		self.beginInsertRows(QtCore.QModelIndex(), self.rowCount(), self.rowCount()) #No parent, insert at end
 		cur_item_id = item.get_id()
 		with self._id_item_map_mutex:
 			assert cur_item_id not in self._id_item_map, "Item with this ID already in model"
 			self._id_item_map[cur_item_id] = item
 			#TODO: only emit dataChanged for this item
 		item.dataChanged.connect(
 			# lambda *args: print(f"Data changed for item {item._id}")
 			lambda item_id=cur_item_id: self.dataChanged.emit(
 				# self.index(0, 0),
 				# self.index(self.rowCount()-1, self.columnCount()-1))
 				self.index(list(self._id_item_map.keys()).index(item_id), 0),
 				self.index(list(self._id_item_map.keys()).index(item_id), self.columnCount()-1))
 		)
 
+
+
+	def append_row(self, item : RunQueueConsoleItem):
+		"""Append a row to the model - consisting of a single ConsoleStandardItem
+		Args:
+			item (ConsoleStandardItem): The item to append (each row corresponds to 1 item)
+		"""
+		self.beginInsertRows(QtCore.QModelIndex(), self.rowCount(), self.rowCount()) #No parent, insert at end
+		self._append_row(item)
 		self.endInsertRows()
 
 	def removeRow(self, row: int, parent : QtCore.QModelIndex) -> None:
 		self.beginRemoveRows(parent, row, row)
 		item_id = list(self._id_item_map.keys())[row]
 		with self._id_item_map_mutex:
 			del self._id_item_map[item_id]
```

### Comparing `configurun-0.2.2/configurun/app/models/run_queue_table_model.py` & `configurun-0.2.3/configurun/app/models/run_queue_table_model.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/network_main_window.py` & `configurun-0.2.3/configurun/app/network_main_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,20 +121,28 @@
 		self.network_connection_widget.cancelClicked.connect(lambda *_: self.connection_window.close())
 		self.network_connection_widget.cancelClicked.connect(lambda *_: self.network_connection_widget.save_histories())
 
 		self.network_connection_widget.connectClicked.connect(
 			lambda *_: self.network_connection_widget.save_histories()
 		)
 
-		self.reconnect_button_1.clicked.connect(self.connection_window.show)
-		self.reconnect_button_2.clicked.connect(self.connection_window.show)
-		#Also move window to front
+
+		#========= Make sure window is shown when (re)connecting ==========
 		self.reconnect_button_1.clicked.connect(lambda *_: self.connection_window.activateWindow())
 		self.reconnect_button_2.clicked.connect(lambda *_: self.connection_window.activateWindow())
+		self.reconnect_button_1.clicked.connect(lambda *_: self.connection_window.show())
+		self.reconnect_button_1.clicked.connect(lambda *_: self.connection_window.setFocus())
+		self.reconnect_button_2.clicked.connect(lambda *_: self.connection_window.show())
+		self.reconnect_button_2.clicked.connect(lambda *_: self.connection_window.setFocus())
+		self.reconnect_button_1.clicked.connect(lambda *_: self.connection_window.raise_())
+		self.reconnect_button_2.clicked.connect(lambda *_: self.connection_window.raise_())
+		#Also move window to front
+		self.open_connection_action.triggered.connect(self.connection_window.setFocus())
 		self.open_connection_action.triggered.connect(self.connection_window.show)
+		self.open_connection_action.triggered.connect(lambda *_: self.connection_window.raise_())
 
 
 
 	def initial_run_queue_load(self) -> None:
 		"""Since this is a client, don't load any RunQueue on startup."""
 
 	def check_if_running_ask_stop_items_before_close(self) -> bool:
```

### Comparing `configurun-0.2.2/configurun/app/ui/main_window_ui.py` & `configurun-0.2.3/configurun/app/ui/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/ui/network_login_widget_ui.py` & `configurun-0.2.3/configurun/app/ui/network_login_widget_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/ui/run_queue_widget_ui.py` & `configurun-0.2.3/configurun/app/ui/run_queue_widget_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/views/run_queue_tree_view.py` & `configurun-0.2.3/configurun/app/views/run_queue_tree_view.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/widgets/network_login_widget.py` & `configurun-0.2.3/configurun/app/widgets/network_login_widget.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/app/widgets/run_queue_widget.py` & `configurun-0.2.3/configurun/app/widgets/run_queue_widget.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/classes/method_call_interceptor.py` & `configurun-0.2.3/configurun/classes/method_call_interceptor.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/classes/run_queue.py` & `configurun-0.2.3/configurun/classes/run_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,16 +476,19 @@
 
 			last_edit_dt = datetime.fromtimestamp(os.path.getmtime(self._cmd_id_name_path_dict[item_id][1]))
 			filepath = self._cmd_id_name_path_dict[item_id][1]
 
 		with open(filepath, "r", encoding="utf-8") as read_file:
 			if fseek_end == -1 and max_bytes == -1: #If just reading the whole file
 				return read_file.read(), last_edit_dt
-			elif fseek_end == -1: #If reading from the end of the file
-				read_file.seek(0, max(0, os.SEEK_END - max_bytes))
+			elif fseek_end == -1: #If reading to the end of the file
+				#Start reading x bytes from the end of the file
+				read_file.seek(0, os.SEEK_END)
+				file_size = read_file.tell()
+				read_file.seek(max(0, file_size - max_bytes), os.SEEK_SET)
 			if max_bytes == -1:
 				return read_file.read(), last_edit_dt
 
 			return read_file.read(max_bytes), last_edit_dt
 
 	def get_command_line_info_list(self) -> typing.Dict[int, typing.Tuple[str, str, int, bool]]:
 		"""
```

### Comparing `configurun-0.2.2/configurun/classes/run_queue_client.py` & `configurun-0.2.3/configurun/classes/run_queue_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 		self._method_reponse_dict_lock = threading.Lock()
 		self._method_id_counter = 0 #Used to keep track of which function call is which
 
 		self._connected_or_connecting = False #Used to make sure that we're only attempting 1 connection at a time
 
 		self._disconnect_flag = True #Whether to stop listening to the server
 
+		self._await_response_lock = threading.Lock() 
+
 
 	def is_connected(self):
 		"""Returns whether the client is currently trying to connect to the server or is connected to the server
 
 		Returns:
 			bool: Whether the client is currently trying to connect to the server or is connected to the server
 				This doesn't indicate that the connection has been accepted by the server yet
@@ -157,37 +159,39 @@
 						args,
 						kwargs
 					)
 				)
 			),
 			aes_cypher_key= self._aes_session_key
 		)
-
-		if function_name == self.get_command_line_output.__name__: #TODO: might be a more elegant way to do this, maybe
-			# request data in multiple chunks? Probably best to limit console-mirror-size as >50mb files
-			# are not very UI-friendly
-			self._await_method_response(method_call_id, timeout=20) #Since log file can be quite large, wait longer
-
-		return self._await_method_response(method_call_id, timeout=5) #Wait for the server to respond to the method call
-			#and return the result
+		try:
+			if function_name == self.get_command_line_output.__name__: #TODO: might be a more elegant way to do this, maybe
+				# request data in multiple chunks? Probably best to limit console-mirror-size as >50mb files
+				# are not very UI-friendly
+				return self._await_method_response(method_call_id, timeout=5) #Since log file can be quite large, wait longer
+
+			return self._await_method_response(method_call_id, timeout=3) #Wait for the server to respond to the method call
+				#and return the result
+		except TimeoutError as exception:
+			log.error(f"Timeout while waiting for response of {function_name}(...) with id {method_call_id} - {exception}")
+			# raise exception
+			return None
 
 	def _await_method_response(self, function_response_id : int, timeout : float):
 		"""
 		Wait for server response after a function call. Response is automatically put in reponse_dict by the server-
 		listener. If, after timeout, no response is received in this dict, a TimeoutError is raised.
 		"""
 		return_queue = self._method_response_dict[function_response_id]
 		try:
 			ret = return_queue.get(block=True, timeout=timeout)
-			log.info(f"Received response from server for method call with id {function_response_id}, response: {ret} "
-	    		f"of type {type(ret)}"
-			)
-		except (TimeoutError, queue.Empty) as exception: #If the queue is empty, then the server did not respond in time
-			raise TimeoutError(f"Timeout while waiting ({timeout}s) for response of method call with \
-		    	id {function_response_id}") from exception
+			log.info(f"Received response from server for method call with id {function_response_id} of type {type(ret)}")
+		except (TimeoutError, queue.Empty) as exception: #If the queue is empty, then the server did not respond in time #pylint: unused-variable
+			raise TimeoutError(f"Timeout while waiting ({timeout}s) for response of method call with" 
+		    	f"id {function_response_id}") #from exception
 		finally: #Always clean up the queue to no longer listen for this id
 			with self._method_reponse_dict_lock:
 				del self._method_response_dict[function_response_id]
 
 		if isinstance(ret, Exception): #Do not return exception types -> raise them instead #TODO: is this what we want?
 			ret.args = (f"Exception raised by server while executing method call with id {function_response_id}: \
 	       		{ret.args[0]}",) + ret.args[1:]
```

### Comparing `configurun-0.2.2/configurun/classes/run_queue_datatypes.py` & `configurun-0.2.3/configurun/classes/run_queue_datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import dill
 from Crypto.Cipher import AES
 from Crypto.PublicKey import RSA
 from Crypto.Random import get_random_bytes
 
 RSA_KEY_SIZE_BITS = 2048 #The size of the key used for encryption/decryption
 PASSWORD_HASH_SIZE = 512 #The size of the password hash in bytes
+MAX_RECV_SIZE = 65_536 #The maximum size of a TCP-package in bytes which we recv per iteration 2^16
 AES_KEY_SIZE = 32 #The size of the used AES key in bytes
 AES_EMPTY_KEY = b"\x00"*16 #16 bytes of "0" - not used when not encrypted
 
 class AuthenticationException(Exception):
 	"""When an error occurs during the authentication process, or when authentication is invalidated
 	"""
 
@@ -294,15 +295,22 @@
 
 		#Receive the transmission data
 		transmission_size = recv_socket.recv(4)
 		transmission_size = c_uint32.from_buffer_copy(transmission_size).value #Read in uint32, convert to python type
 
 		aes_nonce = recv_socket.recv(16) #Receive the nonce used for AES encryption
 
-		data = recv_socket.recv(transmission_size)
+		# data = recv_socket.recv(transmission_size) #NOTE: recv does not guarantee that all data is received
+		#We loop and use recv() until we have received all data using MAX_PACKET_SIZE as the max size of a packet
+		data = bytearray()
+		while len(data) < transmission_size:
+			data.extend(recv_socket.recv(MAX_RECV_SIZE))
+
+		assert(len(data) == transmission_size),\
+			f"Received transmission size {transmission_size} does not match the received data size {len(data)}"
 
 		if aes_cipher_key is not None:
 			aes_cipher = AES.new(aes_cipher_key, AES.MODE_EAX, nonce=aes_nonce)
 			data = aes_cipher.decrypt(data)
 
 
 		new_transmission = Transmission(
```

### Comparing `configurun-0.2.2/configurun/classes/run_queue_server.py` & `configurun-0.2.3/configurun/classes/run_queue_server.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/configuration/argparse_to_dataclass.py` & `configurun-0.2.3/configurun/configuration/argparse_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/configuration/base_options.py` & `configurun-0.2.3/configurun/configuration/base_options.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/configuration/configuration.py` & `configurun-0.2.3/configurun/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/configuration/configuration_model.py` & `configurun-0.2.3/configurun/configuration/configuration_model.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/examples/example_argparse.py` & `configurun-0.2.3/configurun/examples/example_argparse.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/examples/example_configuration.py` & `configurun-0.2.3/configurun/examples/example_configuration.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/examples/example_configuration_sklearn.py` & `configurun-0.2.3/configurun/examples/example_configuration_sklearn.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/examples/example_options/example_options.py` & `configurun-0.2.3/configurun/examples/example_options/example_options.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/examples/example_options/example_sklearn_options.py` & `configurun-0.2.3/configurun/examples/example_options/example_sklearn_options.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/examples/example_target_function.py` & `configurun-0.2.3/configurun/examples/example_target_function.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/res/app_resources_rc.py` & `configurun-0.2.3/configurun/res/app_resources_rc.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun/server/create_server.py` & `configurun-0.2.3/configurun/server/create_server.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/configurun.egg-info/PKG-INFO` & `configurun-0.2.3/configurun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configurun
-Version: 0.2.2
+Version: 0.2.3
 Summary: Cross-platform user-interface tools to create and manage (machine learning) configurations and run them automatically and remotely.
 Home-page: https://github.com/Woutah/configurun
 Author: Wouter Stokman
 License: LGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `configurun-0.2.2/configurun.egg-info/SOURCES.txt` & `configurun-0.2.3/configurun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configurun-0.2.2/setup.py` & `configurun-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The setup script."""
 from setuptools import setup, find_packages
 
 
 setup(
 	name = "configurun",
-	version= "0.2.2",
+	version= "0.2.3",
 	packages=find_packages('.'),
     description=("Cross-platform user-interface tools to create and manage (machine learning) configurations and run them automatically and remotely."),
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author="Wouter Stokman",
     url="https://github.com/Woutah/configurun",
     license="LGPLv2",
```


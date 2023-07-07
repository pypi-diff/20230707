# Comparing `tmp/hahomematic-2023.6.1.tar.gz` & `tmp/hahomematic-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.6.1.tar", last modified: Sun Jun 25 17:57:41 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.0.tar", last modified: Fri Jul  7 13:16:51 2023, max compression
```

## Comparing `hahomematic-2023.6.1.tar` & `hahomematic-2023.7.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.277757 hahomematic-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-25 17:57:41.277757 hahomematic-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.273757 hahomematic-2023.6.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.273757 hahomematic-2023.6.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24401 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    50693 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46635 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.273757 hahomematic-2023.6.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.273757 hahomematic-2023.6.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.277757 hahomematic-2023.6.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.277757 hahomematic-2023.6.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.277757 hahomematic-2023.6.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:57:41.273757 hahomematic-2023.6.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-25 17:57:40.000000 hahomematic-2023.6.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-25 17:57:41.000000 hahomematic-2023.6.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:57:40.000000 hahomematic-2023.6.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:57:39.000000 hahomematic-2023.6.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-25 17:57:41.000000 hahomematic-2023.6.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 17:57:41.000000 hahomematic-2023.6.1/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-06-25 17:57:05.000000 hahomematic-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-25 17:57:41.277757 hahomematic-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.464514 hahomematic-2023.7.0/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50689 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46635 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:16:51.468515 hahomematic-2023.7.0/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-07 13:16:50.000000 hahomematic-2023.7.0/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-07 13:16:51.000000 hahomematic-2023.7.0/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:16:50.000000 hahomematic-2023.7.0/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:16:49.000000 hahomematic-2023.7.0/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-07 13:16:51.000000 hahomematic-2023.7.0/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 13:16:51.000000 hahomematic-2023.7.0/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-07 13:15:53.000000 hahomematic-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 13:16:51.472515 hahomematic-2023.7.0/setup.cfg
```

### Comparing `hahomematic-2023.6.1/LICENSE` & `hahomematic-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/PKG-INFO` & `hahomematic-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.6.1/README.md` & `hahomematic-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/__init__.py` & `hahomematic-2023.7.0/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/backport.py` & `hahomematic-2023.7.0/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.0/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/caches/persistent.py` & `hahomematic-2023.7.0/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/caches/visibility.py` & `hahomematic-2023.7.0/hahomematic/caches/visibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,11 +667,10 @@
     if compare_with is None:
         return None
 
     for key, value in search_elements.items():
         if do_wildcard_search:
             if key.lower().startswith(compare_with.lower()):
                 return value
-        else:
-            if key.lower() == compare_with.lower():
-                return value
+        elif key.lower() == compare_with.lower():
+            return value
     return None
```

### Comparing `hahomematic-2023.6.1/hahomematic/central_unit.py` & `hahomematic-2023.7.0/hahomematic/central_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
             _LOGGER.warning(ex)
             raise
 
     def get_client(self, interface_id: str) -> hmcl.Client:
         """Return a client by interface_id. #CC."""
         if not self.has_client(interface_id=interface_id):
             raise HaHomematicException(
-                f"get_client: interface_id {interface_id} " f"does not exist on {self._attr_name}"
+                f"get_client: interface_id {interface_id} does not exist on {self._attr_name}"
             )
         return self._clients[interface_id]
 
     def get_device(self, device_address: str) -> HmDevice | None:
         """Return homematic device. #CC."""
         return self._devices.get(device_address)
```

### Comparing `hahomematic-2023.6.1/hahomematic/client.py` & `hahomematic-2023.7.0/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/const.py` & `hahomematic-2023.7.0/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/decorators.py` & `hahomematic-2023.7.0/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/exceptions.py` & `hahomematic-2023.7.0/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/exporter.py` & `hahomematic-2023.7.0/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/hmcli.py` & `hahomematic-2023.7.0/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.0/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.0/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.0/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/device.py` & `hahomematic-2023.7.0/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/entity.py` & `hahomematic-2023.7.0/hahomematic/platforms/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -563,13 +563,12 @@
                     if not await self._client.set_value(
                         channel_address=channel_address,
                         paramset_key=PARAMSET_KEY_VALUES,
                         parameter=parameter,
                         value=value,
                     ):
                         return False  # pragma: no cover
-            else:
-                if not await self._client.put_paramset(
-                    address=channel_address, paramset_key=PARAMSET_KEY_VALUES, value=paramset
-                ):
-                    return False  # pragma: no cover
+            elif not await self._client.put_paramset(
+                address=channel_address, paramset_key=PARAMSET_KEY_VALUES, value=paramset
+            ):
+                return False  # pragma: no cover
         return True
```

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/event.py` & `hahomematic-2023.7.0/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,40 +74,37 @@
     if parameter_data[HM_OPERATIONS] & OPERATION_WRITE:
         if parameter_data[HM_TYPE] == TYPE_ACTION:
             if parameter_data[HM_OPERATIONS] == OPERATION_WRITE:
                 if parameter in BUTTON_ACTIONS or device.device_type in HM_VIRTUAL_REMOTE_TYPES:
                     entity_t = HmButton
                 else:
                     entity_t = HmAction
+            elif parameter in CLICK_EVENTS:
+                entity_t = HmButton
             else:
-                if parameter in CLICK_EVENTS:
-                    entity_t = HmButton
-                else:
-                    entity_t = HmSwitch
-        else:
-            if parameter_data[HM_OPERATIONS] == OPERATION_WRITE:
-                entity_t = HmAction
-            elif parameter_data[HM_TYPE] == TYPE_BOOL:
                 entity_t = HmSwitch
-            elif parameter_data[HM_TYPE] == TYPE_ENUM:
-                entity_t = HmSelect
-            elif parameter_data[HM_TYPE] == TYPE_FLOAT:
-                entity_t = HmFloat
-            elif parameter_data[HM_TYPE] == TYPE_INTEGER:
-                entity_t = HmInteger
-            elif parameter_data[HM_TYPE] == TYPE_STRING:
-                entity_t = HmText
-    else:
-        if parameter not in CLICK_EVENTS:
-            # Also check, if sensor could be a binary_sensor due to value_list.
-            if is_binary_sensor(parameter_data):
-                parameter_data[HM_TYPE] = TYPE_BOOL
-                entity_t = HmBinarySensor
-            else:
-                entity_t = HmSensor
+        elif parameter_data[HM_OPERATIONS] == OPERATION_WRITE:
+            entity_t = HmAction
+        elif parameter_data[HM_TYPE] == TYPE_BOOL:
+            entity_t = HmSwitch
+        elif parameter_data[HM_TYPE] == TYPE_ENUM:
+            entity_t = HmSelect
+        elif parameter_data[HM_TYPE] == TYPE_FLOAT:
+            entity_t = HmFloat
+        elif parameter_data[HM_TYPE] == TYPE_INTEGER:
+            entity_t = HmInteger
+        elif parameter_data[HM_TYPE] == TYPE_STRING:
+            entity_t = HmText
+    elif parameter not in CLICK_EVENTS:
+        # Also check, if sensor could be a binary_sensor due to value_list.
+        if is_binary_sensor(parameter_data):
+            parameter_data[HM_TYPE] = TYPE_BOOL
+            entity_t = HmBinarySensor
+        else:
+            entity_t = HmSensor
 
     if entity_t:
         entity = entity_t(
             device=device,
             unique_identifier=unique_identifier,
             channel_address=channel_address,
             paramset_key=paramset_key,
```

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.0/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.0/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/support.py` & `hahomematic-2023.7.0/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/platforms/update.py` & `hahomematic-2023.7.0/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.0/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.0/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/support.py` & `hahomematic-2023.7.0/hahomematic/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,17 +182,16 @@
             return compare_with.lower().startswith(search_elements.lower())
         return compare_with.lower() == search_elements.lower()
     if isinstance(search_elements, Collection):
         for element in search_elements:
             if do_wildcard_search:
                 if compare_with.lower().startswith(element.lower()):
                     return True
-            else:
-                if compare_with.lower() == element.lower():
-                    return True
+            elif compare_with.lower() == element.lower():
+                return True
     return False
 
 
 @dataclass
 class HubData:
     """Dataclass for hub entities."""
```

### Comparing `hahomematic-2023.6.1/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.0/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.0/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.6.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.0/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.6.1
+Version: 2023.7.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.6.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.0/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*


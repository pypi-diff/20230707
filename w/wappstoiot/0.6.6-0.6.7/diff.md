# Comparing `tmp/wappstoiot-0.6.6.tar.gz` & `tmp/wappstoiot-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wappstoiot-0.6.6.tar", last modified: Mon Jun 26 11:15:27 2023, max compression
+gzip compressed data, was "wappstoiot-0.6.7.tar", last modified: Fri Jul  7 11:47:29 2023, max compression
```

## Comparing `wappstoiot-0.6.6.tar` & `wappstoiot-0.6.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.235953 wappstoiot-0.6.6/
--rw-r--r--   0 bach      (1000) bach      (1000)     5336 2023-06-22 10:08:45.000000 wappstoiot-0.6.6/CHANGELOG.md
--rw-rw-r--   0 bach      (1000) bach      (1000)     1064 2022-03-14 08:11:46.000000 wappstoiot-0.6.6/LICENSE
--rw-r--r--   0 bach      (1000) bach      (1000)      115 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/MANIFEST.in
--rw-r--r--   0 bach      (1000) bach      (1000)     8895 2023-06-26 11:15:27.234953 wappstoiot-0.6.6/PKG-INFO
--rw-r--r--   0 bach      (1000) bach      (1000)     3128 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/README.md
--rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-06-26 11:15:27.235953 wappstoiot-0.6.6/setup.cfg
--rw-r--r--   0 bach      (1000) bach      (1000)     2368 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/setup.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.214953 wappstoiot-0.6.6/test/
--rw-r--r--   0 bach      (1000) bach      (1000)     3159 2023-06-22 10:08:45.000000 wappstoiot-0.6.6/test/test_real_world.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.216953 wappstoiot-0.6.6/wappstoiot/
--rw-r--r--   0 bach      (1000) bach      (1000)    11300 2023-06-22 10:08:45.000000 wappstoiot-0.6.6/wappstoiot/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1080 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     8363 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/__main__.py
--rw-r--r--   0 bach      (1000) bach      (1000)      503 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/__main__.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.220953 wappstoiot-0.6.6/wappstoiot/connections/
--rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/__init__.pyi
--rw-rw-r--   0 bach      (1000) bach      (1000)     2469 2022-03-14 08:11:45.000000 wappstoiot-0.6.6/wappstoiot/connections/protocol.py
--rw-r--r--   0 bach      (1000) bach      (1000)      756 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/protocol.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     9934 2023-02-27 15:18:27.000000 wappstoiot-0.6.6/wappstoiot/connections/sslsocket.py
--rw-r--r--   0 bach      (1000) bach      (1000)      938 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/connections/sslsocket.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.224953 wappstoiot-0.6.6/wappstoiot/modules/
--rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    16057 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/device.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3496 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/device.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    10785 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/network.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1695 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/network.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    19243 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/template.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1964 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/template.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    28153 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/modules/value.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3569 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/modules/value.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)       62 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/py.typed
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.226953 wappstoiot-0.6.6/wappstoiot/schema/
--rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    12612 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/schema/base_schema.py
--rw-r--r--   0 bach      (1000) bach      (1000)     8211 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/base_schema.pyi
--rw-rw-r--   0 bach      (1000) bach      (1000)     5598 2022-05-05 14:14:25.000000 wappstoiot-0.6.6/wappstoiot/schema/iot_schema.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1620 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/schema/iot_schema.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.229953 wappstoiot-0.6.6/wappstoiot/service/
--rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    22423 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/service/iot_api.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3438 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/iot_api.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     4180 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/service/template.py
--rw-r--r--   0 bach      (1000) bach      (1000)     2604 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/service/template.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.233953 wappstoiot-0.6.6/wappstoiot/utils/
--rw-r--r--   0 bach      (1000) bach      (1000)      646 2023-02-27 15:18:27.000000 wappstoiot-0.6.6/wappstoiot/utils/Timestamp.py
--rw-r--r--   0 bach      (1000) bach      (1000)      107 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/Timestamp.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)        3 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)      426 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/certificateread.py
--rw-r--r--   0 bach      (1000) bach      (1000)      122 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/certificateread.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)      691 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/name_check.py
--rw-r--r--   0 bach      (1000) bach      (1000)      142 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/name_check.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     2704 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/observer.py
--rw-r--r--   0 bach      (1000) bach      (1000)      403 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/observer.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     2497 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/offline_storage.py
--rw-r--r--   0 bach      (1000) bach      (1000)      665 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/offline_storage.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     6497 2023-06-26 11:10:06.000000 wappstoiot-0.6.6/wappstoiot/utils/tracer.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1304 2023-06-22 10:08:03.000000 wappstoiot-0.6.6/wappstoiot/utils/tracer.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-06-26 11:15:27.218953 wappstoiot-0.6.6/wappstoiot.egg-info/
--rw-r--r--   0 bach      (1000) bach      (1000)     8895 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/PKG-INFO
--rw-r--r--   0 bach      (1000) bach      (1000)     1699 2023-06-26 11:15:27.000000 wappstoiot-0.6.6/wappstoiot.egg-info/SOURCES.txt
--rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/dependency_links.txt
--rw-r--r--   0 bach      (1000) bach      (1000)       51 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/requires.txt
--rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-06-26 11:15:26.000000 wappstoiot-0.6.6/wappstoiot.egg-info/top_level.txt
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.280926 wappstoiot-0.6.7/
+-rw-r--r--   0 bach      (1000) bach      (1000)     5643 2023-07-07 11:44:05.000000 wappstoiot-0.6.7/CHANGELOG.md
+-rw-rw-r--   0 bach      (1000) bach      (1000)     1064 2022-03-14 08:11:46.000000 wappstoiot-0.6.7/LICENSE
+-rw-r--r--   0 bach      (1000) bach      (1000)      115 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/MANIFEST.in
+-rw-r--r--   0 bach      (1000) bach      (1000)     9202 2023-07-07 11:47:29.279926 wappstoiot-0.6.7/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     3128 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/README.md
+-rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-07-07 11:47:29.280926 wappstoiot-0.6.7/setup.cfg
+-rw-r--r--   0 bach      (1000) bach      (1000)     2368 2023-07-07 09:56:12.000000 wappstoiot-0.6.7/setup.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.255926 wappstoiot-0.6.7/test/
+-rw-r--r--   0 bach      (1000) bach      (1000)     3159 2023-06-22 10:08:45.000000 wappstoiot-0.6.7/test/test_real_world.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.257926 wappstoiot-0.6.7/wappstoiot/
+-rw-r--r--   0 bach      (1000) bach      (1000)    11300 2023-07-07 11:44:18.000000 wappstoiot-0.6.7/wappstoiot/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1080 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     8363 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/wappstoiot/__main__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)       94 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/__main__.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.262926 wappstoiot-0.6.7/wappstoiot/connections/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:21.000000 wappstoiot-0.6.7/wappstoiot/connections/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/connections/__init__.pyi
+-rw-rw-r--   0 bach      (1000) bach      (1000)     2469 2023-07-07 11:10:09.000000 wappstoiot-0.6.7/wappstoiot/connections/protocol.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      756 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/connections/protocol.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     9931 2023-07-07 11:25:56.000000 wappstoiot-0.6.7/wappstoiot/connections/sslsocket.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      938 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/connections/sslsocket.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.266926 wappstoiot-0.6.7/wappstoiot/modules/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:32.000000 wappstoiot-0.6.7/wappstoiot/modules/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    16018 2023-07-07 11:13:41.000000 wappstoiot-0.6.7/wappstoiot/modules/device.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3496 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/device.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    10801 2023-07-07 11:14:27.000000 wappstoiot-0.6.7/wappstoiot/modules/network.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1695 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/network.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    24084 2023-07-07 11:02:16.000000 wappstoiot-0.6.7/wappstoiot/modules/template.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     2309 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/template.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    28482 2023-07-07 11:22:31.000000 wappstoiot-0.6.7/wappstoiot/modules/value.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3585 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/value.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)       62 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/wappstoiot/py.typed
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.269926 wappstoiot-0.6.7/wappstoiot/schema/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:46.000000 wappstoiot-0.6.7/wappstoiot/schema/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/schema/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    12677 2023-06-26 11:19:57.000000 wappstoiot-0.6.7/wappstoiot/schema/base_schema.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     8268 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/schema/base_schema.pyi
+-rw-rw-r--   0 bach      (1000) bach      (1000)     5591 2023-07-07 11:19:59.000000 wappstoiot-0.6.7/wappstoiot/schema/iot_schema.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1620 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/schema/iot_schema.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.272926 wappstoiot-0.6.7/wappstoiot/service/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:54.000000 wappstoiot-0.6.7/wappstoiot/service/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/service/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    22495 2023-06-26 11:19:57.000000 wappstoiot-0.6.7/wappstoiot/service/iot_api.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3510 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/service/iot_api.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     4916 2023-07-07 09:43:39.000000 wappstoiot-0.6.7/wappstoiot/service/template.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3180 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/service/template.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.278926 wappstoiot-0.6.7/wappstoiot/utils/
+-rw-r--r--   0 bach      (1000) bach      (1000)      646 2023-02-27 15:18:27.000000 wappstoiot-0.6.7/wappstoiot/utils/Timestamp.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      107 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/Timestamp.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:05:02.000000 wappstoiot-0.6.7/wappstoiot/utils/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)      483 2023-07-07 10:02:18.000000 wappstoiot-0.6.7/wappstoiot/utils/certificateread.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      143 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/certificateread.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)      718 2023-07-07 11:10:24.000000 wappstoiot-0.6.7/wappstoiot/utils/name_check.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      148 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/name_check.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2711 2023-07-07 11:06:16.000000 wappstoiot-0.6.7/wappstoiot/utils/observer.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      403 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/observer.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2562 2023-07-07 11:21:40.000000 wappstoiot-0.6.7/wappstoiot/utils/offline_storage.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      689 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/offline_storage.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     6523 2023-07-07 11:21:20.000000 wappstoiot-0.6.7/wappstoiot/utils/tracer.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1316 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/tracer.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.259926 wappstoiot-0.6.7/wappstoiot.egg-info/
+-rw-r--r--   0 bach      (1000) bach      (1000)     9202 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     1699 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/SOURCES.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/dependency_links.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       51 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/requires.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/top_level.txt
```

### Comparing `wappstoiot-0.6.6/CHANGELOG.md` & `wappstoiot-0.6.7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.6.7 (Jul 07 2023)
+===============================================================================
+## Added
+ * Scandinavian special letters to the legal list
+
+## Changed
+ * Updated the `wappstoiot.ValueTemplate` to version v0.0.5
+ * Set Pydantic version to be `v1.10.11` until migration to `v2` is done.
+
 v0.6.6 (Jun 22 2023)
 ===============================================================================
 ## Added
  * Code Stub.
 
 ## Changed
  * Now inform which characters are illegal in the given name.
```

### Comparing `wappstoiot-0.6.6/LICENSE` & `wappstoiot-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/PKG-INFO` & `wappstoiot-0.6.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wappstoiot
-Version: 0.6.6
+Version: 0.6.7
 Summary: Simple Wappsto Python user-interface to Wappsto IoT
 Home-page: https://github.com/Wappsto/python-wappsto-iot
 Author: Seluxit A/S
 Author-email: support@seluxit.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -121,14 +121,23 @@
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
 
 
 
+v0.6.7 (Jul 07 2023)
+===============================================================================
+## Added
+ * Scandinavian special letters to the legal list
+
+## Changed
+ * Updated the `wappstoiot.ValueTemplate` to version v0.0.5
+ * Set Pydantic version to be `v1.10.11` until migration to `v2` is done.
+
 v0.6.6 (Jun 22 2023)
 ===============================================================================
 ## Added
  * Code Stub.
 
 ## Changed
  * Now inform which characters are illegal in the given name.
```

### Comparing `wappstoiot-0.6.6/README.md` & `wappstoiot-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/setup.py` & `wappstoiot-0.6.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     #     'tox'
     # ],
     package_data={
         'wappstoiot': ["py.typed", "*.pyi", "**/*.pyi"]
     },
     install_requires=[
         'slxjsonrpc>=0.8.1',
-        'pydantic>=1.6.1',
+        'pydantic==1.9.2',
         'requests>=2.25.1'
     ],
     # entry_points={  # TODO: fix __main__.py to be optional.
     #     "console_scripts": "wappstoiot=wappstoiot:__main__"
     # },
     # extras_require={  # TODO: fix __main__.py to be optional.
     #     "cli": [
```

### Comparing `wappstoiot-0.6.6/test/test_real_world.py` & `wappstoiot-0.6.7/test/test_real_world.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/__init__.py` & `wappstoiot-0.6.7/wappstoiot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from .utils import observer
 from .utils import name_check
 
 # #############################################################################
 #                             __init__ Setup Stuff
 # #############################################################################
 
-__version__ = "v0.6.6"
+__version__ = "v0.6.7"
 __auther__ = "Seluxit A/S"
 
 __all__ = [
     'Network',
     'Device',
     'Value',
     'onStatusChange',
```

### Comparing `wappstoiot-0.6.6/wappstoiot/__init__.pyi` & `wappstoiot-0.6.7/wappstoiot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/__main__.py` & `wappstoiot-0.6.7/wappstoiot/__main__.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/connections/protocol.py` & `wappstoiot-0.6.7/wappstoiot/connections/protocol.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         data chunks.
 
         Args:
             Callable: A parser, that returns the parsed data.
                       On Parsing Error, it should raise a
                       ValueError TypeError or any subClasses of those.
                       (Like 'JSONDecodeError' & 'pydantic.ValidationError' is)
+
         Returns:
             The Parsers output.
-
         """
         pass
 
     @abstractmethod
     def connect(self) -> Optional[bool]:
         """
         Connect to the server.
```

### Comparing `wappstoiot-0.6.6/wappstoiot/connections/protocol.pyi` & `wappstoiot-0.6.7/wappstoiot/connections/protocol.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/connections/sslsocket.py` & `wappstoiot-0.6.7/wappstoiot/connections/sslsocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,22 +134,20 @@
         self,
         data: Union[str, bytes]
     ) -> bool:
         """
         Send the str/Bytes to the server.
 
         If given string, it is encoded as 'uft-8' & send.
-
         UNSURE(MBK): Should the encoding be moved outside this class?
 
         Returns:
             True, if the data could be send else
             False.
         """
-
         if isinstance(data, str):
             data = data.encode('utf-8')
 
         try:
             self.socket.sendall(data)
         except ConnectionError:
             msg = "Get a ConnectionError, while trying to send"
@@ -186,17 +184,17 @@
         data chunks.
 
         Args:
             Callable: A parser, that returns the parsed data.
                       On Parsen Error, it should raise a
                       ValueError TypeError or any subClasses of those.
                       (Like 'JSONDecodeError' & 'pydantic.ValidationError' is)
+
         Returns:
             The "parser"'s output.
-
         """
         data = []
         while self.socket or not self.killed.is_set():
             try:
                 data_chunk = self.socket.recv(self.RECEIVE_SIZE)
             except socket.timeout:
                 # This happens every 2 Sec as set in self._socket_setup.
@@ -238,15 +236,14 @@
         Connect to the server.
 
         Attempts a connection to the server on the provided addres and port.
 
         Returns:
             'True' if the connection was successful.
         """
-
         if self.killed.is_set():
             return False
 
         try:
             self.log.info("Trying to Connect.")
             self.observer.post(StatusID.CONNECTING, None)
             # self.socket.settimeout(10)  # Why?
```

### Comparing `wappstoiot-0.6.6/wappstoiot/connections/sslsocket.pyi` & `wappstoiot-0.6.7/wappstoiot/connections/sslsocket.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/device.py` & `wappstoiot-0.6.7/wappstoiot/modules/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import uuid
 import logging
 
 from enum import Enum
 
+from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 from ..service.template import ServiceClass
 
@@ -63,15 +64,15 @@
         serial: Optional[str] = None,
         description: Optional[str] = None,
     ):
 
         self.log = logging.getLogger(__name__)
         self.log.addHandler(logging.NullHandler())
 
-        self.__callbacks: Dict[str, Callable] = {}
+        self.__callbacks: Dict[str, Callable[[...], ...]] = {}
 
         self.parent = parent
         self.element: WSchema.Device
 
         self.children_uuid_mapping: Dict[uuid.UUID, Value] = {}
         self.children_name_mapping: Dict[str, uuid.UUID] = {}
 
@@ -134,24 +135,21 @@
         # TODO(MBK): Check if new devices was added! & Check diff.
         # NOTE: If there was a diff, post local one.
         self.element = element.copy(update=self.element.dict(exclude_none=True))
         self.element.meta = element.meta.copy(update=self.element.meta)
         for nr, value in enumerate(self.element.value):
             self.cloud_id_mapping[nr] = value
 
-    def __argumentCountCheck(self, callback: Callable, requiredArgumentCount: int) -> bool:
-        """
-        Check if the requeried Argument count for given function fits.
-        """
+    def __argumentCountCheck(self, callback: Callable[[Any], Any], requiredArgumentCount: int) -> bool:
+        """Check if the required Argument count for given function fits."""
         allArgument: int = callback.__code__.co_argcount
         the_default_count: int = len(callback.__defaults__) if callback.__defaults__ is not None else 1
         mandatoryArguments: int = callback.__code__.co_argcount - the_default_count
         return (
-            requiredArgumentCount <= allArgument and
-            requiredArgumentCount >= mandatoryArguments
+            requiredArgumentCount <= allArgument and requiredArgumentCount >= mandatoryArguments
         )
 
     # -------------------------------------------------------------------------
     #   Device 'on-' methods
     # -------------------------------------------------------------------------
 
     def onDelete(
@@ -232,17 +230,15 @@
             callback=self.__callbacks['onRefresh']
         )
 
     def onChange(
         self,
         callback: Callable[['Device'], None],
     ) -> Callable[['Device'], None]:
-        """
-        Configure a callback for when a change to the Device have occurred.
-        """
+        """Configure a callback for when a change to the Device have occurred."""
         if not self.__argumentCountCheck(callback, 1):
             raise TypeError("The onChange callback, are called with 1 argument.")
 
         def _cb(obj, method):
             try:
                 if method in WappstoMethod.PUT:
                     callback(self)
@@ -265,17 +261,15 @@
             callback=self.__callbacks['onChange']
         )
 
     def onCreate(
         self,
         callback: Callable[['Device'], None],
     ) -> Callable[['Device'], None]:
-        """
-        Configure a callback for when a request have been make for the Value.
-        """
+        """Configure a callback for when a request have been make for the Value."""
         if not self.__argumentCountCheck(callback, 1):
             raise TypeError("The onCreate callback, are called with 1 argument.")
 
         def _cb(obj, method):
             try:
                 if method in WappstoMethod.POST:
                     callback(self)
@@ -315,17 +309,15 @@
          - version
          - serial
          - description
         """
         pass
 
     def delete(self) -> None:
-        """
-        Request a delete of the Device, & all it's Children.
-        """
+        """Request a delete of the Device, & all it's Children."""
         self.connection.delete_device(uuid=self.uuid)
 
     # -------------------------------------------------------------------------
     #   Other methods
     # -------------------------------------------------------------------------
 
     def createNumberValue(
@@ -499,15 +491,14 @@
         A Wappsto Value is where the changing data can be found & are handled.
 
         If a value_type have been set, that means that the parameters like:
         name, permission, min, max, step, encoding & unit have been set
         for you, to be the right settings for the given type. But you can
         still change it, if you choose sow.
         """
-
         illegal_chars: str = name_check.illegal_characters(name)
 
         if illegal_chars:
             raise ValueError(
                 f"Given name contain a illegal character: {illegal_chars}"
                 f"May only contain: {name_check.wappsto_letters}"
             )
```

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/device.pyi` & `wappstoiot-0.6.7/wappstoiot/modules/device.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/network.py` & `wappstoiot-0.6.7/wappstoiot/modules/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
 import uuid
 
-from typing import Dict, Optional, Callable
+from typing import Any
+from typing import Dict
+from typing import Callable
+from typing import Optional
 
 from ..service.template import ServiceClass
 # from .service.rest_api import RestAPI
 
 from .device import Device
 
 from ..schema import base_schema as WSchema
@@ -25,25 +28,23 @@
     def __init__(
         self,
         name: str,
         connection: ServiceClass,
         network_uuid: uuid.UUID,
         description: str = "",
     ) -> None:
-        """
-        Configure the WappstoIoT settings.
-        """
+        """Configure the WappstoIoT settings."""
         self.log = logging.getLogger(__name__)
         self.log.addHandler(logging.NullHandler())
 
         kwargs = locals()
         self.__uuid: uuid.UUID = network_uuid
         self.element: WSchema.Network = self.schema()
 
-        self.__callbacks: Dict[str, Callable] = {}
+        self.__callbacks: Dict[str, Callable[[...], ...]] = {}
 
         self.children_uuid_mapping: Dict[uuid.UUID, Device] = {}
         self.children_name_mapping: Dict[str, uuid.UUID] = {}
 
         self.cloud_id_mapping: Dict[int, uuid.UUID] = {}
 
         self.connection: ServiceClass = connection
@@ -86,24 +87,21 @@
         return self.element.name
 
     @property
     def uuid(self) -> uuid.UUID:
         """Returns the name of the value."""
         return self.__uuid
 
-    def __argumentCountCheck(self, callback: Callable, requiredArgumentCount: int) -> bool:
-        """
-        Check if the requeried Argument count for given function fits.
-        """
+    def __argumentCountCheck(self, callback: Callable[[Any], Any], requiredArgumentCount: int) -> bool:
+        """Check if the required Argument count for given function fits."""
         allArgument: int = callback.__code__.co_argcount
         the_default_count: int = len(callback.__defaults__) if callback.__defaults__ is not None else 1
         mandatoryArguments: int = callback.__code__.co_argcount - the_default_count
         return (
-            requiredArgumentCount <= allArgument and
-            requiredArgumentCount >= mandatoryArguments
+            requiredArgumentCount <= allArgument and requiredArgumentCount >= mandatoryArguments
         )
 
     # -------------------------------------------------------------------------
     #   Save/Load helper methods
     # -------------------------------------------------------------------------
 
     def __update_self(self, element: WSchema.Network):
@@ -153,17 +151,15 @@
             callback=self.__callbacks['onChange']
         )
 
     def onCreate(
         self,
         callback: Callable[['Network'], None],
     ) -> Callable[['Network'], None]:
-        """
-        Configure a callback for when a create have been make for the Device.
-        """
+        """Configure a callback for when a create have been make for the Device."""
         if not self.__argumentCountCheck(callback, 1):
             raise TypeError("The onCreate callback, is called with 1 argument.")
 
         def _cb(obj, method):
             try:
                 if method == WappstoMethod.POST:
                     callback()
```

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/network.pyi` & `wappstoiot-0.6.7/wappstoiot/modules/network.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/template.py` & `wappstoiot-0.6.7/wappstoiot/modules/template.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """
     Predefined ValueTemplate.
 
     Each of the predefined ValueTemplate, have default
     value parameters set, which include BaseType, name,
     permission, range, step and the unit.
     """
-    __version__ = "0.0.3"
+    __version__ = "0.0.5"
 
     ADDRESS_NAME = "ADDRESS_NAME"
     ALTITUDE_M = "ALTITUDE_M"
     ANGLE = "ANGLE"
     APPARENT_POWER_VA = "APPARENT_POWER_VA"
     BLOB = "BLOB"
     BOOLEAN_ONOFF = "BOOLEAN_ONOFF"
@@ -72,52 +72,77 @@
     DISTANCE_M = "DISTANCE_M"
     DURATION_MIN = "DURATION_MIN"
     DURATION_MSEC = "DURATION_MSEC"
     DURATION_SEC = "DURATION_SEC"
     EMAIL = "EMAIL"
     ENERGY_KWH = "ENERGY_KWH"
     ENERGY_MWH = "ENERGY_MWH"
+    ENERGY_PRICE_DKK_KWH = "ENERGY_PRICE_DKK_KWH"
+    ENERGY_PRICE_DKK_MWH = "ENERGY_PRICE_DKK_MWH"
+    ENERGY_PRICE_EUR_KWH = "ENERGY_PRICE_EUR_KWH"
+    ENERGY_PRICE_EUR_MWH = "ENERGY_PRICE_EUR_MWH"
     ENERGY_WH = "ENERGY_WH"
     FREQUENCY_HZ = "FREQUENCY_HZ"
     HUMIDITY = "HUMIDITY"
     IDENTIFIER = "IDENTIFIER"
     IMAGE_JPG = "IMAGE_JPG"
     IMAGE_PNG = "IMAGE_PNG"
     IMPULSE_KWH = "IMPULSE_KWH"
     INTEGER = "INTEGER"
     JSON = "JSON"
     LATITUDE = "LATITUDE"
+    LOAD_CURVE_ENERGY_KWH = "LOAD_CURVE_ENERGY_KWH"
+    LOAD_CURVE_ENERGY_MWH = "LOAD_CURVE_ENERGY_MWH"
+    LOAD_CURVE_ENERGY_WH = "LOAD_CURVE_ENERGY_WH"
     LONGITUDE = "LONGITUDE"
-    LUMINOUSITY_LX = "LUMINOUSITY_LX"
+    LUMINOSITY_LX = "LUMINOSITY_LX"
     NUMBER = "NUMBER"
-    ORGANISATION = "ORGANISATION"
+    ORGANIZATION = "ORGANIZATION"
     PERCENTAGE = "PERCENTAGE"
     PHONE = "PHONE"
     POSTCODE = "POSTCODE"
     POWER_KW = "POWER_KW"
     POWER_WATT = "POWER_WATT"
     PRECIPITATION_MM = "PRECIPITATION_MM"
     PRESSURE_HPA = "PRESSURE_HPA"
     REACTIVE_ENERGY_KVARH = "REACTIVE_ENERGY_KVARH"
     REACTIVE_POWER_KVAR = "REACTIVE_POWER_KVAR"
+    SPEED_KMH = "SPEED_KMH"
     SPEED_MS = "SPEED_MS"
     STREET = "STREET"
     STRING = "STRING"
     TEMPERATURE_CELSIUS = "TEMPERATURE_CELSIUS"
     TEMPERATURE_FAHRENHEIT = "TEMPERATURE_FAHRENHEIT"
     TEMPERATURE_KELVIN = "TEMPERATURE_KELVIN"
     TIMESTAMP = "TIMESTAMP"
+    TIME_OF_DAY = "TIME_OF_DAY"
+    TOTAL_ENERGY_KWH = "TOTAL_ENERGY_KWH"
+    TOTAL_ENERGY_MWH = "TOTAL_ENERGY_MWH"
+    TOTAL_ENERGY_WH = "TOTAL_ENERGY_WH"
+    TRIGGER = "TRIGGER"
     UNIT_TIME = "UNIT_TIME"
     VOLTAGE_V = "VOLTAGE_V"
     VOLUME_M3 = "VOLUME_M3"
     XML = "XML"
 
 
 valueSettings: Dict[ValueTemplate, ValueSettinsSchema] = {
 
+    ValueTemplate.TRIGGER: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="trigger",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="0",
+        max="0",
+        step="0",
+        unit=None,
+        si_conversion=None,
+    ),
     ValueTemplate.BOOLEAN_TRUEFALSE: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="boolean",
         mapping={'0': 'false', '1': 'true'},
         ordered_mapping=None,
         meaningful_zero=None,
         min="0",
@@ -200,65 +225,137 @@
     ),
     ValueTemplate.POWER_WATT: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="power",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
-        min="0",
+        min="-1000000",
         max="2500",
         step="0.1",
         unit="W",
         si_conversion=None,
     ),
     ValueTemplate.POWER_KW: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="power",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
-        min="0",
+        min="-1000000",
         max="1000000",
         step="0.1",
         unit="kW",
         si_conversion="[W] = 1000 * [kW]",
     ),
     ValueTemplate.ENERGY_WH: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="energy",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
-        min="0",
+        min="-1000000",
         max="100000",
         step="0.1",
         unit="Wh",
-        si_conversion=None,
+        si_conversion="[J] = 3600 * [Wh]",
     ),
     ValueTemplate.ENERGY_KWH: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="energy",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
-        min="0",
+        min="-1000000",
         max="1000000",
         step="0.1",
         unit="kWh",
         si_conversion="[J] = 3600000 * [kWh]",
     ),
     ValueTemplate.ENERGY_MWH: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="energy",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
+        min="-1000000",
+        max="1000000",
+        step="0.1",
+        unit="MWh",
+        si_conversion="[J] = 3600000000 * [MWh]",
+    ),
+    ValueTemplate.TOTAL_ENERGY_WH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="total_energy",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
         min="0",
         max="1000000",
         step="0.1",
+        unit="Wh",
+        si_conversion="[J] = 3600 * [Wh]",
+    ),
+    ValueTemplate.TOTAL_ENERGY_KWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="total_energy",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="0",
+        max="1000000",
+        step="0.1",
+        unit="kWh",
+        si_conversion="[J] = 3600000 * [kWh]  ",
+    ),
+    ValueTemplate.TOTAL_ENERGY_MWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="total_energy",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="0",
+        max="1000000",
+        step="0.1",
+        unit="MWh",
+        si_conversion="[J] = 3600000000 * [MWh]",
+    ),
+    ValueTemplate.LOAD_CURVE_ENERGY_WH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="load_curve_energy",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="-1000000",
+        max="1000000",
+        step="0.1",
+        unit="Wh",
+        si_conversion="[J] = 3600 * [Wh]",
+    ),
+    ValueTemplate.LOAD_CURVE_ENERGY_KWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="load_curve_energy",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="-1000000",
+        max="1000000",
+        step="0.1",
+        unit="kWh",
+        si_conversion="[J] = 3600000 * [kWh]  ",
+    ),
+    ValueTemplate.LOAD_CURVE_ENERGY_MWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="load_curve_energy",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="-1000000",
+        max="1000000",
+        step="0.1",
         unit="MWh",
         si_conversion="[J] = 3600000000 * [MWh]",
     ),
     ValueTemplate.CURRENT_A: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="electric_current",
         mapping=None,
@@ -278,48 +375,96 @@
         meaningful_zero=None,
         min="-5000",
         max="5000",
         step="0.001",
         unit="VA",
         si_conversion=None,
     ),
-    ValueTemplate.FREQUENCY_HZ: ValueSettinsSchema(
+    ValueTemplate.REACTIVE_ENERGY_KVARH: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
-        type="frequency",
+        type="reactive_energy",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
-        min="0",
-        max="30000",
-        step="0.01",
-        unit="Hz",
+        min="-5000",
+        max="5000",
+        step="0.001",
+        unit="kvarh",
         si_conversion=None,
     ),
     ValueTemplate.REACTIVE_POWER_KVAR: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="reactive_power",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
         min="-5000",
         max="5000",
         step="0.001",
         unit="kvar",
         si_conversion=None,
     ),
-    ValueTemplate.REACTIVE_ENERGY_KVARH: ValueSettinsSchema(
+    ValueTemplate.ENERGY_PRICE_EUR_KWH: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
-        type="reactive_energy",
+        type="energy_price",
         mapping=None,
         ordered_mapping=None,
-        meaningful_zero=None,
-        min="-5000",
-        max="5000",
+        meaningful_zero=False,
+        min="-10000",
+        max="10000",
+        step="0.01",
+        unit="EUR/kWh",
+        si_conversion=None,
+    ),
+    ValueTemplate.ENERGY_PRICE_EUR_MWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="energy_price",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=False,
+        min="-10000",
+        max="10000",
         step="0.001",
-        unit="kvarh",
+        unit="EUR/MWh",
+        si_conversion=None,
+    ),
+    ValueTemplate.ENERGY_PRICE_DKK_KWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="energy_price",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=False,
+        min="-10000",
+        max="10000",
+        step="0.01",
+        unit="DKK/kWh",
+        si_conversion=None,
+    ),
+    ValueTemplate.ENERGY_PRICE_DKK_MWH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="energy_price",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=False,
+        min="-10000",
+        max="10000",
+        step="0.001",
+        unit="DKK/MWh",
+        si_conversion=None,
+    ),
+    ValueTemplate.FREQUENCY_HZ: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="frequency",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=None,
+        min="0",
+        max="30000",
+        step="0.01",
+        unit="Hz",
         si_conversion=None,
     ),
     ValueTemplate.TEMPERATURE_CELSIUS: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="temperature",
         mapping=None,
         ordered_mapping=None,
@@ -386,14 +531,26 @@
         meaningful_zero=None,
         min="0",
         max="100",
         step="1",
         unit="m/s",
         si_conversion=None,
     ),
+    ValueTemplate.SPEED_KMH: ValueSettinsSchema(
+        value_type=ValueBaseType.NUMBER,
+        type="speed",
+        mapping=None,
+        ordered_mapping=None,
+        meaningful_zero=True,
+        min="0",
+        max="400",
+        step="0.1",
+        unit="km/h",
+        si_conversion="[ms] = [kmh]*1000/3600",
+    ),
     ValueTemplate.PRECIPITATION_MM: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="precipitation",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
         min="0",
@@ -448,15 +605,15 @@
         max="1100",
         step="1",
         unit="hPa",
         si_conversion="[Pa] = [hPa]/100",
     ),
     ValueTemplate.VOLUME_M3: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
-        type="Volume",
+        type="volume",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=True,
         min="0",
         max="1000000000",
         step="0.001",
         unit="m³",
@@ -512,29 +669,35 @@
         meaningful_zero=None,
         min="0",
         max="5000",
         step="0.001",
         unit="ms",
         si_conversion="[s] = [ms]/1000",
     ),
+    ValueTemplate.TIME_OF_DAY: ValueSettinsSchema(
+        value_type=ValueBaseType.STRING,
+        type="time",
+        max="100",
+        encoding="",
+    ),
     ValueTemplate.DISTANCE_M: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
         type="distance",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
         min="0",
         max="1000",
         step="1",
         unit="m",
         si_conversion=None,
     ),
-    ValueTemplate.LUMINOUSITY_LX: ValueSettinsSchema(
+    ValueTemplate.LUMINOSITY_LX: ValueSettinsSchema(
         value_type=ValueBaseType.NUMBER,
-        type="luminousity",
+        type="luminosity",
         mapping=None,
         ordered_mapping=None,
         meaningful_zero=None,
         min="0",
         max="25000",
         step="1",
         unit="lx",
@@ -644,17 +807,17 @@
     ),
     ValueTemplate.ADDRESS_NAME: ValueSettinsSchema(
         value_type=ValueBaseType.STRING,
         type="address_name",
         max="85",
         encoding="",
     ),
-    ValueTemplate.ORGANISATION: ValueSettinsSchema(
+    ValueTemplate.ORGANIZATION: ValueSettinsSchema(
         value_type=ValueBaseType.STRING,
-        type="organisation",
+        type="organization",
         max="85",
         encoding="",
     ),
     ValueTemplate.EMAIL: ValueSettinsSchema(
         value_type=ValueBaseType.STRING,
         type="email",
         max="128",
```

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/value.py` & `wappstoiot-0.6.7/wappstoiot/modules/value.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         encoding: Optional[str] = None,
         xsd: Optional[str] = None,
         namespace: Optional[str] = None,
         period: Optional[int] = None,  # in Sec
         delta: Optional[Union[int, float]] = None,
         description: Optional[str] = None,
         meaningful_zero: Optional[str] = None,
-        mapping: Optional[bool] = None,
+        mapping: Optional[Dict[str, Any]] = None,
         ordered_mapping: Optional[bool] = None,
         si_conversion: Optional[str] = None,
         unit: Optional[str] = None,
     ):
         self.log = logging.getLogger(__name__)
         self.log.addHandler(logging.NullHandler())
 
@@ -114,26 +114,26 @@
         ] = self.schema()
 
         self.children_name_mapping: Dict[str, uuid.UUID] = {}
 
         self.connection: ServiceClass = parent.connection
 
         subValue = self.__parseValueTemplate(
-                ValueBaseType=value_type,
-                encoding=encoding,
-                mapping=mapping,
-                max_range=max,
-                meaningful_zero=meaningful_zero,
-                min_range=min,
-                namespace=namespace,
-                ordered_mapping=ordered_mapping,
-                si_conversion=si_conversion,
-                step=step,
-                unit=unit,
-                xsd=xsd,
+            ValueBaseType=value_type,
+            encoding=encoding,
+            mapping=mapping,
+            max_range=max,
+            meaningful_zero=meaningful_zero,
+            min_range=min,
+            namespace=namespace,
+            ordered_mapping=ordered_mapping,
+            si_conversion=si_conversion,
+            step=step,
+            unit=unit,
+            xsd=xsd,
         )
 
         element = self.connection.get_value(value_uuid) if value_uuid else None
 
         self.__uuid: uuid.UUID = value_uuid if value_uuid else uuid.uuid4()
 
         self.element = self.schema(
@@ -204,14 +204,15 @@
         The returned timestamp will be the last time Control value was updated,
         unless there isn't one, then it will return None.
         """
         if isinstance(self.control_state.timestamp, datetime):
             return self.control_state.timestamp
         if isinstance(self.control_state.timestamp, str):
             return str_to_datetime(self.control_state.timestamp)
+        return None
 
     def getReportData(self) -> Optional[Union[float, str]]:
         """
         Returns the last Report value.
 
         The returned value will be the last Report value.
         unless there isn't one, then it will return None.
@@ -229,14 +230,15 @@
         The returned timestamp will be the last time Control value was updated,
         unless there isn't one, then it will return None.
         """
         if isinstance(self.report_state.timestamp, datetime):
             return self.report_state.timestamp
         if isinstance(self.report_state.timestamp, str):
             return str_to_datetime(self.report_state.timestamp)
+        return None
 
     @property
     def name(self) -> str:
         """Returns the name of the value."""
         return self.element.name
 
     @property
@@ -244,41 +246,38 @@
         """Returns the uuid of the value."""
         return self.__uuid
 
     # -------------------------------------------------------------------------
     #   Helper methods
     # -------------------------------------------------------------------------
 
-    def __argumentCountCheck(self, callback: Callable, requiredArgumentCount: int) -> bool:
-        """
-        Check if the requeried Argument count for given function fits.
-        """
+    def __argumentCountCheck(self, callback: Callable[[Any], Any], requiredArgumentCount: int) -> bool:
+        """Check if the requeried Argument count for given function fits."""
         allArgument: int = callback.__code__.co_argcount
         the_default_count: int = len(callback.__defaults__) if callback.__defaults__ is not None else 1
         mandatoryArguments: int = callback.__code__.co_argcount - the_default_count
         return (
-            requiredArgumentCount <= allArgument and
-            requiredArgumentCount >= mandatoryArguments
+            requiredArgumentCount <= allArgument and requiredArgumentCount >= mandatoryArguments
         )
 
     def __parseValueTemplate(
         self,
-        ValueBaseType,
-        encoding,
-        mapping,
-        max_range,
-        meaningful_zero,
-        min_range,
-        namespace,
-        ordered_mapping,
-        si_conversion,
-        step,
-        unit,
-        xsd,
-    ):
+        ValueBaseType: ValueBaseType,
+        max_range: float,
+        min_range: Optional[float] = None,
+        step: Optional[float] = None,
+        encoding: Optional[str] = None,
+        mapping: Optional[Dict[str, Any]] = None,
+        meaningful_zero: Optional[bool] = None,
+        namespace: Optional[str] = None,
+        ordered_mapping: Optional[bool] = None,
+        si_conversion: Optional[str] = None,
+        unit: Optional[str] = None,
+        xsd: Optional[str] = None,
+    ) -> None:
 
         if ValueBaseType == ValueBaseType.NUMBER:
             subValue = {
                 "number": WSchema.Number(
                     min=min_range,
                     max=max_range,
                     step=step,
@@ -309,15 +308,15 @@
                     max=max_range,
                     encoding=encoding
                 )
             }
 
         return subValue
 
-    def __update_self(self, element):
+    def __update_self(self, element: WSchema.Value) -> None:
         old_type = type(element)
         new_type = type(self.element)
 
         new_dict = element.copy(update=self.element.dict(exclude_none=True))
         new_dict.meta = element.meta.copy(update=new_dict.meta)
 
         if new_type is old_type:
@@ -350,15 +349,15 @@
             elif old_type is WSchema.XmlValue:
                 new_dict.pop('xml')
             self.log.debug(f"CC: {new_dict}")
             self.element = self.schema(**new_dict)
 
         # TODO: Check for the Difference Value-types & ensure that it is right.
 
-    def __update_state(self):
+    def __update_state(self) -> None:
         state_count = len(self.element.state)
         if self.element.permission == PermissionType.NONE:
             return
         elif state_count == 0:
             self._createStates(self.element.permission)
             return
 
@@ -440,15 +439,15 @@
         self.connection.subscribe_value_event(
             uuid=self.uuid,
             callback=_cb
         )
 
         return callback
 
-    def cancelOnChange(self):
+    def cancelOnChange(self) -> None:
         self.connection.unsubscribe_value_event(
             uuid=self.uuid,
             callback=self.__callbacks['onChange']
         )
 
     def onReport(
         self,
@@ -489,15 +488,15 @@
         self.connection.subscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
             callback=_cb
         )
 
         return callback
 
-    def cancelOnReport(self):
+    def cancelOnReport(self) -> None:
         self.connection.unsubscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
             callback=self.__callbacks['onReport']
         )
 
     def onControl(
         self,
@@ -543,15 +542,15 @@
         self.connection.subscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.CONTROL.name],
             callback=_cb
         )
 
         return callback
 
-    def cancelOnControl(self):
+    def cancelOnControl(self) -> None:
         self.connection.unsubscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.CONTROL.name],
             callback=self.__callbacks['onControl']
         )
 
     def onCreate(
         self,
@@ -581,15 +580,15 @@
         self.connection.subscribe_state_event(
             uuid=self.uuid,
             callback=_cb
         )
 
         return callback
 
-    def cancelOnCreate(self):
+    def cancelOnCreate(self) -> None:
         self.connection.unsubscribe_state_event(
             uuid=self.uuid,
             callback=self.__callbacks['onCreate']
         )
 
     def onRefresh(
         self,
@@ -621,26 +620,25 @@
         self.connection.subscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
             callback=_cb
         )
 
         return callback
 
-    def cancelOnRefresh(self):
+    def cancelOnRefresh(self) -> None:
         self.connection.unsubscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
             callback=self.__callbacks['onRefresh']
         )
 
     def onDelete(
         self,
         callback: Callable[['Value'], None],
     ) -> Callable[['Value'], None]:
         """For when a 'DELETE' request have been called on this element."""
-
         if not self.__argumentCountCheck(callback, 1):
             raise TypeError("The onDelete callback, is called with 1 argument.")
 
         def _cb(obj, method):
             try:
                 if method == WappstoMethod.DELETE:
                     callback(self)
@@ -653,25 +651,25 @@
         self.connection.subscribe_value_event(
             uuid=self.uuid,
             callback=_cb
         )
 
         return callback
 
-    def cancelOnDelete(self):
+    def cancelOnDelete(self) -> None:
         self.connection.unsubscribe_value_event(
             uuid=self.uuid,
             callback=self.__callbacks['onDelete']
         )
 
     # -------------------------------------------------------------------------
     #   Value methods
     # -------------------------------------------------------------------------
 
-    def refresh(self):
+    def refresh(self) -> None:
         raise NotImplementedError("Method: 'refresh' is not Implemented.")
 
     def change(self, name: str, value: Any) -> None:
         """
         Update a parameter in the Value structure.
 
         A parameter that a device can have that can be updated could be:
@@ -682,19 +680,16 @@
          - period
          - delta
          # - meaningful_zero
         """
         # raise NotImplementedError("Method: 'change' is not Implemented.")
         pass
 
-    def delete(self):
-        """
-        Request a delete of the Device, & all it's Children.
-        """
-
+    def delete(self) -> None:
+        """Request a delete of the Device, & all it's Children."""
         self.connection.delete_value(uuid=self.uuid)
 
     def report(
         self,
         value: Union[int, float, str, None],
         timestamp: Optional[datetime] = None
     ) -> None:
@@ -712,16 +707,15 @@
         self.log.info(f"Sending Report for: {self.report_state.meta.id}")
         the_timestamp = timestamp if timestamp is not None else datetime.utcnow()
         data = WSchema.State(
             data=value,
             timestamp=timestamp_converter(the_timestamp)
         )
         if (
-            data.timestamp and self.report_state.timestamp or
-            not self.report_state.timestamp
+            data.timestamp and self.report_state.timestamp or not self.report_state.timestamp
         ):
             self.report_state = self.report_state.copy(update=data.dict(exclude_none=True))
             self.report_state.timestamp = the_timestamp
             if self.report_state.timestamp:
                 self.report_state.timestamp = self.report_state.timestamp.replace(tzinfo=None)
         self.connection.put_state(
             uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
@@ -746,69 +740,67 @@
         self.log.info(f"Sending Control for: {self.control_state.meta.id}")
         the_timestamp = timestamp if timestamp is not None else datetime.utcnow()
         data = WSchema.State(
             data=value,
             timestamp=timestamp_converter(the_timestamp)
         )
         if (
-            data.timestamp and self.control_state.timestamp or
-            not self.control_state.timestamp
+            data.timestamp and self.control_state.timestamp or self.control_state.timestamp
         ):
             self.control_state = self.control_state.copy(update=data.dict(exclude_none=True))
             self.control_state.timestamp = the_timestamp
             if self.control_state.timestamp:
                 self.control_state.timestamp = self.control_state.timestamp.replace(tzinfo=None)
         self.connection.put_state(
             uuid=self.children_name_mapping[WSchema.StateType.CONTROL.name],
             data=data
         )
 
     # -------------------------------------------------------------------------
     #   Other methods
     # -------------------------------------------------------------------------
 
-    def _createStates(self, permission: PermissionType):
+    def _createStates(self, permission: PermissionType) -> None:
         if permission in [PermissionType.READ, PermissionType.READWRITE]:
             self._CreateReport()
         if permission in [PermissionType.WRITE, PermissionType.READWRITE]:
             self._CreateControl()
 
-    def _CreateReport(self):
+    def _CreateReport(self) -> None:
         if not self.children_name_mapping.get(WSchema.StateType.REPORT.name):
             self.children_name_mapping[WSchema.StateType.REPORT.name] = uuid.uuid4()
 
             self.report_state = WSchema.State(
                 data="NA" if self.value_type == ValueBaseType.NUMBER else "",
                 type=WSchema.StateType.REPORT,
                 meta=WSchema.BaseMeta(
                     id=self.children_name_mapping.get(WSchema.StateType.REPORT.name)
                 )
             )
 
             self.connection.post_state(value_uuid=self.uuid, data=self.report_state)
 
-    def _CreateControl(self):
+    def _CreateControl(self) -> None:
         if not self.children_name_mapping.get(WSchema.StateType.CONTROL.name):
             self.children_name_mapping[WSchema.StateType.CONTROL.name] = uuid.uuid4()
 
             self.control_state = WSchema.State(
                 data="NA" if self.value_type == ValueBaseType.NUMBER else "",
                 type=WSchema.StateType.CONTROL,
                 meta=WSchema.BaseMeta(
                     id=self.children_name_mapping[WSchema.StateType.CONTROL.name]
                 )
             )
             self.connection.post_state(value_uuid=self.uuid, data=self.control_state)
 
-        def _cb(obj, method):
+        def _cb(obj, method: WappstoMethod) -> None:
             try:
                 if method == WappstoMethod.PUT:
                     if (
-                        obj.timestamp and self.control_state.timestamp or
-                        not self.control_state.timestamp
+                        obj.timestamp and self.control_state.timestamp or not self.control_state.timestamp
                     ):
                         self.log.info(f"Control Value updated: {obj.meta.id}, {obj.data}")
                         self.control_state = self.control_state.copy(update=obj.dict(exclude_none=True))
                         if self.control_state.timestamp:
                             self.control_state.timestamp = str_to_datetime(self.control_state.timestamp)
                             self.control_state.timestamp = self.control_state.timestamp.replace(tzinfo=None)
             except Exception:
@@ -816,9 +808,9 @@
                 raise
 
         self.connection.subscribe_state_event(
             uuid=self.children_name_mapping[WSchema.StateType.CONTROL.name],
             callback=_cb
         )
 
-    def close(self):
+    def close(self) -> None:
         pass
```

### Comparing `wappstoiot-0.6.6/wappstoiot/modules/value.pyi` & `wappstoiot-0.6.7/wappstoiot/modules/value.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ..service.template import ServiceClass as ServiceClass
 from ..utils.Timestamp import str_to_datetime as str_to_datetime
 from .device import Device as Device
 from .template import ValueBaseType as ValueBaseType
 from _typeshed import Incomplete
 from datetime import datetime
 from enum import Enum
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Dict, Optional, Union
 
 class Period(str, Enum):
     PERIODIC_REFRESH: str
     DROP_UNTIL: str
 
 class Delta(str, Enum):
     ONLY_UPDATE_IF: str
@@ -41,15 +41,15 @@
     schema: Incomplete
     report_state: Incomplete
     control_state: Incomplete
     parent: Incomplete
     element: Incomplete
     children_name_mapping: Incomplete
     connection: Incomplete
-    def __init__(self, parent: Device, value_type: ValueBaseType, name: str, value_uuid: Optional[uuid.UUID], type: Optional[str] = ..., permission: PermissionType = ..., min: Optional[Union[int, float]] = ..., max: Optional[Union[int, float]] = ..., step: Optional[Union[int, float]] = ..., encoding: Optional[str] = ..., xsd: Optional[str] = ..., namespace: Optional[str] = ..., period: Optional[int] = ..., delta: Optional[Union[int, float]] = ..., description: Optional[str] = ..., meaningful_zero: Optional[str] = ..., mapping: Optional[bool] = ..., ordered_mapping: Optional[bool] = ..., si_conversion: Optional[str] = ..., unit: Optional[str] = ...) -> None: ...
+    def __init__(self, parent: Device, value_type: ValueBaseType, name: str, value_uuid: Optional[uuid.UUID], type: Optional[str] = ..., permission: PermissionType = ..., min: Optional[Union[int, float]] = ..., max: Optional[Union[int, float]] = ..., step: Optional[Union[int, float]] = ..., encoding: Optional[str] = ..., xsd: Optional[str] = ..., namespace: Optional[str] = ..., period: Optional[int] = ..., delta: Optional[Union[int, float]] = ..., description: Optional[str] = ..., meaningful_zero: Optional[str] = ..., mapping: Optional[Dict[str, Any]] = ..., ordered_mapping: Optional[bool] = ..., si_conversion: Optional[str] = ..., unit: Optional[str] = ...) -> None: ...
     def getControlData(self) -> Optional[Union[float, str]]: ...
     def getControlTimestamp(self) -> Optional[datetime]: ...
     def getReportData(self) -> Optional[Union[float, str]]: ...
     def getReportTimestamp(self) -> Optional[datetime]: ...
     @property
     def name(self) -> str: ...
     @property
```

### Comparing `wappstoiot-0.6.6/wappstoiot/schema/base_schema.py` & `wappstoiot-0.6.7/wappstoiot/schema/base_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,17 +338,17 @@
     meta: Optional[ValueMeta] = Field(None, title='meta-2.0:create')
     state: Optional[List[Union[State, UUID4]]] = None
     eventlog: Optional[List[Union['EventlogItem', UUID4]]] = None
     info: Optional[Info] = None
 
 
 class Number(BaseModel):
-    min: float
-    max: float
-    step: float
+    min: Union[float, int]
+    max: Union[float, int]
+    step: Union[float, int]
     mapping: Optional[Dict[str, Any]] = None
     meaningful_zero: Optional[bool] = None
     ordered_mapping: Optional[bool] = None
     si_conversion: Optional[str] = None
     unit: Optional[str] = None
 
 
@@ -488,18 +488,22 @@
 class DeleteList(BaseModel):
     deleted: List[UUID4]
     code: int
     message: str = "Deleted"
     meta: ApiMetaInfo
 
 
-WappstoObject = Union[
-    Network,
-    Device,
+Value = Union[
     StringValue,
     NumberValue,
     BlobValue,
     XmlValue,
+]
+
+WappstoObject = Union[
+    Network,
+    Device,
+    Value,
     State,
     IdList,
     DeleteList,
 ]
```

### Comparing `wappstoiot-0.6.6/wappstoiot/schema/base_schema.pyi` & `wappstoiot-0.6.7/wappstoiot/schema/base_schema.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -236,17 +236,17 @@
     status: Optional[EventStatus]
     meta: Optional[ValueMeta]
     state: Optional[List[Union[State, UUID4]]]
     eventlog: Optional[List[Union['EventlogItem', UUID4]]]
     info: Optional[Info]
 
 class Number(BaseModel):
-    min: float
-    max: float
-    step: float
+    min: Union[float, int]
+    max: Union[float, int]
+    step: Union[float, int]
     mapping: Optional[Dict[str, Any]]
     meaningful_zero: Optional[bool]
     ordered_mapping: Optional[bool]
     si_conversion: Optional[str]
     unit: Optional[str]
 
 class String(BaseModel):
@@ -329,8 +329,9 @@
         extra: Incomplete
 
 class DeleteList(BaseModel):
     deleted: List[UUID4]
     code: int
     message: str
     meta: ApiMetaInfo
-WappstoObject = Union[Network, Device, StringValue, NumberValue, BlobValue, XmlValue, State, IdList, DeleteList]
+Value = Union[StringValue, NumberValue, BlobValue, XmlValue]
+WappstoObject = Union[Network, Device, Value, State, IdList, DeleteList]
```

### Comparing `wappstoiot-0.6.6/wappstoiot/schema/iot_schema.py` & `wappstoiot-0.6.7/wappstoiot/schema/iot_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,18 +70,18 @@
     NETWORK = "network"
     DEVICE = "device"
     VALUE = "value"
     STATE = "state"
 
 
 ObjectType2BaseModel: Dict[WappstoObjectType, Any] = {
-        WappstoObjectType.NETWORK: Network,
-        WappstoObjectType.DEVICE: Device,
-        WappstoObjectType.VALUE: ValueUnion,
-        WappstoObjectType.STATE: State,
+    WappstoObjectType.NETWORK: Network,
+    WappstoObjectType.DEVICE: Device,
+    WappstoObjectType.VALUE: ValueUnion,
+    WappstoObjectType.STATE: State,
 }
 
 
 def url_parser(url: str) -> List[Tuple[WappstoObjectType, Optional[uuid.UUID]]]:
     r_list: List[Tuple[WappstoObjectType, Optional[uuid.UUID]]] = []
     obj_type: Optional[WappstoObjectType] = None
     if url is None:
@@ -189,15 +189,16 @@
     def path_check(cls, v, values, **kwargs):
         url_parser(v)
         return v
 
     @validator("data", pre=True, always=True)
     def url_data_mapper(
         cls, v, values, **kwargs
-    ) -> Optional[Union[
+    ) -> Optional[
+        Union[
             Network,
             Device,
             ValueUnion,
             State,
             IdList,
             DeleteList,
         ]
```

### Comparing `wappstoiot-0.6.6/wappstoiot/schema/iot_schema.pyi` & `wappstoiot-0.6.7/wappstoiot/schema/iot_schema.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/service/iot_api.py` & `wappstoiot-0.6.7/wappstoiot/service/iot_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,37 +437,37 @@
     #     self._cb_handler(data=data, method=WappstoMethod.HEAD)
     #     return Success()
 
     # #########################################################################
     #                               Helper API
     # #########################################################################
 
-    def ping(self):
+    def ping(self) -> None:
         return self._no_reply_send(
             data=None,
             url="/network",
             method=WappstoMethod.HEAD
         )
 
     # #########################################################################
     #                               Network API
     # #########################################################################
 
     def subscribe_network_event(
         self,
         uuid: UUID,
         callback: Callable[[Network, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.setdefault(uuid, []).append(callback)
 
     def unsubscribe_network_event(
         self,
         uuid: UUID,
         callback: Callable[[Network, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.get(uuid, []).remove(callback)
 
     def post_network(self, data: Network) -> bool:
         # url=f"/services/2.0/network",
         return self._no_reply_send(
             data=data,
             url="/network/",
@@ -502,22 +502,22 @@
     #                                Device API
     # #########################################################################
 
     def subscribe_device_event(
         self,
         uuid: UUID,
         callback: Callable[[Device, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.setdefault(uuid, []).append(callback)
 
     def unsubscribe_device_event(
         self,
         uuid: UUID,
         callback: Callable[[Device, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.get(uuid, []).remove(callback)
 
     def post_device(self, network_uuid: UUID, data: Device) -> bool:
         # url=f"/services/2.0/{uuid}/device",
         return self._no_reply_send(
             data=data,
             url=f"/network/{network_uuid}/device/",
@@ -567,22 +567,22 @@
     #                                 Value API
     # #########################################################################
 
     def subscribe_value_event(
         self,
         uuid: UUID,
         callback: Callable[[ValueUnion, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.setdefault(uuid, []).append(callback)
 
     def unsubscribe_value_event(
         self,
         uuid: UUID,
         callback: Callable[[Device, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.get(uuid, []).remove(callback)
 
     def post_value(self, device_uuid: UUID, data: ValueUnion) -> bool:
         # url=f"/services/2.0/{uuid}/value",
         return self._no_reply_send(
             data=data,
             url=f"/device/{device_uuid}/value/",
@@ -632,22 +632,22 @@
     #                                State API
     # #########################################################################
 
     def subscribe_state_event(
         self,
         uuid: UUID,
         callback: Callable[[State, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.setdefault(uuid, []).append(callback)
 
     def unsubscribe_state_event(
         self,
         uuid: UUID,
         callback: Callable[[Device, WappstoMethod], None]
-    ):
+    ) -> None:
         self.subscribers.get(uuid, []).remove(callback)
 
     def post_state(self, value_uuid: UUID, data: State) -> bool:
         # url=f"/services/2.0/{uuid}/state",
         return self._no_reply_send(
             data=data,
             url=f"/value/{value_uuid}/state/",
```

### Comparing `wappstoiot-0.6.6/wappstoiot/service/iot_api.pyi` & `wappstoiot-0.6.7/wappstoiot/service/iot_api.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -23,34 +23,34 @@
     connection: Incomplete
     subscribers: Incomplete
     jsonrpc: Incomplete
     killed: Incomplete
     workers: Incomplete
     def __init__(self, ca: Path, crt: Path, key: Path, worker_count: int = ..., fast_send: bool = ...) -> None: ...
     def close(self) -> None: ...
-    def ping(self): ...
-    def subscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethod], None]): ...
-    def unsubscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethod], None]): ...
+    def ping(self) -> None: ...
+    def subscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethod], None]) -> None: ...
+    def unsubscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethod], None]) -> None: ...
     def post_network(self, data: Network) -> bool: ...
     def put_network(self, uuid: UUID, data: Network) -> bool: ...
     def get_network(self, uuid: UUID) -> Optional[Network]: ...
     def delete_network(self, uuid: UUID) -> bool: ...
-    def subscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]): ...
-    def unsubscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]): ...
+    def subscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]) -> None: ...
+    def unsubscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]) -> None: ...
     def post_device(self, network_uuid: UUID, data: Device) -> bool: ...
     def put_device(self, uuid: UUID, data: Device) -> bool: ...
     def get_device_where(self, network_uuid: UUID, **kwargs: str) -> Optional[UUID]: ...
     def get_device(self, uuid: UUID) -> Union[Device, None]: ...
     def delete_device(self, uuid: UUID) -> bool: ...
-    def subscribe_value_event(self, uuid: UUID, callback: Callable[[ValueUnion, WappstoMethod], None]): ...
-    def unsubscribe_value_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]): ...
+    def subscribe_value_event(self, uuid: UUID, callback: Callable[[ValueUnion, WappstoMethod], None]) -> None: ...
+    def unsubscribe_value_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]) -> None: ...
     def post_value(self, device_uuid: UUID, data: ValueUnion) -> bool: ...
     def put_value(self, uuid: UUID, data: ValueUnion) -> bool: ...
     def get_value_where(self, device_uuid: UUID, **kwargs: str) -> Optional[UUID]: ...
     def get_value(self, uuid: UUID) -> Union[ValueUnion, None]: ...
     def delete_value(self, uuid: UUID) -> bool: ...
-    def subscribe_state_event(self, uuid: UUID, callback: Callable[[State, WappstoMethod], None]): ...
-    def unsubscribe_state_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]): ...
+    def subscribe_state_event(self, uuid: UUID, callback: Callable[[State, WappstoMethod], None]) -> None: ...
+    def unsubscribe_state_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]) -> None: ...
     def post_state(self, value_uuid: UUID, data: State) -> bool: ...
     def put_state(self, uuid: UUID, data: State) -> bool: ...
     def get_state(self, uuid: UUID) -> Union[State, None]: ...
     def delete_state(self, uuid: UUID) -> bool: ...
```

### Comparing `wappstoiot-0.6.6/wappstoiot/service/template.py` & `wappstoiot-0.6.7/wappstoiot/service/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,15 +34,23 @@
     # #########################################################################
 
     @abstractmethod
     def subscribe_network_event(
         self,
         uuid: UUID,
         callback: Callable[[Network, WappstoMethods], None]
-    ):
+    ) -> None:
+        pass
+
+    @abstractmethod
+    def unsubscribe_network_event(
+        self,
+        uuid: UUID,
+        callback: Callable[[Network, WappstoMethods], None]
+    ) -> None:
         pass
 
     @abstractmethod
     def post_network(self, data) -> bool:
         # url=f"/services/2.0/network/{uuid}",
         pass
 
@@ -63,15 +71,23 @@
     # #########################################################################
 
     @abstractmethod
     def subscribe_device_event(
         self,
         uuid: UUID,
         callback: Callable[[Device, WappstoMethods], None]
-    ):
+    ) -> None:
+        pass
+
+    @abstractmethod
+    def unsubscribe_device_event(
+        self,
+        uuid: UUID,
+        callback: Callable[[Device, WappstoMethods], None]
+    ) -> None:
         pass
 
     @abstractmethod
     def post_device(self, network_uuid: UUID, data: Device) -> bool:
         # url=f"/services/2.0/{uuid}/device",
         pass
 
@@ -98,15 +114,23 @@
     ValueUnion = Union[StringValue, NumberValue, BlobValue, XmlValue]
 
     @abstractmethod
     def subscribe_value_event(
         self,
         uuid: UUID,
         callback: Callable[[ValueUnion, WappstoMethods], None]
-    ):
+    ) -> None:
+        pass
+
+    @abstractmethod
+    def unsubscribe_value_event(
+        self,
+        uuid: UUID,
+        callback: Callable[[Device, WappstoMethods], None]
+    ) -> None:
         pass
 
     @abstractmethod
     def post_value(self, device_uuid: UUID, data: ValueUnion) -> bool:
         # url=f"/services/2.0/{uuid}/value",
         pass
 
@@ -131,15 +155,23 @@
     # #########################################################################
 
     @abstractmethod
     def subscribe_state_event(
         self,
         uuid: UUID,
         callback: Callable[[State, WappstoMethods], None]
-    ):
+    ) -> None:
+        pass
+
+    @abstractmethod
+    def unsubscribe_state_event(
+        self,
+        uuid: UUID,
+        callback: Callable[[Device, WappstoMethods], None]
+    ) -> None:
         pass
 
     @abstractmethod
     def post_state(self, value_uuid: UUID, data: State) -> bool:
         # url=f"/services/2.0/{uuid}/state",
         pass
```

### Comparing `wappstoiot-0.6.6/wappstoiot/service/template.pyi` & `wappstoiot-0.6.7/wappstoiot/service/template.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -11,50 +11,58 @@
     SENDING: str
     SENDERROR: str
     SEND: str
     ERROR: str
 
 class ServiceClass(ABC, metaclass=abc.ABCMeta):
     @abstractmethod
-    def subscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethods], None]): ...
+    def subscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethods], None]) -> None: ...
+    @abstractmethod
+    def unsubscribe_network_event(self, uuid: UUID, callback: Callable[[Network, WappstoMethods], None]) -> None: ...
     @abstractmethod
     def post_network(self, data) -> bool: ...
     @abstractmethod
     def put_network(self, uuid: UUID, data) -> bool: ...
     @abstractmethod
     def get_network(self, uuid: UUID) -> Union[Network, None]: ...
     @abstractmethod
     def delete_network(self, uuid: UUID) -> bool: ...
     @abstractmethod
-    def subscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethods], None]): ...
+    def subscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethods], None]) -> None: ...
+    @abstractmethod
+    def unsubscribe_device_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethods], None]) -> None: ...
     @abstractmethod
     def post_device(self, network_uuid: UUID, data: Device) -> bool: ...
     @abstractmethod
     def put_device(self, uuid: UUID, data: Device) -> bool: ...
     @abstractmethod
     def get_device_where(self, network_uuid: UUID, **kwargs: str) -> Optional[UUID]: ...
     @abstractmethod
     def get_device(self, uuid: UUID) -> Union[Device, None]: ...
     @abstractmethod
     def delete_device(self, uuid: UUID) -> bool: ...
     ValueUnion: Incomplete
     @abstractmethod
-    def subscribe_value_event(self, uuid: UUID, callback: Callable[[ValueUnion, WappstoMethods], None]): ...
+    def subscribe_value_event(self, uuid: UUID, callback: Callable[[ValueUnion, WappstoMethods], None]) -> None: ...
+    @abstractmethod
+    def unsubscribe_value_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethods], None]) -> None: ...
     @abstractmethod
     def post_value(self, device_uuid: UUID, data: ValueUnion) -> bool: ...
     @abstractmethod
     def put_value(self, uuid: UUID, data: ValueUnion) -> bool: ...
     @abstractmethod
     def get_value_where(self, device_uuid: UUID, **kwargs: str) -> Optional[UUID]: ...
     @abstractmethod
     def get_value(self, uuid: UUID) -> Union[ValueUnion, None]: ...
     @abstractmethod
     def delete_value(self, uuid: UUID) -> bool: ...
     @abstractmethod
-    def subscribe_state_event(self, uuid: UUID, callback: Callable[[State, WappstoMethods], None]): ...
+    def subscribe_state_event(self, uuid: UUID, callback: Callable[[State, WappstoMethods], None]) -> None: ...
+    @abstractmethod
+    def unsubscribe_state_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethods], None]) -> None: ...
     @abstractmethod
     def post_state(self, value_uuid: UUID, data: State) -> bool: ...
     @abstractmethod
     def put_state(self, uuid: UUID, data: State) -> bool: ...
     @abstractmethod
     def get_state(self, uuid: UUID) -> Union[State, None]: ...
     @abstractmethod
```

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/Timestamp.py` & `wappstoiot-0.6.7/wappstoiot/utils/Timestamp.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/name_check.py` & `wappstoiot-0.6.7/wappstoiot/utils/name_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """Contain name checking functions."""
 import string
 
 
-wappsto_letters = string.digits + string.ascii_letters + " -_.~"
+wappsto_letters = string.digits + string.ascii_letters + " -_.~" + 'æøåÆØÅöäÖÄ'
 __wappsto_letter_set = set(wappsto_letters)
 
 
 def legal_name(name: str) -> bool:
     """
     Check if the given name is legal.
 
     Args:
         name: the name to check.
+
     Return:
         True, if it is legal,
         False, if it is illegal.
     """
     return not set(name) - __wappsto_letter_set
 
 
 def illegal_characters(name: str) -> str:
     """
     Check if the given name is illegal.
 
     Args:
         name: the name to check.
+
     Return:
         string with all the illegal characters in the name.
     """
     return ''.join(set(name) - __wappsto_letter_set)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/observer.py` & `wappstoiot-0.6.7/wappstoiot/utils/observer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Contain the Observer functionality.
 
-The Observer Pattern, is as design pattern, that 
+The Observer Pattern, is as design pattern, that
 """
 import logging
 import threading
 
 from typing import Any
 from typing import Dict
 from typing import List
@@ -48,15 +48,15 @@
     """
     Post the event with given event name.
 
     Args:
         event_name: An unique name for the given event.
         data: The given event subscriber might want.
     """
-    def executer():
+    def executer() -> None:
         for fn in subscriber.get(event_name, default_subscriber):
             fn(event_name, data)
 
     # NOTE: Needed for ensure that the receive thread do not get blocked.
     th = threading.Thread(target=executer)
     th.start()
```

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/offline_storage.py` & `wappstoiot-0.6.7/wappstoiot/utils/offline_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-"""
-"""
+"""."""
 import logging
 import time
 
 from abc import ABC
 from abc import abstractmethod
 from contextlib import contextmanager
 from pathlib import Path
 
 
+from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Union
 
 
 class OfflineStorage(ABC):
+
     @abstractmethod
-    def save(self, data: str) -> None: ...
+    def save(self, data: str) -> None:
+        ...
+
     @abstractmethod
-    def load(self, max_count: Optional[int] = None) -> List[str]: ...
+    def load(self, max_count: Optional[int] = None) -> List[str]:
+        ...
 
 
 class OfflineStorageFiles(OfflineStorage):
     """
     Timed over 1M runs.
 
     In [5]: kk = write()
@@ -48,21 +52,21 @@
         self.loc.mkdir(exist_ok=True)
         self.log.info(f"Location created: {self.loc}")
         self._files = sorted(
             x for x in self.loc.iterdir()
             if x.is_file() and x.suffixes and x.suffixes[-1] == self.suffix
         )
 
-    def _sort_files(self, count) -> List[Path]:
+    def _sort_files(self, count: int) -> List[Path]:
         temp = self._files[:count]
         del self._files[:count]
         return temp
 
     @contextmanager
-    def auto_save(self, data: str):
+    def auto_save(self, data: str) -> Generator:
         """Used when replying on a trace."""
         # self.send_pending(name=name)  # Are send on class creation.
         try:
             yield
         except Exception:
             self.save(data=data)
             raise
```

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/offline_storage.pyi` & `wappstoiot-0.6.7/wappstoiot/utils/offline_storage.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import abc
 from _typeshed import Incomplete
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Generator, List, Optional, Union
 
 class OfflineStorage(ABC, metaclass=abc.ABCMeta):
     @abstractmethod
     def save(self, data: str) -> None: ...
     @abstractmethod
     def load(self, max_count: Optional[int] = ...) -> List[str]: ...
 
 class OfflineStorageFiles(OfflineStorage):
     log: Incomplete
     loc: Incomplete
     suffix: str
     def __init__(self, location: Union[Path, str]) -> None: ...
-    def auto_save(self, data: str): ...
+    def auto_save(self, data: str) -> Generator: ...
     def save(self, data: str) -> None: ...
     def load(self, max_count: Optional[int] = ...) -> List[str]: ...
```

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/tracer.py` & `wappstoiot-0.6.7/wappstoiot/utils/tracer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import random
 import string
 
 from contextlib import contextmanager
 from enum import Enum
 
+from typing import Any
 from typing import List
 from typing import Optional
 
 
 import requests
 
 from . import Timestamp
@@ -34,19 +35,19 @@
     ):
         self.log = logging.getLogger(__name__)
         self.log.addHandler(logging.NullHandler())
         self.class_obj = class_obj
         self.tracer = tracer
         self.tracing_obj = tracing_obj
 
-    def __getattr__(self, attr_name):
+    def __getattr__(self, attr_name) -> Any:
         if attr_name not in self.tracing_obj:
             return getattr(self.class_obj, attr_name)
 
-        def wrapper(*args, **kwargs):
+        def wrapper(*args, **kwargs) -> None:
             with self.tracer.tracing():
                 getattr(self.class_obj, attr_name)(*args, **kwargs)
 
         return wrapper
 
 
 class Trace:
@@ -76,18 +77,16 @@
         """Generate a Trace ID."""
         return "WappstoIoT_" + "".join(random.choices(
             string.ascii_letters + string.digits,
             k=10
         ))
 
     @staticmethod
-    def _find_parent_id(jsonrpc_elemt) -> Optional[str]:
-        """
-        Check if a trace package should be send if so it returns the parent ID.
-        """
+    def _find_parent_id(jsonrpc_elemt: dict) -> Optional[str]:
+        """Check if a trace package should be send if so it returns the parent ID."""
         if isinstance(jsonrpc_elemt, dict):
             return jsonrpc_elemt.get(
                 'params', {}).get(
                 'meta', {}).get(
                 'trace', None
             )
         return jsonrpc_elemt.params.meta.trace
```

### Comparing `wappstoiot-0.6.6/wappstoiot/utils/tracer.pyi` & `wappstoiot-0.6.7/wappstoiot/utils/tracer.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from . import Timestamp as Timestamp
 from _typeshed import Incomplete
 from enum import Enum
-from typing import List, Optional
+from typing import Any, List, Optional
 
 force_trace: bool
 
 class TraceStatus(str, Enum):
     PENDING: str
     OK: str
     FAIL: str
 
 class TraceWrapper:
     log: Incomplete
     class_obj: Incomplete
     tracer: Incomplete
     tracing_obj: Incomplete
     def __init__(self, class_obj: object, tracer: object, tracing_obj: List[str]) -> None: ...
-    def __getattr__(self, attr_name): ...
+    def __getattr__(self, attr_name) -> Any: ...
 
 class Trace:
     log: Incomplete
     id: Incomplete
     parent: Incomplete
     name: Incomplete
     timestamp: Incomplete
```

### Comparing `wappstoiot-0.6.6/wappstoiot.egg-info/PKG-INFO` & `wappstoiot-0.6.7/wappstoiot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wappstoiot
-Version: 0.6.6
+Version: 0.6.7
 Summary: Simple Wappsto Python user-interface to Wappsto IoT
 Home-page: https://github.com/Wappsto/python-wappsto-iot
 Author: Seluxit A/S
 Author-email: support@seluxit.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -121,14 +121,23 @@
 
 ## License
 
 This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details.
 
 
 
+v0.6.7 (Jul 07 2023)
+===============================================================================
+## Added
+ * Scandinavian special letters to the legal list
+
+## Changed
+ * Updated the `wappstoiot.ValueTemplate` to version v0.0.5
+ * Set Pydantic version to be `v1.10.11` until migration to `v2` is done.
+
 v0.6.6 (Jun 22 2023)
 ===============================================================================
 ## Added
  * Code Stub.
 
 ## Changed
  * Now inform which characters are illegal in the given name.
```

### Comparing `wappstoiot-0.6.6/wappstoiot.egg-info/SOURCES.txt` & `wappstoiot-0.6.7/wappstoiot.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/fusion-platform-python-sdk-1.7.3.tar.gz` & `tmp/fusion-platform-python-sdk-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-platform-python-sdk-1.7.3.tar", last modified: Mon Jun 26 09:30:19 2023, max compression
+gzip compressed data, was "fusion-platform-python-sdk-1.7.4.tar", last modified: Fri Jul  7 12:49:06 2023, max compression
```

## Comparing `fusion-platform-python-sdk-1.7.3.tar` & `fusion-platform-python-sdk-1.7.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-26 09:30:19.159888 fusion-platform-python-sdk-1.7.3/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.7.3/LICENSE.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.7.3/MANIFEST.in
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-06-26 09:30:19.159577 fusion-platform-python-sdk-1.7.3/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2023-06-26 08:49:45.000000 fusion-platform-python-sdk-1.7.3/README.md
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-26 09:30:19.144261 fusion-platform-python-sdk-1.7.3/fusion_platform/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     6865 2023-06-26 09:30:16.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/__main__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/base.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/command.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-26 09:30:19.146630 fusion-platform-python-sdk-1.7.3/fusion_platform/common/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/common/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/common/raise_thread.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/common/utilities.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4579 2023-06-26 08:54:13.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/detailed_example.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/documentation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1593164 2023-06-07 06:22:45.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/fusion_platform_sdk.pdf
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2237 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/glasgow.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)  1869438 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/lake_district.geojson
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/localisations.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/localise.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-26 09:30:19.156901 fusion-platform-python-sdk-1.7.3/fusion_platform/models/
--rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/__init__.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/credit.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/credit.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/data.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/data.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/data_file.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/data_file.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/fields.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/model.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/organisation.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/organisation.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    50701 2023-05-26 13:32:08.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-05-10 09:30:14.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10487 2023-05-23 06:25:23.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution_log.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution_log.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/service.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/service.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-06-26 09:30:17.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/user.md
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/models/user.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1891 2023-06-26 08:54:13.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/quick_example.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/session.py
--rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-06-26 09:30:16.000000 fusion-platform-python-sdk-1.7.3/fusion_platform/translations.py
-drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-06-26 09:30:19.159104 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/
--rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-06-26 09:30:18.000000 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1773 2023-06-26 09:30:18.000000 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-06-26 09:30:18.000000 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-06-26 09:30:18.000000 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-06-26 09:30:18.000000 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/requires.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-06-26 09:30:18.000000 fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-06-26 09:30:19.159994 fusion-platform-python-sdk-1.7.3/setup.cfg
--rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-06-26 09:30:16.000000 fusion-platform-python-sdk-1.7.3/setup.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.870259 fusion-platform-python-sdk-1.7.4/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1096 2022-02-03 08:52:04.000000 fusion-platform-python-sdk-1.7.4/LICENSE.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      205 2022-03-08 12:17:05.000000 fusion-platform-python-sdk-1.7.4/MANIFEST.in
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-07-07 12:49:06.869967 fusion-platform-python-sdk-1.7.4/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4455 2023-06-26 08:49:45.000000 fusion-platform-python-sdk-1.7.4/README.md
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.856519 fusion-platform-python-sdk-1.7.4/fusion_platform/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     6865 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      268 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/__main__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1456 2023-03-07 10:01:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/base.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      280 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/command.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.857895 fusion-platform-python-sdk-1.7.4/fusion_platform/common/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      133 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/common/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1398 2022-03-21 08:32:55.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/common/raise_thread.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5271 2022-10-06 09:40:52.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/common/utilities.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4579 2023-06-26 08:54:13.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/detailed_example.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4092 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/documentation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  1593164 2023-06-07 06:22:45.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/fusion_platform_sdk.pdf
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     4697 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/glasgow.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)  3746742 2023-07-06 06:17:51.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/lake_district.geojson
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2863 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/localisations.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1189 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/localise.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.867282 fusion-platform-python-sdk-1.7.4/fusion_platform/models/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      137 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/__init__.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1090 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3410 2022-06-01 12:37:49.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      703 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14299 2023-01-27 11:53:10.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2852 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10830 2023-01-13 10:57:50.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    12103 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/fields.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    31868 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/model.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1475 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    14976 2023-06-15 13:13:57.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1952 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    50774 2023-07-07 12:47:31.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     2602 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     8982 2023-07-06 09:45:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     3359 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10513 2023-07-06 06:16:57.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)      312 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution_log.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1854 2022-03-08 12:33:32.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution_log.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5701 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     9735 2023-05-24 05:51:58.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1063 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.md
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5676 2022-06-27 13:37:30.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1891 2023-06-26 08:54:13.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/quick_example.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)    10556 2023-03-28 13:58:58.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/session.py
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     7576 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/fusion_platform/translations.py
+drwxr-xr-x   0 matthewcasey   (501) staff       (20)        0 2023-07-07 12:49:06.869448 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     5143 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1773 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)        1 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       77 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       70 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       16 2023-07-07 12:49:06.000000 fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 matthewcasey   (501) staff       (20)       38 2023-07-07 12:49:06.870365 fusion-platform-python-sdk-1.7.4/setup.cfg
+-rw-r--r--   0 matthewcasey   (501) staff       (20)     1551 2023-07-07 12:49:04.000000 fusion-platform-python-sdk-1.7.4/setup.py
```

### Comparing `fusion-platform-python-sdk-1.7.3/LICENSE.txt` & `fusion-platform-python-sdk-1.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/PKG-INFO` & `fusion-platform-python-sdk-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.7.3
+Version: 1.7.4
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.7.3/README.md` & `fusion-platform-python-sdk-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/__init__.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 files, create and execute processes, monitor their execution and then download the corresponding results. Additional functionality is available directly via the
 API, and this is defined within the corresponding OpenAPI 3.0 specification, which can be obtained via a support request.
 
 &copy; [Digital Content Analysis Technology Ltd](https://www.d-cat.co.uk)
 """
 
 # Do not modify the following two lines as they are maintained by the version.sh script.
-__version__ = '1.7.3'
-__version_date__ = '2023-06-26T09:30:16Z'
+__version__ = '1.7.4'
+__version_date__ = '2023-07-07T12:49:04Z'
 
 # Exclude certain sub-modules from documentation.
 # @formatter:off
 __pdoc__ = {
     'base': False,
     'command': False,
     'common': False,
```

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/base.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/base.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/common/raise_thread.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/common/raise_thread.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/common/utilities.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/common/utilities.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/detailed_example.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/detailed_example.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/documentation.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/documentation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/fusion_platform_sdk.pdf` & `fusion-platform-python-sdk-1.7.4/fusion_platform/fusion_platform_sdk.pdf`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/localisations.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/localisations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/localise.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/localise.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/credit.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/credit.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/credit.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/data.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/data.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/data_file.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/data_file.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/data_file.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/fields.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/fields.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/model.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/model.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/organisation.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/organisation.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/organisation.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         return Option.options_iterator(self._model.get(self.__class__._FIELD_OPTIONS, []))
 
     def __repr__(self):
         """
         Returns:
             A string representation of the object.
         """
-        return f"{self.name} ({self.ssd_id}, intermediate {self.dispatch_intermediate}): {self.documentation_summary}"
+        return f"{self.name} ({self.ssd_id}, intermediate {self.dispatch_intermediate if hasattr(self, self.__class__._FIELD_DISPATCH_INTERMEDIATE) else False}): {self.documentation_summary}"
 
 
 # Define the model schema classes. These are maintained from the API definitions.
 
 class ProcessChainOptionSchema(Schema):
     """
     Nested schema class for SSD chain option.
```

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_execution.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_execution.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_execution.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     cpu = fields.Decimal(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     memory = fields.Decimal(required=True, metadata={'read_only': True})  # Changed to prevent this being updated.
     actions = fields.List(fields.Nested(ProcessServiceExecutionActionSchema()), allow_none=True)
     options = fields.List(fields.Nested(ProcessServiceExecutionOptionSchema()), allow_none=True,
                           metadata={'read_only': True})  # Changed to prevent this being updated.
     inputs = fields.List(fields.UUID(required=True), allow_none=True, metadata={'hide': True})  # Changed to hide as an attribute.
     outputs = fields.List(fields.UUID(required=True), allow_none=True, metadata={'hide': True})  # Changed to hide as an attribute.
+    # Removed storage_id.
     intermediate = fields.Boolean(allow_none=True)
     # Removed task_id.
     # Removed task_definition_id.
     # Removed access_point_ids.
     # Removed security_group_id.
     success = fields.Boolean(allow_none=True, metadata={'read_only': True})  # Changed to prevent this being updated.
```

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/process_service_execution_log.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/process_service_execution_log.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/service.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/service.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/service.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/user.md` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.md`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/models/user.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/models/user.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/quick_example.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/quick_example.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/session.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/session.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform/translations.py` & `fusion-platform-python-sdk-1.7.4/fusion_platform/translations.py`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/PKG-INFO` & `fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-platform-python-sdk
-Version: 1.7.3
+Version: 1.7.4
 Summary: Python SDK used to interact with the Fusion Platform(r)
 Home-page: https://github.com/d-cat-support/fusion-platform-python-sdk
 Author: Digital Content Analysis Technology Ltd
 Author-email: support@d-cat.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion-platform-python-sdk-1.7.3/fusion_platform_python_sdk.egg-info/SOURCES.txt` & `fusion-platform-python-sdk-1.7.4/fusion_platform_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-platform-python-sdk-1.7.3/setup.py` & `fusion-platform-python-sdk-1.7.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Find the package root directory.
 PACKAGE_DIR = pathlib.Path(__file__).parent
 
 # Set up the package.
 # @formatter:off
 setup(
     name='fusion-platform-python-sdk',
-    version='1.7.3',
+    version='1.7.4',
     description='Python SDK used to interact with the Fusion Platform(r)',
     long_description=(PACKAGE_DIR / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/d-cat-support/fusion-platform-python-sdk',
     author='Digital Content Analysis Technology Ltd',
     author_email='support@d-cat.co.uk',
     license='MIT',
```


# Comparing `tmp/pymodaq_plugins_mock-4.0.2.tar.gz` & `tmp/pymodaq_plugins_mock-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_mock-4.0.2.tar", last modified: Tue Apr 25 16:45:13 2023, max compression
+gzip compressed data, was "pymodaq_plugins_mock-4.1.0.tar", last modified: Fri Jul  7 12:07:06 2023, max compression
```

## Comparing `pymodaq_plugins_mock-4.0.2.tar` & `pymodaq_plugins_mock-4.1.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.492589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:00.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:13.488589 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 16:45:13.000000 pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.939533 pymodaq_plugins_mock-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 12:07:06.939533 pymodaq_plugins_mock-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:07:06.939533 pymodaq_plugins_mock-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTauMulti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.939533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:06:57.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:07:06.935533 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-07 12:07:06.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-07 12:07:06.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:07:06.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 12:07:06.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 12:07:06.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 12:07:06.000000 pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_mock-4.0.2/LICENSE` & `pymodaq_plugins_mock-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/PKG-INFO` & `pymodaq_plugins_mock-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_mock
-Version: 4.0.2
+Version: 4.1.0
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_mock-4.0.2/README.rst` & `pymodaq_plugins_mock-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/setup.py` & `pymodaq_plugins_mock-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
         =============== ==============
     """
     _controller_units = ActuatorWrapperWithTau.units
 
     is_multiaxes = True  # set to True if this plugin is controlled for a multiaxis controller (with a unique communication link)
     axes_names = ['X', 'Y', 'Z']  # "list of strings of the multiaxes
     _epsilon = 0.01
-    params = [
-        {'title': 'Tau (ms):', 'name': 'tau', 'type': 'int', 'value': 500, 'tip': 'Characteristic evolution time'}
-        ] + comon_parameters_fun(is_multiaxes, axes_names)
+    params = \
+        [
+            {'title': 'Tau (ms):', 'name': 'tau', 'type': 'int', 'value': 500, 'tip': 'Characteristic evolution time'},
+             ] + comon_parameters_fun(is_multiaxes, axes_names, epsilon=_epsilon)
 
     def ini_attributes(self):
         self.controller: ActuatorWrapperWithTau = None
 
     def get_actuator_value(self):
         # TODO for your custom plugin
         pos = self.controller.get_value()
@@ -37,14 +38,15 @@
 
     def commit_settings(self, param):
         if param.name() == 'tau':
             self.controller.tau = param.value() / 1000  # controller need a tau in seconds while the param tau is in ms
         elif param.name() == 'epsilon':
             self.controller.epsilon = param.value()
 
+
     def ini_stage(self, controller=None):
         """Actuator communication initialization
 
         Parameters
         ----------
         controller: (object)
             custom object of a PyMoDAQ plugin (Slave case). None if only one actuator by controller (Master case)
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from qtpy import QtWidgets
 
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import DataFromPlugins
+from pymodaq.utils.data import DataFromPlugins, DataToExport
 import numpy as np
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters, main
 
 from pymodaq.utils.math_utils import gauss1D
 
 
 class DAQ_0DViewer_Mock(DAQ_Viewer_base):
@@ -88,16 +88,17 @@
                                new_controller='Mock controller')
 
         self.set_Mock_data()
         self.emit_status(ThreadCommand('update_main_settings', [['wait_time'],
                                                                 self.settings.child('wait_time').value(), 'value']))
 
         # initialize viewers with the future type of data
-        self.data_grabed_signal.emit(
-            [DataFromPlugins(name='Mock1', data=[np.array([0])], dim='Data0D', labels=['Mock1', 'label2'])])
+        self.dte_signal_temp.emit(DataToExport('Mock0D', data=[DataFromPlugins(name='Mock1', data=[np.array([0])],
+                                                                               dim='Data0D',
+                                                                               labels=['Mock1', 'label2'])]))
 
         initialized = True
         info = 'RAS'
         return info, initialized
 
     def close(self):
         """
@@ -127,21 +128,24 @@
             data = np.roll(data, self.ind_data)
             if Naverage > 1:
                 data_tot.append(np.array([np.mean(data[0:Naverage - 1])]))
             else:
                 data_tot.append(np.array([data[0]]))
 
         if self.settings.child('sep_viewers').value():
-            dat = [DataFromPlugins(name=f'Mock_{ind:03}', data=[data], dim='Data0D',
-                                   labels=[f'mock data {ind:03}']) for ind, data in enumerate(data_tot)]
-            self.data_grabed_signal.emit(dat)
+            dat = DataToExport('Mock0D',
+                               data=[DataFromPlugins(name=f'Mock_{ind:03}', data=[data], dim='Data0D',
+                                                     labels=[f'mock data {ind:03}']) for ind, data in
+                                     enumerate(data_tot)])
+            self.dte_signal.emit(dat)
 
         else:
-            self.data_grabed_signal.emit([DataFromPlugins(name='Mock0D', data=data_tot,
-                                                          dim='Data0D', labels=['dat0', 'data1'])])
+            self.dte_signal.emit(DataToExport('Mock0D',
+                                              data=[DataFromPlugins(name='Mock0D', data=data_tot,
+                                                                    dim='Data0D', labels=['dat0', 'data1'])]))
         self.ind_data += 1
         if self.settings['lcd']:
             if not self.lcd_init:
                 self.emit_status(ThreadCommand('init_lcd', [dict(labels=['dat0', 'data1'], Nvals=2, digits=6)]))
                 QtWidgets.QApplication.processEvents()
                 self.lcd_init = True
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from qtpy import QtWidgets
 from qtpy.QtCore import Signal, QThread, Slot
 from pymodaq.utils import daq_utils as utils
-from pymodaq.utils.data import DataFromPlugins
+from pymodaq.utils.data import DataFromPlugins, DataToExport
 import numpy as np
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from pymodaq.utils.daq_utils import gauss1D
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 from pymodaq.utils.scanner import ScanParameters
@@ -150,16 +150,17 @@
         else:
             self.controller = "Mock controller"
         self.emit_status(utils.ThreadCommand('update_main_settings', [['wait_time'],
                                                                       self.settings.child(('wait_time')).value(),
                                                                       'value']))
 
         # initialize viewers with the future type of data
-        self.data_grabed_signal.emit(
-            [utils.DataFromPlugins(name='Mock1', data=[np.array(0)], dim='Data0D', labels=['RandomGaussians'])])
+        self.dte_signal_temp.emit(DataToExport('MockAdaptive',
+                                               data=[DataFromPlugins(name='Mock1', data=[np.array(0)],
+                                                                     dim='Data0D', labels=['RandomGaussians'])]))
 
         self.status.initialized = True
         self.status.controller = self.controller
         return self.status
 
     def close(self):
         """
@@ -197,16 +198,17 @@
             if fun_type == 'Gaussians':
                 data = random_hypergaussians1D(np.roll(x_axis1D, -self.ind_data)[0], coeff)
             else:
                 data = diverging1D(np.roll(x_axis1D, -self.ind_data)[0], coeff)
 
         data = np.array([data + self.settings['noise'] * np.random.rand()])
 
-        self.data_grabed_signal.emit([DataFromPlugins(name='MockAdaptive', data=[data],
-                                                            dim='Data0D', )])
+        self.dte_signal.emit(DataToExport('MockAdaptive',
+                                          data=[DataFromPlugins(name='MockAdaptive', data=[data],
+                                                                dim='Data0D', )]))
         self.ind_data += 1
 
     def stop(self):
         """
             not implemented.
         """
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from qtpy.QtCore import Signal
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_TCP_server
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import DataFromPlugins
+from pymodaq.utils.data import DataFromPlugins, Axis, DataToExport
 
 
-class DAQ_0DViewer_TCPServer(DAQ_Viewer_TCP_server):
+class DAQ_1DViewer_TCPServer(DAQ_Viewer_TCP_server):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
         *x_axis*            1D numpy array
         *y_axis*            1D numpy array
         *data*              double precision float array
@@ -25,19 +25,18 @@
     # params = DAQ_TCP_server.params
 
     command_server = Signal(list)
 
     # params=DAQ_TCP_server.params
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state,
-                         grabber_type='0D')  # initialize base class with commom attributes and methods
+                         grabber_type='1D')  # initialize base class with commom attributes and methods
 
         self.x_axis = None
         self.y_axis = None
         self.data = None
 
     def data_ready(self, data):
         """
             Send the grabed data signal.
         """
-
-        self.data_grabed_signal.emit([DataFromPlugins(name='TCPServer', data=data, dim='Data0D')])
+        self.dte_signal.emit(DataToExport('TCP1D', data=[DataFromPlugins(name='TCP Server', data=data, dim='Data1D')]))
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qtpy.QtCore import QThread
 from qtpy import QtWidgets
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
 import numpy as np
 from easydict import EasyDict as edict
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.data import DataFromPlugins, Axis, DataToExport
 from pymodaq.utils.math_utils import gauss1D, linspace_step
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 from pymodaq.utils.parameter.utils import iter_children
 
 
 class DAQ_1DViewer_Mock_spectro(DAQ_Viewer_base):
     """
@@ -195,16 +195,19 @@
                     self.controller = controller
             else:
                 self.controller = "Mock controller"
             self.set_x_axis()
             self.set_Mock_data()
 
             # initialize viewers with the future type of data
-            self.data_grabed_signal_temp.emit([DataFromPlugins(name='Mock1', data=self.data_mock, dim='Data1D',
-                                                               axes=[self.x_axis], labels=['Mock1', 'label2']), ])
+            self.dte_signal_temp.emit(DataToExport('Mock1D',
+                                                   data=[DataFromPlugins(name='Mock1', data=self.data_mock,
+                                                                         dim='Data1D',
+                                                                         axes=[self.x_axis],
+                                                                         labels=['Mock1', 'label2']),]))
 
             self.status.initialized = True
             self.status.controller = self.controller
             self.status.x_axis = self.x_axis
             return self.status
 
         except Exception as e:
@@ -248,18 +251,20 @@
 
             for ind, data in enumerate(data_tmp):
                 data_tot[ind] += data
 
         data_tot = [data / Naverage for data in data_tot]
         QThread.msleep(self.settings.child('exposure_ms').value())
         if not self._update_x_axis:
-            self.data_grabed_signal.emit([DataFromPlugins(name='Mock1D', data=data_tot, dim='Data1D',)])
+            self.dte_signal.emit(DataToExport('Mock1D',
+                                              data=[DataFromPlugins(name='Mock1D', data=data_tot, dim='Data1D',)]))
         else:
-            self.data_grabed_signal.emit([DataFromPlugins(name='Mock1D', data=data_tot, dim='Data1D',
-                                                          axes=[self.x_axis])])
+            self.dte_signal.emit(DataToExport('Mock1D',
+                                              data=[DataFromPlugins(name='Mock1D', data=data_tot, dim='Data1D',
+                                                                    axes=[self.x_axis])]))
             self._update_x_axis = False
 
     def stop(self):
         """
             not implemented.
         """
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 from qtpy.QtCore import Signal
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_TCP_server
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.data import DataFromPlugins, DataToExport
 
 
-class DAQ_1DViewer_TCPServer(DAQ_Viewer_TCP_server):
+class DAQ_0DViewer_TCPServer(DAQ_Viewer_TCP_server):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
         *x_axis*            1D numpy array
         *y_axis*            1D numpy array
         *data*              double precision float array
         ================= ==============================
 
         See Also
         --------
         utility_classes.DAQ_TCP_server
     """
     params_GRABBER = []
-
-    # params = DAQ_TCP_server.params
-
     command_server = Signal(list)
 
-    # params=DAQ_TCP_server.params
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state,
-                         grabber_type='1D')  # initialize base class with commom attributes and methods
+                         grabber_type='0D')  # initialize base class with commom attributes and methods
 
         self.x_axis = None
         self.y_axis = None
         self.data = None
 
-    def data_ready(self, data):
+    def data_ready(self, data: list):
         """
             Send the grabed data signal.
         """
-        self.data_grabed_signal.emit([DataFromPlugins(name='TCP Server', data=data, dim='Data1D')])
+
+        self.dte_signal.emit(DataToExport('TCP0D', data=[DataFromPlugins(name='TCPServer', data=data, dim='Data0D')]))
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qtpy.QtCore import QThread, Slot, QRectF
 from qtpy import QtWidgets
 import numpy as np
 import pymodaq.utils.math_utils as mutils
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main, comon_parameters
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.data import DataFromPlugins, Axis, DataToExport
 from pymodaq.utils.array_manipulation import crop_array_to_axis
 
 
 class DAQ_2DViewer_Mock(DAQ_Viewer_base):
     """Virtual instrument generating 2D data"""
 
     params = comon_parameters + [
@@ -122,16 +122,15 @@
     def ini_detector(self, controller=None):
         self.ini_detector_init(controller, "Mock controller")
 
         self.x_axis = self.get_xaxis()
         self.y_axis = self.get_yaxis()
 
         # initialize viewers with the future type of data but with 0value data
-        self.data_grabed_signal_temp.emit(self.average_data(1, True))
-        # OrderedDict(name='Mock3', data=[np.zeros((128,))], type='Data1D')])
+        self.dte_signal_temp.emit(self.average_data(1, True))
 
         initialized = True
         info = 'Init'
         return info, initialized
 
     def close(self):
         """
@@ -169,20 +168,19 @@
                 self.live = True
                 self.live = False  # don't want to use that for the moment
 
         if self.live:
             while self.live:
                 data = self.average_data(Naverage)
                 QThread.msleep(100)
-                self.data_grabed_signal.emit(data)
+                self.dte_signal.emit(data)
                 QtWidgets.QApplication.processEvents()
         else:
             data = self.average_data(Naverage)
-            QThread.msleep(000)
-            self.data_grabed_signal.emit(data)
+            self.dte_signal.emit(data)
 
     def average_data(self, Naverage, init=False):
         data = []  # list of image (at most 3 for red, green and blue channels)
         data_tmp = np.zeros_like(self.image)
         for ind in range(Naverage):
             data_tmp += self.set_Mock_data()
         data_tmp = data_tmp / Naverage
@@ -190,16 +188,15 @@
         data_tmp = data_tmp * (data_tmp >= self.settings['threshold']) * (init is False)
         for ind in range(self.settings['Nimagespannel']):
             datatmptmp = []
             for indbis in range(self.settings['Nimagescolor']):
                 datatmptmp.append(data_tmp)
             data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D',
                                         axes=[self.y_axis, self.x_axis]))
-        # data.append(OrderedDict(name='Mock2D_1D',data=[np.mean(data_tmp,axis=0)], type='Data1D'))
-        return data
+        return DataToExport('Mock2D', data=data)
 
     def stop(self):
         """
             not implemented.
         """
         self.live = False
         return ""
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qtpy.QtCore import QThread, Slot, QRectF
 from qtpy import QtWidgets
 import numpy as np
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main, comon_parameters
 
 from pymodaq.utils.daq_utils import ThreadCommand
-from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.data import DataFromPlugins, Axis, DataToExport
 from pymodaq.utils.parameter import Parameter
 from pymodaq.utils.parameter.utils import iter_children
 
 
 from pymodaq_plugins_mock.hardware.camera_wrapper import Camera
 
 
@@ -84,15 +84,15 @@
 
         #apply presets to wrapper
         for settings in self.settings.child('cam_settings').children():
             if hasattr(self.controller, settings.name()):
                 setattr(self.controller, settings.name(), settings.value())
 
         # initialize viewers with the future type of data but with 0value data
-        self.data_grabed_signal_temp.emit(self.average_data(1, True),)
+        self.dte_signal_temp.emit(self.average_data(1, True),)
 
         initialized = True
         info = 'Controller ok'
         return info, initialized
 
     def close(self):
         pass
@@ -143,15 +143,15 @@
                 self.live = True
                 # self.live = False  # don't want to use that for the moment
 
         if self.live:
             while self.live:
                 data = self.average_data(Naverage)
                 QThread.msleep(kwargs.get('wait_time', 100))
-                self.data_grabed_signal.emit(data)
+                self.dte_signal.emit(data)
                 QtWidgets.QApplication.processEvents()
         else:
             data = self.average_data(Naverage)
             QThread.msleep(000)
             self.data_grabed_signal.emit(data)
 
     def average_data(self, Naverage, init=False):
@@ -169,15 +169,15 @@
             if self._update_axes:
                 data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D',
                                             axes=[self.x_axis, self.y_axis]))
             else:
                 data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D'))
         if self._update_axes:
             self._update_axes = False
-        return data
+        return DataToExport('MockCamera', data=data)
 
     def stop(self):
         """
             not implemented.
         """
         self.live = False
         return ""
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from qtpy.QtCore import Signal, Slot
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_TCP_server
-from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.data import DataFromPlugins, Axis, DataToExport
 
 
 class DAQ_2DViewer_TCPServer(DAQ_Viewer_TCP_server):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
@@ -33,8 +33,9 @@
         self.data = None
 
     @Slot(list)
     def data_ready(self, data):
         """
             Send the grabed data signal.
         """
-        self.data_grabed_signal.emit([DataFromPlugins(name='TCP Server 2D', data=data, type='Data2D')])
+        self.dte_signal.emit(DataToExport('TCP2D',
+                                          data=[DataFromPlugins(name='TCP Server 2D', data=data, type='Data2D')]))
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from qtpy.QtCore import QThread
 from qtpy import QtWidgets
 import numpy as np
 import pymodaq.utils.daq_utils as utils
-from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.utils.data import Axis, DataFromPlugins, NavAxis
+from pymodaq.utils.data import Axis, DataFromPlugins, NavAxis, DataToExport
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 
 
 class DAQ_NDViewer_Mock(DAQ_Viewer_base):
     """
         =============== ==================
         **Attributes**   **Type**
@@ -32,22 +32,22 @@
             {'title': 'Ny', 'name': 'Ny', 'type': 'int', 'value': 200, 'default': 200, 'min': 1},
             {'title': 'amp', 'name': 'amp', 'type': 'int', 'value': 20, 'default': 20, 'min': 1},
             {'title': 'x0', 'name': 'x0', 'type': 'slide', 'value': 50, 'default': 50, 'min': 0},
             {'title': 'y0', 'name': 'y0', 'type': 'float', 'value': 100, 'default': 100, 'min': 0},
             {'title': 'dx', 'name': 'dx', 'type': 'float', 'value': 20, 'default': 20, 'min': 1},
             {'title': 'dy', 'name': 'dy', 'type': 'float', 'value': 40, 'default': 40, 'min': 1},
             {'title': 'lambda', 'name': 'lambda', 'type': 'float', 'value': 8, 'default': 1, 'min': 0.1},
-            {'title': 'n', 'name': 'n', 'type': 'float', 'value': 1, 'default': 1, 'min': 1},
+            {'title': 'n', 'name': 'n', 'type': 'int', 'value': 1, 'default': 1, 'min': 1},
         ]},
         {'title': 'Temporal properties:', 'name': 'temp_settings', 'type': 'group', 'children': [
             {'title': 'Nt', 'name': 'Nt', 'type': 'int', 'value': 150, 'default': 100, 'min': 1},
             {'title': 'amp', 'name': 'amp', 'type': 'int', 'value': 20, 'default': 20, 'min': 1},
             {'title': 't0', 'name': 't0', 'type': 'slide', 'value': 50, 'default': 50, 'min': 0},
             {'title': 'dt', 'name': 'dt', 'type': 'float', 'value': 20, 'default': 20, 'min': 1},
-            {'title': 'n', 'name': 'n', 'type': 'float', 'value': 1, 'default': 1, 'min': 1},
+            {'title': 'n', 'name': 'n', 'type': 'int', 'value': 1, 'default': 1, 'min': 1},
         ]},
 
         {'title': 'Cam. Prop.:', 'name': 'cam_settings', 'type': 'group', 'children': []},
     ]
 
     def __init__(self, parent=None,
                  params_state=None):  # init_params is a list of tuple where each tuple contains info on a 1D channel (Ntps,amplitude, width, position and noise)
@@ -144,41 +144,31 @@
             Initialisation procedure of the detector initializing the status dictionnary.
 
             See Also
             --------
             daq_utils.ThreadCommand, get_xaxis, get_yaxis
         """
         self.status.update(edict(initialized=False, info="", x_axis=None, y_axis=None, controller=None))
-        try:
-
-            if self.settings.child(('controller_status')).value() == "Slave":
-                if controller is None:
-                    raise Exception('no controller has been defined externally while this detector is a slave one')
-                else:
-                    self.controller = controller
+        if self.settings.child(('controller_status')).value() == "Slave":
+            if controller is None:
+                raise Exception('no controller has been defined externally while this detector is a slave one')
             else:
-                self.controller = "Mock controller"
+                self.controller = controller
+        else:
+            self.controller = "Mock controller"
+
+        self.set_Mock_data()
+        # # initialize viewers with the future type of data
+        # self.dte_signal_temp.emit(DataToExport('MockND',
+        #                                        data=[DataFromPlugins(name='MockND', data=[np.zeros((128, 30, 10))],
+        #                                                              dim='DataND',
+        #                                                              nav_indexes=(0, 1))]))
 
-            self.set_Mock_data()
-            # initialize viewers with the future type of data
-            self.data_grabed_signal_temp.emit(
-                [DataFromPlugins(name='MockND', data=[np.zeros((128, 30, 10))], dim='DataND',
-                                 nav_axes=(0, 1)), ])
-
-            self.status.x_axis = self.x_axis
-            self.status.y_axis = self.y_axis
-            self.status.initialized = True
-            self.status.controller = self.controller
-            return self.status
-
-        except Exception as e:
-            self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
-            self.status.info = getLineInfo() + str(e)
-            self.status.initialized = False
-            return self.status
+        initialized = True
+        return 'ok', initialized
 
     def close(self):
         """
             not implemented.
         """
         pass
 
@@ -204,32 +194,38 @@
                 self.live = True
                 self.live = False  # don't want to use that for the moment
 
         if self.live:
             while self.live:
                 data = self.average_data(Naverage)
                 QThread.msleep(100)
-                self.data_grabed_signal.emit(data)
+                self.dte_signal.emit(data)
                 QtWidgets.QApplication.processEvents()
         else:
             data = self.average_data(Naverage)
             QThread.msleep(000)
-            self.data_grabed_signal.emit(data)
+            self.dte_signal.emit(data)
 
     def average_data(self, Naverage):
         data_tmp = np.zeros_like(self.image)
         for ind in range(Naverage):
             data_tmp += self.set_Mock_data()
         data_tmp = data_tmp / Naverage
 
-        data = [DataFromPlugins(name='MockND_{:d}'.format(ind), data=[data_tmp], dim='DataND', nav_axes=(1, 0),
-                                nav_x_axis=NavAxis(data=self.x_axis, label='X space', nav_index=1),
-                                nav_y_axis=NavAxis(data=self.y_axis, label='Y space', nav_index=0),
-                                x_axis=Axis(data=self.time_axis, label='time label'))]
+        data = DataToExport('MockND',
+                            data=[DataFromPlugins(name='MockND_{:d}'.format(ind), data=[data_tmp], dim='DataND',
+                                                  nav_indexes=(0, 1),
+                                                  axes=[Axis(data=self.x_axis, label='X space', index=1),
+                                                        Axis(data=self.y_axis, label='Y space', index=0),
+                                                        Axis(data=self.time_axis, label='time label', index=2)])])
         return data
 
     def stop(self):
         """
             not implemented.
         """
         self.live = False
         return ""
+
+
+if __name__ == '__main__':
+    main(__file__, init=True)
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/hardware/camera_wrapper.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/hardware/camera_wrapper.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/PKG-INFO` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-mock
-Version: 4.0.2
+Version: 4.1.0
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymodaq_plugins_mock-4.0.2/src/pymodaq_plugins_mock.egg-info/SOURCES.txt` & `pymodaq_plugins_mock-4.1.0/src/pymodaq_plugins_mock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 src/pymodaq_plugins_mock.egg-info/entry_points.txt
 src/pymodaq_plugins_mock.egg-info/requires.txt
 src/pymodaq_plugins_mock.egg-info/top_level.txt
 src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
 src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
 src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
 src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
+src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTauMulti.py
 src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
 src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
 src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
 src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
 src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
 src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
 src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
```


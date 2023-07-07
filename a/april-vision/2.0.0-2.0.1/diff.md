# Comparing `tmp/april_vision-2.0.0.tar.gz` & `tmp/april_vision-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "april_vision-2.0.0.tar", last modified: Thu Jun  1 22:06:15 2023, max compression
+gzip compressed data, was "april_vision-2.0.1.tar", last modified: Fri Jul  7 20:50:09 2023, max compression
```

## Comparing `april_vision-2.0.0.tar` & `april_vision-2.0.1.tar`

### file list

```diff
@@ -1,67 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-01 22:05:46.000000 april_vision-2.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 22:05:46.000000 april_vision-2.0.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-01 22:05:46.000000 april_vision-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 22:05:46.000000 april_vision-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-01 22:05:46.000000 april_vision-2.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 22:06:15.159263 april_vision-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-01 22:05:46.000000 april_vision-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/april_vision/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/calibrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/FaceTime HD Camera.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech B500.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech C270.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech C905.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Logitech C920.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/Microdia Integrated_Webcam_HD.xml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/calibrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/annotate_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/annotate_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/camera_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/marker_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/marker_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/tools/family_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/tools/list_cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/cli/vision_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/detect_cameras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/examples/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/examples/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/frame_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/april_vision/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/helpers/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-01 22:05:46.000000 april_vision-2.0.0/april_vision/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/april_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 22:06:15.000000 april_vision-2.0.0/april_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-01 22:05:46.000000 april_vision-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-01 22:06:15.159263 april_vision-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 22:05:46.000000 april_vision-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.155263 april_vision-2.0.0/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/stubs/cv2/
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-01 22:05:46.000000 april_vision-2.0.0/stubs/cv2/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:06:15.159263 april_vision-2.0.0/stubs/pyquaternion/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 22:05:46.000000 april_vision-2.0.0/stubs/pyquaternion/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-01 22:05:46.000000 april_vision-2.0.0/stubs/pyquaternion/quaternion.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.495933 april_vision-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-07 20:49:41.000000 april_vision-2.0.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.475932 april_vision-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.483933 april_vision-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 20:49:41.000000 april_vision-2.0.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-07 20:49:41.000000 april_vision-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 20:49:41.000000 april_vision-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-07 20:49:41.000000 april_vision-2.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-07 20:50:09.495933 april_vision-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-07 20:49:41.000000 april_vision-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.483933 april_vision-2.0.1/april_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.487933 april_vision-2.0.1/april_vision/calibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/calibrations/Logitech B500.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/calibrations/Logitech C270.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/calibrations/Logitech C905.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/calibrations/Logitech C920.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/calibrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.491933 april_vision-2.0.1/april_vision/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/annotate_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/annotate_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/camera_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/marker_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/marker_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.491933 april_vision-2.0.1/april_vision/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/tools/family_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/tools/list_cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/cli/vision_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/detect_cameras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.491933 april_vision-2.0.1/april_vision/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/examples/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/examples/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/frame_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.495933 april_vision-2.0.1/april_vision/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/helpers/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/helpers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/helpers/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-07 20:49:41.000000 april_vision-2.0.1/april_vision/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.487933 april_vision-2.0.1/april_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 20:50:09.000000 april_vision-2.0.1/april_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-07 20:49:41.000000 april_vision-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-07 20:50:09.495933 april_vision-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-07 20:49:41.000000 april_vision-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.479933 april_vision-2.0.1/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.495933 april_vision-2.0.1/stubs/cv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-07 20:49:41.000000 april_vision-2.0.1/stubs/cv2/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:50:09.495933 april_vision-2.0.1/stubs/pyquaternion/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-07 20:49:41.000000 april_vision-2.0.1/stubs/pyquaternion/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-07 20:49:41.000000 april_vision-2.0.1/stubs/pyquaternion/quaternion.pyi
```

### Comparing `april_vision-2.0.0/.github/workflows/check.yml` & `april_vision-2.0.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/.gitignore` & `april_vision-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/LICENSE` & `april_vision-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/PKG-INFO` & `april_vision-2.0.1/april_vision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: april_vision
-Version: 2.0.0
+Name: april-vision
+Version: 2.0.1
 Summary: An AprilTags wrapper with camera discovery and axis conversion.
 Home-page: https://github.com/WillB97/april_vision
 Author: "Will Barber, Joshua Perriman"
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `april_vision-2.0.0/README.md` & `april_vision-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/__init__.py` & `april_vision-2.0.1/april_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/calibrations/FaceTime HD Camera.xml` & `april_vision-2.0.1/april_vision/calibrations/Logitech B500.xml`

 * *Files 23% similar despite different names*

#### Comparing `april_vision-2.0.0/april_vision/calibrations/FaceTime HD Camera.xml` & `april_vision-2.0.1/april_vision/calibrations/Logitech B500.xml`

```diff
@@ -1,34 +1,36 @@
 <?xml version="1.0" encoding="utf-8"?>
 <opencv_storage>
-  <calibrationDate>&quot;Sun Oct 10 16:29:49 2021&quot;</calibrationDate>
-  <framesCount>29</framesCount>
-  <cameraResolution>1280 720</cameraResolution>
+  <calibrationDate>&quot;Wed 23 Nov 2022 21:23:00 GMT&quot;</calibrationDate>
+  <framesCount>15</framesCount>
+  <cameraResolution>1280 1024</cameraResolution>
   <cameraMatrix type_id="opencv-matrix">
     <rows>3</rows>
     <cols>3</cols>
     <dt>d</dt>
-    <data>1.0059832255301474e+03 0. 6.3600363812582748e+02 0.
-    1.0059832255301474e+03 3.9032987567991756e+02 0. 0. 1.</data>
+    <data>1.05711133e+03 0. 6.02433099e+02
+    0. 1.06661029e+03 4.51876692e+02
+    0. 0. 1.</data>
   </cameraMatrix>
   <cameraMatrix_std_dev type_id="opencv-matrix">
     <rows>4</rows>
     <cols>1</cols>
     <dt>d</dt>
-    <data>0. 1.8390897483985235e+01 4.9795155412210459e+00
-    5.5464984166225326e+00</data>
+    <data>0. 1.4841088432691212e+01 4.7206079728271524e+00
+    4.2203301535161479e+00</data>
   </cameraMatrix_std_dev>
   <dist_coeffs type_id="opencv-matrix">
     <rows>1</rows>
     <cols>5</cols>
     <dt>d</dt>
-    <data>6.8703433405016029e-02 0. 0. 0. -2.4193185280867940e-01</data>
+    <data>-0.0930654 0.30046762 -0.00657921 -0.00055965 -0.48481949</data>
   </dist_coeffs>
   <dist_coeffs_std_dev type_id="opencv-matrix">
     <rows>5</rows>
     <cols>1</cols>
     <dt>d</dt>
-    <data>1.2370831283282813e-02 0. 0. 0. 7.8882690649474521e-02</data>
+    <data>4.4573481761620787e-03 4.5353543208646336e-03 9.4635517516124560e-04
+    8.7616716255079267e-04 0.</data>
   </dist_coeffs_std_dev>
-  <avg_reprojection_error>4.8677611488489964e-01</avg_reprojection_error>
-  <vidpid>&quot;FaceTime HD Camera&quot;</vidpid>
+  <avg_reprojection_error>7.7260806740601118e-01</avg_reprojection_error>
+  <vidpid>&quot;046d:0807&quot;</vidpid>
 </opencv_storage>
```

### Comparing `april_vision-2.0.0/april_vision/calibrations/Logitech C270.xml` & `april_vision-2.0.1/april_vision/calibrations/Logitech C270.xml`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/calibrations/Logitech C905.xml` & `april_vision-2.0.1/april_vision/calibrations/Logitech C905.xml`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/calibrations/Logitech C920.xml` & `april_vision-2.0.1/april_vision/calibrations/Logitech C920.xml`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/__init__.py` & `april_vision-2.0.1/april_vision/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/annotate_image.py` & `april_vision-2.0.1/april_vision/cli/annotate_image.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/annotate_video.py` & `april_vision-2.0.1/april_vision/cli/annotate_video.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/calibrate.py` & `april_vision-2.0.1/april_vision/cli/calibrate.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/live.py` & `april_vision-2.0.1/april_vision/cli/live.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/marker_benchmark.py` & `april_vision-2.0.1/april_vision/cli/marker_benchmark.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/marker_generator.py` & `april_vision-2.0.1/april_vision/cli/marker_generator.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/tools/__init__.py` & `april_vision-2.0.1/april_vision/cli/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/tools/family_details.py` & `april_vision-2.0.1/april_vision/cli/tools/family_details.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/tools/list_cameras.py` & `april_vision-2.0.1/april_vision/cli/tools/list_cameras.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/utils.py` & `april_vision-2.0.1/april_vision/cli/utils.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/cli/vision_debug.py` & `april_vision-2.0.1/april_vision/cli/vision_debug.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/detect_cameras.py` & `april_vision-2.0.1/april_vision/detect_cameras.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/examples/camera.py` & `april_vision-2.0.1/april_vision/examples/camera.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/frame_sources.py` & `april_vision-2.0.1/april_vision/frame_sources.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/helpers/markers.py` & `april_vision-2.0.1/april_vision/helpers/markers.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/helpers/sender.py` & `april_vision-2.0.1/april_vision/helpers/sender.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/marker.py` & `april_vision-2.0.1/april_vision/marker.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/utils.py` & `april_vision-2.0.1/april_vision/utils.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision/vision.py` & `april_vision-2.0.1/april_vision/vision.py`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/april_vision.egg-info/PKG-INFO` & `april_vision-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: april-vision
-Version: 2.0.0
+Name: april_vision
+Version: 2.0.1
 Summary: An AprilTags wrapper with camera discovery and axis conversion.
 Home-page: https://github.com/WillB97/april_vision
 Author: "Will Barber, Joshua Perriman"
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `april_vision-2.0.0/april_vision.egg-info/SOURCES.txt` & `april_vision-2.0.1/april_vision.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 april_vision/vision.py
 april_vision.egg-info/PKG-INFO
 april_vision.egg-info/SOURCES.txt
 april_vision.egg-info/dependency_links.txt
 april_vision.egg-info/entry_points.txt
 april_vision.egg-info/requires.txt
 april_vision.egg-info/top_level.txt
-april_vision/calibrations/FaceTime HD Camera.xml
 april_vision/calibrations/Logitech B500.xml
 april_vision/calibrations/Logitech C270.xml
 april_vision/calibrations/Logitech C905.xml
 april_vision/calibrations/Logitech C920.xml
-april_vision/calibrations/Microdia Integrated_Webcam_HD.xml
 april_vision/calibrations/__init__.py
 april_vision/cli/__init__.py
 april_vision/cli/annotate_image.py
 april_vision/cli/annotate_video.py
 april_vision/cli/calibrate.py
 april_vision/cli/camera_benchmark.py
 april_vision/cli/live.py
```

### Comparing `april_vision-2.0.0/pyproject.toml` & `april_vision-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/setup.cfg` & `april_vision-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/stubs/cv2/__init__.pyi` & `april_vision-2.0.1/stubs/cv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `april_vision-2.0.0/stubs/pyquaternion/quaternion.pyi` & `april_vision-2.0.1/stubs/pyquaternion/quaternion.pyi`

 * *Files identical despite different names*


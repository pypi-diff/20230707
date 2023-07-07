# Comparing `tmp/track_generator-0.5.0.tar.gz` & `tmp/track_generator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track_generator-0.5.0.tar", last modified: Fri Jul  7 07:56:11 2023, max compression
+gzip compressed data, was "track_generator-0.5.1.tar", last modified: Fri Jul  7 09:00:08 2023, max compression
```

## Comparing `track_generator-0.5.0.tar` & `track_generator-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 07:55:57.000000 track_generator-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 07:56:11.183455 track_generator-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 07:55:57.000000 track_generator-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 07:56:11.183455 track_generator-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-07 07:55:57.000000 track_generator-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.179455 track_generator-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 07:55:57.000000 track_generator-0.5.0/tests/test_track_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/coordinate_system.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.179455 track_generator-0.5.0/track_generator/gazebo_model_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/model.config.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/model.sdf.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/setup.bash.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/track.material.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     4464 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/generator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3763 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/ground_truth_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/gui/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gui/track_live_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14575 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/painter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/segment_templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/segment_templates/crosswalk.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/segment_templates/intersection.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2336 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/starter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26049 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/track.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9571 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/xml_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.179455 track_generator-0.5.0/track_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-07-07 07:55:57.000000 track_generator-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-07 08:59:58.000000 track_generator-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 09:00:08.035945 track_generator-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 08:59:58.000000 track_generator-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 09:00:08.035945 track_generator-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-07 08:59:58.000000 track_generator-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.031945 track_generator-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 08:59:58.000000 track_generator-0.5.1/tests/test_track_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/coordinate_system.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/gazebo_model_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/model.config.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/model.sdf.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/setup.bash.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gazebo_model_templates/track.material.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4464 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3763 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/ground_truth_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/gui/qml/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gui/qml/track_live_view.qml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/gui/track_live_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14575 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/painter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator/segment_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/segment_templates/crosswalk.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/segment_templates/intersection.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2365 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/starter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26049 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9571 2023-07-07 08:59:58.000000 track_generator-0.5.1/track_generator/xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:00:08.035945 track_generator-0.5.1/track_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 09:00:08.000000 track_generator-0.5.1/track_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-07-07 08:59:58.000000 track_generator-0.5.1/versioneer.py
```

### Comparing `track_generator-0.5.0/PKG-INFO` & `track_generator-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track_generator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Track generator
 Home-page: https://github.com/twyleg/track_generator
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: svg model vehicles track
```

### Comparing `track_generator-0.5.0/README.md` & `track_generator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/setup.py` & `track_generator-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/coordinate_system.py` & `track_generator-0.5.1/track_generator/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/gazebo_model_generator.py` & `track_generator-0.5.1/track_generator/gazebo_model_generator.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/gazebo_model_templates/model.sdf.template` & `track_generator-0.5.1/track_generator/gazebo_model_templates/model.sdf.template`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/generator.py` & `track_generator-0.5.1/track_generator/generator.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/ground_truth_generator.py` & `track_generator-0.5.1/track_generator/ground_truth_generator.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/gui/track_live_view.py` & `track_generator-0.5.1/track_generator/gui/track_live_view.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/painter.py` & `track_generator-0.5.1/track_generator/painter.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/segment_templates/crosswalk.svg` & `track_generator-0.5.1/track_generator/segment_templates/crosswalk.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/segment_templates/intersection.svg` & `track_generator-0.5.1/track_generator/segment_templates/intersection.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/starter.py` & `track_generator-0.5.1/track_generator/starter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (C) 2022 twyleg
-import os
 import argparse
 import sys
+from pathlib import Path
 
 from track_generator import __version__
 from track_generator import generator
 
 
 def subcommand_generate_track():
     parser = argparse.ArgumentParser(description="Generates a track")
     parser.add_argument(
         "track_files", metavar="track_file", type=str, nargs="+", help="a track file (XML) to generate the track from"
     )
     parser.add_argument(
         "-o",
         "--output",
         dest="output",
-        default=os.path.join(os.getcwd(), "output"),
+        default=Path.cwd() / "output",
         help='Output directory for generated tracks. Default="./"',
     )
     parser.add_argument("--png", action="store_true", help="Generate output PNG (SVG only by default).")
     parser.add_argument("--gazebo", action="store_true", help="Generate Gazebo model for track.")
     parser.add_argument("--ground_truth", action="store_true", help="Generate ground truth data for track.")
     args = parser.parse_args(sys.argv[2:])
 
@@ -32,20 +32,21 @@
     parser.add_argument(
         "track_file", metavar="track_file", type=str, help="a track file (XML) to generate the track from"
     )
     parser.add_argument(
         "-o",
         "--output",
         dest="output",
-        default=os.path.join(os.getcwd(), "output"),
+        default=Path.cwd() / "output",
         help='Output directory for generated tracks. Default="./"',
     )
     args = parser.parse_args(sys.argv[2:])
 
-    generator.generate_track_live(args.track_file, args.output)
+    track_filepath = Path(args.track_file)
+    generator.generate_track_live(track_filepath, args.output)
 
 
 def subcommand_generate_trajectory():
     """TODO: Implement"""
     pass
```

### Comparing `track_generator-0.5.0/track_generator/track.py` & `track_generator-0.5.1/track_generator/track.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator/xml_reader.py` & `track_generator-0.5.1/track_generator/xml_reader.py`

 * *Files identical despite different names*

### Comparing `track_generator-0.5.0/track_generator.egg-info/PKG-INFO` & `track_generator-0.5.1/track_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track-generator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Track generator
 Home-page: https://github.com/twyleg/track_generator
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: svg model vehicles track
```

### Comparing `track_generator-0.5.0/track_generator.egg-info/SOURCES.txt` & `track_generator-0.5.1/track_generator.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 track_generator.egg-info/top_level.txt
 track_generator/gazebo_model_templates/model.config.template
 track_generator/gazebo_model_templates/model.sdf.template
 track_generator/gazebo_model_templates/setup.bash.template
 track_generator/gazebo_model_templates/track.material.template
 track_generator/gui/__init__.py
 track_generator/gui/track_live_view.py
+track_generator/gui/qml/track_live_view.qml
 track_generator/segment_templates/crosswalk.svg
 track_generator/segment_templates/intersection.svg
```

### Comparing `track_generator-0.5.0/versioneer.py` & `track_generator-0.5.1/versioneer.py`

 * *Files identical despite different names*


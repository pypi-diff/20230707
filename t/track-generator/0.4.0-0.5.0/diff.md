# Comparing `tmp/track_generator-0.4.0.tar.gz` & `tmp/track_generator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track_generator-0.4.0.tar", last modified: Tue Mar 21 05:54:55 2023, max compression
+gzip compressed data, was "track_generator-0.5.0.tar", last modified: Fri Jul  7 07:56:11 2023, max compression
```

## Comparing `track_generator-0.4.0.tar` & `track_generator-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:54:55.649834 track_generator-0.4.0/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      125 2023-03-07 21:07:52.000000 track_generator-0.4.0/MANIFEST.in
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)     1986 2023-03-21 05:54:55.649834 track_generator-0.4.0/PKG-INFO
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)     1722 2023-03-07 21:07:52.000000 track_generator-0.4.0/README.md
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)        6 2023-03-21 05:54:54.000000 track_generator-0.4.0/VERSION.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       38 2023-03-21 05:54:55.649834 track_generator-0.4.0/setup.cfg
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      826 2023-03-21 05:50:33.000000 track_generator-0.4.0/setup.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:54:55.649834 track_generator-0.4.0/track_generator/
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/__init__.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)       60 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/__main__.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     1484 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/coordinate_system.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     2982 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gazebo_model_generator.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:54:55.649834 track_generator-0.4.0/track_generator/gazebo_model_templates/
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)      148 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gazebo_model_templates/model.config.template
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)      999 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gazebo_model_templates/model.sdf.template
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)      150 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gazebo_model_templates/setup.bash.template
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)      336 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gazebo_model_templates/track.material.template
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     4361 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/generator.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     3460 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/ground_truth_generator.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:54:55.649834 track_generator-0.4.0/track_generator/gui/
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gui/__init__.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     1285 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/gui/track_live_view.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)    12971 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/painter.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:54:55.649834 track_generator-0.4.0/track_generator/segment_templates/
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     5670 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/segment_templates/crosswalk.svg
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     7488 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/segment_templates/intersection.svg
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     2361 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/starter.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)    23866 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/track.py
--rwxrwxr-x   0 twyleg   (30000) twyleg   (30003)     9536 2023-03-21 05:50:33.000000 track_generator-0.4.0/track_generator/xml_reader.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-03-21 05:54:55.649834 track_generator-0.4.0/track_generator.egg-info/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)     1986 2023-03-21 05:54:55.000000 track_generator-0.4.0/track_generator.egg-info/PKG-INFO
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)     1004 2023-03-21 05:54:55.000000 track_generator-0.4.0/track_generator.egg-info/SOURCES.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)        1 2023-03-21 05:54:55.000000 track_generator-0.4.0/track_generator.egg-info/dependency_links.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       67 2023-03-21 05:54:55.000000 track_generator-0.4.0/track_generator.egg-info/entry_points.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       50 2023-03-21 05:54:55.000000 track_generator-0.4.0/track_generator.egg-info/requires.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       16 2023-03-21 05:54:55.000000 track_generator-0.4.0/track_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 07:55:57.000000 track_generator-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 07:56:11.183455 track_generator-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 07:55:57.000000 track_generator-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 07:56:11.183455 track_generator-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-07 07:55:57.000000 track_generator-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.179455 track_generator-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-07 07:55:57.000000 track_generator-0.5.0/tests/test_track_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/coordinate_system.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.179455 track_generator-0.5.0/track_generator/gazebo_model_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/model.config.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/model.sdf.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/setup.bash.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gazebo_model_templates/track.material.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4464 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3763 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/ground_truth_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1284 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/gui/track_live_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14575 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/painter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.183455 track_generator-0.5.0/track_generator/segment_templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5670 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/segment_templates/crosswalk.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7488 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/segment_templates/intersection.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2336 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/starter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26049 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/track.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9571 2023-07-07 07:55:57.000000 track_generator-0.5.0/track_generator/xml_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 07:56:11.179455 track_generator-0.5.0/track_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 07:56:11.000000 track_generator-0.5.0/track_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-07-07 07:55:57.000000 track_generator-0.5.0/versioneer.py
```

### Comparing `track_generator-0.4.0/PKG-INFO` & `track_generator-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: track_generator
-Version: 0.4.0
+Version: 0.5.0
 Summary: Track generator
 Home-page: https://github.com/twyleg/track_generator
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: svg model vehicles track
-Platform: UNKNOWN
 
 # Track Generator
 
 Simple generator to create tracks (ground textures for vehicle simulations)
 from parametric descriptions.
 
 For example, the following parametric description of a track in XML will lead
@@ -79,8 +78,7 @@
 left hand side cartesian coordinate system. This is important for internal operations but shouldn't bother the user.
 
 ![coordiante systems](doc/img/svg/coordinate_systems.svg)
 
 ## Examples
 
 Example track definitions can be found under [examples/](examples/)
-
```

### Comparing `track_generator-0.4.0/README.md` & `track_generator-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `track_generator-0.4.0/setup.py` & `track_generator-0.5.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # Copyright (C) 2022 twyleg
 import os
+import versioneer
 from setuptools import find_packages, setup
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="track_generator",
-    version=read('VERSION.txt'),
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     author="Torsten Wylegala",
     author_email="mail@twyleg.de",
     description=("Track generator"),
     license="GPL 3.0",
     keywords="svg model vehicles track",
     url="https://github.com/twyleg/track_generator",
     packages=find_packages(),
     include_package_data=True,
-    long_description=read('README.md'),
-    install_requires=[
-        'pytransform3d',
-        'numpy',
-        'drawsvg==1.9',
-        'watchdog',
-        'PySide6'
-    ],
+    long_description=read("README.md"),
+    install_requires=["pytransform3d", "numpy", "drawsvg==1.9", "watchdog~=3.0.0", "pyside6~=6.5.1"],
     entry_points={
-        'console_scripts': [
-            'track_generator = track_generator.starter:start',
+        "console_scripts": [
+            "track_generator = track_generator.starter:start",
         ]
-    }
+    },
 )
```

### Comparing `track_generator-0.4.0/track_generator/coordinate_system.py` & `track_generator-0.5.0/track_generator/coordinate_system.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,42 +4,41 @@
 import pytransform3d.transformations as pytr
 from typing import Optional, List
 
 
 class WorldCoordinateSystem:
     def __init__(self):
         self.local_to_world = pytr.transform_from(
-            pyrot.matrix_from_axis_angle(np.array([0.0, 0.0, 1.0, 0.0])),
-            np.array([0.0, 0.0, 0.0])
+            pyrot.matrix_from_axis_angle(np.array([0.0, 0.0, 1.0, 0.0])), np.array([0.0, 0.0, 0.0])
         )
 
 
 class CartesianSystem2d:
-
-    def __init__(self, x: float, y: float, yaw: float, parent: Optional['CartesianSystem'] = WorldCoordinateSystem()):
-
+    def __init__(self, x: float, y: float, yaw: float, parent: Optional["CartesianSystem"] = WorldCoordinateSystem()):
         p = np.array([x, y, 0.0])
         a = np.array([0.0, 0.0, 1.0, np.deg2rad(yaw)])
         local_to_parent = pytr.transform_from(pyrot.matrix_from_axis_angle(a), p)
         parent_to_world = parent.local_to_world
         self.local_to_world = pytr.concat(local_to_parent, parent_to_world)
 
 
 class Point2d:
     def __init__(self, x_l: float, y_l: float, local_coordinate_system: CartesianSystem2d):
         self.local_coordinate_system = local_coordinate_system
         self.x_l = x_l
         self.y_l = y_l
 
-        point_world = pytr.transform(self.local_coordinate_system.local_to_world, np.array([self.x_l, self.y_l, 0.0, 1.0]))
+        point_world = pytr.transform(
+            self.local_coordinate_system.local_to_world, np.array([self.x_l, self.y_l, 0.0, 1.0])
+        )
         self.x_w = point_world[0]
         self.y_w = point_world[1]
 
     def __str__(self):
-        return f'Local: ({self.x_l},{self.y_l}), World: ({self.x_w},{self.y_w})'
+        return f"Local: ({self.x_l},{self.y_l}), World: ({self.x_w},{self.y_w})"
 
 
 Polygon = List[Point2d]
 
 # class Polygon(List[Point2d]):
 #     def __init__(self, *args):
-#         super().__init__(self, *args)
+#         super().__init__(self, *args)
```

### Comparing `track_generator-0.4.0/track_generator/gazebo_model_generator.py` & `track_generator-0.5.0/track_generator/gazebo_model_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,68 +6,61 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 def write(path, data):
-    return open(path, 'w').write(data)
+    return open(path, "w").write(data)
 
 
 class GazeboModelGenerator:
-
     def __init__(self, track_name: str, output_directory: str):
         self.track_name = track_name
         self.output_directory = output_directory
         self.gazebo_models_directory: Optional[str] = None
         self.track_directory: Optional[str] = None
         self.track_materials_scripts_directory: Optional[str] = None
         self.track_materials_textures_directory: Optional[str] = None
 
     def create_directory_structure(self, track_name: str):
-        self.gazebo_models_directory = os.path.join(self.output_directory, 'gazebo_models')
+        self.gazebo_models_directory = os.path.join(self.output_directory, "gazebo_models")
         self.track_directory = os.path.join(self.gazebo_models_directory, track_name)
-        self.track_materials_scripts_directory = os.path.join(self.track_directory, 'materials', 'scripts')
-        self.track_materials_textures_directory = os.path.join(self.track_directory, 'materials', 'textures')
+        self.track_materials_scripts_directory = os.path.join(self.track_directory, "materials", "scripts")
+        self.track_materials_textures_directory = os.path.join(self.track_directory, "materials", "textures")
 
         os.makedirs(self.gazebo_models_directory, exist_ok=True)
         os.makedirs(self.track_directory, exist_ok=True)
         os.makedirs(self.track_materials_scripts_directory, exist_ok=True)
         os.makedirs(self.track_materials_textures_directory, exist_ok=True)
 
     def generate_track_material(self):
-        template = Template(read('gazebo_model_templates/track.material.template'))
+        template = Template(read("gazebo_model_templates/track.material.template"))
         output = template.substitute(
-            material_name=f'{self.track_name}_material',
-            texture_file_name=f'{self.track_name}.png'
+            material_name=f"{self.track_name}_material", texture_file_name=f"{self.track_name}.png"
         )
-        write(os.path.join(self.track_materials_scripts_directory, 'track.material'), output)
+        write(os.path.join(self.track_materials_scripts_directory, "track.material"), output)
 
     def generate_track_sdf(self, track: Track):
-        template = Template(read('gazebo_model_templates/model.sdf.template'))
-        output = template.substitute(
-            name=self.track_name,
-            width=track.width,
-            height=track.height
-        )
-        write(os.path.join(self.track_directory, 'model.sdf'), output)
+        template = Template(read("gazebo_model_templates/model.sdf.template"))
+        output = template.substitute(name=self.track_name, width=track.width, height=track.height)
+        write(os.path.join(self.track_directory, "model.sdf"), output)
 
     def generate_track_config(self, track: Track):
-        template = Template(read('gazebo_model_templates/model.config.template'))
+        template = Template(read("gazebo_model_templates/model.config.template"))
         output = template.substitute(
             name=self.track_name,
             version=track.version,
             desc=self.track_name,
         )
-        write(os.path.join(self.track_directory, 'model.config'), output)
+        write(os.path.join(self.track_directory, "model.config"), output)
 
     def generate_setup_script(self):
-        output = read('gazebo_model_templates/setup.bash.template')
-        write(os.path.join(self.gazebo_models_directory, 'setup.bash'), output)
+        output = read("gazebo_model_templates/setup.bash.template")
+        write(os.path.join(self.gazebo_models_directory, "setup.bash"), output)
 
     def generate_gazebo_model(self, track: Track):
         self.create_directory_structure(self.track_name)
         self.generate_track_material()
         self.generate_track_sdf(track)
         self.generate_track_config(track)
         self.generate_setup_script()
-
```

### Comparing `track_generator-0.4.0/track_generator/gazebo_model_templates/model.sdf.template` & `track_generator-0.5.0/track_generator/gazebo_model_templates/model.sdf.template`

 * *Files identical despite different names*

### Comparing `track_generator-0.4.0/track_generator/generator.py` & `track_generator-0.5.0/track_generator/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 # Copyright (C) 2022 twyleg
 import os
-from typing import List
+from pathlib import Path
+from typing import List, Callable
 
 from track_generator import xml_reader
 from track_generator.painter import Painter
 from track_generator.gazebo_model_generator import GazeboModelGenerator
 from track_generator.gui.track_live_view import TrackLiveView
 from track_generator.ground_truth_generator import GroundTruthGenerator
 
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 
-def _create_output_directory_if_required(output_directory):
-    os.makedirs(output_directory, exist_ok=True)
+def _create_output_directory_if_required(output_dirpath: Path):
+    output_dirpath.mkdir(exist_ok=True)
 
 
-def _get_track_name_from_file_path(file_path: str) -> str:
-    filename = os.path.basename(file_path)
+def _get_track_name_from_file_path(track_filepath: Path) -> str:
+    filename = os.path.basename(track_filepath)
     filename_without_extension, _ = os.path.splitext(filename)
     return filename_without_extension
 
 
-def generate_track(track_files: List[str], root_output_directory: str, generate_png=False,
-                   generate_gazebo_project=False, generate_ground_truth=False) -> List[str]:
+def generate_track(
+    track_filepaths: List[Path],
+    root_output_dirpath: Path,
+    generate_png=False,
+    generate_gazebo_project=False,
+    generate_ground_truth=False,
+) -> List[str]:
     """
     Generate tracks (SVG, Gazebo project, etc) from given track files (XML)
-    :param track_files: List of track files
-    :param root_output_directory: The output directory to write results to. Subdirectories for every track will be
+    :param track_filepaths: List of track files
+    :param root_output_dirpath: The output directory to write results to. Subdirectories for every track will be
     generated.
     :param generate_png: Flag whether a png image should be created for the track
     :param generate_gazebo_project:Flag whether gazebo project files should be created for the track
     :return: List of output directories for the tracks
     """
-    track_output_directories: List[str] = []
-    for track_file in track_files:
-        track = xml_reader.read_track(track_file)
+    track_output_directories: List[Path] = []
+    for track_filepath in track_filepaths:
+        track = xml_reader.read_track(track_filepath)
         track.calc()
 
-        track_name = _get_track_name_from_file_path(track_file)
-        track_output_directory = os.path.join(root_output_directory, track_name)
+        track_name = _get_track_name_from_file_path(track_filepath)
+        track_output_directory = root_output_dirpath / track_name
         _create_output_directory_if_required(track_output_directory)
         track_output_directories.append(track_output_directory)
 
         painter = Painter()
         painter.draw_track(track)
         painter.save_svg(track_name, track_output_directory)
         if generate_png:
@@ -52,50 +58,52 @@
         if generate_gazebo_project:
             gazebo_model_generator = GazeboModelGenerator(track_name, track_output_directory)
             gazebo_model_generator.generate_gazebo_model(track)
 
             painter.save_png(track_name, gazebo_model_generator.track_materials_textures_directory)
 
         painter.draw_track_verbose(track)
-        painter.save_svg(track_name, track_output_directory, file_name_postfix='_verbose')
+        painter.save_svg(track_name, track_output_directory, file_name_postfix="_verbose")
 
         if generate_ground_truth:
             ground_truth_generator = GroundTruthGenerator(track_name, track_output_directory)
             ground_truth_generator.generate_ground_truth(track)
     return track_output_directories
 
 
 class FileChangedHandler(FileSystemEventHandler):
-
-    def __init__(self, input_filepath, callback):
+    def __init__(self, input_filepath: Path, callback: Callable):
         self.input_filepath = input_filepath
         self.callback = callback
 
-    def on_any_event(self, event):
-        if event.is_directory:
-            return None
-        elif event.event_type == 'closed' and event.src_path == self.input_filepath:
+    # def on_any_event(self, event) -> None:
+    #     pass
+
+    def on_closed(self, event) -> None:
+        event_filepath = Path(event.src_path)
+        if event_filepath == self.input_filepath:
             self.callback()
+        return None
 
 
-def generate_track_live(track_file: str, root_output_directory: str) -> str:
+def generate_track_live(track_file: Path, root_output_directory: Path) -> None:
     """
     Generate tracks (SVG, Gazebo project, etc) from given track files (XML)
     :param track_file: Track file
     :param root_output_directory: The output directory to write results to. Subdirectories for every track will be
     generated.
     :return: Output directory for the track
     """
-    track_file_directory = os.path.dirname(track_file)
+    track_file_directory = track_file.parent
     track_name = _get_track_name_from_file_path(track_file)
-    output_file_path = os.path.join(root_output_directory, track_name, f'{track_name}.svg')
+    output_file_path = os.path.join(root_output_directory, track_name, f"{track_name}.svg")
     track_live_view = TrackLiveView(output_file_path)
 
     def update():
-        print(f'Track file changed, regenerating track ({track_file})')
+        print(f"Track file changed, regenerating track ({track_file})")
         generate_track([track_file], root_output_directory, generate_png=False, generate_gazebo_project=False)
         track_live_view.update()
 
     event_handler = FileChangedHandler(track_file, update)
 
     update()
 
@@ -106,8 +114,8 @@
     track_live_view.run()
 
     observer.stop()
     observer.join()
 
 
 def generate_trajectory():
-    print('generate_trajectory not implemented yet')
+    print("generate_trajectory not implemented yet")
```

### Comparing `track_generator-0.4.0/track_generator/ground_truth_generator.py` & `track_generator-0.5.0/track_generator/ground_truth_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 from xml.etree import cElementTree as ET, ElementTree
 from xml.etree import ElementTree
 from xml.dom import minidom
 
-from track_generator.track import Segment, Track, Start, Straight, Arc, Crosswalk, Intersection, Gap, ParkingArea, TrafficIsland, Clothoid
+from track_generator.track import (
+    Segment,
+    Track,
+    Start,
+    Straight,
+    Arc,
+    Crosswalk,
+    Intersection,
+    Gap,
+    ParkingArea,
+    TrafficIsland,
+    Clothoid,
+)
 
-class GroundTruthGenerator:
 
+class GroundTruthGenerator:
     def __init__(self, track_name: str, output_directory: str):
         self.track_name = track_name
         self.output_directory = output_directory
-        self.root = ET.Element('GroundTruth', {'version': '0.0.1'})
-        self.points = ET.SubElement(self.root, 'Points')
+        self.root = ET.Element("GroundTruth", {"version": "0.0.1"})
+        self.points = ET.SubElement(self.root, "Points")
 
     def generate_ground_truth(self, track: Track):
         for segment in track.segments:
             self.generate_segment(segment)
-        with open(self.output_directory + 'ground_truth.xml', 'w') as f:
-            f.write(minidom.parseString(ET.tostring(self.root, 'utf-8')).toprettyxml(indent='\t'))
+        with open(self.output_directory + "ground_truth.xml", "w") as f:
+            f.write(minidom.parseString(ET.tostring(self.root, "utf-8")).toprettyxml(indent="\t"))
 
     def generate_segment(self, segment: Segment):
         if isinstance(segment, Start):
             pass
         elif isinstance(segment, (Straight, ParkingArea, Gap, Crosswalk)):
             self.generate_straight(segment)
         elif isinstance(segment, Arc):
@@ -28,40 +40,58 @@
         elif isinstance(segment, Intersection):
             self.generate_intersection(segment)
         elif isinstance(segment, TrafficIsland):
             self.generate_traffic_island(segment)
         elif isinstance(segment, Clothoid):
             self.generate_clothoid(segment)
         else:
-            raise RuntimeError(f'Error in GroundTruthGenerator: {segment} not found')
-        
+            raise RuntimeError(f"Error in GroundTruthGenerator: {segment} not found")
+
     def generate_straight(self, segment: Straight):
-        for i,_ in enumerate(segment.center_line_polygon):
-            self.write_points([segment.left_line_polygon[i].x_w, segment.left_line_polygon[i].y_w],
-                [segment.right_line_polygon[i].x_w, segment.right_line_polygon[i].y_w])
+        for i, _ in enumerate(segment.center_line_polygon):
+            self.write_points(
+                [segment.left_line_polygon[i].x_w, segment.left_line_polygon[i].y_w],
+                [segment.right_line_polygon[i].x_w, segment.right_line_polygon[i].y_w],
+            )
 
     def generate_arc(self, segment: Arc):
-        self.write_points([segment.start_point_left.x_w, segment.start_point_left.y_w],
-            [segment.start_point_right.x_w, segment.start_point_right.y_w])
-    
+        self.write_points(
+            [segment.start_point_left.x_w, segment.start_point_left.y_w],
+            [segment.start_point_right.x_w, segment.start_point_right.y_w],
+        )
+
     def generate_intersection(self, segment: Intersection):
-        for i,_ in enumerate(segment.corner_line_polygons[0]):
-            self.write_points([segment.corner_line_polygons[0][i].x_w, segment.corner_line_polygons[0][i].y_w],
-                [segment.corner_line_polygons[1][i].x_w, segment.corner_line_polygons[1][i].y_w])
-        for i,_ in enumerate(segment.corner_line_polygons[0]):
-            self.write_points([segment.corner_line_polygons[2][i].x_w, segment.corner_line_polygons[2][i].y_w],
-                [segment.corner_line_polygons[3][i].x_w, segment.corner_line_polygons[3][i].y_w])
+        for i, _ in enumerate(segment.corner_line_polygons[0]):
+            self.write_points(
+                [segment.corner_line_polygons[0][i].x_w, segment.corner_line_polygons[0][i].y_w],
+                [segment.corner_line_polygons[1][i].x_w, segment.corner_line_polygons[1][i].y_w],
+            )
+        for i, _ in enumerate(segment.corner_line_polygons[0]):
+            self.write_points(
+                [segment.corner_line_polygons[2][i].x_w, segment.corner_line_polygons[2][i].y_w],
+                [segment.corner_line_polygons[3][i].x_w, segment.corner_line_polygons[3][i].y_w],
+            )
 
     def generate_traffic_island(self, segment: TrafficIsland):
-        for i,_ in enumerate(segment.line_polygons[2]):
-            self.write_points([segment.line_polygons[2][i].x_w, segment.line_polygons[2][i].y_w],
-                [segment.line_polygons[3][i].x_w, segment.line_polygons[3][i].y_w])
+        for i, _ in enumerate(segment.line_polygons[2]):
+            self.write_points(
+                [segment.line_polygons[2][i].x_w, segment.line_polygons[2][i].y_w],
+                [segment.line_polygons[3][i].x_w, segment.line_polygons[3][i].y_w],
+            )
 
     def generate_clothoid(self, segment: Clothoid):
-        for i,_ in enumerate(segment.lines[0]):
-            self.write_points([segment.lines[1][i].x_w, segment.lines[1][i].y_w],
-                [segment.lines[2][i].x_w, segment.lines[2][i].y_w])
+        for i, _ in enumerate(segment.lines[0]):
+            self.write_points(
+                [segment.lines[1][i].x_w, segment.lines[1][i].y_w], [segment.lines[2][i].x_w, segment.lines[2][i].y_w]
+            )
 
     def write_points(self, point_1: list, point_2: list):
-        ET.SubElement(self.points, 'Point', {
-            'x_1': str(point_1[0]), 'y_1': str(point_1[1]),
-            'x_2': str(point_2[0]), 'y_2': str(point_2[1]),})
+        ET.SubElement(
+            self.points,
+            "Point",
+            {
+                "x_1": str(point_1[0]),
+                "y_1": str(point_1[1]),
+                "x_2": str(point_2[0]),
+                "y_2": str(point_2[1]),
+            },
+        )
```

### Comparing `track_generator-0.4.0/track_generator/gui/track_live_view.py` & `track_generator-0.5.0/track_generator/gui/track_live_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 from PySide6.QtGui import QGuiApplication
 from PySide6.QtQml import QQmlApplicationEngine
 from PySide6.QtCore import QObject, Signal, Property
 
 
 class TrackLiveView:
-
     class Model(QObject):
         def __init__(self, filename: str) -> None:
             QObject.__init__(self)
             self._filename = filename
 
         def get_filename(self) -> str:
             return self._filename
@@ -32,14 +31,14 @@
 
     def __init__(self, output_file_path: str):
         self.app = QGuiApplication(sys.argv)
         self.engine = QQmlApplicationEngine()
         self.model = TrackLiveView.Model(output_file_path)
 
         self.engine.rootContext().setContextProperty("model", self.model)
-        self.engine.load(os.fspath(Path(__file__).resolve().parent / 'qml/track_live_view.qml'))
+        self.engine.load(os.fspath(Path(__file__).resolve().parent / "qml/track_live_view.qml"))
 
     def update(self):
         self.model.reloadImage.emit()
 
     def run(self):
         self.app.exec()
```

### Comparing `track_generator-0.4.0/track_generator/painter.py` & `track_generator-0.5.0/track_generator/painter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,89 @@
 # Copyright (C) 2022 twyleg
 import os
 import math
 import drawSvg as draw
 
 from typing import Optional
-from track_generator.track import Track, Start, Straight, Arc, Crosswalk, Intersection, Gap, ParkingArea, TrafficIsland, Clothoid
+from track_generator.track import (
+    Track,
+    Start,
+    Straight,
+    Arc,
+    Crosswalk,
+    Intersection,
+    Gap,
+    ParkingArea,
+    TrafficIsland,
+    Clothoid,
+)
 from track_generator.coordinate_system import Point2d, Polygon
 
 DEFAULT_LINE_WIDTH = 0.020
 DEFAULT_TRACK_WIDTH = 0.800
 
-DEFAULT_TRACK_COLOR = '#000000'
-DEFAULT_LINE_COLOR = '#ffffff'
+DEFAULT_TRACK_COLOR = "#000000"
+DEFAULT_LINE_COLOR = "#ffffff"
 
-class Painter:
 
+class Painter:
     def __init__(self):
         self.d: Optional[draw.Drawing] = None
 
     def draw_polygon(self, polygon: Polygon, **kwargs) -> None:
         if len(polygon) < 2:
             return
         for i in range(1, len(polygon)):
             p0 = polygon[i - 1]
             p1 = polygon[i]
             self.d.append(draw.Line(p0.x_w, p0.y_w, p1.x_w, p1.y_w, **kwargs))
 
     def draw_point(self, p: Point2d):
-        self.d.append(draw.Circle(p.x_w,
-                                  p.y_w,
-                                  0.010,
-                                  fill='red', stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
+        self.d.append(draw.Circle(p.x_w, p.y_w, 0.010, fill="red", stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
 
-        self.d.append(draw.Text(f'{p.x_w:.3f}\n{p.y_w:.3f}', 0.1, p.x_w + 0.032, p.y_w, fill='red'))
+        self.d.append(draw.Text(f"{p.x_w:.3f}\n{p.y_w:.3f}", 0.1, p.x_w + 0.032, p.y_w, fill="red"))
 
     def draw_arc_center_point(self, p: Point2d, radian_angle, radius):
-        self.d.append(draw.Circle(p.x_w,
-                                  p.y_w,
-                                  0.010,
-                                  fill='red', stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
+        self.d.append(draw.Circle(p.x_w, p.y_w, 0.010, fill="red", stroke_width=0, stroke=DEFAULT_TRACK_COLOR))
 
-        self.d.append(draw.Text(f'{p.x_w:.3f}\n{p.y_w:.3f}\nr={radius:.3f}\na={radian_angle:.1f}°', 0.1, p.x_w + 0.032, p.y_w, fill='red'))
+        self.d.append(
+            draw.Text(
+                f"{p.x_w:.3f}\n{p.y_w:.3f}\nr={radius:.3f}\na={radian_angle:.1f}°",
+                0.1,
+                p.x_w + 0.032,
+                p.y_w,
+                fill="red",
+            )
+        )
 
     def draw_start_verbose(self, segment: Start):
         self.draw_point(segment.start_point)
 
     def draw_straight(self, segment: Straight):
-
-        self.draw_polygon(segment.center_line_polygon, fill=DEFAULT_TRACK_COLOR, stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH)
-        self.draw_polygon(segment.center_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none',
-                            style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0,fill-opacity:0")
+        self.draw_polygon(
+            segment.center_line_polygon,
+            fill=DEFAULT_TRACK_COLOR,
+            stroke=DEFAULT_TRACK_COLOR,
+            stroke_width=DEFAULT_TRACK_WIDTH,
+        )
+        self.draw_polygon(
+            segment.center_line_polygon,
+            stroke=DEFAULT_LINE_COLOR,
+            stroke_width=DEFAULT_LINE_WIDTH,
+            fill="none",
+            style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0,fill-opacity:0",
+        )
         # stroke-miterlimit:4;stroke-dasharray:0.08,0.16;stroke-dashoffset:0;stroke-width:0.02
 
-        self.draw_polygon(segment.left_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
-        self.draw_polygon(segment.right_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+        self.draw_polygon(
+            segment.left_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
+        )
+        self.draw_polygon(
+            segment.right_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
+        )
 
     def draw_straight_verbose(self, segment: Straight):
         self.draw_point(segment.center_line_polygon[0])
         self.draw_point(segment.left_line_polygon[0])
         self.draw_point(segment.right_line_polygon[0])
 
     def draw_arc(self, segment: Arc):
@@ -67,137 +93,247 @@
         if segment.direction_clockwise:
             final_end_angle = end_angle + 90
             final_start_angle = start_angle + 90
         else:
             final_end_angle = end_angle - 90
             final_start_angle = start_angle - 90
 
-        self.d.append(draw.Arc(segment.center_point.x_w, segment.center_point.y_w, math.fabs(segment.radius), final_start_angle, final_end_angle,
-                               cw=segment.direction_clockwise, stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH, fill='none'))
-
-        self.d.append(draw.Arc(segment.center_point.x_w, segment.center_point.y_w, math.fabs(segment.radius) - 0.380, final_start_angle,
-                               final_end_angle, cw=segment.direction_clockwise, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none'))
-
-        self.d.append(draw.Arc(segment.center_point.x_w, segment.center_point.y_w, math.fabs(segment.radius) + 0.380, final_start_angle,
-                               final_end_angle, cw=segment.direction_clockwise, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none'))
-
-        self.d.append(draw.Arc(segment.center_point.x_w, segment.center_point.y_w, math.fabs(segment.radius), final_start_angle, final_end_angle,
-                               cw=segment.direction_clockwise, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none',
-                               style="stroke-miterlimit:4;stroke-dasharray:0.160,0.160;stroke-dashoffset:0"))
+        self.d.append(
+            draw.Arc(
+                segment.center_point.x_w,
+                segment.center_point.y_w,
+                math.fabs(segment.radius),
+                final_start_angle,
+                final_end_angle,
+                cw=segment.direction_clockwise,
+                stroke=DEFAULT_TRACK_COLOR,
+                stroke_width=DEFAULT_TRACK_WIDTH,
+                fill="none",
+            )
+        )
+
+        self.d.append(
+            draw.Arc(
+                segment.center_point.x_w,
+                segment.center_point.y_w,
+                math.fabs(segment.radius) - 0.380,
+                final_start_angle,
+                final_end_angle,
+                cw=segment.direction_clockwise,
+                stroke=DEFAULT_LINE_COLOR,
+                stroke_width=DEFAULT_LINE_WIDTH,
+                fill="none",
+            )
+        )
+
+        self.d.append(
+            draw.Arc(
+                segment.center_point.x_w,
+                segment.center_point.y_w,
+                math.fabs(segment.radius) + 0.380,
+                final_start_angle,
+                final_end_angle,
+                cw=segment.direction_clockwise,
+                stroke=DEFAULT_LINE_COLOR,
+                stroke_width=DEFAULT_LINE_WIDTH,
+                fill="none",
+            )
+        )
+
+        self.d.append(
+            draw.Arc(
+                segment.center_point.x_w,
+                segment.center_point.y_w,
+                math.fabs(segment.radius),
+                final_start_angle,
+                final_end_angle,
+                cw=segment.direction_clockwise,
+                stroke=DEFAULT_LINE_COLOR,
+                stroke_width=DEFAULT_LINE_WIDTH,
+                fill="none",
+                style="stroke-miterlimit:4;stroke-dasharray:0.160,0.160;stroke-dashoffset:0",
+            )
+        )
 
     def draw_arc_verbose(self, segment: Arc):
         end_angle = segment.direction_angle
         start_angle = segment.start_direction_angle
 
         if segment.direction_clockwise:
             final_end_angle = end_angle + 90
             final_start_angle = start_angle + 90
         else:
             final_end_angle = end_angle - 90
             final_start_angle = start_angle - 90
 
-        p = draw.Path(fill='none', stroke='blue', stroke_width=DEFAULT_LINE_WIDTH)
-        p.arc(segment.center_point.x_w, segment.center_point.y_w, math.fabs(segment.radius), final_end_angle, final_start_angle, cw=not segment.direction_clockwise)
-        p.arc(segment.center_point.x_w, segment.center_point.y_w, 0, final_start_angle, final_end_angle, cw=segment.direction_clockwise, includeL=True)
+        p = draw.Path(fill="none", stroke="blue", stroke_width=DEFAULT_LINE_WIDTH)
+        p.arc(
+            segment.center_point.x_w,
+            segment.center_point.y_w,
+            math.fabs(segment.radius),
+            final_end_angle,
+            final_start_angle,
+            cw=not segment.direction_clockwise,
+        )
+        p.arc(
+            segment.center_point.x_w,
+            segment.center_point.y_w,
+            0,
+            final_start_angle,
+            final_end_angle,
+            cw=segment.direction_clockwise,
+            includeL=True,
+        )
         p.Z()
         self.d.append(p)
 
         self.draw_arc_center_point(segment.center_point, segment.radian_angle, segment.radius)
         self.draw_point(segment.start_point_center)
         self.draw_point(segment.start_point_left)
         self.draw_point(segment.start_point_right)
 
     def draw_crosswalk(self, segment: Crosswalk):
-        self.draw_polygon(segment.center_line_polygon, fill='#eeee00', stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH)
-        self.draw_polygon(segment.left_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
-        self.draw_polygon(segment.right_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+        self.draw_polygon(
+            segment.center_line_polygon, fill="#eeee00", stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH
+        )
+        self.draw_polygon(
+            segment.left_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
+        )
+        self.draw_polygon(
+            segment.right_line_polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none"
+        )
 
         for polygon in segment.line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=0.03, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=0.03, fill="none")
 
     def draw_intersection(self, segment: Intersection):
-
         for polygon in segment.base_line_polygons:
-            self.draw_polygon(polygon, fill='#eeee00', stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH)
+            self.draw_polygon(polygon, fill="#eeee00", stroke=DEFAULT_TRACK_COLOR, stroke_width=DEFAULT_TRACK_WIDTH)
 
         for polygon in segment.corner_line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
 
         for polygon in segment.stop_line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH*2, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH * 2, fill="none")
 
         for polygon in segment.center_line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none',
-                            style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0")
+            self.draw_polygon(
+                polygon,
+                stroke=DEFAULT_LINE_COLOR,
+                stroke_width=DEFAULT_LINE_WIDTH,
+                fill="none",
+                style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0",
+            )
 
     def draw_traffic_island(self, segment: TrafficIsland):
-        self.d.append(draw.Lines(
-            segment.background_polygon[0].x_w, segment.background_polygon[0].y_w,
-            segment.background_polygon[1].x_w, segment.background_polygon[1].y_w,
-            segment.background_polygon[2].x_w, segment.background_polygon[2].y_w,
-            segment.background_polygon[3].x_w, segment.background_polygon[3].y_w,
-            segment.background_polygon[4].x_w, segment.background_polygon[4].y_w,
-            segment.background_polygon[5].x_w, segment.background_polygon[5].y_w,
-            segment.background_polygon[6].x_w, segment.background_polygon[6].y_w,
-            segment.background_polygon[7].x_w, segment.background_polygon[7].y_w,
-            close=False,
-            fill=DEFAULT_TRACK_COLOR))
+        self.d.append(
+            draw.Lines(
+                segment.background_polygon[0].x_w,
+                segment.background_polygon[0].y_w,
+                segment.background_polygon[1].x_w,
+                segment.background_polygon[1].y_w,
+                segment.background_polygon[2].x_w,
+                segment.background_polygon[2].y_w,
+                segment.background_polygon[3].x_w,
+                segment.background_polygon[3].y_w,
+                segment.background_polygon[4].x_w,
+                segment.background_polygon[4].y_w,
+                segment.background_polygon[5].x_w,
+                segment.background_polygon[5].y_w,
+                segment.background_polygon[6].x_w,
+                segment.background_polygon[6].y_w,
+                segment.background_polygon[7].x_w,
+                segment.background_polygon[7].y_w,
+                close=False,
+                fill=DEFAULT_TRACK_COLOR,
+            )
+        )
 
         for polygon in segment.line_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
 
         for polygon in segment.crosswalk_lines_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=0.03, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=0.03, fill="none")
 
     def draw_parking_area(self, segment: ParkingArea):
         self.draw_straight(segment)
 
         for polygon in segment.outline_polygon:
             # Background
-            self.d.append(draw.Lines(
-                polygon[0].x_w, polygon[0].y_w,
-                polygon[1].x_w, polygon[1].y_w,
-                polygon[2].x_w, polygon[2].y_w,
-                polygon[3].x_w, polygon[3].y_w,
-                close=False,
-                fill=DEFAULT_TRACK_COLOR))
+            self.d.append(
+                draw.Lines(
+                    polygon[0].x_w,
+                    polygon[0].y_w,
+                    polygon[1].x_w,
+                    polygon[1].y_w,
+                    polygon[2].x_w,
+                    polygon[2].y_w,
+                    polygon[3].x_w,
+                    polygon[3].y_w,
+                    close=False,
+                    fill=DEFAULT_TRACK_COLOR,
+                )
+            )
             # Outline
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
 
         for polygon in segment.spot_seperator_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
 
         for polygon in segment.blocker_polygons:
-            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill='none')
+            self.draw_polygon(polygon, stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH, fill="none")
 
     def draw_clothoid(self, segment: Clothoid):
         background: tuple(float) = ()
         for p in segment.background_polygon:
             background += (p.x_w, p.y_w)
-        self.d.append(draw.Lines(background[0], background[1], *background, fill=DEFAULT_TRACK_COLOR, stroke=DEFAULT_TRACK_COLOR, stroke_width=2*DEFAULT_LINE_WIDTH))
+        self.d.append(
+            draw.Lines(
+                background[0],
+                background[1],
+                *background,
+                fill=DEFAULT_TRACK_COLOR,
+                stroke=DEFAULT_TRACK_COLOR,
+                stroke_width=2 * DEFAULT_LINE_WIDTH,
+            )
+        )
         middle_line: tuple(float) = ()
         for p in segment.lines[0]:
             middle_line += (p.x_w, p.y_w)
-        self.d.append(draw.Lines(*middle_line, fill='none', stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH
-                        ,style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0"))
+        self.d.append(
+            draw.Lines(
+                *middle_line,
+                fill="none",
+                stroke=DEFAULT_LINE_COLOR,
+                stroke_width=DEFAULT_LINE_WIDTH,
+                style="stroke-miterlimit:4;stroke-dasharray:0.16,0.16;stroke-dashoffset:0",
+            )
+        )
         left_line: tuple(float) = ()
         for p in segment.lines[1]:
             left_line += (p.x_w, p.y_w)
-        self.d.append(draw.Lines(*left_line, fill='none', stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH))
+        self.d.append(draw.Lines(*left_line, fill="none", stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH))
         right_line: tuple(float) = ()
         for p in segment.lines[2]:
             right_line += (p.x_w, p.y_w)
-        self.d.append(draw.Lines(*right_line, fill='none', stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH))
-    
+        self.d.append(draw.Lines(*right_line, fill="none", stroke=DEFAULT_LINE_COLOR, stroke_width=DEFAULT_LINE_WIDTH))
+
     def draw_template_based_segment(self, segment, template_file_path: str):
-        self.d.append(draw.Image(segment.start_point_center.x_w - (segment.width / 2.0), segment.start_point_center.y_w, segment.width, segment.height,
-                                 template_file_path,
-                                 embed=True,
-                                 transform=f'rotate({-(segment.direction_angle - 90.0)} , {segment.start_point_center.x_w}, {-segment.start_point_center.y_w})'))
-    
+        self.d.append(
+            draw.Image(
+                segment.start_point_center.x_w - (segment.width / 2.0),
+                segment.start_point_center.y_w,
+                segment.width,
+                segment.height,
+                template_file_path,
+                embed=True,
+                transform=f"rotate({-(segment.direction_angle - 90.0)} , {segment.start_point_center.x_w}, {-segment.start_point_center.y_w})",
+            )
+        )
+
     def draw_segment(self, segment):
         if isinstance(segment, Start):
             pass
         elif isinstance(segment, Gap):
             pass
         elif isinstance(segment, Crosswalk):
             self.draw_crosswalk(segment)
@@ -223,33 +359,39 @@
             self.draw_straight_verbose(segment)
         elif isinstance(segment, Arc):
             self.draw_arc_verbose(segment)
 
     def draw_track(self, track: Track):
         self.d = draw.Drawing(track.width, track.height, origin=track.origin, displayInline=False)
         self.d.setPixelScale(1000)
-        self.d.append(draw.Rectangle(0, 0, track.width, track.height, fill=track.background.color.color,
-                                     fill_opacity=track.background.color.opacity))
+        self.d.append(
+            draw.Rectangle(
+                0,
+                0,
+                track.width,
+                track.height,
+                fill=track.background.color.color,
+                fill_opacity=track.background.color.opacity,
+            )
+        )
 
         if track.background.image:
             img = track.background.image
-            self.d.append(draw.Image(img.x, img.y,
-                                     img.width, img.height,
-                                     img.file,
-                                     embed=True,
-                                     preserveAspectRatio='none'))
+            self.d.append(
+                draw.Image(img.x, img.y, img.width, img.height, img.file, embed=True, preserveAspectRatio="none")
+            )
 
         for segment in track.segments:
             self.draw_segment(segment)
 
     def draw_track_verbose(self, track: Track):
         for segment in track.segments:
             self.draw_segment_verbose(segment)
 
-    def save_svg(self, track_name: str, output_directory: str, file_name_postfix: str = ''):
+    def save_svg(self, track_name: str, output_directory: str, file_name_postfix: str = ""):
         output_file_path = os.path.join(output_directory, track_name)
-        self.d.saveSvg(f'{output_file_path}{file_name_postfix}.svg')
+        self.d.saveSvg(f"{output_file_path}{file_name_postfix}.svg")
 
     def save_png(self, track_name: str, output_directory: str):
         output_file_path = os.path.join(output_directory, track_name)
         self.d.setPixelScale(1000)
-        self.d.savePng(f'{output_file_path}.png')
+        self.d.savePng(f"{output_file_path}.png")
```

### Comparing `track_generator-0.4.0/track_generator/segment_templates/crosswalk.svg` & `track_generator-0.5.0/track_generator/segment_templates/crosswalk.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.4.0/track_generator/segment_templates/intersection.svg` & `track_generator-0.5.0/track_generator/segment_templates/intersection.svg`

 * *Files identical despite different names*

### Comparing `track_generator-0.4.0/track_generator/starter.py` & `track_generator-0.5.0/track_generator/starter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 # Copyright (C) 2022 twyleg
 import os
 import argparse
 import sys
 
+from track_generator import __version__
 from track_generator import generator
 
 
-VERSION = '0.0.1'
-
-
 def subcommand_generate_track():
-    parser = argparse.ArgumentParser(description='Generates a track')
-    parser.add_argument('track_files', metavar='track_file', type=str, nargs='+',
-                        help='a track file (XML) to generate the track from')
-    parser.add_argument('-o', '--output', dest='output', default=os.path.join(os.getcwd(), 'output'),
-                        help='Output directory for generated tracks. Default="./"')
-    parser.add_argument('--png', action='store_true',
-                        help='Generate output PNG (SVG only by default).')
-    parser.add_argument('--gazebo', action='store_true',
-                        help='Generate Gazebo model for track.')
-    parser.add_argument('--ground_truth', action='store_true',
-                        help='Generate ground truth data for track.')
+    parser = argparse.ArgumentParser(description="Generates a track")
+    parser.add_argument(
+        "track_files", metavar="track_file", type=str, nargs="+", help="a track file (XML) to generate the track from"
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        dest="output",
+        default=os.path.join(os.getcwd(), "output"),
+        help='Output directory for generated tracks. Default="./"',
+    )
+    parser.add_argument("--png", action="store_true", help="Generate output PNG (SVG only by default).")
+    parser.add_argument("--gazebo", action="store_true", help="Generate Gazebo model for track.")
+    parser.add_argument("--ground_truth", action="store_true", help="Generate ground truth data for track.")
     args = parser.parse_args(sys.argv[2:])
 
     generator.generate_track(args.track_files, args.output, args.png, args.gazebo, args.ground_truth)
 
 
 def subcommand_generate_track_live():
-    parser = argparse.ArgumentParser(description='Generates a track')
-    parser.add_argument('track_file', metavar='track_file', type=str,
-                        help='a track file (XML) to generate the track from')
-    parser.add_argument('-o', '--output', dest='output', default=os.path.join(os.getcwd(), 'output'),
-                        help='Output directory for generated tracks. Default="./"')
+    parser = argparse.ArgumentParser(description="Generates a track")
+    parser.add_argument(
+        "track_file", metavar="track_file", type=str, help="a track file (XML) to generate the track from"
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        dest="output",
+        default=os.path.join(os.getcwd(), "output"),
+        help='Output directory for generated tracks. Default="./"',
+    )
     args = parser.parse_args(sys.argv[2:])
 
     generator.generate_track_live(args.track_file, args.output)
 
 
 def subcommand_generate_trajectory():
-    """ TODO: Implement """
+    """TODO: Implement"""
     pass
 
 
 def start():
-    parser = argparse.ArgumentParser(usage='track_generator <command> [<args>] <track_file>')
-    parser.add_argument('command', help='track_generator commands')
-    parser.add_argument('-v', '--version', help='show version and exit', action='version', version=VERSION)
+    parser = argparse.ArgumentParser(usage="track_generator <command> [<args>] <track_file>")
+    parser.add_argument("command", help="track_generator commands")
+    parser.add_argument("-v", "--version", help="show version and exit", action="version", version=__version__)
     args = parser.parse_args(sys.argv[1:2])
 
-    if args.command == 'generate_track':
+    if args.command == "generate_track":
         subcommand_generate_track()
-    elif args.command == 'generate_track_live':
+    elif args.command == "generate_track_live":
         subcommand_generate_track_live()
-    elif args.command == 'generate_trajectory':
+    elif args.command == "generate_trajectory":
         subcommand_generate_trajectory()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     start()
-
```

### Comparing `track_generator-0.4.0/track_generator/xml_reader.py` & `track_generator-0.5.0/track_generator/xml_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (C) 2022 twyleg
 import os
 import xml.etree.ElementTree as ET
+from pathlib import Path
 
 from track_generator.track import *
 
 
 class ElementMissingException(Exception):
     def __init__(self, element_name: str, parent_element: ET.Element):
         self.element_name = element_name
@@ -19,234 +20,230 @@
         self.attribute_name = attribute_name
         self.element = element
 
     def __str__(self):
         return f'AttributeMissingException: missing attribute="{self.attribute_name}" in element "{self.element.tag}""'
 
 
-def read_track(xml_input_file_path: str) -> Track:
-    tree = ET.parse(xml_input_file_path)
+def read_track(xml_input_filepath: Path) -> Track:
+    tree = ET.parse(xml_input_filepath)
     root = tree.getroot()
 
     version = _read_root(root)
     width, height = _read_size(root)
     x, y = _read_origin(root)
-    background = _read_background(root, xml_input_file_path)
+    background = _read_background(root, xml_input_filepath)
     segments = _read_segments(root)
 
     return Track(version, width, height, (x, y), background, segments)
 
 
 def _read_root(root: ET.Element) -> str:
-    version = root.get('version')
+    version = root.get("version")
 
     if version is None:
-        raise AttributeMissingException('version', root)
+        raise AttributeMissingException("version", root)
 
     return version
 
 
 def _read_size(root: ET.Element) -> Tuple[float, float]:
-
-    size_element = root.find('Size')
+    size_element = root.find("Size")
 
     if size_element is None:
-        raise ElementMissingException('Size', root)
+        raise ElementMissingException("Size", root)
 
-    width = size_element.get('width')
-    height = size_element.get('height')
+    width = size_element.get("width")
+    height = size_element.get("height")
 
     if width is None:
-        raise AttributeMissingException('width', size_element)
+        raise AttributeMissingException("width", size_element)
 
     if height is None:
-        raise AttributeMissingException('height', size_element)
+        raise AttributeMissingException("height", size_element)
 
     return float(width), float(height)
 
 
 def _read_origin(root: ET.Element) -> Tuple[float, float]:
-
-    origin_element = root.find('Origin')
+    origin_element = root.find("Origin")
 
     if origin_element is None:
-        raise ElementMissingException('Origin', root)
+        raise ElementMissingException("Origin", root)
 
-    x = origin_element.get('x')
-    y = origin_element.get('y')
+    x = origin_element.get("x")
+    y = origin_element.get("y")
 
     if x is None:
-        raise AttributeMissingException('x', origin_element)
+        raise AttributeMissingException("x", origin_element)
 
     if y is None:
-        raise AttributeMissingException('y', origin_element)
+        raise AttributeMissingException("y", origin_element)
 
     return float(x), float(y)
 
 
-def _read_background(root: ET.Element, xml_file_path: str) -> Background:
-
-    background_element = root.find('Background')
+def _read_background(root: ET.Element, xml_filepath: Path) -> Background:
+    background_element = root.find("Background")
 
     if background_element is None:
-        raise ElementMissingException('Background', root)
+        raise ElementMissingException("Background", root)
 
-    color = background_element.get('color')
-    opacity = background_element.get('opacity')
+    color = background_element.get("color")
+    opacity = background_element.get("opacity")
 
     if color is None:
-        raise AttributeMissingException('color', background_element)
+        raise AttributeMissingException("color", background_element)
 
     if opacity is None:
-        raise AttributeMissingException('opacity', background_element)
+        raise AttributeMissingException("opacity", background_element)
 
-    background_color = Background.Color(color, opacity)
+    background_color = Background.Color(color, float(opacity))
 
-    background_image_element = root.find('BackgroundImage')
+    background_image_element = root.find("BackgroundImage")
     background_image = None
 
     if background_image_element is not None:
-        file = background_image_element.get('file')
-        x = float(background_image_element.get('x'))
-        y = float(background_image_element.get('y'))
-        width = float(background_image_element.get('width'))
-        height = float(background_image_element.get('height'))
+        file = background_image_element.get("file")
+        x = float(background_image_element.get("x"))
+        y = float(background_image_element.get("y"))
+        width = float(background_image_element.get("width"))
+        height = float(background_image_element.get("height"))
 
         if not os.path.isabs(file):
-            xml_file_basedir = os.path.dirname(xml_file_path)
+            xml_file_basedir = os.path.dirname(xml_filepath)
             file = os.path.join(xml_file_basedir, file)
 
         background_image = Background.Image(file, x, y, width, height)
 
     return Background(background_color, background_image)
 
 
 def _read_segments(root: ET.Element):
-
     segments_element = root.find("Segments")
 
     if segments_element is None:
-        raise ElementMissingException('Segments', root)
+        raise ElementMissingException("Segments", root)
 
     segments = []
 
     for segment_element in segments_element:
-        if segment_element.tag == 'Start':
+        if segment_element.tag == "Start":
             segments.append(_read_start_element(segment_element))
-        elif segment_element.tag in ['Straight', 'BlockedArea']:
+        elif segment_element.tag in ["Straight", "BlockedArea"]:
             segments.append(_read_straight_element(segment_element))
-        elif segment_element.tag == 'Turn':
+        elif segment_element.tag == "Turn":
             segments.append(_read_turn_element(segment_element))
-        elif segment_element.tag == 'Crosswalk':
+        elif segment_element.tag == "Crosswalk":
             segments.append(_read_crosswalk_element(segment_element))
-        elif segment_element.tag == 'Intersection':
+        elif segment_element.tag == "Intersection":
             segments.append(_read_intersection_element(segment_element))
-        elif segment_element.tag == 'Gap':
+        elif segment_element.tag == "Gap":
             segments.append(_read_gap_element(segment_element))
-        elif segment_element.tag == 'ParkingArea':
+        elif segment_element.tag == "ParkingArea":
             segments.append(_read_parking_area_element(segment_element))
-        elif segment_element.tag == 'TrafficIsland':
+        elif segment_element.tag == "TrafficIsland":
             segments.append(_read_traffic_island_element(segment_element))
-        elif segment_element.tag == 'Clothoid':
+        elif segment_element.tag == "Clothoid":
             segments.append(_read_clothoid_element(segment_element))
 
     return segments
 
 
 def _read_start_element(start_element: ET.Element):
-    x = start_element.get('x')
-    y = start_element.get('y')
-    direction_angle = start_element.get('direction_angle')
+    x = start_element.get("x")
+    y = start_element.get("y")
+    direction_angle = start_element.get("direction_angle")
 
     if x is None:
-        raise AttributeMissingException('x', start_element)
+        raise AttributeMissingException("x", start_element)
     elif y is None:
-        raise AttributeMissingException('y', start_element)
+        raise AttributeMissingException("y", start_element)
     elif direction_angle is None:
-        raise AttributeMissingException('direction_angle', start_element)
+        raise AttributeMissingException("direction_angle", start_element)
 
     return Start(float(x), float(y), float(direction_angle))
 
 
 def _read_straight_element(straight_element: ET.Element):
-    length = straight_element.get('length')
+    length = straight_element.get("length")
 
     if length is None:
-        raise AttributeMissingException('length', straight_element)
+        raise AttributeMissingException("length", straight_element)
 
     return Straight(float(length))
 
 
 def _read_turn_element(turn_element: ET.Element):
-    direction = turn_element.get('direction')
-    radius = turn_element.get('radius')
-    radian = turn_element.get('radian')
+    direction = turn_element.get("direction")
+    radius = turn_element.get("radius")
+    radian = turn_element.get("radian")
 
     if direction is None:
-        raise AttributeMissingException('direction', turn_element)
+        raise AttributeMissingException("direction", turn_element)
     elif radius is None:
-        raise AttributeMissingException('radius', turn_element)
+        raise AttributeMissingException("radius", turn_element)
     elif radian is None:
-        raise AttributeMissingException('radian', turn_element)
+        raise AttributeMissingException("radian", turn_element)
 
-    cw = True if direction == 'right' else False
+    cw = True if direction == "right" else False
 
     return Arc(float(radius), float(radian), cw)
 
 
 def _read_crosswalk_element(crosswalk_element: ET.Element):
-    length = crosswalk_element.get('length')
+    length = crosswalk_element.get("length")
 
     if length is None:
-        raise AttributeMissingException('length', crosswalk_element)
+        raise AttributeMissingException("length", crosswalk_element)
 
     return Crosswalk(float(length))
 
 
 def _read_intersection_element(intersection_element: ET.Element):
-    length = intersection_element.get('length')
-    direction = IntersectionDirection(str(intersection_element.get('direction')))
+    length = intersection_element.get("length")
+    direction = IntersectionDirection(str(intersection_element.get("direction")))
     if length is None:
-        raise AttributeMissingException('length', intersection_element)
+        raise AttributeMissingException("length", intersection_element)
     return Intersection(float(length), direction)
 
 
 def _read_gap_element(straight_element: ET.Element):
-    length = straight_element.get('length')
-    direction = IntersectionDirection(str(straight_element.get('direction')))
+    length = straight_element.get("length")
+    direction = IntersectionDirection(str(straight_element.get("direction")))
     if length is None:
-        raise AttributeMissingException('length', straight_element)
+        raise AttributeMissingException("length", straight_element)
 
     return Gap(float(length), direction)
 
 
 def _read_spot_element(spot_element: ET.Element) -> ParkingArea.ParkingLot.Spot:
-    type = spot_element.get('type')
-    length = spot_element.get('length')
+    type = spot_element.get("type")
+    length = spot_element.get("length")
     return ParkingArea.ParkingLot.Spot(type, float(length))
 
 
 def _read_parking_lot_element(parking_lot_element: ET.Element) -> ParkingArea.ParkingLot:
-    start = parking_lot_element.get('start')
-    depth = parking_lot_element.get('depth')
-    opening_ending_angle = parking_lot_element.get('opening_ending_angle')
+    start = parking_lot_element.get("start")
+    depth = parking_lot_element.get("depth")
+    opening_ending_angle = parking_lot_element.get("opening_ending_angle")
     spots: List[ParkingArea.ParkingLot.Spot] = []
 
     for spot_element in parking_lot_element:
         spot = _read_spot_element(spot_element)
         spots.append(spot)
 
     return ParkingArea.ParkingLot(float(start), float(depth), float(opening_ending_angle), spots)
 
 
 def _read_parking_area_element(parking_area_element: ET.Element):
-    length = parking_area_element.get('length')
+    length = parking_area_element.get("length")
 
     if length is None:
-        raise AttributeMissingException('length', parking_area_element)
+        raise AttributeMissingException("length", parking_area_element)
 
     right_lots: List[ParkingArea.ParkingLot] = []
     left_lots: List[ParkingArea.ParkingLot] = []
 
     right_lots_element = parking_area_element.find("RightLots")
     for parking_lot_element in right_lots_element:
         parking_lot = _read_parking_lot_element(parking_lot_element)
@@ -257,22 +254,23 @@
         parking_lot = _read_parking_lot_element(parking_lot_element)
         left_lots.append(parking_lot)
 
     return ParkingArea(float(length), right_lots, left_lots)
 
 
 def _read_traffic_island_element(traffic_island_element: ET.Element):
-    island_width = traffic_island_element.get('island_width')
-    crosswalk_length = traffic_island_element.get('crosswalk_length')
-    curve_segment_length = traffic_island_element.get('curve_segment_length')
-    curvature = traffic_island_element.get('curvature')
+    island_width = traffic_island_element.get("island_width")
+    crosswalk_length = traffic_island_element.get("crosswalk_length")
+    curve_segment_length = traffic_island_element.get("curve_segment_length")
+    curvature = traffic_island_element.get("curvature")
 
     return TrafficIsland(float(island_width), float(crosswalk_length), float(curve_segment_length), float(curvature))
 
+
 def _read_clothoid_element(clothoid_element: ET.Element) -> Clothoid:
-    a = clothoid_element.get('a')
-    angle = clothoid_element.get('angle')
-    angle_offset = clothoid_element.get('angle_offset')
-    direction = ClothoidDirection.RIGHT if clothoid_element.get('direction') == 'right' else ClothoidDirection.LEFT
-    type = ClothoidType(str(clothoid_element.get('type')))
+    a = clothoid_element.get("a")
+    angle = clothoid_element.get("angle")
+    angle_offset = clothoid_element.get("angle_offset")
+    direction = ClothoidDirection.RIGHT if clothoid_element.get("direction") == "right" else ClothoidDirection.LEFT
+    type = ClothoidType(str(clothoid_element.get("type")))
 
-    return Clothoid(float(a), float(angle), float(angle_offset), direction, str(type))
+    return Clothoid(float(a), float(angle), float(angle_offset), direction, ClothoidType(type))
```

### Comparing `track_generator-0.4.0/track_generator.egg-info/PKG-INFO` & `track_generator-0.5.0/track_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: track-generator
-Version: 0.4.0
+Version: 0.5.0
 Summary: Track generator
 Home-page: https://github.com/twyleg/track_generator
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: svg model vehicles track
-Platform: UNKNOWN
 
 # Track Generator
 
 Simple generator to create tracks (ground textures for vehicle simulations)
 from parametric descriptions.
 
 For example, the following parametric description of a track in XML will lead
@@ -79,8 +78,7 @@
 left hand side cartesian coordinate system. This is important for internal operations but shouldn't bother the user.
 
 ![coordiante systems](doc/img/svg/coordinate_systems.svg)
 
 ## Examples
 
 Example track definitions can be found under [examples/](examples/)
-
```

### Comparing `track_generator-0.4.0/track_generator.egg-info/SOURCES.txt` & `track_generator-0.5.0/track_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 MANIFEST.in
 README.md
-VERSION.txt
+setup.cfg
 setup.py
+versioneer.py
+tests/test_track_generator.py
 track_generator/__init__.py
 track_generator/__main__.py
+track_generator/_version.py
 track_generator/coordinate_system.py
 track_generator/gazebo_model_generator.py
 track_generator/generator.py
 track_generator/ground_truth_generator.py
 track_generator/painter.py
 track_generator/starter.py
 track_generator/track.py
```


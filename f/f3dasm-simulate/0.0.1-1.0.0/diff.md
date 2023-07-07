# Comparing `tmp/f3dasm_simulate-0.0.1.tar.gz` & `tmp/f3dasm_simulate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/martin/Documents/GitHub/f3dasm_simulate/dist/.tmp-t0ze2qoq/f3dasm_simulate-0.0.1.tar", last modified: Mon Jun 19 13:42:51 2023, max compression
+gzip compressed data, was "f3dasm_simulate-1.0.0.tar", last modified: Fri Jul  7 13:52:09 2023, max compression
```

## Comparing `f3dasm_simulate-0.0.1.tar` & `f3dasm_simulate-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,57 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1507 2023-06-19 13:35:57.000000 f3dasm_simulate-0.0.1/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-19 13:35:57.000000 f3dasm_simulate-0.0.1/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     1768 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      970 2023-06-19 13:35:57.000000 f3dasm_simulate-0.0.1/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-06-19 13:42:42.000000 f3dasm_simulate-0.0.1/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-19 13:35:57.000000 f3dasm_simulate-0.0.1/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-06-19 13:35:57.000000 f3dasm_simulate-0.0.1/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      996 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate/
--rw-rw-r--   0 martin    (1000) martin    (1000)      976 2023-06-19 13:41:33.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      859 2023-06-19 13:35:57.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate/example_module.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1768 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      343 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       16 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/src/f3dasm_simulate.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-19 13:42:51.000000 f3dasm_simulate-0.0.1/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)      102 2023-06-19 13:38:38.000000 f3dasm_simulate-0.0.1/tests/test_add_one.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1507 2023-06-19 13:35:57.000000 f3dasm_simulate-1.0.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-06-19 13:35:57.000000 f3dasm_simulate-1.0.0/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      712 2023-06-19 13:50:43.000000 f3dasm_simulate-1.0.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-06-19 13:35:57.000000 f3dasm_simulate-1.0.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-07-07 13:13:18.000000 f3dasm_simulate-1.0.0/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      996 2023-07-07 13:52:09.401110 f3dasm_simulate-1.0.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.393110 f3dasm_simulate-1.0.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.393110 f3dasm_simulate-1.0.0/src/f3dasm_simulate/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1217 2023-07-07 12:33:50.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1177 2023-07-07 11:28:44.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10222 2023-06-27 11:44:54.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/amplitudesampler.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1549 2023-06-27 11:44:54.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/cddm.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    28325 2023-06-27 11:44:54.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/circle_particles.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2622 2023-06-23 14:41:02.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/loading.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7588 2023-06-27 11:44:54.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/material.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3443 2023-06-27 11:44:54.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/microstructure.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7986 2023-06-27 11:44:54.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/microstructure_generator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1509 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/overwrite_inputs.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      115 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      599 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5049 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/common_procedure.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12690 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/geometry_modeling.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1037 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/jobs.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10442 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/loading_condition.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4969 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/materials.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1721 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/mesh.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6392 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/periodical_boundary_condition.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8939 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/post_process.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2421 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/basic_analysis_scripts/steps.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      473 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12696 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/hollow_plate_sve.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    13019 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/single_material_sve.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    13566 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/two_materials_rve.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12348 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/two_materials_sve.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    29715 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/scriptbase/benchmark_abaqus_scripts/veni_rve.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    12402 2023-07-05 14:53:28.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/simulator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2791 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/simulator_assertinputs.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3822 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/simulator_info.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1724 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/simulator_part.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    64565 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/sphere_particles.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2193 2023-06-23 08:08:30.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      859 2023-06-19 13:35:57.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate/example_module.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.393110 f3dasm_simulate-1.0.0/src/f3dasm_simulate.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1510 2023-07-07 13:52:09.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2351 2023-07-07 13:52:09.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-07 13:52:09.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       14 2023-07-07 13:52:09.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       16 2023-07-07 13:52:09.000000 f3dasm_simulate-1.0.0/src/f3dasm_simulate.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:52:09.397110 f3dasm_simulate-1.0.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      102 2023-06-19 13:38:38.000000 f3dasm_simulate-1.0.0/tests/test_add_one.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `f3dasm_simulate-0.0.1/LICENSE` & `f3dasm_simulate-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm_simulate-0.0.1/setup.cfg` & `f3dasm_simulate-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `f3dasm_simulate-0.0.1/src/f3dasm_simulate/__init__.py` & `f3dasm_simulate-1.0.0/src/f3dasm_simulate/abaqus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 
 # Third-party
 
+
 # Local
-from .example_module import add_one
+from ..example_module import add_one
+from . import (loading, material, microstructure, overwrite_inputs, simulator,
+               simulator_info)
+from .cddm import VonMisesPlasticElasticPathLoads
+from .simulator import AbaqusSimulator
 
 #                                                        Authorship and Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
```

### Comparing `f3dasm_simulate-0.0.1/src/f3dasm_simulate/example_module.py` & `f3dasm_simulate-1.0.0/src/f3dasm_simulate/example_module.py`

 * *Files identical despite different names*


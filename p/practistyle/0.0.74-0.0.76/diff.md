# Comparing `tmp/practistyle-0.0.74.tar.gz` & `tmp/practistyle-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "practistyle-0.0.74.tar", last modified: Fri Jul  7 09:47:11 2023, max compression
+gzip compressed data, was "practistyle-0.0.76.tar", last modified: Fri Jul  7 09:50:43 2023, max compression
```

## Comparing `practistyle-0.0.74.tar` & `practistyle-0.0.76.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:47:11.393074 practistyle-0.0.74/
--rw-r--r--   0 truman    (1000) truman    (1000)      119 2023-07-07 09:47:11.393074 practistyle-0.0.74/PKG-INFO
--rw-r--r--   0 truman    (1000) truman    (1000)    38376 2023-07-07 09:33:08.000000 practistyle-0.0.74/README.md
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:47:11.392074 practistyle-0.0.74/practistyle/
--rw-r--r--   0 truman    (1000) truman    (1000)      469 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/__init__.py
--rw-r--r--   0 truman    (1000) truman    (1000)     2231 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/active_obj.py
--rw-r--r--   0 truman    (1000) truman    (1000)     4029 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/box.py
--rw-r--r--   0 truman    (1000) truman    (1000)    16013 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/camera.py
--rw-r--r--   0 truman    (1000) truman    (1000)     1271 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/cube.py
--rw-r--r--   0 truman    (1000) truman    (1000)     1414 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/cylinder.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:47:11.392074 practistyle-0.0.74/practistyle/data/
--rw-r--r--   0 truman    (1000) truman    (1000)       75 2023-07-07 09:33:08.000000 practistyle-0.0.74/practistyle/data/__init__.py
--rw-r--r--   0 truman    (1000) truman    (1000)     3468 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/editor.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:47:11.393074 practistyle-0.0.74/practistyle/end_effector/
--rw-r--r--   0 truman    (1000) truman    (1000)      105 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/end_effector/__init__.py
--rw-r--r--   0 truman    (1000) truman    (1000)     2363 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/end_effector/gripper.py
--rw-r--r--   0 truman    (1000) truman    (1000)     1885 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/end_effector/suction.py
--rw-r--r--   0 truman    (1000) truman    (1000)     3112 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/placer.py
--rw-r--r--   0 truman    (1000) truman    (1000)    10083 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/printer.py
--rw-r--r--   0 truman    (1000) truman    (1000)     3554 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/render.py
--rw-r--r--   0 truman    (1000) truman    (1000)    23568 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/robot.py
--rw-r--r--   0 truman    (1000) truman    (1000)     6760 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/scene.py
--rw-r--r--   0 truman    (1000) truman    (1000)     3199 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/stacker.py
--rw-r--r--   0 truman    (1000) truman    (1000)     6852 2023-07-07 09:33:10.000000 practistyle-0.0.74/practistyle/workflow.py
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:47:11.392074 practistyle-0.0.74/practistyle.egg-info/
--rw-r--r--   0 truman    (1000) truman    (1000)      119 2023-07-07 09:47:11.000000 practistyle-0.0.74/practistyle.egg-info/PKG-INFO
--rw-r--r--   0 truman    (1000) truman    (1000)      731 2023-07-07 09:47:11.000000 practistyle-0.0.74/practistyle.egg-info/SOURCES.txt
--rw-r--r--   0 truman    (1000) truman    (1000)        1 2023-07-07 09:47:11.000000 practistyle-0.0.74/practistyle.egg-info/dependency_links.txt
--rw-r--r--   0 truman    (1000) truman    (1000)       21 2023-07-07 09:47:11.000000 practistyle-0.0.74/practistyle.egg-info/requires.txt
--rw-r--r--   0 truman    (1000) truman    (1000)       61 2023-07-07 09:47:11.000000 practistyle-0.0.74/practistyle.egg-info/top_level.txt
-drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:47:11.393074 practistyle-0.0.74/py3dbp/
--rw-r--r--   0 truman    (1000) truman    (1000)       41 2023-07-03 00:49:14.000000 practistyle-0.0.74/py3dbp/__init__.py
--rw-r--r--   0 truman    (1000) truman    (1000)      988 2023-07-03 00:49:14.000000 practistyle-0.0.74/py3dbp/auxiliary_methods.py
--rw-r--r--   0 truman    (1000) truman    (1000)    14284 2023-07-03 00:49:14.000000 practistyle-0.0.74/py3dbp/binpacking.py
--rw-r--r--   0 truman    (1000) truman    (1000)      261 2023-07-03 00:49:14.000000 practistyle-0.0.74/py3dbp/constants.py
--rw-r--r--   0 truman    (1000) truman    (1000)       38 2023-07-07 09:47:11.394074 practistyle-0.0.74/setup.cfg
--rw-r--r--   0 truman    (1000) truman    (1000)      652 2023-07-07 09:33:10.000000 practistyle-0.0.74/setup.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:50:43.218699 practistyle-0.0.76/
+-rw-r--r--   0 truman    (1000) truman    (1000)      119 2023-07-07 09:50:43.218699 practistyle-0.0.76/PKG-INFO
+-rw-r--r--   0 truman    (1000) truman    (1000)    38376 2023-07-07 09:33:08.000000 practistyle-0.0.76/README.md
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:50:43.216699 practistyle-0.0.76/practistyle/
+-rw-r--r--   0 truman    (1000) truman    (1000)      469 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/__init__.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     2231 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/active_obj.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     4029 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/box.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    16013 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/camera.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     1271 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/cube.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     1414 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/cylinder.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:50:43.217699 practistyle-0.0.76/practistyle/data/
+-rw-r--r--   0 truman    (1000) truman    (1000)       75 2023-07-07 09:33:08.000000 practistyle-0.0.76/practistyle/data/__init__.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     3468 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/editor.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:50:43.217699 practistyle-0.0.76/practistyle/end_effector/
+-rw-r--r--   0 truman    (1000) truman    (1000)      105 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/end_effector/__init__.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     2363 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/end_effector/gripper.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     1885 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/end_effector/suction.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     3112 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/placer.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    10083 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/printer.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     3554 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/render.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    23568 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/robot.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     6760 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/scene.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     3199 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/stacker.py
+-rw-r--r--   0 truman    (1000) truman    (1000)     6852 2023-07-07 09:33:10.000000 practistyle-0.0.76/practistyle/workflow.py
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:50:43.217699 practistyle-0.0.76/practistyle.egg-info/
+-rw-r--r--   0 truman    (1000) truman    (1000)      119 2023-07-07 09:50:43.000000 practistyle-0.0.76/practistyle.egg-info/PKG-INFO
+-rw-r--r--   0 truman    (1000) truman    (1000)      731 2023-07-07 09:50:43.000000 practistyle-0.0.76/practistyle.egg-info/SOURCES.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)        1 2023-07-07 09:50:43.000000 practistyle-0.0.76/practistyle.egg-info/dependency_links.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)       21 2023-07-07 09:50:43.000000 practistyle-0.0.76/practistyle.egg-info/requires.txt
+-rw-r--r--   0 truman    (1000) truman    (1000)       61 2023-07-07 09:50:43.000000 practistyle-0.0.76/practistyle.egg-info/top_level.txt
+drwxr-xr-x   0 truman    (1000) truman    (1000)        0 2023-07-07 09:50:43.217699 practistyle-0.0.76/py3dbp/
+-rw-r--r--   0 truman    (1000) truman    (1000)       41 2023-07-03 00:49:14.000000 practistyle-0.0.76/py3dbp/__init__.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      988 2023-07-03 00:49:14.000000 practistyle-0.0.76/py3dbp/auxiliary_methods.py
+-rw-r--r--   0 truman    (1000) truman    (1000)    14284 2023-07-03 00:49:14.000000 practistyle-0.0.76/py3dbp/binpacking.py
+-rw-r--r--   0 truman    (1000) truman    (1000)      261 2023-07-03 00:49:14.000000 practistyle-0.0.76/py3dbp/constants.py
+-rw-r--r--   0 truman    (1000) truman    (1000)       38 2023-07-07 09:50:43.218699 practistyle-0.0.76/setup.cfg
+-rw-r--r--   0 truman    (1000) truman    (1000)      652 2023-07-07 09:33:10.000000 practistyle-0.0.76/setup.py
```

### Comparing `practistyle-0.0.74/README.md` & `practistyle-0.0.76/README.md`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/active_obj.py` & `practistyle-0.0.76/practistyle/active_obj.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/box.py` & `practistyle-0.0.76/practistyle/box.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/camera.py` & `practistyle-0.0.76/practistyle/camera.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/cube.py` & `practistyle-0.0.76/practistyle/cube.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/cylinder.py` & `practistyle-0.0.76/practistyle/cylinder.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/editor.py` & `practistyle-0.0.76/practistyle/editor.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/end_effector/gripper.py` & `practistyle-0.0.76/practistyle/end_effector/gripper.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/end_effector/suction.py` & `practistyle-0.0.76/practistyle/end_effector/suction.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/placer.py` & `practistyle-0.0.76/practistyle/placer.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/printer.py` & `practistyle-0.0.76/practistyle/printer.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/render.py` & `practistyle-0.0.76/practistyle/render.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/robot.py` & `practistyle-0.0.76/practistyle/robot.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/scene.py` & `practistyle-0.0.76/practistyle/scene.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/stacker.py` & `practistyle-0.0.76/practistyle/stacker.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle/workflow.py` & `practistyle-0.0.76/practistyle/workflow.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/practistyle.egg-info/SOURCES.txt` & `practistyle-0.0.76/practistyle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/py3dbp/auxiliary_methods.py` & `practistyle-0.0.76/py3dbp/auxiliary_methods.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/py3dbp/binpacking.py` & `practistyle-0.0.76/py3dbp/binpacking.py`

 * *Files identical despite different names*

### Comparing `practistyle-0.0.74/setup.py` & `practistyle-0.0.76/setup.py`

 * *Files identical despite different names*


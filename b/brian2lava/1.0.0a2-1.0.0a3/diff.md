# Comparing `tmp/brian2lava-1.0.0a2.tar.gz` & `tmp/brian2lava-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brian2lava-1.0.0a2.tar", last modified: Fri May 19 13:30:48 2023, max compression
+gzip compressed data, was "brian2lava-1.0.0a3.tar", last modified: Fri Jul  7 08:40:07 2023, max compression
```

## Comparing `brian2lava-1.0.0a2.tar` & `brian2lava-1.0.0a3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       80 2023-03-26 23:21:40.000000 brian2lava-1.0.0a2/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2178 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1423 2023-05-19 13:30:09.000000 brian2lava-1.0.0a2/README.md
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.818439 brian2lava-1.0.0a2/brian2lava/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       47 2023-05-15 08:19:12.000000 brian2lava-1.0.0a2/brian2lava/__init__.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.818439 brian2lava-1.0.0a2/brian2lava/codegen/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     5722 2023-03-26 23:36:06.000000 brian2lava-1.0.0a2/brian2lava/codegen/codeobject.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    35555 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/codegen/lava_generator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3479 2023-03-26 23:38:15.000000 brian2lava-1.0.0a2/brian2lava/codegen/templater.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.822439 brian2lava-1.0.0a2/brian2lava/codegen/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1058 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/activation_processing.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      731 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/common_group.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      436 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_get_indices.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      633 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      553 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get_conditional.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      512 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1760 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set_conditional.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      537 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/ratemonitor.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      521 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/reset.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7522 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/spatialstateupdate.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1179 2023-03-26 07:47:47.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/spikegenerator.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/spikemonitor.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)        1 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/statemonitor.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      419 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/stateupdate.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1305 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/summed_variable.py_
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1213 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1713 2023-03-26 21:28:29.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_array.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    11153 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_generator.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      524 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_push_spikes.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1860 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_transmit.py_
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1672 2023-03-26 07:47:47.000000 brian2lava-1.0.0a2/brian2lava/codegen/templates/threshold.py_
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/brian2lava/device/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6977 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3090 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/activate.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    16121 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/arrays.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    23642 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/device/build.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3332 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/codeobject.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    25580 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/device/run.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    10616 2023-05-19 09:41:04.000000 brian2lava-1.0.0a2/brian2lava/device/synapses.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7050 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/device/variables.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1618 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/device/writer.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/brian2lava/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      929 2023-04-15 20:02:40.000000 brian2lava-1.0.0a2/brian2lava/templates/process.py.j2
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1338 2023-05-15 08:19:31.000000 brian2lava-1.0.0a2/brian2lava/templates/process_model.py.j2
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/brian2lava/writer/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1369 2023-03-14 08:59:44.000000 brian2lava-1.0.0a2/brian2lava/writer/py.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 13:30:48.818439 brian2lava-1.0.0a2/brian2lava.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2178 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1743 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      107 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       11 2023-05-19 13:30:48.000000 brian2lava-1.0.0a2/brian2lava.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-05-19 13:30:48.826439 brian2lava-1.0.0a2/setup.cfg
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1009 2023-05-19 13:28:48.000000 brian2lava-1.0.0a2/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.995366 brian2lava-1.0.0a3/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       80 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/MANIFEST.in
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2178 2023-07-07 08:40:07.995366 brian2lava-1.0.0a3/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1423 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/README.md
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.987366 brian2lava-1.0.0a3/brian2lava/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       47 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/__init__.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.991366 brian2lava-1.0.0a3/brian2lava/codegen/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2623 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/codeobject.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    39759 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/lava_generator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3479 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templater.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.991366 brian2lava-1.0.0a3/brian2lava/codegen/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1220 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/activation_processing.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      731 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/common_group.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      436 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/group_get_indices.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      633 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_get.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      553 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_get_conditional.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      512 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_set.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1760 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_set_conditional.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      537 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/ratemonitor.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      521 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/reset.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7522 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/spatialstateupdate.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1179 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/spikegenerator.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/spikemonitor.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)        1 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/statemonitor.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      419 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/stateupdate.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1305 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/summed_variable.py_
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1131 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2399 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_create_array.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    11666 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_create_generator.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      498 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_push_spikes.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1441 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_transmit.py_
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1676 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/codegen/templates/threshold.py_
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.995366 brian2lava-1.0.0a3/brian2lava/device/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7341 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1886 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/activate.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    17942 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/arrays.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    29825 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/build.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6043 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/codeobject.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    27708 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/run.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    10067 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/synapses.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     9867 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/device/variables.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1618 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/device/writer.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.995366 brian2lava-1.0.0a3/brian2lava/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      929 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/templates/process.py.j2
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2193 2023-07-07 08:02:02.000000 brian2lava-1.0.0a3/brian2lava/templates/process_model.py.j2
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.995366 brian2lava-1.0.0a3/brian2lava/writer/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1369 2023-06-05 07:21:07.000000 brian2lava-1.0.0a3/brian2lava/writer/py.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-07 08:40:07.991366 brian2lava-1.0.0a3/brian2lava.egg-info/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2178 2023-07-07 08:40:07.000000 brian2lava-1.0.0a3/brian2lava.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1743 2023-07-07 08:40:07.000000 brian2lava-1.0.0a3/brian2lava.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-07-07 08:40:07.000000 brian2lava-1.0.0a3/brian2lava.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      107 2023-07-07 08:40:07.000000 brian2lava-1.0.0a3/brian2lava.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       11 2023-07-07 08:40:07.000000 brian2lava-1.0.0a3/brian2lava.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-07-07 08:40:07.995366 brian2lava-1.0.0a3/setup.cfg
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1009 2023-07-07 08:40:01.000000 brian2lava-1.0.0a3/setup.py
```

### Comparing `brian2lava-1.0.0a2/PKG-INFO` & `brian2lava-1.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brian2lava
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: An open source Brian2 interface for the neuromorphic computing framework Lava
 Home-page: https://gitlab.com/tetzlab/brian2lava
 Author: Carlo Michaelis, Francesco Negri, Winfried Oed, Jannik Luboeinski, Andrew Lehr, Tristan Stöber
 Author-email: carlo.michaelis@gmail.com
 License: MIT
 Description: # Brian2Lava
```

### Comparing `brian2lava-1.0.0a2/README.md` & `brian2lava-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/lava_generator.py` & `brian2lava-1.0.0a3/brian2lava/codegen/lava_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from brian2.parsing.rendering import NumpyNodeRenderer
 from brian2.core.functions import DEFAULT_FUNCTIONS, timestep
 from brian2.core.variables import Constant, ArrayVariable
 from brian2.utils.stringtools import get_identifiers, word_substitute, indent
 from brian2.utils.logger import get_logger
 from brian2.core.functions import Function
 from brian2.groups.neurongroup import NeuronGroup
+from brian2.synapses.synapses import Synapses
 from brian2.units.unitsafefunctions import exprel
 
 from brian2.codegen.generators.base import CodeGenerator
 
 
 # TODO remove, only for development
 from pprint import pprint
@@ -387,14 +388,51 @@
             # Also index _vectorisation_idx so that e.g. rand() works correctly
             subs['_vectorisation_idx'] = f"_vectorisation_idx[{repl_string}]"
 
             line = word_substitute(line, subs)
             line = line.replace(repl_string, index)
 
         return line
+    
+    def check_for_brian2lava_support(self,scalar_statements,vector_statements):
+        """
+        Check some features of the codeobject to be generated to make sure that brian2lava supports these operations
+        """
+        from brian2 import get_device
+
+        # Conditions like: S.connect('v_pre!=v_post') are not supported
+        # Go through all the variables used in the statements and make sure they don't belong to NeuronGroups
+        if 'synapses_create' in self.template_name:
+            created_vars = set()
+            # In the scalar statements we only collect possible created scalar variables (useful for differential equations)
+            for name,statements in scalar_statements.items():
+                created_vars = created_vars.union({stmt.var for stmt in statements if stmt.op == ':='})
+            # We only care about vector statements in this case
+            for name,statements in vector_statements.items():
+                created_vars = created_vars.union({stmt.var for stmt in statements if stmt.op == ':='})
+                for stmt in statements:
+                    vars_str = [stmt.var]
+                    vars_str.extend([id for id in get_identifiers(stmt.expr)])
+                    for var_str in vars_str:
+                        # Created vars are not a problem, they're handled by the generator
+                        if var_str in created_vars:
+                            continue
+
+                        var = self.variables[var_str]
+                        # Vars without an owner are not a problem, they will be added as constants
+                        if not hasattr(var,"owner"):
+                            continue
+
+                        if isinstance(var.owner,NeuronGroup) and not isinstance(var,Constant):
+                            msg = """Initializing Synapses with variables from other objects is currently not supported.
+                            For example:
+                            Synapses.connect('v_pre!=v_post')
+                            Will raise this error if v_pre and v_post belong to a NeuronGroup.
+                            """
+                            raise NotImplementedError(msg)
 
 
     def translate_statement_sequence(self, scalar_statements, vector_statements):
         """
         Takes lines of code and defines Jinja variables, stored in Python dictionaries.
 
         Parameters
@@ -410,14 +448,17 @@
             Jinja variables containing compiled *scalar* code.
         vector_code : `dict`
             Jinja variables containing compiled *vector* code.
         kwds : `dict`
             Jinja variables containing additional custom variables (so called 'keywords').
         """
 
+        # First make sure we can handle this codeobject
+        self.check_for_brian2lava_support(scalar_statements, vector_statements)
+
         # If we're dealing with synapses, we buffer the translation and manage their two functions separately
         if self.template_name == 'synapses':
             # Get the statements which are only related to synapses (the neuronal part of transmission is handled by another template)
             scalar_statements,vector_statements = self.manage_neuron_activations(scalar_statements,vector_statements)
 
             # Use these statements to manage synaptic transmission
             self.manage_synaptic_behavior(scalar_statements,vector_statements)
@@ -547,31 +588,37 @@
             for stmt in block:
                 if stmt.var in created_vars:
                     if stmt.var in neuron_created_vars:
                         # Make the operator a simple '=' since the := operator is not recognized by the 
                         # brian parser.
                         stmt.op = '='
                         neuron_scalar_statements[name].append(stmt)
+                    # If it wasn't created for the neuron it goes in the synaptic statements
+                    synapse_scalar_statements[name].append(stmt)
                     continue
                 var = self.variables[stmt.var]
                 if isinstance(var.owner,NeuronGroup):
                     neuron_scalar_statements[name].append(stmt)
                     continue
                 synapse_scalar_statements[name].append(stmt)
-            
-        
+
         for name, block in vector_statements.items():
             # Collecting all of the created vars.
             created_vars = {stmt.var for stmt in block if stmt.op == ':='}
             for stmt in block:
+                # We don't copy subexpressions, because they are handled internally in brian
+                if stmt.subexpression:
+                    continue
                 # Again the created vars are added to the statements if they are used by the neuron statements
                 if stmt.var in created_vars:
                     if stmt.var in neuron_created_vars:
                         stmt.op = '='
                         neuron_vector_statements[name].append(stmt)
+                    # If it wasn't created for the neuron it goes in the synaptic statements
+                    synapse_vector_statements[name].append(stmt)
                     continue
                 var = self.variables[stmt.var]
                 if isinstance(var.owner,NeuronGroup):
                     neuron_vector_statements[name].append(stmt)
                     continue
                 synapse_vector_statements[name].append(stmt)
         
@@ -582,15 +629,15 @@
         # Create the 'activation_processing' codeobject handling synaptic effects on neurons
         all_neuron_statements = [statement for block in neuron_scalar_statements.values() for statement in block]
         all_neuron_statements += [statement for block in neuron_vector_statements.values() for statement in block]
         
         code_str = '\n'.join([stmt.var+stmt.op+str(stmt.expr) for stmt in all_neuron_statements])
         abstract_code = {None: code_str}
 
-        codeobj_name = pathway.target.name +'_'+ self.owner.name + '_' + pathway.prepost + '_' + 'activation_processing'
+        codeobj_name = pathway.target.name +'_'+ self.owner.name + '_' + pathway.objname + '_' + 'activation_processing'
         # TODO: Check whether this kwd is actually required or not, for now I'll stay on the safe side
         kwds = {'pathway': pathway}
         # TODO: Figure out if it's better to use this function or 'create_runner_object()'
         device.code_object(
             owner= pathway.target,
             name = codeobj_name,
             abstract_code = abstract_code,
@@ -646,16 +693,16 @@
                 msg = f"""Learning rules requiring variables which are not strictly local to synapses is currently not supported.
                 Define all variables required for learning inside the Synapses object or as constants. The var {var.name} belongs to {var.owner}
                 and not to {self.owner}
                 """
                 raise ValueError(msg)
 
         # Generate the codeobject needed for synaptic transmission. It doesn't need any code as the functionality is included in the template.
-        prepost = 'pre' if 'pre' in self.name else 'post'
-        codeobj_name = f'{self.owner.name}_{prepost}_synapses_transmit'
+        objname = device._pathway.objname
+        codeobj_name = f'{self.owner.name}_{objname}_synapses_transmit'
         device.code_object(
             owner= self.owner,
             name = codeobj_name,
             abstract_code = {None: ''},
             variables = self.variables,
             template_name = 'synapses_transmit',
             variable_indices = self.variable_indices,
@@ -678,41 +725,60 @@
         # TODO Francesco: I'm wondering if this is the correct way to add the 'USES_VARIABLES' from templates
         # check: https://github.com/brian-team/brian2/blob/3cf65d4c5c8fa1512cf0a6deb515a8cdc81ae9e5/brian2/codegen/templates.py (186-217)
         # It seems that the templates themselves should take care of this. Further investigation is needed.
         constants = []
         for varname,var in self.variables.items():
             if isinstance(var, Constant):
                 constants.append(f'{varname} = {var.get_value()}')
-            elif isinstance(var, ArrayVariable) and var.constant and var.owner == self.owner:
+                                                                    # Owner should be same as generator, except for SynapticPathays
+            elif isinstance(var, ArrayVariable) and var.constant and (var.owner == self.owner or hasattr(self.owner,'synapses')):
                 # TODO This has to be handled differently. For the moment we just avoid adding these to the template constants.
-                if self.template_name == 'synapses_create_generator' and (varname == '_synaptic_pre' or varname == '_synaptic_post'):
+                if 'synapses' in self.template_name and (varname == '_synaptic_pre' or varname == '_synaptic_post'):
                     continue 
-                constants.append(f'{varname} = {self.get_array_name(var,template_name=self.template_name)}[0]')
+                constants.append(f'{varname} = {self.get_array_name(var,template_name=self.template_name)}')
             kwds['constants'] = constants
 
-        if 'synapses' in self.owner.name:
-            # This is only needed for the templates related to pathways
-            if self.template_name == 'synapses' or self.template_name == 'synapses_transmit':
-                # TODO: there might be a better way to access this value
-                prepost = 'pre' if 'pre' in self.name else 'post'
-                kwds['prepost'] = prepost
-                kwds['spiking_synapses'] = self.get_array_name(self.owner.variables[f"lava_spiking_synapses_{prepost}"])
+        # This is only needed for the templates related to pathways
+        if self.template_name == 'synapses' or self.template_name == 'synapses_transmit':
+            # TODO: there might be a better way to access this value
+            pathway = device._pathway
+            kwds['prepost'] = pathway.prepost
+            synapses_name = self.owner.name
+            kwds['spiking_synapses'] = self.get_array_name(self.owner.variables[f"spiking_{synapses_name}_{pathway.objname}"])
+        
+        # This could be incorporated above, but I want to make it clear that it's only used in this template
+        if self.template_name == 'synapses_transmit':
+            pathway = device._pathway
+            # TODO: This is a bit ugly, but since spike queues don't function properly if no delays are defined,
+            #  we have to define two different pipelines for each case.
+            # Add the spike queue variable name, used in synapses_transmit template if delays are defined
+            try:
+                spike_queue = device.spike_queues[f'{synapses_name}_{pathway.objname}_spike_queue']['name']
+                # We use this form because we want to keep the spiking_synapses variable to a fixed length otherwise lava will complain
+                kwds['read_spikes'] = f"np.isin(np.arange(len({self.get_array_name(pathway.synapse_sources)})),{spike_queue}.peek())"
+                kwds['advance_queue'] = spike_queue + '.advance()'
+            # Otherwise, we simply read from the spike ports.
+            except KeyError:
+                spiking_synapses = self.get_array_name(self.owner.variables[f'spiking_{self.owner.name}_{pathway.objname}'])
+                kwds['read_spikes'] = spiking_synapses
+                kwds['advance_queue'] = ''
+
 
         # Read the required synaptic variables which are to be sent to neurons
         # and send them out through the correct port.
         if self.template_name == 'synapses_transmit':  
             read_syn_vars = []
             syn_output_vars = []
             syn_output_ports = []          
             ports = device.lava_ports
             for port in ports.values():
-                if not port['pathway'].synapses == self.owner or not port['varname'] in list(self.variables.keys()) or port['pathway'].prepost not in self.name:
+                if not port['pathway'].synapses == self.owner or not port['varname'] in list(self.variables.keys()) or port['pathway'].objname not in self.name:
                     continue
                 varname = port['varname']
-                lava_name = device.get_array_name(self.owner.variables[varname])
+                lava_name = device.get_array_name(self.variables[varname])
                 # Not sure about this
                 _idx = self.variable_indices[varname]
                 read_syn_vars.append(f'{varname} = {lava_name}[{_idx}]')
                 syn_output_vars.append(varname)
                 syn_output_ports.append(port['portname'])
             kwds['read_syn_vars'] = read_syn_vars
             kwds['syn_output_vars'] = syn_output_vars
```

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templater.py` & `brian2lava-1.0.0a3/brian2lava/codegen/templater.py`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/activation_processing.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/activation_processing.py_`

 * *Files 13% similar despite different names*

```diff
@@ -8,20 +8,22 @@
     {{ c }}
     {% endfor%}
 
     # Collect all the incoming variables from the synapses
     # We could have multiple inputs depending on the synaptic model:
     # e.g. if we have v += w + g*I and both w and g are synaptic variables, but I is a neuronal variable.
     # This allows for more generalizable models. 
-    # TODO: handle the case in which no neuronal variable is on the right of the equation (i.e. just send the result of the operation).
+    # NOTE: In order to reduce the number of required ports one could calculate the result of the expression above
+    # and send only that part, but that requires making sure that the calculation can be handled by synapses alone 
+    # (i.e. no neuron vars on the right of the equation).
     {% for var in read_port_input %}
     {{var}}
     {% endfor %}
 
-    # We assume there is always one InPort in the NeuronGroup
+    # We assume there is always at least one InPort in the NeuronGroup
     # To check which indices to use we check for our "nan equivalent": {{nan}}
     _activation_indices = np.where({{neur_input_vars[0]}}!= {{nan}})[0]
 
     # scalar code
     _vectorisation_idx = 1
     {{scalar_code|autoindent}}
```

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/common_group.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/common_group.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_get.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_get_conditional.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_get_conditional.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_set.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/group_variable_set_conditional.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/group_variable_set_conditional.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/ratemonitor.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/ratemonitor.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/reset.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/reset.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/spatialstateupdate.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/spatialstateupdate.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/spikegenerator.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/spikegenerator.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/summed_variable.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/summed_variable.py_`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses.py_`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 
     # constants
     {% for c in constants %}
     {{ c }}
     {% endfor%}
 
     # Read which of the synapses have spiked in this timestep
-    _spiking_synapses = {{spiking_synapses}}.nonzero()[0]
+    _spiking_synapses = np.nonzero({{spiking_synapses}})[0]
 
     if len(_spiking_synapses):
         # scalar code
         {# Note that we don't write to scalar variables conditionally. The scalar code
             should therefore only include the calculation of scalar expressions
             that are used below for writing to a vector variable #}
         {{scalar_code|autoindent}}
 
         _idx = _spiking_synapses
 
         {{vector_code|autoindent}}
         
-    # Reset the spiking synapses
-    {{spiking_synapses}} = {{spiking_synapses}}*0
-
 {% endblock %}
```

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_array.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_create_array.py_`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 {#
 USES_VARIABLES { _synaptic_pre, _synaptic_post, sources, targets, N,
-                  N_pre, N_post, _source_offset, _target_offset }
+                  N_pre, N_post, _source_offset, _target_offset, N_incoming, N_outgoing }
 #}
 {# WRITES_TO_READ_ONLY_VARIABLES { _synaptic_pre, _synaptic_post, N}
 #}
 {# This is to show that we don't need to index the sources/targets #}
 {# ITERATE_ALL { _idx } #}
 {% extends 'common_group.py_' %}
 
 {% block maincode %}
-{# After this code has been executed, the arrays _real_sources and
+    # Constants
+    {% for c in constants %}
+    {{ c }}
+    {% endfor%}
+    {# After this code has been executed, the arrays _real_sources and
     _real_variables contain the final indices. Having any code here at all is
     only necessary for supporting subgroups #}
     {{vector_code|autoindent}}
 
     _old_num_synapses = {{N_init}}
     _new_num_synapses = _old_num_synapses + len({{sources_init}})
 
     # Resize all dependent dynamic arrays (synaptic weights, delays, etc.) and set
     # the total number of synapses
-    # TODO: when we implement a separate synapses process we could just use owner._resize() as shown below
     {% for var in owner._registered_variables %}
     {# We have to set the varnames manually instead of using filters because we need a special naming for this template #}
     {% set varname = get_array_name(var,access_data = False, template_name = 'synapses_create_array') %}
     {{varname}} = _numpy.resize({{varname}}, _new_num_synapses)
     {% endfor %}
 
     {{_dynamic__synaptic_pre_init}}[_old_num_synapses:] = _real_sources
     {{_dynamic__synaptic_post_init}}[_old_num_synapses:] = _real_targets
 
     {{N_init}} = _new_num_synapses
-    #_owner._resize(_new_num_synapses) #For now we keep this but should be deleted
 
-    # And update N_incoming, N_outgoing and synapse_number
-    #_owner._update_synapse_numbers(_old_num_synapses) #For now we keep this but should be deleted
+    # And update N_incoming, N_outgoing
+    post_with_offset = int(N_post) + _target_offset
+    pre_with_offset = int(N_pre) + _source_offset
+    N_incoming = _numpy.resize(N_incoming, post_with_offset)
+    N_outgoing = _numpy.resize(N_outgoing, pre_with_offset)
+
+    N_incoming[:] += _numpy.bincount({{_dynamic__synaptic_post_init}}[_old_num_synapses:], minlength=len(N_incoming))
+    N_outgoing[:] += _numpy.bincount({{_dynamic__synaptic_pre_init}}[_old_num_synapses:], minlength=len(N_outgoing))
+
+    # Save these numbers as attributes
+    {{get_array_name(variables['N_incoming'],template_name = 'synapses_create_array')}} = N_incoming
+    {{get_array_name(variables['N_outgoing'],template_name = 'synapses_create_array')}} = N_outgoing
+
+    # Last thing to update is synapse_number, but for now I'll skip this because it can be handled by calling
+    # synapses._update_synapse_numbers() directly after the simulation is done.
+
 {% endblock %}
```

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_create_generator.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_create_generator.py_`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
     {#
     USES_VARIABLES { _synaptic_pre, _synaptic_post, N,
-                    N_pre, N_post, _source_offset, _target_offset }
+                    N_pre, N_post, _source_offset, _target_offset, N_incoming, N_outgoing }
     #}
     {# WRITES_TO_READ_ONLY_VARIABLES { _synaptic_pre, _synaptic_post, N}
     #}
     {# ITERATE_ALL { _idx } #}
     {% extends 'common_group.py_' %}
 
     {% block maincode %}
@@ -197,25 +197,32 @@
         {{_dynamic__synaptic_post_init}} = _numpy.resize({{_dynamic__synaptic_post_init}},_new_num_synapses)
         {{_dynamic__synaptic_pre_init}}[_cur_num_synapses:] = _pre_idx
         {{_dynamic__synaptic_post_init}}[_cur_num_synapses:] = _post_idx
         _cur_num_synapses += _numnew
 
     # Resize all dependent dynamic arrays (synaptic weights, delays, etc.) and set
     # the total number of synapses
-
-    # Resize all dependent dynamic arrays (synaptic weights, delays, etc.) and set
-    # the total number of synapses
-    # TODO: when we implement a separate synapses process we could just use owner._resize() as shown below
     {% for var in owner._registered_variables %}
     {# We have to set the varnames manually instead of using filters because we need a special naming for this template #}
     {% set varname = get_array_name(var,access_data = False, template_name = 'synapses_create_generator') %}
     {{varname}} = _numpy.resize({{varname}}, _cur_num_synapses)
     {% endfor %}
 
     {{N_init}} = _numpy.array([_cur_num_synapses],dtype = 'int32')
-    # TODO to be deleted unless we implement the resize method.
-    #_owner._resize(_cur_num_synapses)
 
-    # And update N_incoming, N_outgoing and synapse_number
-    #_owner._update_synapse_numbers(_old_num_synapses)
+    # And update N_incoming, N_outgoing
+    post_with_offset = int(N_post) + _target_offset
+    pre_with_offset = int(N_pre) + _source_offset
+    N_incoming = _numpy.resize(N_incoming, post_with_offset)
+    N_outgoing = _numpy.resize(N_outgoing, pre_with_offset)
+
+    N_incoming[:] += _numpy.bincount({{_dynamic__synaptic_post_init}}[_old_num_synapses:], minlength=len(N_incoming))
+    N_outgoing[:] += _numpy.bincount({{_dynamic__synaptic_pre_init}}[_old_num_synapses:], minlength=len(N_outgoing))
+
+    # Save these numbers as attributes
+    {{get_array_name(variables['N_incoming'],template_name = 'synapses_create_array')}} = N_incoming
+    {{get_array_name(variables['N_outgoing'],template_name = 'synapses_create_array')}} = N_outgoing
+
+    # Last thing to update is synapse_number, but for now I'll skip this because it can be handled by calling
+    # synapses._update_synapse_numbers() directly after the simulation is done.
 
     {% endblock %}
```

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/synapses_transmit.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/synapses_transmit.py_`

 * *Files 26% similar despite different names*

```diff
@@ -4,24 +4,16 @@
 {% block maincode %}
 
     # constants
     {% for c in constants %}
     {{ c }}
     {% endfor%}
 
-    _spiking_indices = self.s_in_{{prepost}}.recv()
-
-    # Only look at the spiking neurons (assuming one-dimensional array shape)
-    _spiking_neurons = _numpy.nonzero(_spiking_indices)[0]
-    
-    {# From the point of view of the synaptic pathway the incoming signals are always from
-        the synapse_sources indices (sources and targets are switched for retrograde activations) #}
-    {% set _synapse_sources = get_array_name(pathway.synapse_sources) %}
-    # In case no synapse-related neuron is spiking we'll get an array of 'False'
-    _spiking_synapses = _numpy.array([x in _spiking_neurons for x in {{_synapse_sources}}])
+    # Read the spiking synapses received at this timestep
+    _spiking_synapses = {{read_spikes}}
 
     # scalar code
     {# Note that we don't write to scalar variables conditionally. The scalar code
     should therefore only include the calculation of scalar expressions
     that are used below for writing to a vector variable #}
     {{scalar_code|autoindent}}
 
@@ -30,21 +22,22 @@
     _vectorisation_idx = _idx
     
     # Read the synaptic variables to send out
     {% for read_var in read_syn_vars%}
     {{read_var}}
     {% endfor %}
 
-    # Send out the needed variables, non-stimulated synapses will be encoded by {{nan}}
+    # Send out the needed variables, non-stimulated synapses will be encoded by kwds['nan'] = {{nan}}
     # TODO This is not very elegant at the moment..
     {% for a_out,port in zip(syn_output_vars,syn_output_ports) %}
-    {{a_out}}_array = _numpy.ones({{_synapse_sources}}.shape, dtype = {{a_out}}.dtype) * {{nan}}
+    {{a_out}}_array = _numpy.ones({{get_array_name(pathway.synapse_sources)}}.shape, dtype = {{a_out}}.dtype) * {{nan}}
     {{a_out}}_array[_idx] = {{a_out}}
     self.{{port}}_out.send({{a_out}}_array)
     {% endfor %}
 
-    # Save the spiking synapses for the next learning phase
-    {{spiking_synapses}}= _idx
+    # Write the spiking synapses to an attribute in case we need it for learning
+    # This is required because in the next line we advance the spike queue!
+    {{spiking_synapses}} = np.array(_spiking_synapses)
 
-    # Advance the spike queue # Currently we don't support a spike queue
-    #_queue.advance()
+    # Advance the spike queue 
+    {{advance_queue}}
 {% endblock %}
```

### Comparing `brian2lava-1.0.0a2/brian2lava/codegen/templates/threshold.py_` & `brian2lava-1.0.0a3/brian2lava/codegen/templates/threshold.py_`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         _events, = _cond.nonzero()
 
     {#  Get the name of the array that stores these events (e.g. the spikespace array) #}
     {% set _eventspace = get_array_name(eventspace_variable) %}
     {{_eventspace}}[-1] = len(_events)
     {{_eventspace}}[:len(_events)] = _events
     # Check which neurons have spiked and send out the spikes
-    spikes = np.zeros(N)
+    spikes = _numpy.zeros(N)
     spikes[{{_eventspace}}[:len(_events)]] = 1
     self.{{owner.name}}_s_out.send(spikes)
 
     {% if _uses_refractory %}
     # Set the neuron to refractory
     {{not_refractory}}[_events] = False
     {{lastspike}}[_events] = {{t}}
```

### Comparing `brian2lava-1.0.0a2/brian2lava/device/__init__.py` & `brian2lava-1.0.0a3/brian2lava/device/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import jinja2
 import os
 import numpy as np
+from collections import defaultdict
 
 #from types import SimpleNamespace
 from weakref import WeakKeyDictionary
 
 # Import Brian2 modules
 from brian2.devices.device import all_devices, Device
 from brian2.utils.logger import get_logger
@@ -58,28 +59,31 @@
 
         # Define an empty set to store clocks
         self.clocks = set([])
 
         # Stores weak references from a `Variable` objects to the containing value(s)
         # Methods to handle the arrays are provided in `arrays.py`
         self.arrays = {}  # FIXME is was originally a WeakKeyDictionary()
+        self.array_cache = {}
+        self.proc_init_queue = defaultdict(list) # In CPP device 'main_queue' a list, but we need a queue for each process
+        self.proc_model_add_code = defaultdict(set) # Additional code for process models. Defaults to set to avoid duplicates, ordering shouldn't matter.
 
         # Define empty dicts to store code objects and abstract code
         self.code_objects = {}
 
         # Brian network objects
         self.net_objects = set()
 
         # Store Lava variables
         # Key: variable name, Value: variable definition (e.g. 'np.empty(...)')
-        self.N = None
         self.lava_variables = {}
         self.lava_variable_names = {}
         
         # Store the ports required to connect processes
+        self.spike_queues = {}
         self.lava_ports = {}
 
         # Brian template functions that belong to the process,
         # instead of the process model, e.g. 'group_variable_set'
         self.init_template_functions = [
             'group_variable_set',
             'group_variable_set_conditional',
@@ -116,17 +120,14 @@
         self.lava_variables_to_monitor = []
         self.lava_monitors = {}
         # Add monitors for additional variables (only for SpikeMonitors)
         self.additional_monitors = {}
         #self.brian_monitors = {}
 
         self.monitor_types = {'state': 0, 'spike': 1}  # SimpleNamespace(**{ 'state': 0, 'spike': 1 })
-        
-        # Init a variable to store the Lava process
-        self.process = None
 
         # Stores if the network did run
         self.did_run = False  # FIXME necessary?: Yes? since otherwise the user
         # can use multiple run calls but if he does it the objects and network
         # might have changed but the compiled code for lava is still the old
         # one. He needs to do a device.reini(), device.activat() to reinit the
         # whole build process again. WIth this flag here we chan check this.
@@ -147,15 +148,16 @@
         activate, seed, reinit
     )
 
     # Build the network
     from .build import (
         build, render_templates, get_compiled_code, get_jinja_environment,
         get_lava_proc_variables, get_lava_proc_model_variables,
-        get_lava_function_calls, get_lava_ports_definitions
+        get_lava_function_calls, get_lava_ports_definitions, generate_init_queue,
+        generate_additional_code, get_proc_model_init_code, get_lrn_guard_code
     )
 
     # Writer for writing rendered templates
     from .writer import (
         prepare_directory, write_templates
     )
```

### Comparing `brian2lava-1.0.0a2/brian2lava/device/arrays.py` & `brian2lava-1.0.0a3/brian2lava/device/arrays.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,23 @@
     `any`
         Values of the array variable as list
     """
 
     # Log that a value was requested from arrays
     self.logger.diagnostic(f'get_value {var.name}')
 
-    return self.arrays[var]
+    # The variable should be stored in self.arrays, if it's None then the device hasn't been run yet.
+    if self.arrays.get(var, None) is not None:
+        return self.arrays[var]
+    
+    raise NotImplementedError(
+                "Cannot retrieve the values of state "
+                "variables in standalone code before the "
+                "simulation has been run."
+            )
 
 def get_dtype_name(var):
     """
     Get the data type of a variable and return its name as a string - serves to avoid expressions like 'np.bool' that are deprecated since NumPy 1.24.
     In the case of a NumPy data type, returns the name with the prefix 'np.'.
 
     Parameters
@@ -56,15 +64,14 @@
 
     # Check if Python or NumPy data type is used
     if dtype in [bool, int, float, complex, str, np.int32, np.int64, np.float32, np.float64]:
         ret = dtype.name.replace('32', '').replace('64', '')
     else:
         ret = "np." + dtype.name
 
-    #print(f'get_dtype_name({var}) = {ret}')
     return ret
 
 
 def get_lava_var_name(self, var):
     """
     Get a lava variable name based on an array variable.
 
@@ -91,15 +98,15 @@
         lava_var_name = ''
         if var.name == 't': lava_var_name = '_defaultclock_t'
         if var.name == 'i': lava_var_name = var.owner.source.name +'_s_out'
         # Manage the case of additional variables in the SpikeMonitor
         else: lava_var_name = f'_{var.owner.source.name}_{var.name}'
         return lava_var_name
     else:
-        return f'_{var.owner.name}_{var.name}'
+        return self.get_array_name(var,prefix=None)
 
 
 def get_array_name(self, var, access_data=True, prefix='self.'):
     """
     Gets the name of an array variable.
 
     Parameters
@@ -199,25 +206,31 @@
         #      Constant values like N or __indices are currently ignored
         if isinstance(var, DynamicArrayVariable):
             if isinstance(var.owner.record,bool):
                 # we only add a monitor if the record flag is not set to False, which means that the
                 # monitor is not used for recording.
                 if var.owner.record == False:
                     if isinstance(var.owner,SpikeMonitor):
-                        self.logger.warn("Currently, setting 'record=False' in the SpikeMonitor is not supported. It will be in future releases")
+                        self.logger.warn("Currently, setting 'record=False' in the SpikeMonitor is being ignored. It will be implemented in future releases")
                     else:
                         return   
             else:
+                msg = """[EFFICIENCY]: Setting recording indices is currently not supported by Lava. 
+                        The monitor will record all indices, which will then be filtered by brian2lava at a 
+                        later stage (so that the output will be compatible with what expected from Brian). 
+                        For this reason, the current implementation will be significantly slower than the 
+                        Brian implementation for larger simulations."""
                 # Check if the user is trying to record specific indices
-                if len(var.owner.record) != len(var.owner.source) and var.name != 't':
-                    self.logger.warn("""[EFFICIENCY]: Setting recording indices is currently not supported by Lava. 
-                    The monitor will record all indices, which will then be filtered by brian2lava at a 
-                    later stage (so that the output will be compatible with what expected from Brian). 
-                    For this reason, the current implementation will be significantly slower than the 
-                    Brian implementation for larger simulations.""")
+                try:
+                    if len(var.owner.record) != len(var.owner.source) and var.name != 't':
+                        self.logger.warn(msg)
+                # This error is raised in case len(source) is not defined yet (we need to run the simulation first), 
+                # in this case the warning still applies, though.
+                except NotImplementedError:
+                    self.logger.warn(msg)
 
             # Get monitor type name from owner ('state' or 'spike')
             monitor_type_name = get_monitor_type_name(var.owner)
 
             # We don't need a monitor for spike timings since this measurement is 
             # handled differently.
             if var.name == 't' and monitor_type_name == 'spike':
@@ -273,20 +286,22 @@
                 'lava_monitor': None,  # The Lava monitor, instance is added later during 'run'
                 'process_name': None # The name of the process that is monitored, will be set in 'run'
             }
     else:
         
         dtype_name = get_dtype_name(arr)
         type_name = dtype_name
+
         # Add the definition of a numpy array as string for lava
-        var_definition = f'np.empty({var.size}, dtype={type_name})'
+        # By default we initialize to zero, as it's generally a safe value.
+        var_definition = f'np.zeros({var.size}, dtype={type_name})'
 
         # TODO is the key unique?
         # See also: https://github.com/brian-team/brian2/pull/304
-        name = f'_{var.owner.name}_{var.name}'
+        name = self.get_array_name(var,prefix=None)
         self.lava_variables[name] = {
             'name': var.name,
             'owner': var.owner.name,
             'definition': var_definition,
             'size': var.size,
             'shape': np.shape(arr),
             'type': type_name,
@@ -307,18 +322,18 @@
     var : `ArrayVariable`
         The array variable to initialize with zeros
     dtype : `dtype`
         The data type to use for the array
     """
 
     # Redefine variable definition for Lava variables
-    name = f'_{var.owner.name}_{var.name}'
+    name = self.get_array_name(var,prefix=None)
     if name in self.lava_variables.keys():
         lv = self.lava_variables[name]
-        lv['definition'] = f'np.zeros({lv["size"]}, dtype={lv["dtype"]})'
+        lv['definition'] = f"np.zeros({lv['size']}, dtype={lv['dtype']})"
     
     # Log that an empty array was initialized
     self.logger.diagnostic(f'init_with_zeros {var.name}')
     
     self.arrays[var][:] = 0
 
 
@@ -334,78 +349,92 @@
     start : `int`
         Start value of the range
     dtype : `dtype`
         The data type to use for the array
     """
 
     # Redefine variable definition for Lava variables
-    name = f'_{var.owner.name}_{var.name}'
+    name = self.get_array_name(var,prefix=None)
     if name in self.lava_variables.keys():
         lv = self.lava_variables[name]
-        lv['definition'] = f'np.arange({start}, {lv["size"]+start}, dtype={lv["dtype"]})'
+        lv['definition'] = f"np.arange({start}, {lv['size']+start}, dtype={lv['dtype']})"
     
     # Log that an array was created based on numpy arange
     self.logger.diagnostic(f'init_with_arange, arange from {start} to {var.get_len()+start}')
     
     self.arrays[var][:] = np.arange(start, stop=var.get_len()+start, dtype=dtype)
 
 
 def fill_with_array(self, var, arr):
     """
-    Fill array vatiable `var` with the values given in an array `arr` and add it to the `arrays` list.
+    Fill array variable `var` with the values given in an array `arr` and add it to the `arrays` list.
+    Instead of modifying the definition of the variable itself, we add a line of code to the init queue
+    which will be executed at initialization of the process. This allows the user to modify variables
+    seamlessly any number of times without incurring into bugs.
+    The methodology we use is compatible with the one used in the CPPStandaloneDevice:
+    https://github.com/brian-team/brian2/blob/master/brian2/devices/cpp_standalone/device.py#L415
     
     Parameters
     ----------
     var : `ArrayVariable`
         The array variable to fill
     arr : `ndarray`
         The array values that should be copied to `var`
     """
 
     arr = np.asarray(arr)
     # Redefine variable definition for Lava variables
-    name = f'_{var.owner.name}_{var.name}'
+    name = self.get_array_name(var,prefix=None)
     if name in self.lava_variables.keys():
         lv = self.lava_variables[name]
 
         # Check if 'arr' is given as scalar
         is_scalar = not bool(len(np.shape(arr)))
         
-        # If 'arr' is scalar and size is 1, add a simple array
+        # If 'arr' is scalar and size is 1, we set the whole var to that value
+        # This accounts for variables initially initialized to [0.] but which will be resized later on.
+        # FIXME: the 'size' key could cause other bugs in the future, so it needs to be addressed!
         if is_scalar and lv['size'] == 1:
-            lv['definition'] = f'np.array([{arr}], dtype={lv["dtype"]})'
+            self.proc_init_queue[var.owner.name].append(('set_by_single_value', (name,':',arr.item())))
         # If 'arr' is scalar and size > 1, add an array that repeats the value accordingly
         elif is_scalar and lv['size'] > 1:
-            lv['definition'] = f'np.array(np.repeat({arr}, {lv["size"]}), dtype={lv["dtype"]})'
+            self.proc_init_queue[var.owner.name].append(
+                (
+                'set_by_constant', (name,arr.item())
+                )
+            )
         # If 'arr' is actually an array, it's just transformed to a string definition
         else:
+            if not lv['size'] == arr.shape[0]:
+                raise ValueError(f"The array used to set variable {name} is not of the same size as the variable. {lv['size']}!={arr.shape[0]}")
             arr_str = np.array2string(np.array(arr), separator=', ')
-            lv['definition'] = f'np.array({arr_str}, dtype={lv["dtype"]})'
+            self.proc_init_queue[var.owner.name].append(
+                ('set_by_array', (name,arr_str))
+            )
 
     # Log that an array was filled with given values
     self.logger.diagnostic(f'fill_with_array, add {arr} to {var.name}')
     
     # Set array value
-    self.arrays[var][:] = arr
+    if isinstance(var, DynamicArrayVariable):
+        # Following CPPStandalone example, we can't correctly know the 
+        # value of a dynamic array, so for now we don't save it at all
+        self.arrays[var] = None
+    else:
+        self.arrays[var][:] = arr
 
 def resize(self, var, new_size):
     """
     Method called most times a DynamicArray variable is created. Updates the size of a DynamicArray.
+    We add this operation to the initialization queue for the lava processes in order to keep the ordering consistent.
     """
-    # First resize it in our array-cache
-    # We use this form due to an error when trying to resize an array which is referenced by another array.
-    self.arrays[var] = np.resize(self.arrays[var], new_size)
-
-    # Change the size of the variable in our variable dictionary
-    # We also make sure to update the default definition in case the variable
-    # is not initialized with a 'fill_with' method afterwards (in most cases it is).
-    # This is probably redundant but ensures no bugs come up later on.
-    name = f'_{var.owner.name}_{var.name}'
+    # This is an operation we can still manage with the array cache (useful for synaptic numbers such as N_incoming and N_outgoing)
+    if self.arrays.get(var,None) is not None:
+        self.arrays[var] = np.resize(self.arrays[var], new_size)
+    # Change the size of the variable in our init_queue
+    name = self.get_array_name(var,prefix=None)
     if name in self.lava_variables.keys():
-        lv = self.lava_variables[name]
-        lv["size"] = new_size
-        if 'np.empty' in lv["definition"]:
-            lv["definition"] = f'np.empty({lv["size"]}, dtype={lv["dtype"]})'
+        self.proc_init_queue[var.owner.name].append(('resize_array', (name,new_size)))
```

### Comparing `brian2lava-1.0.0a2/brian2lava/device/build.py` & `brian2lava-1.0.0a3/brian2lava/device/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -128,38 +128,53 @@
     self.logger.diagnostic(s)
 
     s = "Extracted process model methods:\n"
     for item in process_model_methods:
         s += f'{item}\n'
     self.logger.diagnostic(s)
 
-    # Get a list of ordered function calls to be implemented in
-    # the 'run' and '__init__' function
-    # TODO rename to 'process' and 'process_model' functions
-    lava_init_function_calls, lava_run_function_calls, learning_function_calls = self.get_lava_function_calls(obj)
+    # PROCESS-RELATED CODE ----------------------------------
+
+    # Generate the code required by the init queue
+    lava_init_function_calls = self.generate_init_queue(obj)
 
     # Get the port definitions for process and process model
     proc_ports, proc_model_ports = self.get_lava_ports_definitions(obj)
     
     # Get formatted variables for lava process
-    proc_variables_init, proc_variables_lava = self.get_lava_proc_variables(obj, lava_init_function_calls)
+    proc_variables_init, proc_variables_lava = self.get_lava_proc_variables(obj)
     
     # Log extracted lava process variables
     s = "Extracted lava process variables:\n"
     for item in proc_variables_lava:
         s += f'{item}\n'
     self.logger.diagnostic(s)
     
+    # PROCESS MODEL-RELATED CODE ---------------------------
+
     # Get formatted variables for lava process **model**
     lava_proc_model_variables = self.get_lava_proc_model_variables(obj)
     
     # Add the port initializations:
     proc_variables_lava = proc_ports + proc_variables_lava
     lava_proc_model_variables = proc_model_ports + lava_proc_model_variables
 
+    # Get a list of ordered function calls to be implemented in
+    # the 'run_spk' and 'run_lrn' methods.
+    lava_run_function_calls, learning_function_calls = self.get_lava_function_calls(obj)
+
+    # If any additional code for process models was defined, add it 
+    additional_code = self.generate_additional_code(obj)
+
+    # If some variables are exclusive to process model and they need initialization:
+    proc_model_initialization_code = self.get_proc_model_init_code(obj)
+
+    # If learning is enabled, define the learning guard function
+    lrn_guard_code = self.get_lrn_guard_code(obj)
+
     # Log extracted lava process variables
     s = "Extracted lava process model variables:\n"
     for item in lava_proc_model_variables:
         s += f'{item}\n'
     self.logger.diagnostic(s)
     
     # Get jinja environment
@@ -175,18 +190,21 @@
         required_imports=collect_required_imports(process_methods),
         name = obj.name
     )
     
     # Load and render 'process model'
     process_model_template = env.get_template('process_model.py.j2')
     process_model_rendered = process_model_template.render(
+        additional_code = additional_code,
+        proc_model_initialization_code = proc_model_initialization_code,
         methods=process_model_methods,
         run_functions=lava_run_function_calls,
         lrn_functions = learning_function_calls,
         variables=lava_proc_model_variables,
+        lrn_guard_code = lrn_guard_code,
         required_imports=collect_required_imports(process_model_methods),
         name = obj.name
     )
     
     return process_rendered, process_model_rendered
 
 
@@ -232,18 +250,22 @@
     process_model_methods : `string[]`
         Process methods to include into the `process model`
     """
     
     # Define variables to collect lava code
     process_methods = ''
     process_model_methods = ''
-        
+    
+    # We don't want to only consider this 'obj' but also all of its contained objects
+    # For example, if delays are defined with an expression, this codeobject is not directly owned by the Synapses.
+    objects = [o for o in obj.contained_objects]
+    objects.append(obj)
     # Iterate over code objects
     for code_object in self.code_objects.values():
-        if code_object.owner.name == obj.name:
+        if code_object.owner in objects:
             lava_code_tmp = None
             for block in ['before_run','run','after_run']:
                 # Get compiled code for specific code object and block
                 lava_code_tmp = code_object.compiled_code[block]
                 
                 # Add the code collected from the code objects to either
                 # the Lava process or the Lava process model
@@ -252,23 +274,23 @@
                         process_methods += lava_code_tmp + '\n\n'
                     else:
                         process_model_methods += lava_code_tmp + '\n\n'
 
     return process_methods.splitlines(), process_model_methods.splitlines()
 
 
-def collect_required_imports(abstract_code):
+def collect_required_imports(code):
     """
     Search for functions in abstract code that require an import (e.g. random function)
     and return these imports as array.
     
     Parameters
     ----------
-    abstract_code : 'string''
-        The whole abstract code as string
+    code : 'string''
+        The whole genrated code as string
     
     Returns
     -------
     required_imports : `string[]`
         Array of strings that contain required imports
     """
     
@@ -301,22 +323,23 @@
         'arccos': 'from numpy import arccos',
         'arctan': 'from numpy import arctan',
         'clip': 'from numpy import clip'   
     }
     
     # Create empty array to collect required imports
     required_imports = []
-    # Check if relevant function is in abstract code and if yes, add import
+    # Check if relevant function is in the code and if yes, add import
     for func, imp in potential_imports.items():
-        for line in abstract_code:
+        for line in code:
             if f'{func}(' in line:
                 required_imports.append(imp)
                 # avoid multiple imports of the same function
                 break
     
+    
     return required_imports     
 
 def get_lava_ports_definitions(self, obj):
     """
     TODO
 
     Parameters
@@ -343,23 +366,30 @@
         proc_model_ports.append(f"{spike_port}: PyOutPort = LavaPyType(PyOutPort.VEC_DENSE, bool, precision=1)")
         for var in self.lava_ports.values():
             if not obj.name == var['receiver']:
                 continue
             portname = var['portname']
             proc_ports.append(f"self.{portname}_in = InPort(shape=(0,))",)
             port_type = 'float' if not 'idx' in portname else 'int,precision = 1'
-            proc_model_ports.append(f"{portname}_in: PyInPort = LavaPyType(PyInPort.VEC_DENSE, {port_type})")   
+            proc_model_ports.append(f"{portname}_in: PyInPort = LavaPyType(PyInPort.VEC_DENSE, {port_type})")  
             
     elif isinstance(obj,Synapses):
         # First receive the incoming spikes from the neurons
         for pathway in obj._pathways:
-            # Note that in this case the port doesn't need the obj.name prefix since we don't read values from it!
+            # Even though we can have more than 2 pathways, source and target are only 2, so at best
+            # we'll have one spiking port for presynaptic neurons and one for postsynaptic ones.
+            # Since the ports are a set, having duplicates here is not a problem.
             prepost = pathway.prepost
+            objname = pathway.objname
             proc_ports.append(f'self.s_in_{prepost} = InPort(shape=(0,))')
             proc_model_ports.append(f"s_in_{prepost}: PyInPort = LavaPyType(PyInPort.VEC_DENSE, bool, precision=1)")
+
+            # Add the receiving mechanism to the process model
+            self.proc_model_add_code[obj.name].add(('spike_port',(prepost)))
+
         # Then make ports for synaptic transmission to neurons
         for var in self.lava_ports.values():
             for pathway in obj._pathways:
                 if not var['pathway'] == pathway:
                     continue
                 portname = var['portname']
                 shape_var = self.get_array_name(obj.variables['_synaptic_pre'], prefix = 'self.init')
@@ -375,15 +405,15 @@
     proc_model_ports = list(set(proc_model_ports))
     if len(proc_model_ports):
         proc_model_ports[-1] += '\n'
 
     return proc_ports, proc_model_ports
 
 
-def get_lava_proc_variables(self, obj, lava_init_function_calls):
+def get_lava_proc_variables(self, obj):
     """
     Takes variable name/value pairs and generates a list of variables
     for the lava process
 
     Parameters
     ----------
     obj : lava_object
@@ -405,32 +435,23 @@
     formatted_variables_lava = []
 
     for name, var in self.lava_variables.items():
         if not var['owner'] == obj.name and not var['owner'] == obj.clock.name:
             continue
         elif var['owner'] == obj.name:
             init_var_name = f'self.init{name}'
-            numpy_definition = var["definition"]
+            numpy_definition = var['definition']
 
             # Statement for the definition of an array variable in Lava
             formatted_variables_init.append(f'{init_var_name} = {numpy_definition}')
             
             # Check if Brian provides us with an init function for the variable,
             # that contains instructions to set user-defined initial values
-            init_func = None
-            if name in lava_init_function_calls:
-                init_func = lava_init_function_calls[name]
-                exp = f'Var(shape={var["shape"]}, init={init_func})'
-            # Otherwise init with init variable that contains a plain numpy definition
-            else:
-                # Here I look at the shape of the init variable instead, it's useful if at the beginning
-                # the shape is set to (0,) in brian due to the fact that they will resize this array.
-                # This is because the lava shape of a variable doesn't get update according to the shape of its
-                # init value.
-                exp = f'Var(shape={init_var_name}.shape, init={init_var_name})'
+            exp = f'Var(shape={init_var_name}.shape, init={init_var_name})'
+
         # NOTE: implementing multiple clocks will require checking on each obj.clock.name
         elif var['owner'] == obj.clock.name:
             dt = obj.clock.dt_
             exp = f'Var(shape= (1,), init = np.array([{dt}]))'
         
         # Statement for the definition of an array variable in Lava
         formatted_variables_lava.append(f'self.{name} = {exp}')
@@ -456,24 +477,21 @@
     # Init variable to store formatted variables for a Lava process model
     formatted_variables = []
     
     # Then the variables themselves
     for name, var in self.lava_variables.items():
         if var['owner'] == obj.name or var['owner'] == obj.clock.name:
             # Check if array or not
-            value_type_arr = 'np.ndarray' if var["size"] > 1 else var["type"]
+            value_type_arr = 'np.ndarray' if var['size'] > 1 else var['type']
 
             # Format the expression to what a Lava process expects
             exp = f'LavaPyType({value_type_arr}, {var["type"]})'
 
             # Statement for the definition of an array variable in Lava
             formatted_variables.append(f'{name}: {value_type_arr} = {exp}')
-
-            # Statement for the definition of an actual variable
-            #formatted_variables.append(f'{var["name"]}: {value_type_arr} = {exp}')
         
     return formatted_variables
 
 
 def get_lava_function_calls(self, obj):
     """
     Given the code objects we return an ordered list of function calls that should
@@ -488,70 +506,171 @@
     -------
     init_calls : `string[]`
         A list of code that describes methods for the `process`
     run_calls : `string[]`
         A list of code that describes methods for the `process model`
     """
     run_calls = []
-    init_calls = []
     lrn_calls = []
 
     # Collect code objects for process
-    code_objects = [c_o for c_o in list(self.code_objects.values()) if c_o.owner.name == obj.name]
-
+    code_objects = [c_o for c_o in list(self.code_objects.values()) if c_o.owner == obj]
     # Iterate over all code blocks and code objects
     # NOTE: The after_run code blocks are not really used at any point yet. 
     # FIXME: I take them out for now, because their behavior should be implemented differently!
     for block in ['_before_run()', '_run()']:
         for code_obj in code_objects:
             # If the codeobject is not empty, assign function names to related lists
             if code_obj.compiled_code[block[1:-2]] is not None:
                 function_name = f'self.{code_obj.name}{block}'
-                # These functions are added to the lava process and initialize variables
+                # These are handled later on by the init queue
                 if code_obj.template_name in self.init_template_functions:
-                    init_calls.append(function_name)
+                    continue
                 elif code_obj.template_name == 'synapses':
                     lrn_calls.append(function_name)
                 # These functions handle the simulation and are part of the lava process model
                 else:
                     run_calls.append(function_name)
     run_calls = schedule_sort(run_calls, obj)
 
-    # # Postprocess init calls
-    # for key, values in init_calls_lists.items():
-    #     # If we have only one init function for the variable, just take it
-    #     if len(values) == 1:
-    #         init_calls[key] = values[0]
-    #     # If we have two or more init functions for the variable,
-    #     # we need to construct a lambda function that calls all init functions
-    #     else:
-    #         # Starting string definition for lambda function that calls all functions
-    #         st = '(lambda: ['
-    #         suffix = '])()[-1]'
-    #         # Iteratively add all function calls as string
-    #         for i, v in enumerate(values):
-    #             st += f'{v}'
-    #             if (i+1) < len(values):
-    #                 st += ', '
-    #         # Add suffix and add to init calls
-    #         st += suffix
-    #         init_calls[key] = st
-
-    # If in any of our code objects there's a time variable (probably always)
-    # Add a line to update at each time step
+    # Add a line to update the time variables at each time step
     obj_varnames = obj.variables.keys()
     if 't' in obj_varnames:
         # TODO: this has to be made more generalizable to multiple clocks
         run_calls.append('self._defaultclock_t += self._defaultclock_dt')
-    if 't_in_timesteps':
+    if 't_in_timesteps' in obj_varnames:
         run_calls.append('self._defaultclock_timestep += 1')
     
 
-    return init_calls, run_calls, lrn_calls
+    return run_calls, lrn_calls
+
+def generate_init_queue(self,obj):
+    init_queue_lines = []
+    # Also go through the objects contained in the main BrianObject (e.g. Thresholder, Resetter and Stateupdater for NeuronGroup)
+    obj_list = [contained_obj for contained_obj in obj.contained_objects]
+    # Obviously take the main object into consideration
+    obj_list.append(obj)
+
+    # We assume that init queue lines for different objects are independent of each other so the order doesn't matter
+    for _obj in obj_list:
+        for func, args in self.proc_init_queue[_obj.name]:
+            if func == 'code_object':
+                codeobj = args
+                if not codeobj.template_name in self.init_template_functions:
+                    raise ValueError(f"Wrong object in init queue: {codeobj.template_name}")
+                init_queue_lines.append(f"self.{codeobj.name}_run()")
+            elif func == 'set_by_single_value':
+                array_name, item, value = args
+                init_queue_lines.append(f"self.init{array_name}[{item}] = {value}")
+            elif func == 'set_by_constant':
+                array_name, value = args
+                init_queue_lines.append(f"self.init{array_name}[:] = {value}")
+            elif func == 'set_by_array':
+                array_name, input_array = args
+                init_queue_lines.append(f"self.init{array_name}[:] = {input_array}")
+            elif func == 'resize_array':
+                array_name,new_size = args
+                init_queue_lines.append(f"self.init{array_name}.resize({new_size})")
+            elif func == 'set_array_by_array':
+                # TODO: Make sure this is correct!
+                array_name, indices, value = args
+                init_queue_lines.append(f"self.init{array_name}[{indices}] = {value}")
+
+    return init_queue_lines
+
+def generate_additional_code(self,obj):
+    """
+    Additional lines of code that might be required for the correct functioning of process models.
+    Potentially, even the user could define some code to add here, but this is not supported yet.
+
+    """
+    add_code_lines = []
+    
+    # As for the init queue, consider any possible contained object (this is most likely not necessary but keep for consistency)
+    obj_list = [contained_obj for contained_obj in obj.contained_objects]
+    obj_list.append(obj)
+
+    for _obj in obj_list:
+        for func,args in self.proc_model_add_code[_obj.name]:
+            # Read spikes at each timestep from the pre and post pathways
+            if func == 'spike_port':
+                prepost = args
+                # This line is added whether or not a spike queue is present
+                add_code_lines.append(f"_spiking_neurons = np.nonzero(self.s_in_{prepost}.recv())[0]")
+                spike_queue_owners = [queue['owner'] for queue in self.spike_queues.values()]
+                for pathway in obj._pathways:
+                    # Process all the pathways with the same 'prepost' in one go.
+                    if pathway.prepost == prepost:
+                        pathway_name = pathway.objname
+                        # Here we read the name of the spike queue from the parent object and the pathway
+                        spike_queue = f'{obj.name}_{pathway_name}_spike_queue'
+                        # If such a spike queue exists, then we push the spikes to it
+                        if spike_queue in self.spike_queues.keys():
+                            spike_queue_var = self.spike_queues[spike_queue]['name']
+                            add_code_lines.append(f"{spike_queue_var}.push(_spiking_neurons)")
+                        # If the pathway doesn't require a spike queue we just read from spike ports
+                        else:
+                            # TODO: Ideally in future implementations we use get_array_name() for both of these variables..
+                            spiking_synapses_var = self.get_array_name(pathway.synapses.variables[f'spiking_{obj.name}_{pathway_name}'])
+                            synaptic_pre = self.get_array_name(pathway.synapse_sources)
+                            add_code_lines.append(f"{spiking_synapses_var} = [x in _spiking_neurons for x in {synaptic_pre}]")
+
+            # Just to take into account this possibility, even though it is not yet implemented:
+            elif func == 'user_code':
+                add_code_lines.append([line for line in args])
+    
+    return add_code_lines
+
+def get_proc_model_init_code(self,obj):
+    """
+    Potential code to be injected at the beginning of the run_spk function. Used for the initialization of the SpikeQueue.
+    We do it here and not in the __init__ method because we want to use variable names and not manually write the delays array to 
+    a string. If this is too inefficient it can always be changed later on.
+    """
+
+    lines = []
+    # At the moment this is only used for synapses (spike queue)
+    if not isinstance(obj, Synapses):
+        return []
+    for name,queue in self.spike_queues.items():
+        # If this queue doesn't belong to this object, skip it
+        if not obj == queue['owner']:
+            continue
+
+        lines.append(f"{queue['name']} = SpikeQueue({queue['start']},{queue['stop']})")
+        lines.append(f"{queue['name']}.prepare({queue['delays']},{queue['dt']},{queue['sources']})")
+    
+    return lines
+
+def get_lrn_guard_code(self,obj):
+    """
+    Get the definition of the learning phase guard function. This function should return a bool
+    indicating whether or not the learning phase should take place during this timestep or not.
+
+    We obtain this by checking if any spike was received by the spiking ports.
+    """
+    if not isinstance(obj,Synapses):
+        return ""
+    
+    lines = []
+    # A trick to optimize writing the required code
+    return_stmt = "return False "
+    spike_ports = set()
+    for pathway in obj._pathways:
+        spike_ports.add(pathway.prepost)
+    
+
+    for prepost in spike_ports:
+        spiking_synapses_var = self.get_array_name(obj.variables[f"spiking_{obj.name}_{prepost}"])
+        lines.append(f"spiking_{prepost} = len(np.nonzero({spiking_synapses_var})[0]) > 0")
+        return_stmt += f"+ spiking_{prepost}"
+    lines.append(return_stmt)
+
 
+    return lines
 
 def schedule_sort(func_list, obj):
     """
     TODO
 
     Parameters
     ----------
@@ -584,22 +703,34 @@
         
         #If the function doesn't correspond to the contained objects then it must be
         # the activation_processing code object, which doesn't have a corresponding CodeRunner object.
         # NOTE: This might be changed in future updates
         if not len(code_runner):
             # We want to receive the activations and update the neuron at the start of the timestep.
             # NOTE: The various run_ functions from lava might prove useful here in the future.
-            assert 'activation_processing' in func_call
+            assert 'activation_processing' in func_call # or 'synapses_transmit' in func_call
             schedule['synapses'].insert(0, func_call)
             continue
 
         if not len(code_runner) == 1:
             raise ValueError(f"""More than one CodeRunner corresponding to the same code_object. 
             Try restarting the simulation. If the bug persists please report it to us.
             CodeRunners: {code_runner}""")
         code_runner = code_runner[0]
-        schedule[code_runner.when].insert(code_runner.order,func_call)
+    
+        try:
+            schedule[code_runner.when].insert(code_runner.order,func_call)
+        # If the keywords 'before' or 'after' are used, we put them at the beginning or end of the 
+        # corresponding schedule.
+        except KeyError:
+            if 'before' in code_runner.when:
+                when = code_runner.when.replace("before_","")
+                schedule[when].insert(0,func_call)
+            elif 'after' in code_runner.when:
+                when = code_runner.when.replace("after_", "")
+                schedule[when].append(func_call)
+
     ordered_list = []
     for when in schedule:
         ordered_list = list(chain(ordered_list, schedule[when]))
 
     return ordered_list
```

### Comparing `brian2lava-1.0.0a2/brian2lava/device/run.py` & `brian2lava-1.0.0a3/brian2lava/device/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,34 +23,33 @@
         profile=False,
         level=0,
         **kwds
     ):
     """
     Performs preparations and checks and finally calls the `build` method from the device.
 
-    Parameters
-    ----------
-    TODO
-
     Notes
     -----
-    This is called very early in the process and overwrites the `run()` method from `brian2.core.Network.run()`.
+    Overwrites the `run()` method from `brian2.core.Network.run()` so for reference, see:
+    https://brian2.readthedocs.io/en/stable/reference/brian2.core.network.Network.html#brian2.core.network.Network.run
+
+    Note that in the current implementation, the following arguments are not supported and will thus be ignored or raise an error:
+        - report -> ignored
+        - report_period -> ignored
+        - profile -> error
     """
     # Before doing anything check that the objects used by the user 
     # are supported by lava.
     check_for_brian2lava_support(net)
     
     # Store duration in device
     self.duration = duration
     
     # Log that the network run method was called
     self.logger.diagnostic("Network run is executing.")
-
-    # Add the network from the current run call to the set of networks within this device
-    #self.networks.add(net)
     
     # If keyword arguments are given, notify the user that these arguments are not used in Brian2Lava
     if kwds:
         self.logger.warn(
             'Unsupported keyword argument(s) provided for run: {}'.format(', '.join(kwds.keys()))
         )
         
@@ -60,59 +59,76 @@
     
     # FIXME Set clocks
     net._clocks = {obj.clock for obj in net.sorted_objects}
     t_end = net.t+duration
     for clock in net._clocks:
         clock.set_interval(net.t, t_end)
     
+    # Manage Spike Queues. TODO: Move this in a better place if possible
+    # For now I put it here because I want this to happen as soon as possible during the
+    # run call. (But still after any variable definition has been made (e.g. setting delays.))
+    for obj in net.sorted_objects:
+        if isinstance(obj,Synapses):
+            for pathway in obj._pathways:
+                # The spike queue is only added if delays are defined.
+                has_spike_queue = False
+                try:
+                    if len(pathway._delays.get_value()):
+                        has_spike_queue = True
+                # The device will raise this error if the delay variable was modified 
+                # and requires to be manipulated during runtime (e.g. S.delays = 'expression').
+                except NotImplementedError:
+                    has_spike_queue = True
+                                
+                if has_spike_queue:
+                    spike_queue = f'{obj.name}_{pathway.objname}_spike_queue'
+                    # In case no delay was specified, we use an empty array
+                    delays = self.get_array_name(pathway._delays)
+                    self.spike_queues[spike_queue] = {
+                        'name' : 'self.'+spike_queue,
+                        'delays': delays,
+                        'dt': str(pathway.source.clock.dt_),
+                        'sources': self.get_array_name(pathway.synapse_sources),
+                        'start': pathway.source.start,
+                        'stop': pathway.source.stop,
+                        'owner': obj
+                    }
+    
     # Get the local namespace, if no namespace was given
     if namespace is None:
         namespace = get_local_namespace(level=level+2)
 
     # Call before_run with namespace
     net.before_run(namespace)
     
-    
-    # Get all synapses objects
-    #self.synapses |= {s for s in net.objects if isinstance(s, Synapses)}
-    
     # Update device clocks by network clocks
     self.clocks.update(net._clocks)
     if len(self.clocks) > 1:
         raise NotImplementedError("Currently multiple clocks are not supported by brian2lava.")
     
     # Set current time to end time (FIXME why? and whyt is the difference between self.t and self.t_?)
     # NOTE by carlo: self.t is with unit, self.t_ is without unit
     net.t_ = float(t_end)
-
-    # Gets the number of neurons for the neuron group
-    # FIXME this currenty assumes only *one* NeuronGroup
-    #       If multiple neuron groups are present, this needs to be changed
-    # NOTE Francesco: Is this needed for anything?
-    for obj in net.objects:
-        if isinstance(obj, NeuronGroup):
-            self.N = obj._N
     
     # FIXME Taken from CPPStandaloneDevice, but unclear what it means
     # In the CPP device it is noted that this is a hack
     # https://github.com/brian-team/brian2/blob/master/brian2/devices/cpp_standalone/device.py#L1404
     for clock in self.clocks:
         if clock.name == 'clock':
             clock._name = '_clock'
     
     # Collect code objects from network objects
     # Right now these lines don't really do anything since we're never referencing the 
     # variable code_objects again in this method
     code_objects = []
     self.lava_objects = {}
     for obj in net.sorted_objects:
-        # FIXME: Is this required? What does obj.active actually do?
         if obj.active:
-            # These are (currently) the only BrianObjects that generate their own process
-            # NOTE: This must be changed when implementing other Brian classes
+            # Only the objects that generate a lava process are added to the lava_objects dict 
+            # (so we avoid children of objects like StateUpdater and so on.)
             if any([isinstance(obj,supp_obj) for supp_obj in self.supported_processes]):
                 self.lava_objects[obj.name] = obj
             for codeobj in obj._code_objects:
                 # NOTE: For code cleanup, this is never actually used anywhere. Interesting that they save the objects as tuples of (clock,object)
                 code_objects.append((obj.clock, codeobj))
     
 
@@ -135,26 +151,21 @@
     #                        f"'stderr', or a callable function/object, "
     #                        f"but it is of type {type(report)}")
     #    report_callback(0*second, 0.0, t_start, duration)
 
     
     # TODO? At least in the CPPStandaloneDevice, there is some more code here,
     # that seems to generate some basic code lines ...
-
-    #for a in self.arrays:
-    #    if (a.name == 't') and isinstance(a.owner, Clock):
-    #        print(a.get_value())
     
     # Call network after_run method
-    # NOTE: Is this supposed to be here? Why not after calling the build function? 
     net.after_run()
     
     # Call build method
     if self.build_on_run:
-        if self.did_run:  # FIXME necessary?
+        if self.did_run: # Building a network with previously run objects still in it can cause unwanted behavior
             raise RuntimeError("The network has already been built and run "
                                "before. Use set_device with "
                                "build_on_run=False and an explicit "
                                "device.build call to use multiple run "
                                "statements with this device.")
         self.build(direct_call=False, **self.build_options)
 
@@ -165,49 +176,55 @@
     Parameters
     ----------
     net : brian2.network.Network
 
     raises : NotImplementedError
             If any of the objects in the Network are not currently supported by brian2lava
     """
-    from brian2 import get_device
+    from brian2 import get_device, Synapses
     device = get_device()
     # Raise an error if the user is trying to implement unsupported objects
     objects = []
     for obj in net.sorted_objects:
+        # CMake a list of the unsupported objects present in the network (if any)
         if any([isinstance(obj,unsupp_obj) for unsupp_obj in device.unsupported_processes]):
             obj_type = type(obj).__name__
             objects.append(obj_type)
         for contained_obj in obj.contained_objects:
             if any([isinstance(contained_obj,unsupp_obj) for unsupp_obj in device.unsupported_processes]):
                 obj_type = type(contained_obj).__name__
                 objects.append(obj_type)
-        if isinstance(obj, Synapses):
-            for pathway in obj._pathways:
-                if len(pathway.delay.variable.get_value()):
-                    objects.append("Delay in Synapses")
-                    break
-            
+        
+        # Check that no (event-driven) equations are defined in synapses, since these are not good for brian2lava.
+        if isinstance(obj,Synapses):
+            if obj.event_driven is not None:
+                device.logger.warn(
+                    """Using the (event-driven) specifier in synaptic models will most likely lead to 
+                    unwanted behavior, because event-driven effects in lava are handled at the END of a timestep 
+                    (so after synapses have already propagated the incoming signals).
+                    This is due to the intrinsic asynchronicity present in Lava and particularly in neuromorphic hardware. 
+                    For this reason, we recommend using the (clock-driven) specifier instead.
+                    """
+                )
         
     if len(objects):
         objects_repr = '\n\t\t'.join(objects)
-        msg = f"""
-        The following objects or functionalities are not supported by brian2lava, yet:
+        msg = f"""The following objects or functionalities are not supported by brian2lava, yet:
                 {objects_repr}
         You can expect them in future releases. You can also ask for features 
         on the official brian2lava repo on GitLab:
         https://gitlab.com/brian2lava/brian2lava/-/tree/main
         """
         raise NotImplementedError(msg)
         
 
 
 def compile_templates(directory, names):
     """
-    Compiles the rendered templates and returns the obtained process model
+    Compiles the rendered templates and returns a dictionary containing the instantiated processes
 
     Parameters
     ----------
     directory : `string`
         The project directory, necessary to find files to compile.
     names : network object names
         Names of network objects that are used for the Lava templates
@@ -215,40 +232,38 @@
     Returns
     -------
     compiled_processes: `Process`
         The compiled Lava process
     """
     # Execute Lava process and Lava process model
     # Add all outcomes to global scope
-    compiled_processes = {}
+    instantiated_processes = {}
     for name in names:
-        exec(open(f'{directory}/{name}_process.py').read(), globals())
-        exec(open(f'{directory}/{name}_process_model.py').read(), globals())
-    
-        exec(f"compiled_processes['{name}'] = {name}_P(name = '{name}')")
+        with open(f'{directory}/{name}_process.py') as process_file:
+            exec(process_file.read(),globals())
+        with open(f'{directory}/{name}_process_model.py') as process_model_file:
+            exec(process_model_file.read(),globals())
+            
+        # Get the process class
+        process = globals()[f'{name}_P']
+        # Instantiate the process and add it to the compiled processes
+        instantiated_processes[name] = process(name = name)
     
     # Get instance of the processes
-    return compiled_processes 
+    return instantiated_processes 
 
 
 def run_processes(self):
     """
     Executes the Lava simulation.
 
     We first compile the templates, initialize Lava and add configured monitors.
     Finally, the compiled Lava code is executed and monitor data is extracted.
     """
     
-    # TODO should we use the exec or the import version?
-    # NOTE import seems not to work at the moment, exec works
-    #import sys
-    #sys.path.append(self.project_dir)
-    #from process_model import ProcessModel
-    #from process import Process
-    
     # Compile templates
     processes = compile_templates(self.project_dir, [obj for obj in self.lava_objects])
 
     
     # NOTE adding one step is necessary such that spikes are evaluated
     #      correctly by Lava and match Brian results
     num_steps = int(self.duration/self.defaultclock.dt) + 1
@@ -256,16 +271,17 @@
     # First initialize the monitors
     for process in processes.values():
         self.init_lava_monitors(process, num_steps)
 
     # Connect the ports of connected processes
     self.connect_lava_ports(processes)
     root_processes = self.select_root_processes(processes)
+
     # Log that the run method was called
-    self.logger.diagnostic(f'Running Lava simulation for {self.duration} ({num_steps} steps)')
+    self.logger.debug(f'Running Lava simulation for {self.duration} ({num_steps} steps)')
     print(f'Running Lava simulation for {self.duration} ({num_steps} steps)')
     
     # Run the simulation
     for process in root_processes:
         self.logger.debug(f"Running process: {process.name}")
         # Prepare simulation
         run_cfg = Loihi1SimCfg()
@@ -285,26 +301,24 @@
 
     # Stop processes to terminate execution
     for process in root_processes:
         process.stop()
 
     # Indicate that the network simulation did run
     self.did_run = True
-    for process in processes.values():
-        del process
 
 
 def connect_lava_ports(self, processes):
     """
     Connect the ports of the connected processes.
 
     Parameters
     ----------
-    processes : `Process[]`
-        Compiled Lava processes.
+    processes : dict(`Process[]`)
+        Dictionary of instantiated Lava processes.
     """
 
     for var in self.lava_ports.values():
         portname = var['portname']
         pathway = var['pathway']
 
         # First connect the spiking sources to the synapses
@@ -404,29 +418,31 @@
         root_nodes.append(processes[list(component)[0]])
 
     return root_nodes
 
 
 def init_lava_monitors(self, process, num_steps):
     """
-    Initializes monitors, defined by the user in Brian.
+    Initializes Lava monitors as required by the monitors defined by the user in Brian.
     In case a monitor has additional variables to be monitored, the function this method wraps 
     is called recursively.
 
     Parameters
     ----------
     process : `Process`
-        Lava process that is provided with a monitor
+        Lava process. If the process possesses a variable which is to be monitored, the monitor is initialized.
     num_steps : `int`
-        Number of steps for which the monitor shall be active
+        Number of steps for which the monitor shall be active. In the current implementation this is set to
+          the number of steps in the simulation.
 
     Notes
     -----
-    Each probed Lava variable can be assigned to multiple monitors defined in Brian.
-    E.g. time can be necessary for a state and a spike monitor, while time is only probed once from Lava.
+    Lava variables can only be accessed by one Monitor at a time. This means that if a variable is probed
+    by multiple Brian monitors, it will be probed only once by Lava. The reference to the variable values is then 
+    handled by referencing the same monitor object in the different Brian monitors.
     """
 
     def init_lava_monitor(m,num_steps):
         """
         We define this extra method because it can be called recursively for additional variables
         """
         # If you find a process which should be monitored, look at which variable should be monitored
@@ -502,48 +518,55 @@
                 # Get initial values from process
                 init_raw = getattr(process, f'_{getattr(process,"name")}__spikespace').init
                 i_init_data = np.nonzero(init_raw)[0]
                 t_init_data = np.nonzero(init_raw)[0]*self.defaultclock.dt
 
                 # Get the data from the monitor, for both i and t the data is the same
                 raw = get_monitor_values(m)
-                t_data = (np.nonzero(raw)[1] * self.defaultclock.dt)
+                t_data = (np.nonzero(raw)[0] * self.defaultclock.dt)
 
                 # Format it correctly
                 t_data = np.concatenate((t_init_data, t_data))
-                i_data = np.concatenate((i_init_data,np.nonzero(raw)[0]))
+                i_data = np.concatenate((i_init_data,np.nonzero(raw)[1]))
                 count = np.bincount(i_data,minlength = m['var'].owner.source.N)
                 
                 # Store the monitor data into the device arrays
                 self.arrays[var] = i_data
                 self.arrays[var.owner.variables["t"]] = t_data
                 self.arrays[var.owner.variables['count']] = count
+
+                # Also set the N variable of the SpikeMonitor in order to be able to use indices properly
+                self.arrays[var.owner.variables['N']] = np.array([len(t_data)])
+
+                # Deal with the additional variables
                 for additional_monitor in m['additional_var_monitors']:
                     # New variable to update in the arrays
                     add_var = additional_monitor['var']
-                    data = get_monitor_values(additional_monitor)[:,:-2]
-                    # Get initial values from process
+                    data = get_monitor_values(additional_monitor)[:-2,:]
+
+                    # Get initial values from process and prepare to concatenate
                     init_data = getattr(process, additional_monitor['lava_var_name']).init
-                    init_data = init_data.reshape(init_data.shape[0], 1)
+                    init_data = np.expand_dims(init_data,0)
                     # Select only the correct time points for the spiking neurons
-                    data = np.concatenate((init_data, data), axis=1)[i_data,np.nonzero(raw)[1]]
+                    data = np.concatenate((init_data, data), axis=0)[np.nonzero(raw)[1],i_data]
                     self.arrays[add_var] = data
 
         # In case of a state monitor, just take the raw data from Lava
         if m['type'] == self.monitor_types['state']:
 
             # NOTE remove additional simulation steps from monitor to match Brian simulation
-            data = get_monitor_values(m)[:,:-2]
+            data = get_monitor_values(m)[:-2,:]
             
             # Get initial values from process
             init_data = getattr(process, m['lava_var_name']).init
 
             if len(init_data) > 0:
-                init_data = init_data.reshape(init_data.shape[0], 1)
-                data = np.concatenate((init_data, data), axis=1)
+                # Account for the extra dimension for the concatenation
+                init_data = np.expand_dims(init_data,0)
+                data = np.concatenate((init_data, data), axis=0)
         
             # Just formatting to make sure that we always have two dimensions
             # as used in brian for state monitor values (only for variables other than time)
             if var.name == 't':
                 self.arrays[var] = np.squeeze(data)
                 continue
 
@@ -553,22 +576,18 @@
 
             # If record is set to some specific indices, we only store the data at those indices
             # Note that this is very inefficient, but in Lava it's impossible to select indices
             # to record from a monitor. This is only to keep the results consistent with Brian.
             if isinstance(m['indices'],np.ndarray):
                 # This case happens for variables that were not defined before calling the run() method
                 if m['indices'].shape == (0,):
-                    m['indices'] = np.arange(len(data))
-                data = data[m['indices']]
+                    m['indices'] = np.arange(data.shape[1])
+                data = data[:,m['indices']]
 
-            # In brian, by design, the __getattr__ from StateMonitors will transpose the data before returning it (but not for the time variable)
-            # So here we transpose one additional time to account for this.
-            # Found it: see https://github.com/brian-team/brian2/blob/master/brian2/monitors/statemonitor.py#L378
-            # It seems that this is done by design.. https://brian.discourse.group/t/how-to-get-all-data-from-all-monitors/302/4
-            self.arrays[var] = np.transpose(data)
+            self.arrays[var] = data
 
 def get_monitor_values(monitor):
     """
     Get data from a Lava monitor.
 
     Parameters
     ----------
@@ -579,16 +598,15 @@
     # Define variables
     lava_monitor = monitor['lava_monitor']
     lava_var_name = monitor['lava_var_name']
     process_name = monitor['process_name']
     
 
     # Return lava monitor values
-    data = lava_monitor.get_data()[process_name][lava_var_name]
-    data = np.transpose(np.array(data))
+    data = np.array(lava_monitor.get_data()[process_name][lava_var_name])
 
     return data
 
 
 def update_brian_class_attributes(self,processes):
     """
     Update class attributes of Brian objects.
@@ -599,30 +617,31 @@
     Args:
         processes: List of Lava processes
     """
     self.logger.debug("Updating Brian class attributes..")
     # Iterate over processes
     for p in processes.values():
         obj = self.lava_objects[p.name]
-        for varname,var in obj.variables.items():
-            p_varname = self.get_array_name(var,prefix = None)
-
-            if hasattr(p,p_varname):
-                # NOTE: These next 2 lines are useful for fixing the reinit() issue.
-                # if "synaptic_pre" in p_varname or "synaptic_post" in p_varname:
-                #     print(p_varname, getattr(p,p_varname).get())
-
-                # This should almost never happen but sometimes some simulation 
-                # settings can produce arrays with length 0. We ignore these.
-                if getattr(p,p_varname).shape == (0,):
-                    self.logger.debug(f"Array {p_varname} has length 0, ignoring..")
+        # We have to check for variables also in the objects contained in each of our objects (e.g. SynapticPathway inside Synapses)
+        obj_to_check = [o for o in obj.contained_objects if hasattr(o,"variables")]
+        obj_to_check.append(obj)
+        for _obj in obj_to_check:
+            for varname,var in _obj.variables.items():
+                # SpikeQueue is a variable, but has no owner (and should not be accessed anyways)
+                if not hasattr(var,'owner'):
                     continue
+                p_varname = self.get_array_name(var,prefix = None)
 
-                dtype = var.dtype
-                self.arrays[var] = np.array(getattr(p,p_varname).get(), dtype=dtype)
-                    
-
-        if isinstance(obj, Synapses):
-            # Update the variables counting the number of synapses
-            # TODO: Verify that this is not needed during the simulation
-            # as right now we only update these variables AFTER running a simulation..
-            obj._update_synapse_numbers(0)
+                if hasattr(p,p_varname):
+                    # Empty array variables cannot be handled by lava get() so we just set it to an empty array manually.
+                    if getattr(p,p_varname).shape == (0,):
+                        dtype = var.dtype
+                        self.arrays[var] = np.array([],dtype=dtype)
+                    else:
+                        dtype = var.dtype
+                        self.arrays[var] = np.array(getattr(p,p_varname).get(), dtype=dtype)
+
+            if isinstance(_obj, Synapses):
+                # Update the variables counting the number of synapses
+                # TODO: Verify that this is not needed during the simulation
+                # as right now we only update these variables AFTER running a simulation..
+                _obj._update_synapse_numbers(len(_obj))
```

### Comparing `brian2lava-1.0.0a2/brian2lava/device/synapses.py` & `brian2lava-1.0.0a3/brian2lava/device/synapses.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,54 +73,24 @@
         self, synapses, condition=None, i=None, j=None, p=1., n=1,
         skip_if_invalid=False, namespace=None, level=0
     ):
     """
     Connects synapses.
 
     This method overwrites the `connect` function from Brian.
-
-    Parameters
-    ----------
-    synapses : `Synapses`
-        Equals the `self` of the original `connect` function from Brian,
-        which is an instance of the `Synapses` class.
-    condition : str, bool, optional
-        A boolean or string expression that evaluates to a boolean.
-        The expression can depend on indices ``i`` and ``j`` and on
-        pre- and post-synaptic variables. Can be combined with
-        arguments ``n``, and ``p`` but not ``i`` or ``j``.
-    i : int, ndarray of int, str, optional
-        The presynaptic neuron indices  It can be an index or array of
-        indices if combined with the ``j`` argument, or it can be a string
-        generator expression.
-    j : int, ndarray of int, str, optional
-        The postsynaptic neuron indices. It can be an index or array of
-        indices if combined with the ``i`` argument, or it can be a string
-        generator expression.
-    p : float, str, optional
-        The probability to create ``n`` synapses wherever the ``condition``
-        evaluates to true. Cannot be used with generator syntax for ``j``.
-    n : int, str, optional
-        The number of synapses to create per pre/post connection pair.
-        Defaults to 1.
-    skip_if_invalid : bool, optional
-        If set to True, rather than raising an error if you try to
-        create an invalid/out of range pair (i, j) it will just
-        quietly skip those synapses.
-    namespace : dict-like, optional
-        A namespace that will be used in addition to the group-specific
-        namespaces (if defined). If not specified, the locals
-        and globals around the run function will be used.
-    level : int, optional
-        How deep to go up the stack frame to look for the locals/global
-        (see ``namespace`` argument).
+    The only change we do to the Brian core function is to add a lava-specific
+    variable to the registered variables, and at the end of the connection process
+    we add the codeobject generated by the synapse to the initialization queue.
+    # TODO Maybe there is a better way to do this which is more mantainable.
     """
     # First, add the spiking synapses variable to the lava_variables
     self._add_spiking_synapses_vars(synapses)
-    # Check types
+
+    # STANDARD BRIAN CODE -------------------------------------------
+    # check types
     synapses._verify_connect_argument_types(condition, i, j, n, p)
 
     synapses._connect_called = True
 
     # Get namespace information
     if namespace is None:
         namespace = get_local_namespace(level=level + 2)
@@ -128,71 +98,104 @@
     try:  # wrap everything to catch IndexError
         # which connection case are we in?
         # 1: Connection condition
         if condition is None and i is None and j is None:
             condition = True
         if condition is not None:
             if i is not None or j is not None:
-                raise ValueError("Cannot combine condition with i or j "
-                                    "arguments")
-            if condition is False or condition == 'False':
+                raise ValueError("Cannot combine condition with i or j arguments")
+            if condition is False or condition == "False":
                 # Nothing to do
                 return
             j = synapses._condition_to_generator_expression(condition, p, namespace)
-            self.logger.debug("Using synapses from generator")
-            synapses._add_synapses_generator(j, n, skip_if_invalid=skip_if_invalid,
-                                            namespace=namespace, level=level + 2,
-                                            over_presynaptic=True)
+            synapses._add_synapses_generator(
+                j,
+                n,
+                skip_if_invalid=skip_if_invalid,
+                namespace=namespace,
+                level=level + 2,
+                over_presynaptic=True,
+            )
         # 2: connection indices
-        elif (i is not None and j is not None) and not (isinstance(i, str) or isinstance(j, str)):
+        elif (i is not None and j is not None) and not (
+            isinstance(i, str) or isinstance(j, str)
+        ):
             if skip_if_invalid:
-                raise ValueError("Can only use skip_if_invalid with string "
-                                    "syntax")
+                raise ValueError("Can only use skip_if_invalid with string syntax")
             i, j, n = synapses._verify_connect_array_arguments(i, j, n)
-            self.logger.debug("Using synapses from arrays")
             synapses._add_synapses_from_arrays(i, j, n, p, namespace=namespace)
         # 3: Generator expression over post-synaptic cells (i='...')
         elif isinstance(i, str):
-            i = synapses._finalize_generator_expression(i, j, p, 'i', 'j')
-            self.logger.debug("Using synapses from generator")
-            synapses._add_synapses_generator(i, n, skip_if_invalid=skip_if_invalid,
-                                            namespace=namespace, level=level + 2,
-                                            over_presynaptic=False)
+            i = synapses._finalize_generator_expression(i, j, p, "i", "j")
+            synapses._add_synapses_generator(
+                i,
+                n,
+                skip_if_invalid=skip_if_invalid,
+                namespace=namespace,
+                level=level + 2,
+                over_presynaptic=False,
+            )
         # 4: Generator expression over pre-synaptic cells (i='...')
         elif isinstance(j, str):
-            j = synapses._finalize_generator_expression(j, i, p, 'j', 'i')
-            self.logger.debug("Using synapses from generator")
-            synapses._add_synapses_generator(j, n, skip_if_invalid=skip_if_invalid,
-                                            namespace=namespace, level=level + 2,
-                                            over_presynaptic=True)
+            j = synapses._finalize_generator_expression(j, i, p, "j", "i")
+            synapses._add_synapses_generator(
+                j,
+                n,
+                skip_if_invalid=skip_if_invalid,
+                namespace=namespace,
+                level=level + 2,
+                over_presynaptic=True,
+            )
         else:
-            raise ValueError("Must specify at least one of condition, i or "
-                                "j arguments")
+            raise ValueError(
+                "Must specify at least one of condition, i or j arguments"
+            )
     except IndexError as e:
-        raise IndexError("Tried to create synapse indices outside valid "
-                            "range. Original error message: " + str(e))
-
+        raise IndexError(
+            "Tried to create synapse indices outside valid "
+            "range. Original error message: "
+            + str(e)
+        )
+    # ----------------------------------------------------------------------    
+
+    # Add the codeobject determining synaptic connections to the init queue for synapses
+    generator_objects = [codeobj for codeobj in self.code_objects.values() if codeobj.owner == synapses and 'synapses_create' in codeobj.template_name]
+
+    # Make sure that we don't insert duplicates in the queue
+    for func, args in self.proc_init_queue[synapses.name]:
+        if func == 'code_object':
+            codeobj = args
+            # If the codeobject was already added during a potential previous call of connect
+            if codeobj in generator_objects:
+                generator_objects.remove(codeobj)
+    
+    # Insert the new generators in the init queue
+    for codeobj in generator_objects:
+        self.proc_init_queue[synapses.name].append(('code_object',codeobj))
 
 def _add_spiking_synapses_vars(self,synapses):
     """
     Adds a variable to the lava_variables which will store the spiking synapses from the last
     timestep. The vector is then used to update the synaptic variables in the run_lrn function if
     the synapses are plastic.
     """
-    
     for pathway in synapses._pathways:
-        prepost = pathway.prepost
-        name = f"lava_spiking_synapses_{prepost}"
-        size = 1
 
-        # This needs to be a dynamic array as its shape will change during the simulation
-        synapses.variables.add_dynamic_array(name,size,dtype = "int")
+        # The spiking_synapses variable is always added
+        spiking_synapses = f"spiking_{synapses.name}_{pathway.objname}"
+        size = 1
 
-        # Register this variable so that it will be correctly resized during the initialization.
-        synapses.register_variable(synapses.variables[name])
+        # Only add the variable once for each pathway.
+        if not spiking_synapses in synapses.variables.keys():
+            # This needs to be a dynamic array as its shape will change during the simulation
+            synapses.variables.add_dynamic_array(spiking_synapses,size,dtype = "bool")
+
+            # Register this variable so that it will be correctly resized during the initialization.
+            synapses.register_variable(synapses.variables[spiking_synapses])
+        
 
 
 def determine_lava_ports(self, pathway, variables):
     """
     Extracts the synaptic variables to be sent to the neurongroups and determine the Lava ports required for that.
 
     Parameters
@@ -218,22 +221,23 @@
     for varname,var in variables.items():
         if isinstance(var, Function) or not isinstance(var.owner, Synapses):
             continue
         synaptic_vars.append(varname)
 
     # Var names are kept in their original form, but the ports are separated depending on the pathway
     for varname in synaptic_vars:
-        portname = pathway.synapses.name +'_'+ pathway.prepost +'_'+ varname
+        portname = pathway.synapses.name +'_'+ pathway.objname +'_'+ varname
         self.lava_ports[portname] = {
             'varname': varname, # Required by code generation
             'portname': portname,
             'pathway': pathway,
             'sender' : pathway.source.name,
             'receiver': pathway.target.name
         }
 
     ports = '\n\t'.join([port  for port in self.lava_ports])
     msg = f"""Saved ports for synaptic transmission from synapses {pathway.synapses.name} to {pathway.target.name}:
     Ports required:
     {ports}
     """
-    self.logger.diagnostic(msg)
+    self.logger.diagnostic(msg)
+
```

### Comparing `brian2lava-1.0.0a2/brian2lava/device/writer.py` & `brian2lava-1.0.0a3/brian2lava/device/writer.py`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/templates/process.py.j2` & `brian2lava-1.0.0a3/brian2lava/templates/process.py.j2`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava/writer/py.py` & `brian2lava-1.0.0a3/brian2lava/writer/py.py`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/brian2lava.egg-info/PKG-INFO` & `brian2lava-1.0.0a3/brian2lava.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brian2lava
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: An open source Brian2 interface for the neuromorphic computing framework Lava
 Home-page: https://gitlab.com/tetzlab/brian2lava
 Author: Carlo Michaelis, Francesco Negri, Winfried Oed, Jannik Luboeinski, Andrew Lehr, Tristan Stöber
 Author-email: carlo.michaelis@gmail.com
 License: MIT
 Description: # Brian2Lava
```

### Comparing `brian2lava-1.0.0a2/brian2lava.egg-info/SOURCES.txt` & `brian2lava-1.0.0a3/brian2lava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brian2lava-1.0.0a2/setup.py` & `brian2lava-1.0.0a3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
 	name='brian2lava',
-	version='1.0.0a2',  # consider adding '__version__' to 'brian2lava.__init__.py', but requires unified management of versions
+	version='1.0.0a3',  # consider adding '__version__' to 'brian2lava.__init__.py', but requires unified management of versions
 	author='Carlo Michaelis, Francesco Negri, Winfried Oed, Jannik Luboeinski, Andrew Lehr, Tristan Stöber',
 	author_email='carlo.michaelis@gmail.com',
 	packages=['brian2lava', 'brian2lava.device', 'brian2lava.codegen', 'brian2lava.writer'],
 	python_requires='>3.8',
 	url='https://gitlab.com/tetzlab/brian2lava',
 	license='MIT',
 	description='An open source Brian2 interface for the neuromorphic computing framework Lava',
```


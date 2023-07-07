# Comparing `tmp/valohai-yaml-0.9.tar.gz` & `tmp/valohai-yaml-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/valohai-yaml-0.9.tar", last modified: Wed Jul 31 12:57:26 2019, max compression
+gzip compressed data, was "dist/valohai-yaml-0.9.1.tar", last modified: Thu Aug 22 09:45:38 2019, max compression
```

## Comparing `valohai-yaml-0.9.tar` & `valohai-yaml-0.9.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/
--rw-r--r--   0 akx        (501) staff       (20)       76 2017-01-16 09:21:12.000000 valohai-yaml-0.9/MANIFEST.in
--rw-r--r--   0 akx        (501) staff       (20)      711 2019-07-31 12:57:26.000000 valohai-yaml-0.9/PKG-INFO
--rw-r--r--   0 akx        (501) staff       (20)     1368 2019-06-05 11:43:51.000000 valohai-yaml-0.9/README.md
--rw-r--r--   0 akx        (501) staff       (20)      387 2019-07-31 12:57:26.000000 valohai-yaml-0.9/setup.cfg
--rw-r--r--   0 akx        (501) staff       (20)     1543 2019-04-10 14:59:16.000000 valohai-yaml-0.9/setup.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml/
--rw-r--r--   0 akx        (501) staff       (20)      115 2019-07-31 12:55:55.000000 valohai-yaml-0.9/valohai_yaml/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)      837 2019-02-14 13:11:11.000000 valohai-yaml-0.9/valohai_yaml/__main__.py
--rw-r--r--   0 akx        (501) staff       (20)       79 2019-04-10 14:59:16.000000 valohai-yaml-0.9/valohai_yaml/_compat.py
--rw-r--r--   0 akx        (501) staff       (20)     2844 2019-04-10 14:58:58.000000 valohai-yaml-0.9/valohai_yaml/commands.py
--rw-r--r--   0 akx        (501) staff       (20)     2477 2019-04-11 10:17:11.000000 valohai-yaml-0.9/valohai_yaml/lint.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml/objs/
--rw-r--r--   0 akx        (501) staff       (20)      401 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)     1045 2019-04-11 10:17:11.000000 valohai-yaml-0.9/valohai_yaml/objs/base.py
--rw-r--r--   0 akx        (501) staff       (20)     3717 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/config.py
--rw-r--r--   0 akx        (501) staff       (20)      691 2019-04-11 10:17:11.000000 valohai-yaml-0.9/valohai_yaml/objs/endpoint.py
--rw-r--r--   0 akx        (501) staff       (20)      344 2019-03-21 17:07:46.000000 valohai-yaml-0.9/valohai_yaml/objs/environment_variable.py
--rw-r--r--   0 akx        (501) staff       (20)      226 2019-02-14 13:11:11.000000 valohai-yaml-0.9/valohai_yaml/objs/file.py
--rw-r--r--   0 akx        (501) staff       (20)      350 2019-02-14 13:11:11.000000 valohai-yaml-0.9/valohai_yaml/objs/input.py
--rw-r--r--   0 akx        (501) staff       (20)      601 2019-02-14 13:11:11.000000 valohai-yaml-0.9/valohai_yaml/objs/mount.py
--rw-r--r--   0 akx        (501) staff       (20)     3466 2019-04-11 12:33:35.000000 valohai-yaml-0.9/valohai_yaml/objs/parameter.py
--rw-r--r--   0 akx        (501) staff       (20)      983 2018-07-16 06:52:08.000000 valohai-yaml-0.9/valohai_yaml/objs/parameter_map.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml/objs/pipelines/
--rw-r--r--   0 akx        (501) staff       (20)        0 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/pipelines/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)     2982 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/pipelines/edge.py
--rw-r--r--   0 akx        (501) staff       (20)      265 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/pipelines/execution_node.py
--rw-r--r--   0 akx        (501) staff       (20)      463 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/pipelines/node.py
--rw-r--r--   0 akx        (501) staff       (20)      878 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/objs/pipelines/pipeline.py
--rw-r--r--   0 akx        (501) staff       (20)     4695 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/objs/step.py
--rw-r--r--   0 akx        (501) staff       (20)      694 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/objs/utils.py
--rw-r--r--   0 akx        (501) staff       (20)      671 2019-01-28 16:52:00.000000 valohai-yaml-0.9/valohai_yaml/parsing.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml/schema/
--rw-r--r--   0 akx        (501) staff       (20)      215 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/schema/base.yaml
--rw-r--r--   0 akx        (501) staff       (20)     1265 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/endpoint.yaml
--rw-r--r--   0 akx        (501) staff       (20)      785 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/environment-variable-item.yaml
--rw-r--r--   0 akx        (501) staff       (20)      487 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/schema/execution-node.yaml
--rw-r--r--   0 akx        (501) staff       (20)      398 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/file-item.yaml
--rw-r--r--   0 akx        (501) staff       (20)      645 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/input-item.yaml
--rw-r--r--   0 akx        (501) staff       (20)      584 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/mount-item.yaml
--rw-r--r--   0 akx        (501) staff       (20)      258 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/output-item.yaml
--rw-r--r--   0 akx        (501) staff       (20)     1449 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/param-item.yaml
--rw-r--r--   0 akx        (501) staff       (20)      763 2019-07-31 12:55:45.000000 valohai-yaml-0.9/valohai_yaml/schema/pipeline.yaml
--rw-r--r--   0 akx        (501) staff       (20)     1408 2019-06-05 11:43:51.000000 valohai-yaml-0.9/valohai_yaml/schema/step.yaml
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml/utils/
--rw-r--r--   0 akx        (501) staff       (20)      757 2019-02-14 13:11:11.000000 valohai-yaml-0.9/valohai_yaml/utils/__init__.py
--rw-r--r--   0 akx        (501) staff       (20)      280 2019-04-11 10:17:11.000000 valohai-yaml-0.9/valohai_yaml/utils/lint.py
--rw-r--r--   0 akx        (501) staff       (20)     1339 2019-02-14 13:11:11.000000 valohai-yaml-0.9/valohai_yaml/utils/terminal.py
--rw-r--r--   0 akx        (501) staff       (20)     2776 2019-04-10 14:58:47.000000 valohai-yaml-0.9/valohai_yaml/validation.py
-drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/
--rw-r--r--   0 akx        (501) staff       (20)      711 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/PKG-INFO
--rw-r--r--   0 akx        (501) staff       (20)     1470 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 akx        (501) staff       (20)        1 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 akx        (501) staff       (20)       61 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/entry_points.txt
--rw-r--r--   0 akx        (501) staff       (20)       60 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/requires.txt
--rw-r--r--   0 akx        (501) staff       (20)       13 2019-07-31 12:57:26.000000 valohai-yaml-0.9/valohai_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/
+-rw-r--r--   0 akx        (501) staff       (20)       76 2017-01-16 09:21:12.000000 valohai-yaml-0.9.1/MANIFEST.in
+-rw-r--r--   0 akx        (501) staff       (20)      713 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/PKG-INFO
+-rw-r--r--   0 akx        (501) staff       (20)     1368 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/README.md
+-rw-r--r--   0 akx        (501) staff       (20)      387 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/setup.cfg
+-rw-r--r--   0 akx        (501) staff       (20)     1543 2019-04-10 14:59:16.000000 valohai-yaml-0.9.1/setup.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml/
+-rw-r--r--   0 akx        (501) staff       (20)      117 2019-08-22 09:44:44.000000 valohai-yaml-0.9.1/valohai_yaml/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)      837 2019-02-14 13:11:11.000000 valohai-yaml-0.9.1/valohai_yaml/__main__.py
+-rw-r--r--   0 akx        (501) staff       (20)       79 2019-04-10 14:59:16.000000 valohai-yaml-0.9.1/valohai_yaml/_compat.py
+-rw-r--r--   0 akx        (501) staff       (20)     2898 2019-08-22 09:44:12.000000 valohai-yaml-0.9.1/valohai_yaml/commands.py
+-rw-r--r--   0 akx        (501) staff       (20)     2569 2019-08-05 11:36:32.000000 valohai-yaml-0.9.1/valohai_yaml/lint.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml/objs/
+-rw-r--r--   0 akx        (501) staff       (20)      401 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/objs/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)     1045 2019-04-11 10:17:11.000000 valohai-yaml-0.9.1/valohai_yaml/objs/base.py
+-rw-r--r--   0 akx        (501) staff       (20)     4923 2019-08-22 08:13:29.000000 valohai-yaml-0.9.1/valohai_yaml/objs/config.py
+-rw-r--r--   0 akx        (501) staff       (20)      691 2019-04-11 10:17:11.000000 valohai-yaml-0.9.1/valohai_yaml/objs/endpoint.py
+-rw-r--r--   0 akx        (501) staff       (20)      344 2019-03-21 17:07:46.000000 valohai-yaml-0.9.1/valohai_yaml/objs/environment_variable.py
+-rw-r--r--   0 akx        (501) staff       (20)      226 2019-02-14 13:11:11.000000 valohai-yaml-0.9.1/valohai_yaml/objs/file.py
+-rw-r--r--   0 akx        (501) staff       (20)      350 2019-02-14 13:11:11.000000 valohai-yaml-0.9.1/valohai_yaml/objs/input.py
+-rw-r--r--   0 akx        (501) staff       (20)      601 2019-02-14 13:11:11.000000 valohai-yaml-0.9.1/valohai_yaml/objs/mount.py
+-rw-r--r--   0 akx        (501) staff       (20)     3466 2019-04-11 12:33:35.000000 valohai-yaml-0.9.1/valohai_yaml/objs/parameter.py
+-rw-r--r--   0 akx        (501) staff       (20)      983 2018-07-16 06:52:08.000000 valohai-yaml-0.9.1/valohai_yaml/objs/parameter_map.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/
+-rw-r--r--   0 akx        (501) staff       (20)        0 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)     2605 2019-08-05 11:36:32.000000 valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/edge.py
+-rw-r--r--   0 akx        (501) staff       (20)      689 2019-08-05 11:36:32.000000 valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/execution_node.py
+-rw-r--r--   0 akx        (501) staff       (20)      463 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/node.py
+-rw-r--r--   0 akx        (501) staff       (20)      878 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/pipeline.py
+-rw-r--r--   0 akx        (501) staff       (20)     4695 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/objs/step.py
+-rw-r--r--   0 akx        (501) staff       (20)      694 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/objs/utils.py
+-rw-r--r--   0 akx        (501) staff       (20)      671 2019-01-28 16:52:00.000000 valohai-yaml-0.9.1/valohai_yaml/parsing.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml/schema/
+-rw-r--r--   0 akx        (501) staff       (20)      215 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/schema/base.yaml
+-rw-r--r--   0 akx        (501) staff       (20)     1265 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/endpoint.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      785 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/environment-variable-item.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      487 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/schema/execution-node.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      398 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/file-item.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      645 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/input-item.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      584 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/mount-item.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      258 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/output-item.yaml
+-rw-r--r--   0 akx        (501) staff       (20)     1449 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/param-item.yaml
+-rw-r--r--   0 akx        (501) staff       (20)      763 2019-07-31 12:55:45.000000 valohai-yaml-0.9.1/valohai_yaml/schema/pipeline.yaml
+-rw-r--r--   0 akx        (501) staff       (20)     1408 2019-06-05 11:43:51.000000 valohai-yaml-0.9.1/valohai_yaml/schema/step.yaml
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml/utils/
+-rw-r--r--   0 akx        (501) staff       (20)      757 2019-02-14 13:11:11.000000 valohai-yaml-0.9.1/valohai_yaml/utils/__init__.py
+-rw-r--r--   0 akx        (501) staff       (20)      280 2019-04-11 10:17:11.000000 valohai-yaml-0.9.1/valohai_yaml/utils/lint.py
+-rw-r--r--   0 akx        (501) staff       (20)     1339 2019-02-14 13:11:11.000000 valohai-yaml-0.9.1/valohai_yaml/utils/terminal.py
+-rw-r--r--   0 akx        (501) staff       (20)     2776 2019-04-10 14:58:47.000000 valohai-yaml-0.9.1/valohai_yaml/validation.py
+drwxr-xr-x   0 akx        (501) staff       (20)        0 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/
+-rw-r--r--   0 akx        (501) staff       (20)      713 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 akx        (501) staff       (20)     1470 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 akx        (501) staff       (20)        1 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 akx        (501) staff       (20)       61 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 akx        (501) staff       (20)       60 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/requires.txt
+-rw-r--r--   0 akx        (501) staff       (20)       13 2019-08-22 09:45:38.000000 valohai-yaml-0.9.1/valohai_yaml.egg-info/top_level.txt
```

### Comparing `valohai-yaml-0.9/PKG-INFO` & `valohai-yaml-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valohai-yaml
-Version: 0.9
+Version: 0.9.1
 Summary: Valohai.yaml validation and parsing
 Home-page: https://github.com/valohai/valohai-yaml
 Author: Valohai
 Author-email: info@valohai.com
 Maintainer: Aarni Koskela
 Maintainer-email: akx@iki.fi
 License: MIT
```

### Comparing `valohai-yaml-0.9/README.md` & `valohai-yaml-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/setup.py` & `valohai-yaml-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/__main__.py` & `valohai-yaml-0.9.1/valohai_yaml/__main__.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/commands.py` & `valohai-yaml-0.9.1/valohai_yaml/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import unicode_literals
 
 import re
 import warnings
 
+from valohai_yaml._compat import text_type
 from valohai_yaml.objs.parameter_map import LegacyParameterMap
 from valohai_yaml.utils import listify
 
 try:
     from shlex import quote
 except ImportError:  # pragma: no cover
     from pipes import quote
@@ -33,15 +34,15 @@
         parameter_name = value.split(':', 1)[1]
         if parameter_name in parameter_map.parameters:
             return quote_multiple(parameter_map.build_parameter_by_name(parameter_name))
     elif value.startswith('parameter-value:'):
         parameter_name = value.split(':', 1)[1]
         value = parameter_map.values.get(parameter_name)
         if value:
-            return quote(value)
+            return quote(text_type(value))
     return match.group(0)  # Return the original otherwise
 
 
 def build_command(command, parameter_map):
     """
     Build command line(s) using the given parameter map.
```

### Comparing `valohai-yaml-0.9/valohai_yaml/lint.py` & `valohai-yaml-0.9.1/valohai_yaml/lint.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     def warnings(self):
         return (m for m in self.messages if m['type'] == 'warning')
 
     @property
     def errors(self):
         return (m for m in self.messages if m['type'] == 'error')
 
+    def is_valid(self):
+        return (self.warning_count == 0 and self.error_count == 0)
+
 
 def lint_file(file_path):
     """
     Validate & lint `file_path` and return a LintResult.
 
     :param file_path: YAML filename
     :type file_path: str
```

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/base.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/base.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/config.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 
 class Config(Item):
     """
     Represents a `valohai.yaml` file.
     """
 
+    # Warnings that may be stuck on the top-level config during its parsing.
+    _parse_warnings = None
+
     def __init__(self, steps=(), endpoints=(), pipelines=()):
         assert all(isinstance(step, Step) for step in steps)
         self.steps = OrderedDict((step.name, step) for step in steps)
         assert all(isinstance(endpoint, Endpoint) for endpoint in endpoints)
         self.endpoints = OrderedDict((endpoint.name, endpoint) for endpoint in endpoints)
         assert all(isinstance(pipeline, Pipeline) for pipeline in pipelines)
         self.pipelines = OrderedDict((pipeline.name, pipeline) for pipeline in pipelines)
@@ -29,53 +32,81 @@
         Parse a Config structure out of a Python dict (that's likely deserialized from YAML).
 
         :param data: Config-y dict
         :type data: dict
         :return: Config object
         :rtype: valohai_yaml.objs.Config
         """
-        pipelines = []
-        endpoints = []
-        steps = []
-        parsers = {
-            'step': (steps, Step.parse),
-            'endpoint': (endpoints, Endpoint.parse),
-            'pipeline': (pipelines, Pipeline.parse),
-            'blueprint': (pipelines, Pipeline.parse),  # Alias allowed for now
-        }
+        parsers = cls.get_top_level_parsers()
+        parse_warnings = []
         for datum in data:
             assert isinstance(datum, dict)
             for type, (items, parse) in parsers.items():
                 if type in datum:
                     items.append(parse(datum[type]))
                     break
             else:
-                raise ValueError('No parser for {0}'.format(datum))
+                parse_warnings.append('No parser for {0}'.format(datum))
         inst = cls(
-            steps=steps,
-            endpoints=endpoints,
-            pipelines=pipelines,
+            steps=parsers['step'][0],
+            endpoints=parsers['endpoint'][0],
+            pipelines=parsers['pipeline'][0],
         )
         inst._original_data = data
+        inst._parse_warnings = parse_warnings
         return inst
 
+    @classmethod
+    def get_top_level_parsers(cls):
+        """
+        Get the parsers for top-level elements in a configuration file.
+
+        The return value is a little baroque due to the alias for `pipeline`/`blueprint`:
+        it's a dict that maps top-level element names to a 2-tuple of target list objects and parse functions.
+        """
+        pipeline_tuple = ([], Pipeline.parse)
+        return {
+            'step': ([], Step.parse),
+            'endpoint': ([], Endpoint.parse),
+            'pipeline': pipeline_tuple,
+            'blueprint': pipeline_tuple,  # Alias allowed for now
+        }
+
     def serialize(self):
         return list(chain(
             ({'step': step.serialize()} for step in self.steps.values()),
             ({'endpoint': endpoint.serialize()} for endpoint in self.endpoints.values()),
             ({'pipeline': pipeline.serialize()} for pipeline in self.pipelines.values()),
         ))
 
-    def lint(self, lint_result, context):
+    def lint(self, lint_result=None, context=None):
+        """
+        Lint the configuration.
+
+        :param lint_result: LintResult object. Optional; if not passed in, one is constructed.
+        :param context: Optional context dictionary; should likely not be passed in at top level.
+        :return: The lint result object used.
+        """
+        if context is None:
+            context = {}
+        if lint_result is None:
+            from valohai_yaml.lint import LintResult
+            lint_result = LintResult()
         context = dict(context, config=self)
+
+        if self._parse_warnings:
+            for warning in self._parse_warnings:
+                lint_result.add_warning(warning)
+
         lint_iterables(lint_result, context, (
             self.steps,
             self.endpoints,
             self.pipelines,
         ))
+        return lint_result
 
     def get_step_by(self, **kwargs):
         """
         Get the first step that matches all the passed named arguments.
 
         Has special argument index not present in the real step.
```

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/endpoint.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/endpoint.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/mount.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/mount.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/parameter.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/parameter.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/parameter_map.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/parameter_map.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/pipelines/edge.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/edge.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,18 +80,7 @@
             lint_result.add_error(
                 'Pipeline {pipeline} target type {type} (between {source_node} and {target_node}) not valid'.format(
                     pipeline=pipeline.name,
                     source_node=self.source_node,
                     target_node=self.target_node,
                     type=self.target_type,
                 ))
-
-    def serialize_expanded(self):
-        return {
-            'source_node': self.source_node,
-            'source_type': self.source_type,
-            'source_key': self.source_key,
-            'target_node': self.target_node,
-            'target_type': self.target_type,
-            'target_key': self.target_key,
-            'configuration': self.configuration,
-        }
```

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/pipelines/pipeline.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/step.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/step.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/objs/utils.py` & `valohai-yaml-0.9.1/valohai_yaml/objs/utils.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/parsing.py` & `valohai-yaml-0.9.1/valohai_yaml/parsing.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/endpoint.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/endpoint.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/environment-variable-item.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/environment-variable-item.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/input-item.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/input-item.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/mount-item.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/mount-item.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/param-item.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/param-item.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/pipeline.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/pipeline.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/schema/step.yaml` & `valohai-yaml-0.9.1/valohai_yaml/schema/step.yaml`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/utils/__init__.py` & `valohai-yaml-0.9.1/valohai_yaml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/utils/terminal.py` & `valohai-yaml-0.9.1/valohai_yaml/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml/validation.py` & `valohai-yaml-0.9.1/valohai_yaml/validation.py`

 * *Files identical despite different names*

### Comparing `valohai-yaml-0.9/valohai_yaml.egg-info/PKG-INFO` & `valohai-yaml-0.9.1/valohai_yaml.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valohai-yaml
-Version: 0.9
+Version: 0.9.1
 Summary: Valohai.yaml validation and parsing
 Home-page: https://github.com/valohai/valohai-yaml
 Author: Valohai
 Author-email: info@valohai.com
 Maintainer: Aarni Koskela
 Maintainer-email: akx@iki.fi
 License: MIT
```

### Comparing `valohai-yaml-0.9/valohai_yaml.egg-info/SOURCES.txt` & `valohai-yaml-0.9.1/valohai_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*


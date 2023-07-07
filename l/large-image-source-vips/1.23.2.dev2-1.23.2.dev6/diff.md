# Comparing `tmp/large-image-source-vips-1.23.2.dev2.tar.gz` & `tmp/large-image-source-vips-1.23.2.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.23.2.dev2.tar", last modified: Mon Jul  3 20:19:26 2023, max compression
+gzip compressed data, was "large-image-source-vips-1.23.2.dev6.tar", last modified: Fri Jul  7 19:29:32 2023, max compression
```

## Comparing `large-image-source-vips-1.23.2.dev2.tar` & `large-image-source-vips-1.23.2.dev6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-03 20:19:26.006908 large-image-source-vips-1.23.2.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-07-03 20:19:26.006908 large-image-source-vips-1.23.2.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-03 20:19:26.006908 large-image-source-vips-1.23.2.dev2/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-07-03 20:17:23.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-03 20:17:23.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-03 20:19:26.006908 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-07-03 20:19:25.000000 large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-03 20:19:26.006908 large-image-source-vips-1.23.2.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-07-03 20:17:23.000000 large-image-source-vips-1.23.2.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 19:29:32.388111 large-image-source-vips-1.23.2.dev6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-07-07 19:29:32.388111 large-image-source-vips-1.23.2.dev6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 19:29:32.388111 large-image-source-vips-1.23.2.dev6/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-07-07 19:27:44.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-07 19:27:44.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 19:29:32.388111 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-07-07 19:29:32.000000 large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-07 19:29:32.388111 large-image-source-vips-1.23.2.dev6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-07-07 19:27:44.000000 large-image-source-vips-1.23.2.dev6/setup.py
```

### Comparing `large-image-source-vips-1.23.2.dev2/LICENSE` & `large-image-source-vips-1.23.2.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.2.dev2/PKG-INFO` & `large-image-source-vips-1.23.2.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.2.dev2
+Version: 1.23.2.dev6
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.2.dev2/README.rst` & `large-image-source-vips-1.23.2.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.2.dev2/large_image_source_vips/__init__.py` & `large-image-source-vips-1.23.2.dev6/large_image_source_vips/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.2.dev2/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.23.2.dev6/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.2.dev2
+Version: 1.23.2.dev6
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.2.dev2/setup.py` & `large-image-source-vips-1.23.2.dev6/setup.py`

 * *Files identical despite different names*


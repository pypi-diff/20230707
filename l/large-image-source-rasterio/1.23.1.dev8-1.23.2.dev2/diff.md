# Comparing `tmp/large-image-source-rasterio-1.23.1.dev8.tar.gz` & `tmp/large-image-source-rasterio-1.23.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.23.1.dev8.tar", last modified: Tue Jun 27 17:25:15 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.23.2.dev2.tar", last modified: Mon Jul  3 20:19:06 2023, max compression
```

## Comparing `large-image-source-rasterio-1.23.1.dev8.tar` & `large-image-source-rasterio-1.23.2.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 17:25:15.935316 large-image-source-rasterio-1.23.1.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-27 17:25:15.935316 large-image-source-rasterio-1.23.1.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 17:25:15.931316 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43037 2023-06-27 17:23:37.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-27 17:23:37.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 17:25:15.931316 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-27 17:25:15.000000 large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-27 17:25:15.935316 large-image-source-rasterio-1.23.1.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-27 17:23:37.000000 large-image-source-rasterio-1.23.1.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-03 20:19:06.754771 large-image-source-rasterio-1.23.2.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-07-03 20:19:06.754771 large-image-source-rasterio-1.23.2.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-03 20:19:06.754771 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43030 2023-07-03 20:17:23.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-07-03 20:17:23.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-03 20:19:06.754771 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-07-03 20:19:06.000000 large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-03 20:19:06.754771 large-image-source-rasterio-1.23.2.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-07-03 20:17:23.000000 large-image-source-rasterio-1.23.2.dev2/setup.py
```

### Comparing `large-image-source-rasterio-1.23.1.dev8/LICENSE` & `large-image-source-rasterio-1.23.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev8/PKG-INFO` & `large-image-source-rasterio-1.23.2.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.1.dev8
+Version: 1.23.2.dev2
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.1.dev8/README.rst` & `large-image-source-rasterio-1.23.2.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,16 @@
                 #     # TODO: find band number - this is incorrect
                 #     info["maskband"] = dataset.mask_flag_enums[i - 1][1].value
 
                 # Only keep values that aren't None or the empty string
                 infoSet[i] = {k: v for k, v in info.items() if v not in (None, '')}
 
         # set the value to cache if needed
-        cache is False or getattr(self, '_bandInfo', infoSet)
+        if cache:
+            self._bandInfo = infoSet
 
         return infoSet
 
     def getMetadata(self):
         metadata = super().getMetadata()
         with self._getDatasetLock:
             # check if the file is geospatial
```

### Comparing `large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev8/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.23.2.dev2/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.1.dev8
+Version: 1.23.2.dev2
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.1.dev8/setup.py` & `large-image-source-rasterio-1.23.2.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,18 @@
     install_requires=[
         f'large-image{limit_version}',
         'rasterio>=1.3',  # to get the statistics attribute (<=> gdalinfo)
         'packaging',
     ],
     extras_require={
         'girder': f'girder-large-image{limit_version}',
-        'all': 'rio-cogeo',
+        'all': [
+            'rio-cogeo',
+            'pydantic<2',
+        ],
     },
     keywords='large_image, tile source',
     packages=find_packages(exclude=['test', 'test.*']),
     url='https://github.com/girder/large_image',
     python_requires='>=3.8',
     entry_points={
         'large_image.source': [
```


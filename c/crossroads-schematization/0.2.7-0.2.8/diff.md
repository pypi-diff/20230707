# Comparing `tmp/crossroads-schematization-0.2.7.tar.gz` & `tmp/crossroads-schematization-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.2.7.tar", last modified: Fri Jul  7 09:48:01 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.8.tar", last modified: Fri Jul  7 10:23:22 2023, max compression
```

## Comparing `crossroads-schematization-0.2.7.tar` & `crossroads-schematization-0.2.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 09:48:01.937509 crossroads-schematization-0.2.7/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.7/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-07 09:48:01.937509 crossroads-schematization-0.2.7/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.7/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 09:48:01.933509 crossroads-schematization-0.2.7/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-07 09:48:01.000000 crossroads-schematization-0.2.7/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     1188 2023-07-07 09:48:01.000000 crossroads-schematization-0.2.7/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-07 09:48:01.000000 crossroads-schematization-0.2.7/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-07 09:48:01.000000 crossroads-schematization-0.2.7/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-07 09:48:01.000000 crossroads-schematization-0.2.7/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 09:48:01.933509 crossroads-schematization-0.2.7/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-07 07:58:52.000000 crossroads-schematization-0.2.7/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     8217 2023-07-06 12:33:37.000000 crossroads-schematization-0.2.7/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    52583 2023-07-07 07:58:48.000000 crossroads-schematization-0.2.7/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    26204 2023-07-07 07:57:23.000000 crossroads-schematization-0.2.7/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.7/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 09:48:01.933509 crossroads-schematization-0.2.7/crschem/resources/
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 09:48:01.937509 crossroads-schematization-0.2.7/crschem/resources/400/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.7/crschem/resources/400/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.7/crschem/resources/400/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.7/crschem/resources/400/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.7/crschem/resources/400/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.7/crschem/resources/400/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.7/crschem/resources/400/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.7/crschem/resources/400/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.7/crschem/resources/400/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.7/crschem/resources/400/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.7/crschem/resources/400/style-96.xml
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 09:48:01.937509 crossroads-schematization-0.2.7/crschem/resources/500/
--rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/crossing-3-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/crossing-3-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/island-96-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/island-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/point-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/point-96.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.7/crschem/resources/500/style-96.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.7/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.7/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-07 09:48:01.937509 crossroads-schematization-0.2.7/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.7/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.8/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.8/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.843182 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1188 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-07-07 10:23:22.000000 crossroads-schematization-0.2.8/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.843182 crossroads-schematization-0.2.8/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-07-07 10:22:54.000000 crossroads-schematization-0.2.8/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     8217 2023-07-06 12:33:37.000000 crossroads-schematization-0.2.8/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    52583 2023-07-07 07:58:48.000000 crossroads-schematization-0.2.8/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    26625 2023-07-07 10:17:53.000000 crossroads-schematization-0.2.8/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.8/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.843182 crossroads-schematization-0.2.8/crschem/resources/
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/crschem/resources/400/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.8/crschem/resources/400/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.8/crschem/resources/400/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.8/crschem/resources/400/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     3458 2023-07-07 10:21:11.000000 crossroads-schematization-0.2.8/crschem/resources/400/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3456 2023-07-07 10:21:17.000000 crossroads-schematization-0.2.8/crschem/resources/400/style-96.xml
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/crschem/resources/500/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1941 2023-07-07 10:01:36.000000 crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1932 2023-07-07 10:02:54.000000 crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1519 2023-07-07 10:06:34.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1516 2023-07-07 10:06:11.000000 crossroads-schematization-0.2.8/crschem/resources/500/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-07-04 11:33:53.000000 crossroads-schematization-0.2.8/crschem/resources/500/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     3458 2023-07-07 10:21:05.000000 crossroads-schematization-0.2.8/crschem/resources/500/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3457 2023-07-07 10:20:48.000000 crossroads-schematization-0.2.8/crschem/resources/500/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.8/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.8/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-07-07 10:23:22.847182 crossroads-schematization-0.2.8/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.8/setup.py
```

### Comparing `crossroads-schematization-0.2.7/PKG-INFO` & `crossroads-schematization-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.7
+Version: 0.2.8
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.7/README.md` & `crossroads-schematization-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.8/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.7
+Version: 0.2.8
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.7/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.2.8/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/cmd.py` & `crossroads-schematization-0.2.8/crschem/cmd.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/crossroad.py` & `crossroads-schematization-0.2.8/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.8/crschem/crossroad_schematization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from shapely.geometry import Point, LineString, MultiLineString, LinearRing, Polygon
+from shapely.geometry import Point, LineString, MultiLineString, LinearRing, Polygon, box
+from shapely import affinity
 import osmnx
 import os
 import networkx
 import numpy as np
 import copy
 import itertools
 import geopandas
@@ -542,14 +543,22 @@
         mapnik.render_to_file(m, filename)
 
 
     def toGDFInnerRegion(self):
         d = {'type': ['inner_region'], 'geometry': [self.inner_region]}
         return geopandas.GeoDataFrame(d, crs=2154)
 
+    def toGDFOuterRegion(self):
+        bbox = self.inner_region.bounds
+        area = affinity.scale(box(*bbox), 1.1, 1.1)
+        outer = area.difference(self.inner_region)
+
+        d = {'type': ['outer_region'], 'geometry': [outer]}
+        return geopandas.GeoDataFrame(d, crs=2154)
+
 
     def toGeojson(self, filename, only_reachable_islands = False, crs = "EPSG:4326"):
         df = pandas.concat([self.toGDFInnerRegion().to_crs(crs),
                             c.TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs),
                             c.Branch.toGDFBranches(self.branches).to_crs(crs),
                             c.TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs),
                             c.Crossing.toGDFCrossings(self.crossings).to_crs(crs)])
@@ -557,14 +566,15 @@
         df.to_file(filename, driver='GeoJSON')
 
 
     def toShapefiles(self, filename, only_reachable_islands = False, crs = "EPSG:4326"):
         filename, file_extension = os.path.splitext(filename)
 
         self.toGDFInnerRegion().to_crs(crs).to_file(filename + "-inner" + file_extension) # region
+        self.toGDFOuterRegion().to_crs(crs).to_file(filename + "-outer" + file_extension) # region
         c.TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs).to_file(filename + "-sidewalks" + file_extension) # lines
         c.Branch.toGDFBranches(self.branches).to_crs(crs).to_file(filename + "-branches" + file_extension) # lines
         
         # islands can be points and lines
         islands = c.TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs)
         islands[islands.geometry.type == 'LineString'].to_file(filename + "-islands-lines" + file_extension)
         islands[islands.geometry.type == 'Point'].to_file(filename + "-islands-points" + file_extension)
```

### Comparing `crossroads-schematization-0.2.7/crschem/processing.py` & `crossroads-schematization-0.2.8/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/crossing-3-300.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/crossing-3-96.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/crossing-3-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/island-300-white.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/island-300.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/island-96-white.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/island-96-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/island-96.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/island-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/point-300.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/point-96.svg` & `crossroads-schematization-0.2.8/crschem/resources/400/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/style-300.xml` & `crossroads-schematization-0.2.8/crschem/resources/400/style-300.xml`

 * *Files 3% similar despite different names*

#### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/style-300.xml` & `crossroads-schematization-0.2.8/crschem/resources/400/style-300.xml`

```diff
@@ -5,14 +5,19 @@
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
       <PolygonPatternSymbolizer file="point-300.svg"/>
     </Rule>
   </Style>
+  <Style name="outer">
+    <Rule>
+      <PolygonSymbolizer fill="#fff"/>
+    </Rule>
+  </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
       <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="sidewalks">
@@ -72,14 +77,21 @@
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-outer.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/style-96.xml` & `crossroads-schematization-0.2.8/crschem/resources/400/style-96.xml`

 * *Files 1% similar despite different names*

#### Comparing `crossroads-schematization-0.2.7/crschem/resources/400/style-96.xml` & `crossroads-schematization-0.2.8/crschem/resources/400/style-96.xml`

```diff
@@ -5,14 +5,19 @@
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
       <PolygonPatternSymbolizer file="point-96.svg"/>
     </Rule>
   </Style>
+  <Style name="outer">
+    <Rule>
+      <PolygonSymbolizer fill="#fff"/>
+    </Rule>
+  </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
       <LineSymbolizer stroke="#fff" stroke-width="16" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="sidewalks">
@@ -72,14 +77,21 @@
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-outer.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/crossing-3-300.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-96.svg`

 * *Files 9% similar despite different names*

```diff
@@ -3,116 +3,119 @@
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 7665 7273 696f  ..<svg.   versio
 00000080: 6e3d 2231 2e31 220a 2020 2069 643d 2273  n="1.1".   id="s
-00000090: 7667 3222 0a20 2020 7769 6474 683d 2231  vg2".   width="1
-000000a0: 3539 2e32 3837 3038 220a 2020 2068 6569  59.28708".   hei
-000000b0: 6768 743d 2231 3338 2e30 3438 3831 220a  ght="138.04881".
+00000090: 7667 3222 0a20 2020 7769 6474 683d 2233  vg2".   width="3
+000000a0: 392e 3535 3737 3734 220a 2020 2068 6569  9.557774".   hei
+000000b0: 6768 743d 2233 342e 3238 3334 3031 220a  ght="34.283401".
 000000c0: 2020 2076 6965 7742 6f78 3d22 3020 3020     viewBox="0 0 
-000000d0: 3135 392e 3238 3730 3820 3133 382e 3034  159.28708 138.04
-000000e0: 3838 3122 0a20 2020 736f 6469 706f 6469  881".   sodipodi
+000000d0: 3339 2e35 3537 3737 3420 3334 2e32 3833  39.557774 34.283
+000000e0: 3430 3122 0a20 2020 736f 6469 706f 6469  401".   sodipodi
 000000f0: 3a64 6f63 6e61 6d65 3d22 6372 6f73 7369  :docname="crossi
-00000100: 6e67 2d33 2d33 3030 2e73 7667 220a 2020  ng-3-300.svg".  
-00000110: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
-00000120: 6e3d 2231 2e32 2e32 2028 6230 6138 3438  n="1.2.2 (b0a848
-00000130: 3635 3431 2c20 3230 3232 2d31 322d 3031  6541, 2022-12-01
-00000140: 2922 0a20 2020 786d 6c6e 733a 696e 6b73  )".   xmlns:inks
-00000150: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
-00000160: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
-00000170: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
-00000180: 6522 0a20 2020 786d 6c6e 733a 736f 6469  e".   xmlns:sodi
-00000190: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
-000001a0: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
-000001b0: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
-000001c0: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
-000001d0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
-000001e0: 332e 6f72 672f 3230 3030 2f73 7667 220a  3.org/2000/svg".
-000001f0: 2020 2078 6d6c 6e73 3a73 7667 3d22 6874     xmlns:svg="ht
-00000200: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00000210: 3230 3030 2f73 7667 223e 0a20 203c 6465  2000/svg">.  <de
-00000220: 6673 0a20 2020 2020 6964 3d22 6465 6673  fs.     id="defs
-00000230: 3622 202f 3e0a 2020 3c73 6f64 6970 6f64  6" />.  <sodipod
-00000240: 693a 6e61 6d65 6476 6965 770a 2020 2020  i:namedview.    
-00000250: 2069 643d 226e 616d 6564 7669 6577 3422   id="namedview4"
-00000260: 0a20 2020 2020 7061 6765 636f 6c6f 723d  .     pagecolor=
-00000270: 2223 6666 6666 6666 220a 2020 2020 2062  "#ffffff".     b
-00000280: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
-00000290: 3636 3622 0a20 2020 2020 626f 7264 6572  666".     border
-000002a0: 6f70 6163 6974 793d 2231 2e30 220a 2020  opacity="1.0".  
-000002b0: 2020 2069 6e6b 7363 6170 653a 7368 6f77     inkscape:show
-000002c0: 7061 6765 7368 6164 6f77 3d22 3222 0a20  pageshadow="2". 
-000002d0: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
-000002e0: 656f 7061 6369 7479 3d22 302e 3022 0a20  eopacity="0.0". 
-000002f0: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
-00000300: 6563 6865 636b 6572 626f 6172 643d 2230  echeckerboard="0
-00000310: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000320: 6465 736b 636f 6c6f 723d 2223 6431 6431  deskcolor="#d1d1
-00000330: 6431 220a 2020 2020 2073 686f 7767 7269  d1".     showgri
-00000340: 643d 2266 616c 7365 220a 2020 2020 2069  d="false".     i
-00000350: 6e6b 7363 6170 653a 7a6f 6f6d 3d22 342e  nkscape:zoom="4.
-00000360: 3132 3737 3637 3322 0a20 2020 2020 696e  1277673".     in
-00000370: 6b73 6361 7065 3a63 783d 2236 312e 3431  kscape:cx="61.41
-00000380: 3333 3435 220a 2020 2020 2069 6e6b 7363  3345".     inksc
-00000390: 6170 653a 6379 3d22 3130 322e 3233 3434  ape:cy="102.2344
-000003a0: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
-000003b0: 3a77 696e 646f 772d 7769 6474 683d 2231  :window-width="1
-000003c0: 3932 3022 0a20 2020 2020 696e 6b73 6361  920".     inksca
-000003d0: 7065 3a77 696e 646f 772d 6865 6967 6874  pe:window-height
-000003e0: 3d22 3130 3139 220a 2020 2020 2069 6e6b  ="1019".     ink
-000003f0: 7363 6170 653a 7769 6e64 6f77 2d78 3d22  scape:window-x="
-00000400: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
-00000410: 3a77 696e 646f 772d 793d 2230 220a 2020  :window-y="0".  
-00000420: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-00000430: 6f77 2d6d 6178 696d 697a 6564 3d22 3122  ow-maximized="1"
-00000440: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
-00000450: 7572 7265 6e74 2d6c 6179 6572 3d22 6738  urrent-layer="g8
-00000460: 2220 2f3e 0a20 203c 670a 2020 2020 2069  " />.  <g.     i
-00000470: 6e6b 7363 6170 653a 6772 6f75 706d 6f64  nkscape:groupmod
-00000480: 653d 226c 6179 6572 220a 2020 2020 2069  e="layer".     i
-00000490: 6e6b 7363 6170 653a 6c61 6265 6c3d 2249  nkscape:label="I
-000004a0: 6d61 6765 220a 2020 2020 2069 643d 2267  mage".     id="g
-000004b0: 3822 3e0a 2020 2020 3c72 6563 740a 2020  8">.    <rect.  
-000004c0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000004d0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-000004e0: 7769 6474 683a 302e 3830 3237 3037 3b73  width:0.802707;s
-000004f0: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
-00000500: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
-00000510: 6f69 6e3a 6265 7665 6c22 0a20 2020 2020  oin:bevel".     
-00000520: 2020 6964 3d22 7265 6374 3238 3722 0a20    id="rect287". 
-00000530: 2020 2020 2020 7769 6474 683d 2231 3539        width="159
-00000540: 2e32 3837 3038 220a 2020 2020 2020 2068  .28708".       h
-00000550: 6569 6768 743d 2231 3338 2e30 3438 3831  eight="138.04881
-00000560: 220a 2020 2020 2020 2078 3d22 3022 0a20  ".       x="0". 
-00000570: 2020 2020 2020 793d 2230 220a 2020 2020        y="0".    
-00000580: 2020 2072 793d 2237 2e37 3939 3830 3835     ry="7.7998085
-00000590: 2220 2f3e 0a20 2020 203c 7265 6374 0a20  " />.    <rect. 
-000005a0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-000005b0: 6c3a 2330 3030 3030 303b 7374 726f 6b65  l:#000000;stroke
-000005c0: 2d77 6964 7468 3a30 2e38 3032 3730 373b  -width:0.802707;
-000005d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a72  stroke-linecap:r
-000005e0: 6f75 6e64 3b73 7472 6f6b 652d 6c69 6e65  ound;stroke-line
-000005f0: 6a6f 696e 3a62 6576 656c 220a 2020 2020  join:bevel".    
-00000600: 2020 2069 643d 2272 6563 7436 3032 220a     id="rect602".
-00000610: 2020 2020 2020 2077 6964 7468 3d22 3132         width="12
-00000620: 2e35 3936 3136 3422 0a20 2020 2020 2020  .596164".       
-00000630: 6865 6967 6874 3d22 3937 2e35 3034 3033  height="97.50403
-00000640: 3622 0a20 2020 2020 2020 783d 2232 372e  6".       x="27.
-00000650: 3437 3737 3236 220a 2020 2020 2020 2079  477726".       y
-00000660: 3d22 3231 2e35 3131 3934 2220 2f3e 0a20  ="21.51194" />. 
-00000670: 2020 203c 7265 6374 0a20 2020 2020 2020     <rect.       
-00000680: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-00000690: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-000006a0: 3a30 2e38 3032 3730 373b 7374 726f 6b65  :0.802707;stroke
-000006b0: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
-000006c0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a62  troke-linejoin:b
-000006d0: 6576 656c 220a 2020 2020 2020 2069 643d  evel".       id=
-000006e0: 2272 6563 7436 3032 2d33 220a 2020 2020  "rect602-3".    
-000006f0: 2020 2077 6964 7468 3d22 3132 2e35 3936     width="12.596
-00000700: 3136 3422 0a20 2020 2020 2020 6865 6967  164".       heig
-00000710: 6874 3d22 3937 2e35 3034 3033 3622 0a20  ht="97.504036". 
-00000720: 2020 2020 2020 783d 2231 3138 2e30 3332        x="118.032
-00000730: 3038 220a 2020 2020 2020 2079 3d22 3231  08".       y="21
-00000740: 2e35 3131 3934 2220 2f3e 0a20 203c 2f67  .51194" />.  </g
-00000750: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
+00000100: 6e67 2d33 2d39 362e 7376 6722 0a20 2020  ng-3-96.svg".   
+00000110: 696e 6b73 6361 7065 3a76 6572 7369 6f6e  inkscape:version
+00000120: 3d22 312e 322e 3220 2862 3061 3834 3836  ="1.2.2 (b0a8486
+00000130: 3534 312c 2032 3032 322d 3132 2d30 3129  541, 2022-12-01)
+00000140: 220a 2020 2078 6d6c 6e73 3a69 6e6b 7363  ".   xmlns:inksc
+00000150: 6170 653d 2268 7474 703a 2f2f 7777 772e  ape="http://www.
+00000160: 696e 6b73 6361 7065 2e6f 7267 2f6e 616d  inkscape.org/nam
+00000170: 6573 7061 6365 732f 696e 6b73 6361 7065  espaces/inkscape
+00000180: 220a 2020 2078 6d6c 6e73 3a73 6f64 6970  ".   xmlns:sodip
+00000190: 6f64 693d 2268 7474 703a 2f2f 736f 6469  odi="http://sodi
+000001a0: 706f 6469 2e73 6f75 7263 6566 6f72 6765  podi.sourceforge
+000001b0: 2e6e 6574 2f44 5444 2f73 6f64 6970 6f64  .net/DTD/sodipod
+000001c0: 692d 302e 6474 6422 0a20 2020 786d 6c6e  i-0.dtd".   xmln
+000001d0: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
+000001e0: 2e6f 7267 2f32 3030 302f 7376 6722 0a20  .org/2000/svg". 
+000001f0: 2020 786d 6c6e 733a 7376 673d 2268 7474    xmlns:svg="htt
+00000200: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
+00000210: 3030 302f 7376 6722 3e0a 2020 3c64 6566  000/svg">.  <def
+00000220: 730a 2020 2020 2069 643d 2264 6566 7336  s.     id="defs6
+00000230: 2220 2f3e 0a20 203c 736f 6469 706f 6469  " />.  <sodipodi
+00000240: 3a6e 616d 6564 7669 6577 0a20 2020 2020  :namedview.     
+00000250: 6964 3d22 6e61 6d65 6476 6965 7734 220a  id="namedview4".
+00000260: 2020 2020 2070 6167 6563 6f6c 6f72 3d22       pagecolor="
+00000270: 2366 6666 6666 6622 0a20 2020 2020 626f  #ffffff".     bo
+00000280: 7264 6572 636f 6c6f 723d 2223 3636 3636  rdercolor="#6666
+00000290: 3636 220a 2020 2020 2062 6f72 6465 726f  66".     bordero
+000002a0: 7061 6369 7479 3d22 312e 3022 0a20 2020  pacity="1.0".   
+000002b0: 2020 696e 6b73 6361 7065 3a73 686f 7770    inkscape:showp
+000002c0: 6167 6573 6861 646f 773d 2232 220a 2020  ageshadow="2".  
+000002d0: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
+000002e0: 6f70 6163 6974 793d 2230 2e30 220a 2020  opacity="0.0".  
+000002f0: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
+00000300: 6368 6563 6b65 7262 6f61 7264 3d22 3022  checkerboard="0"
+00000310: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
+00000320: 6573 6b63 6f6c 6f72 3d22 2364 3164 3164  eskcolor="#d1d1d
+00000330: 3122 0a20 2020 2020 7368 6f77 6772 6964  1".     showgrid
+00000340: 3d22 6661 6c73 6522 0a20 2020 2020 696e  ="false".     in
+00000350: 6b73 6361 7065 3a7a 6f6f 6d3d 2231 332e  kscape:zoom="13.
+00000360: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
+00000370: 3a63 783d 2232 322e 3833 3538 3231 220a  :cx="22.835821".
+00000380: 2020 2020 2069 6e6b 7363 6170 653a 6379       inkscape:cy
+00000390: 3d22 392e 3032 3938 3530 3822 0a20 2020  ="9.0298508".   
+000003a0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
+000003b0: 772d 7769 6474 683d 2231 3932 3022 0a20  w-width="1920". 
+000003c0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+000003d0: 646f 772d 6865 6967 6874 3d22 3130 3139  dow-height="1019
+000003e0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+000003f0: 7769 6e64 6f77 2d78 3d22 3022 0a20 2020  window-x="0".   
+00000400: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
+00000410: 772d 793d 2230 220a 2020 2020 2069 6e6b  w-y="0".     ink
+00000420: 7363 6170 653a 7769 6e64 6f77 2d6d 6178  scape:window-max
+00000430: 696d 697a 6564 3d22 3122 0a20 2020 2020  imized="1".     
+00000440: 696e 6b73 6361 7065 3a63 7572 7265 6e74  inkscape:current
+00000450: 2d6c 6179 6572 3d22 6738 2220 2f3e 0a20  -layer="g8" />. 
+00000460: 203c 670a 2020 2020 2069 6e6b 7363 6170   <g.     inkscap
+00000470: 653a 6772 6f75 706d 6f64 653d 226c 6179  e:groupmode="lay
+00000480: 6572 220a 2020 2020 2069 6e6b 7363 6170  er".     inkscap
+00000490: 653a 6c61 6265 6c3d 2249 6d61 6765 220a  e:label="Image".
+000004a0: 2020 2020 2069 643d 2267 3822 0a20 2020       id="g8".   
+000004b0: 2020 7472 616e 7366 6f72 6d3d 2274 7261    transform="tra
+000004c0: 6e73 6c61 7465 2830 2c2d 392e 3034 3939  nslate(0,-9.0499
+000004d0: 3330 3629 223e 0a20 2020 203c 7265 6374  306)">.    <rect
+000004e0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+000004f0: 696c 6c3a 2366 6666 6666 663b 7374 726f  ill:#ffffff;stro
+00000500: 6b65 2d77 6964 7468 3a30 2e31 3939 3334  ke-width:0.19934
+00000510: 373b 7374 726f 6b65 2d6c 696e 6563 6170  7;stroke-linecap
+00000520: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6c69  :round;stroke-li
+00000530: 6e65 6a6f 696e 3a62 6576 656c 220a 2020  nejoin:bevel".  
+00000540: 2020 2020 2069 643d 2272 6563 7432 3837       id="rect287
+00000550: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
+00000560: 3339 2e35 3537 3737 3422 0a20 2020 2020  39.557774".     
+00000570: 2020 6865 6967 6874 3d22 3334 2e32 3833    height="34.283
+00000580: 3430 3122 0a20 2020 2020 2020 783d 2230  401".       x="0
+00000590: 220a 2020 2020 2020 2079 3d22 392e 3034  ".       y="9.04
+000005a0: 3939 3330 3622 0a20 2020 2020 2020 7279  99306".       ry
+000005b0: 3d22 312e 3933 3730 3234 3822 202f 3e0a  ="1.9370248" />.
+000005c0: 2020 2020 3c72 6563 740a 2020 2020 2020      <rect.      
+000005d0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+000005e0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+000005f0: 683a 302e 3235 3139 3639 3b73 7472 6f6b  h:0.251969;strok
+00000600: 652d 6c69 6e65 6361 703a 726f 756e 643b  e-linecap:round;
+00000610: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00000620: 6265 7665 6c22 0a20 2020 2020 2020 6964  bevel".       id
+00000630: 3d22 7265 6374 3630 322d 3336 2d35 220a  ="rect602-36-5".
+00000640: 2020 2020 2020 2077 6964 7468 3d22 332e         width="3.
+00000650: 3935 3339 3138 3522 0a20 2020 2020 2020  9539185".       
+00000660: 6865 6967 6874 3d22 3234 2e32 3134 3430  height="24.21440
+00000670: 3922 0a20 2020 2020 2020 783d 2232 392e  9".       x="29.
+00000680: 3331 3233 3935 220a 2020 2020 2020 2079  312395".       y
+00000690: 3d22 3134 2e33 3932 3236 3222 202f 3e0a  ="14.392262" />.
+000006a0: 2020 2020 3c72 6563 740a 2020 2020 2020      <rect.      
+000006b0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+000006c0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+000006d0: 683a 302e 3235 3139 3639 3b73 7472 6f6b  h:0.251969;strok
+000006e0: 652d 6c69 6e65 6361 703a 726f 756e 643b  e-linecap:round;
+000006f0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00000700: 6265 7665 6c22 0a20 2020 2020 2020 6964  bevel".       id
+00000710: 3d22 7265 6374 3630 322d 3336 220a 2020  ="rect602-36".  
+00000720: 2020 2020 2077 6964 7468 3d22 332e 3935       width="3.95
+00000730: 3339 3138 3522 0a20 2020 2020 2020 6865  39185".       he
+00000740: 6967 6874 3d22 3234 2e32 3134 3430 3922  ight="24.214409"
+00000750: 0a20 2020 2020 2020 783d 2235 2e39 3938  .       x="5.998
+00000760: 3133 3635 220a 2020 2020 2020 2079 3d22  1365".       y="
+00000770: 3134 2e33 3932 3236 3222 202f 3e0a 2020  14.392262" />.  
+00000780: 3c2f 673e 0a3c 2f73 7667 3e0a            </g>.</svg>.
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/crossing-3-96.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/crossing-3-300.svg`

 * *Files 9% similar despite different names*

```diff
@@ -3,121 +3,120 @@
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 7665 7273 696f  ..<svg.   versio
 00000080: 6e3d 2231 2e31 220a 2020 2069 643d 2273  n="1.1".   id="s
-00000090: 7667 3222 0a20 2020 7769 6474 683d 2235  vg2".   width="5
-000000a0: 3022 0a20 2020 6865 6967 6874 3d22 3433  0".   height="43
-000000b0: 2e33 3333 3333 3222 0a20 2020 7669 6577  .333332".   view
-000000c0: 426f 783d 2230 2030 2035 3020 3433 2e33  Box="0 0 50 43.3
-000000d0: 3333 3333 3222 0a20 2020 736f 6469 706f  33332".   sodipo
-000000e0: 6469 3a64 6f63 6e61 6d65 3d22 6372 6f73  di:docname="cros
-000000f0: 7369 6e67 2d33 2d39 362e 7376 6722 0a20  sing-3-96.svg". 
-00000100: 2020 696e 6b73 6361 7065 3a76 6572 7369    inkscape:versi
-00000110: 6f6e 3d22 312e 322e 3220 2862 3061 3834  on="1.2.2 (b0a84
-00000120: 3836 3534 312c 2032 3032 322d 3132 2d30  86541, 2022-12-0
-00000130: 3129 220a 2020 2078 6d6c 6e73 3a69 6e6b  1)".   xmlns:ink
-00000140: 7363 6170 653d 2268 7474 703a 2f2f 7777  scape="http://ww
-00000150: 772e 696e 6b73 6361 7065 2e6f 7267 2f6e  w.inkscape.org/n
-00000160: 616d 6573 7061 6365 732f 696e 6b73 6361  amespaces/inksca
-00000170: 7065 220a 2020 2078 6d6c 6e73 3a73 6f64  pe".   xmlns:sod
-00000180: 6970 6f64 693d 2268 7474 703a 2f2f 736f  ipodi="http://so
-00000190: 6469 706f 6469 2e73 6f75 7263 6566 6f72  dipodi.sourcefor
-000001a0: 6765 2e6e 6574 2f44 5444 2f73 6f64 6970  ge.net/DTD/sodip
-000001b0: 6f64 692d 302e 6474 6422 0a20 2020 786d  odi-0.dtd".   xm
-000001c0: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
-000001d0: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
-000001e0: 0a20 2020 786d 6c6e 733a 7376 673d 2268  .   xmlns:svg="h
-000001f0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
-00000200: 2f32 3030 302f 7376 6722 3e0a 2020 3c64  /2000/svg">.  <d
-00000210: 6566 730a 2020 2020 2069 643d 2264 6566  efs.     id="def
-00000220: 7336 2220 2f3e 0a20 203c 736f 6469 706f  s6" />.  <sodipo
-00000230: 6469 3a6e 616d 6564 7669 6577 0a20 2020  di:namedview.   
-00000240: 2020 6964 3d22 6e61 6d65 6476 6965 7734    id="namedview4
-00000250: 220a 2020 2020 2070 6167 6563 6f6c 6f72  ".     pagecolor
-00000260: 3d22 2366 6666 6666 6622 0a20 2020 2020  ="#ffffff".     
-00000270: 626f 7264 6572 636f 6c6f 723d 2223 3636  bordercolor="#66
-00000280: 3636 3636 220a 2020 2020 2062 6f72 6465  6666".     borde
-00000290: 726f 7061 6369 7479 3d22 312e 3022 0a20  ropacity="1.0". 
-000002a0: 2020 2020 696e 6b73 6361 7065 3a73 686f      inkscape:sho
-000002b0: 7770 6167 6573 6861 646f 773d 2232 220a  wpageshadow="2".
-000002c0: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
-000002d0: 6765 6f70 6163 6974 793d 2230 2e30 220a  geopacity="0.0".
-000002e0: 2020 2020 2069 6e6b 7363 6170 653a 7061       inkscape:pa
-000002f0: 6765 6368 6563 6b65 7262 6f61 7264 3d22  gecheckerboard="
-00000300: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
-00000310: 3a64 6573 6b63 6f6c 6f72 3d22 2364 3164  :deskcolor="#d1d
-00000320: 3164 3122 0a20 2020 2020 7368 6f77 6772  1d1".     showgr
-00000330: 6964 3d22 6661 6c73 6522 0a20 2020 2020  id="false".     
-00000340: 696e 6b73 6361 7065 3a7a 6f6f 6d3d 2233  inkscape:zoom="3
-00000350: 2e33 3522 0a20 2020 2020 696e 6b73 6361  .35".     inksca
-00000360: 7065 3a63 783d 222d 3338 2e39 3535 3232  pe:cx="-38.95522
-00000370: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
-00000380: 3a63 793d 2239 302e 3434 3737 3631 220a  :cy="90.447761".
-00000390: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
-000003a0: 6e64 6f77 2d77 6964 7468 3d22 3139 3230  ndow-width="1920
-000003b0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000003c0: 7769 6e64 6f77 2d68 6569 6768 743d 2231  window-height="1
-000003d0: 3031 3922 0a20 2020 2020 696e 6b73 6361  019".     inksca
-000003e0: 7065 3a77 696e 646f 772d 783d 2230 220a  pe:window-x="0".
-000003f0: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
-00000400: 6e64 6f77 2d79 3d22 3022 0a20 2020 2020  ndow-y="0".     
-00000410: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-00000420: 6d61 7869 6d69 7a65 643d 2231 220a 2020  maximized="1".  
-00000430: 2020 2069 6e6b 7363 6170 653a 6375 7272     inkscape:curr
-00000440: 656e 742d 6c61 7965 723d 2267 3822 202f  ent-layer="g8" /
-00000450: 3e0a 2020 3c67 0a20 2020 2020 696e 6b73  >.  <g.     inks
-00000460: 6361 7065 3a67 726f 7570 6d6f 6465 3d22  cape:groupmode="
-00000470: 6c61 7965 7222 0a20 2020 2020 696e 6b73  layer".     inks
-00000480: 6361 7065 3a6c 6162 656c 3d22 496d 6167  cape:label="Imag
-00000490: 6522 0a20 2020 2020 6964 3d22 6738 223e  e".     id="g8">
-000004a0: 0a20 2020 203c 670a 2020 2020 2020 2069  .    <g.       i
-000004b0: 643d 2267 3732 3422 0a20 2020 2020 2020  d="g724".       
-000004c0: 7472 616e 7366 6f72 6d3d 2273 6361 6c65  transform="scale
-000004d0: 2830 2e33 3333 3333 3333 3329 223e 0a20  (0.33333333)">. 
-000004e0: 2020 2020 203c 7265 6374 0a20 2020 2020       <rect.     
-000004f0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00000500: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00000510: 6964 7468 3a30 2e37 3535 3930 363b 7374  idth:0.755906;st
-00000520: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
-00000530: 6e64 3b73 7472 6f6b 652d 6c69 6e65 6a6f  nd;stroke-linejo
-00000540: 696e 3a62 6576 656c 220a 2020 2020 2020  in:bevel".      
-00000550: 2020 2069 643d 2272 6563 7432 3837 220a     id="rect287".
-00000560: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
-00000570: 3135 3022 0a20 2020 2020 2020 2020 6865  150".         he
-00000580: 6967 6874 3d22 3133 3022 0a20 2020 2020  ight="130".     
-00000590: 2020 2020 783d 2230 220a 2020 2020 2020      x="0".      
-000005a0: 2020 2079 3d22 3022 0a20 2020 2020 2020     y="0".       
-000005b0: 2020 7279 3d22 372e 3334 3530 3438 2220    ry="7.345048" 
-000005c0: 2f3e 0a20 2020 2020 203c 7265 6374 0a20  />.      <rect. 
-000005d0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00000090: 7667 3222 0a20 2020 7769 6474 683d 2231  vg2".   width="1
+000000a0: 3239 2e37 3834 3632 220a 2020 2068 6569  29.78462".   hei
+000000b0: 6768 743d 2231 3132 2e34 3830 3031 220a  ght="112.48001".
+000000c0: 2020 2076 6965 7742 6f78 3d22 3020 3020     viewBox="0 0 
+000000d0: 3132 392e 3738 3436 3220 3131 322e 3438  129.78462 112.48
+000000e0: 3030 3122 0a20 2020 736f 6469 706f 6469  001".   sodipodi
+000000f0: 3a64 6f63 6e61 6d65 3d22 6372 6f73 7369  :docname="crossi
+00000100: 6e67 2d33 2d33 3030 2e73 7667 220a 2020  ng-3-300.svg".  
+00000110: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
+00000120: 6e3d 2231 2e32 2e32 2028 6230 6138 3438  n="1.2.2 (b0a848
+00000130: 3635 3431 2c20 3230 3232 2d31 322d 3031  6541, 2022-12-01
+00000140: 2922 0a20 2020 786d 6c6e 733a 696e 6b73  )".   xmlns:inks
+00000150: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
+00000160: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
+00000170: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
+00000180: 6522 0a20 2020 786d 6c6e 733a 736f 6469  e".   xmlns:sodi
+00000190: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
+000001a0: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
+000001b0: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
+000001c0: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
+000001d0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+000001e0: 332e 6f72 672f 3230 3030 2f73 7667 220a  3.org/2000/svg".
+000001f0: 2020 2078 6d6c 6e73 3a73 7667 3d22 6874     xmlns:svg="ht
+00000200: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000210: 3230 3030 2f73 7667 223e 0a20 203c 6465  2000/svg">.  <de
+00000220: 6673 0a20 2020 2020 6964 3d22 6465 6673  fs.     id="defs
+00000230: 3622 202f 3e0a 2020 3c73 6f64 6970 6f64  6" />.  <sodipod
+00000240: 693a 6e61 6d65 6476 6965 770a 2020 2020  i:namedview.    
+00000250: 2069 643d 226e 616d 6564 7669 6577 3422   id="namedview4"
+00000260: 0a20 2020 2020 7061 6765 636f 6c6f 723d  .     pagecolor=
+00000270: 2223 6666 6666 6666 220a 2020 2020 2062  "#ffffff".     b
+00000280: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
+00000290: 3636 3622 0a20 2020 2020 626f 7264 6572  666".     border
+000002a0: 6f70 6163 6974 793d 2231 2e30 220a 2020  opacity="1.0".  
+000002b0: 2020 2069 6e6b 7363 6170 653a 7368 6f77     inkscape:show
+000002c0: 7061 6765 7368 6164 6f77 3d22 3222 0a20  pageshadow="2". 
+000002d0: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
+000002e0: 656f 7061 6369 7479 3d22 302e 3022 0a20  eopacity="0.0". 
+000002f0: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
+00000300: 6563 6865 636b 6572 626f 6172 643d 2230  echeckerboard="0
+00000310: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000320: 6465 736b 636f 6c6f 723d 2223 6431 6431  deskcolor="#d1d1
+00000330: 6431 220a 2020 2020 2073 686f 7767 7269  d1".     showgri
+00000340: 643d 2266 616c 7365 220a 2020 2020 2069  d="false".     i
+00000350: 6e6b 7363 6170 653a 7a6f 6f6d 3d22 312e  nkscape:zoom="1.
+00000360: 3435 3933 3836 3122 0a20 2020 2020 696e  4593861".     in
+00000370: 6b73 6361 7065 3a63 783d 222d 312e 3337  kscape:cx="-1.37
+00000380: 3034 3339 3222 0a20 2020 2020 696e 6b73  04392".     inks
+00000390: 6361 7065 3a63 793d 2231 332e 3031 3931  cape:cy="13.0191
+000003a0: 3733 220a 2020 2020 2069 6e6b 7363 6170  73".     inkscap
+000003b0: 653a 7769 6e64 6f77 2d77 6964 7468 3d22  e:window-width="
+000003c0: 3139 3230 220a 2020 2020 2069 6e6b 7363  1920".     inksc
+000003d0: 6170 653a 7769 6e64 6f77 2d68 6569 6768  ape:window-heigh
+000003e0: 743d 2231 3031 3922 0a20 2020 2020 696e  t="1019".     in
+000003f0: 6b73 6361 7065 3a77 696e 646f 772d 783d  kscape:window-x=
+00000400: 2230 220a 2020 2020 2069 6e6b 7363 6170  "0".     inkscap
+00000410: 653a 7769 6e64 6f77 2d79 3d22 3022 0a20  e:window-y="0". 
+00000420: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+00000430: 646f 772d 6d61 7869 6d69 7a65 643d 2231  dow-maximized="1
+00000440: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000450: 6375 7272 656e 742d 6c61 7965 723d 2267  current-layer="g
+00000460: 3822 202f 3e0a 2020 3c67 0a20 2020 2020  8" />.  <g.     
+00000470: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
+00000480: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
+00000490: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
+000004a0: 496d 6167 6522 0a20 2020 2020 6964 3d22  Image".     id="
+000004b0: 6738 220a 2020 2020 2074 7261 6e73 666f  g8".     transfo
+000004c0: 726d 3d22 7472 616e 736c 6174 6528 302c  rm="translate(0,
+000004d0: 2d32 352e 3536 3838 3034 2922 3e0a 2020  -25.568804)">.  
+000004e0: 2020 3c72 6563 740a 2020 2020 2020 2073    <rect.       s
+000004f0: 7479 6c65 3d22 6669 6c6c 3a23 6666 6666  tyle="fill:#ffff
+00000500: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00000510: 302e 3635 3430 3333 3b73 7472 6f6b 652d  0.654033;stroke-
+00000520: 6c69 6e65 6361 703a 726f 756e 643b 7374  linecap:round;st
+00000530: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6265  roke-linejoin:be
+00000540: 7665 6c22 0a20 2020 2020 2020 6964 3d22  vel".       id="
+00000550: 7265 6374 3238 3722 0a20 2020 2020 2020  rect287".       
+00000560: 7769 6474 683d 2231 3239 2e37 3834 3632  width="129.78462
+00000570: 220a 2020 2020 2020 2068 6569 6768 743d  ".       height=
+00000580: 2231 3132 2e34 3830 3031 220a 2020 2020  "112.48001".    
+00000590: 2020 2078 3d22 3022 0a20 2020 2020 2020     x="0".       
+000005a0: 793d 2232 352e 3536 3838 3034 220a 2020  y="25.568804".  
+000005b0: 2020 2020 2072 793d 2236 2e33 3535 3136       ry="6.35516
+000005c0: 3137 2220 2f3e 0a20 2020 203c 7265 6374  17" />.    <rect
+000005d0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
 000005e0: 696c 6c3a 2330 3030 3030 303b 7374 726f  ill:#000000;stro
-000005f0: 6b65 2d77 6964 7468 3a30 2e37 3535 3930  ke-width:0.75590
-00000600: 363b 7374 726f 6b65 2d6c 696e 6563 6170  6;stroke-linecap
+000005f0: 6b65 2d77 6964 7468 3a30 2e38 3032 3730  ke-width:0.80270
+00000600: 373b 7374 726f 6b65 2d6c 696e 6563 6170  7;stroke-linecap
 00000610: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6c69  :round;stroke-li
 00000620: 6e65 6a6f 696e 3a62 6576 656c 220a 2020  nejoin:bevel".  
-00000630: 2020 2020 2020 2069 643d 2272 6563 7436         id="rect6
-00000640: 3032 220a 2020 2020 2020 2020 2077 6964  02".         wid
-00000650: 7468 3d22 3131 2e38 3631 3735 3622 0a20  th="11.861756". 
-00000660: 2020 2020 2020 2020 6865 6967 6874 3d22          height="
-00000670: 3931 2e38 3139 3135 3322 0a20 2020 2020  91.819153".     
-00000680: 2020 2020 783d 2232 352e 3837 3536 3634      x="25.875664
-00000690: 220a 2020 2020 2020 2020 2079 3d22 3230  ".         y="20
-000006a0: 2e32 3537 3730 3622 202f 3e0a 2020 2020  .257706" />.    
-000006b0: 2020 3c72 6563 740a 2020 2020 2020 2020    <rect.        
-000006c0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
-000006d0: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-000006e0: 683a 302e 3735 3539 3036 3b73 7472 6f6b  h:0.755906;strok
-000006f0: 652d 6c69 6e65 6361 703a 726f 756e 643b  e-linecap:round;
-00000700: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-00000710: 6265 7665 6c22 0a20 2020 2020 2020 2020  bevel".         
-00000720: 6964 3d22 7265 6374 3630 322d 3322 0a20  id="rect602-3". 
-00000730: 2020 2020 2020 2020 7769 6474 683d 2231          width="1
-00000740: 312e 3836 3137 3536 220a 2020 2020 2020  1.861756".      
-00000750: 2020 2068 6569 6768 743d 2239 312e 3831     height="91.81
-00000760: 3931 3533 220a 2020 2020 2020 2020 2078  9153".         x
-00000770: 3d22 3131 312e 3135 3033 3322 0a20 2020  ="111.15033".   
-00000780: 2020 2020 2020 793d 2232 302e 3235 3737        y="20.2577
-00000790: 3036 2220 2f3e 0a20 2020 203c 2f67 3e0a  06" />.    </g>.
-000007a0: 2020 3c2f 673e 0a3c 2f73 7667 3e0a         </g>.</svg>.
+00000630: 2020 2020 2069 643d 2272 6563 7436 3032       id="rect602
+00000640: 2d33 2d37 2d35 220a 2020 2020 2020 2077  -3-7-5".       w
+00000650: 6964 7468 3d22 3132 2e35 3936 3136 3522  idth="12.596165"
+00000660: 0a20 2020 2020 2020 6865 6967 6874 3d22  .       height="
+00000670: 3739 2e34 3434 3735 3622 0a20 2020 2020  79.444756".     
+00000680: 2020 783d 2239 362e 3137 3036 3932 220a    x="96.170692".
+00000690: 2020 2020 2020 2079 3d22 3433 2e30 3936         y="43.096
+000006a0: 3339 3722 202f 3e0a 2020 2020 3c72 6563  397" />.    <rec
+000006b0: 740a 2020 2020 2020 2073 7479 6c65 3d22  t.       style="
+000006c0: 6669 6c6c 3a23 3030 3030 3030 3b73 7472  fill:#000000;str
+000006d0: 6f6b 652d 7769 6474 683a 302e 3830 3237  oke-width:0.8027
+000006e0: 3037 3b73 7472 6f6b 652d 6c69 6e65 6361  07;stroke-lineca
+000006f0: 703a 726f 756e 643b 7374 726f 6b65 2d6c  p:round;stroke-l
+00000700: 696e 656a 6f69 6e3a 6265 7665 6c22 0a20  inejoin:bevel". 
+00000710: 2020 2020 2020 6964 3d22 7265 6374 3630        id="rect60
+00000720: 322d 332d 3722 0a20 2020 2020 2020 7769  2-3-7".       wi
+00000730: 6474 683d 2231 322e 3539 3631 3635 220a  dth="12.596165".
+00000740: 2020 2020 2020 2068 6569 6768 743d 2237         height="7
+00000750: 392e 3434 3437 3536 220a 2020 2020 2020  9.444756".      
+00000760: 2078 3d22 3230 2e30 3535 3431 3222 0a20   x="20.055412". 
+00000770: 2020 2020 2020 793d 2234 332e 3039 3633        y="43.0963
+00000780: 3937 2220 2f3e 0a20 203c 2f67 3e0a 3c2f  97" />.  </g>.</
+00000790: 7376 673e 0a                             svg>.
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/island-300-white.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/island-300.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/island-96-white.svg`

 * *Files 5% similar despite different names*

```diff
@@ -2,93 +2,93 @@
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
-00000080: 2232 352e 346d 6d22 0a20 2020 6865 6967  "25.4mm".   heig
-00000090: 6874 3d22 3235 2e34 6d6d 220a 2020 2076  ht="25.4mm".   v
-000000a0: 6965 7742 6f78 3d22 3020 3020 3235 2e34  iewBox="0 0 25.4
-000000b0: 2032 352e 3422 0a20 2020 7665 7273 696f   25.4".   versio
+00000080: 2231 322e 376d 6d22 0a20 2020 6865 6967  "12.7mm".   heig
+00000090: 6874 3d22 3132 2e37 6d6d 220a 2020 2076  ht="12.7mm".   v
+000000a0: 6965 7742 6f78 3d22 3020 3020 3132 2e37  iewBox="0 0 12.7
+000000b0: 2031 322e 3722 0a20 2020 7665 7273 696f   12.7".   versio
 000000c0: 6e3d 2231 2e31 220a 2020 2069 643d 2273  n="1.1".   id="s
 000000d0: 7667 3522 0a20 2020 696e 6b73 6361 7065  vg5".   inkscape
 000000e0: 3a76 6572 7369 6f6e 3d22 312e 322e 3220  :version="1.2.2 
 000000f0: 2862 3061 3834 3836 3534 312c 2032 3032  (b0a8486541, 202
 00000100: 322d 3132 2d30 3129 220a 2020 2073 6f64  2-12-01)".   sod
 00000110: 6970 6f64 693a 646f 636e 616d 653d 2269  ipodi:docname="i
-00000120: 736c 616e 642e 7376 6722 0a20 2020 786d  sland.svg".   xm
-00000130: 6c6e 733a 696e 6b73 6361 7065 3d22 6874  lns:inkscape="ht
-00000140: 7470 3a2f 2f77 7777 2e69 6e6b 7363 6170  tp://www.inkscap
-00000150: 652e 6f72 672f 6e61 6d65 7370 6163 6573  e.org/namespaces
-00000160: 2f69 6e6b 7363 6170 6522 0a20 2020 786d  /inkscape".   xm
-00000170: 6c6e 733a 736f 6469 706f 6469 3d22 6874  lns:sodipodi="ht
-00000180: 7470 3a2f 2f73 6f64 6970 6f64 692e 736f  tp://sodipodi.so
-00000190: 7572 6365 666f 7267 652e 6e65 742f 4454  urceforge.net/DT
-000001a0: 442f 736f 6469 706f 6469 2d30 2e64 7464  D/sodipodi-0.dtd
-000001b0: 220a 2020 2078 6d6c 6e73 3d22 6874 7470  ".   xmlns="http
-000001c0: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-000001d0: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
-000001e0: 3a73 7667 3d22 6874 7470 3a2f 2f77 7777  :svg="http://www
-000001f0: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00000200: 223e 0a20 203c 736f 6469 706f 6469 3a6e  ">.  <sodipodi:n
-00000210: 616d 6564 7669 6577 0a20 2020 2020 6964  amedview.     id
-00000220: 3d22 6e61 6d65 6476 6965 7737 220a 2020  ="namedview7".  
-00000230: 2020 2070 6167 6563 6f6c 6f72 3d22 2366     pagecolor="#f
-00000240: 6666 6666 6622 0a20 2020 2020 626f 7264  fffff".     bord
-00000250: 6572 636f 6c6f 723d 2223 3636 3636 3636  ercolor="#666666
-00000260: 220a 2020 2020 2062 6f72 6465 726f 7061  ".     borderopa
-00000270: 6369 7479 3d22 312e 3022 0a20 2020 2020  city="1.0".     
-00000280: 696e 6b73 6361 7065 3a73 686f 7770 6167  inkscape:showpag
-00000290: 6573 6861 646f 773d 2232 220a 2020 2020  eshadow="2".    
-000002a0: 2069 6e6b 7363 6170 653a 7061 6765 6f70   inkscape:pageop
-000002b0: 6163 6974 793d 2230 2e30 220a 2020 2020  acity="0.0".    
-000002c0: 2069 6e6b 7363 6170 653a 7061 6765 6368   inkscape:pagech
-000002d0: 6563 6b65 7262 6f61 7264 3d22 3022 0a20  eckerboard="0". 
-000002e0: 2020 2020 696e 6b73 6361 7065 3a64 6573      inkscape:des
-000002f0: 6b63 6f6c 6f72 3d22 2364 3164 3164 3122  kcolor="#d1d1d1"
-00000300: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
-00000310: 6f63 756d 656e 742d 756e 6974 733d 226d  ocument-units="m
-00000320: 6d22 0a20 2020 2020 7368 6f77 6772 6964  m".     showgrid
-00000330: 3d22 6661 6c73 6522 0a20 2020 2020 696e  ="false".     in
-00000340: 6b73 6361 7065 3a7a 6f6f 6d3d 2232 2e31  kscape:zoom="2.1
-00000350: 3934 3636 3938 220a 2020 2020 2069 6e6b  946698".     ink
-00000360: 7363 6170 653a 6378 3d22 3135 312e 3237  scape:cx="151.27
-00000370: 3536 3122 0a20 2020 2020 696e 6b73 6361  561".     inksca
-00000380: 7065 3a63 793d 2233 352e 3534 3036 3534  pe:cy="35.540654
-00000390: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000003a0: 7769 6e64 6f77 2d77 6964 7468 3d22 3139  window-width="19
-000003b0: 3230 220a 2020 2020 2069 6e6b 7363 6170  20".     inkscap
-000003c0: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
-000003d0: 2231 3035 3122 0a20 2020 2020 696e 6b73  "1051".     inks
-000003e0: 6361 7065 3a77 696e 646f 772d 783d 2230  cape:window-x="0
-000003f0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000400: 7769 6e64 6f77 2d79 3d22 3130 3830 220a  window-y="1080".
-00000410: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
-00000420: 6e64 6f77 2d6d 6178 696d 697a 6564 3d22  ndow-maximized="
-00000430: 3122 0a20 2020 2020 696e 6b73 6361 7065  1".     inkscape
-00000440: 3a63 7572 7265 6e74 2d6c 6179 6572 3d22  :current-layer="
-00000450: 6c61 7965 7231 2220 2f3e 0a20 203c 6465  layer1" />.  <de
-00000460: 6673 0a20 2020 2020 6964 3d22 6465 6673  fs.     id="defs
-00000470: 3222 202f 3e0a 2020 3c67 0a20 2020 2020  2" />.  <g.     
-00000480: 696e 6b73 6361 7065 3a6c 6162 656c 3d22  inkscape:label="
-00000490: 4361 6c71 7565 2031 220a 2020 2020 2069  Calque 1".     i
-000004a0: 6e6b 7363 6170 653a 6772 6f75 706d 6f64  nkscape:groupmod
-000004b0: 653d 226c 6179 6572 220a 2020 2020 2069  e="layer".     i
-000004c0: 643d 226c 6179 6572 3122 0a20 2020 2020  d="layer1".     
-000004d0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-000004e0: 6c61 7465 282d 3235 2e33 3939 3939 392c  late(-25.399999,
-000004f0: 2d32 352e 3339 3939 3939 2922 3e0a 2020  -25.399999)">.  
-00000500: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00000510: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
-00000520: 3030 3030 3b73 7472 6f6b 653a 6e6f 6e65  0000;stroke:none
-00000530: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00000540: 3039 3434 3333 383b 7374 726f 6b65 2d6c  0944338;stroke-l
-00000550: 696e 6563 6170 3a72 6f75 6e64 3b73 7472  inecap:round;str
-00000560: 6f6b 652d 6c69 6e65 6a6f 696e 3a62 6576  oke-linejoin:bev
-00000570: 656c 220a 2020 2020 2020 2069 643d 2270  el".       id="p
-00000580: 6174 6832 3334 220a 2020 2020 2020 2063  ath234".       c
-00000590: 783d 2233 382e 3039 3939 3938 220a 2020  x="38.099998".  
-000005a0: 2020 2020 2063 793d 2233 382e 3039 3939       cy="38.0999
-000005b0: 3938 220a 2020 2020 2020 2072 3d22 3132  98".       r="12
-000005c0: 2e37 2220 2f3e 0a20 203c 2f67 3e0a 3c2f  .7" />.  </g>.</
-000005d0: 7376 673e 0a                             svg>.
+00000120: 736c 616e 642d 3936 2d77 6869 7465 2e73  sland-96-white.s
+00000130: 7667 220a 2020 2078 6d6c 6e73 3a69 6e6b  vg".   xmlns:ink
+00000140: 7363 6170 653d 2268 7474 703a 2f2f 7777  scape="http://ww
+00000150: 772e 696e 6b73 6361 7065 2e6f 7267 2f6e  w.inkscape.org/n
+00000160: 616d 6573 7061 6365 732f 696e 6b73 6361  amespaces/inksca
+00000170: 7065 220a 2020 2078 6d6c 6e73 3a73 6f64  pe".   xmlns:sod
+00000180: 6970 6f64 693d 2268 7474 703a 2f2f 736f  ipodi="http://so
+00000190: 6469 706f 6469 2e73 6f75 7263 6566 6f72  dipodi.sourcefor
+000001a0: 6765 2e6e 6574 2f44 5444 2f73 6f64 6970  ge.net/DTD/sodip
+000001b0: 6f64 692d 302e 6474 6422 0a20 2020 786d  odi-0.dtd".   xm
+000001c0: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
+000001d0: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
+000001e0: 0a20 2020 786d 6c6e 733a 7376 673d 2268  .   xmlns:svg="h
+000001f0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
+00000200: 2f32 3030 302f 7376 6722 3e0a 2020 3c73  /2000/svg">.  <s
+00000210: 6f64 6970 6f64 693a 6e61 6d65 6476 6965  odipodi:namedvie
+00000220: 770a 2020 2020 2069 643d 226e 616d 6564  w.     id="named
+00000230: 7669 6577 3722 0a20 2020 2020 7061 6765  view7".     page
+00000240: 636f 6c6f 723d 2223 6666 6666 6666 220a  color="#ffffff".
+00000250: 2020 2020 2062 6f72 6465 7263 6f6c 6f72       bordercolor
+00000260: 3d22 2336 3636 3636 3622 0a20 2020 2020  ="#666666".     
+00000270: 626f 7264 6572 6f70 6163 6974 793d 2231  borderopacity="1
+00000280: 2e30 220a 2020 2020 2069 6e6b 7363 6170  .0".     inkscap
+00000290: 653a 7368 6f77 7061 6765 7368 6164 6f77  e:showpageshadow
+000002a0: 3d22 3222 0a20 2020 2020 696e 6b73 6361  ="2".     inksca
+000002b0: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
+000002c0: 302e 3022 0a20 2020 2020 696e 6b73 6361  0.0".     inksca
+000002d0: 7065 3a70 6167 6563 6865 636b 6572 626f  pe:pagecheckerbo
+000002e0: 6172 643d 2230 220a 2020 2020 2069 6e6b  ard="0".     ink
+000002f0: 7363 6170 653a 6465 736b 636f 6c6f 723d  scape:deskcolor=
+00000300: 2223 6431 6431 6431 220a 2020 2020 2069  "#d1d1d1".     i
+00000310: 6e6b 7363 6170 653a 646f 6375 6d65 6e74  nkscape:document
+00000320: 2d75 6e69 7473 3d22 6d6d 220a 2020 2020  -units="mm".    
+00000330: 2073 686f 7767 7269 643d 2266 616c 7365   showgrid="false
+00000340: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000350: 7a6f 6f6d 3d22 322e 3139 3436 3639 3822  zoom="2.1946698"
+00000360: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
+00000370: 783d 2239 382e 3634 3830 3937 220a 2020  x="98.648097".  
+00000380: 2020 2069 6e6b 7363 6170 653a 6379 3d22     inkscape:cy="
+00000390: 3636 2e39 3830 3436 3322 0a20 2020 2020  66.980463".     
+000003a0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+000003b0: 7769 6474 683d 2231 3932 3022 0a20 2020  width="1920".   
+000003c0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
+000003d0: 772d 6865 6967 6874 3d22 3130 3139 220a  w-height="1019".
+000003e0: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
+000003f0: 6e64 6f77 2d78 3d22 3022 0a20 2020 2020  ndow-x="0".     
+00000400: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+00000410: 793d 2230 220a 2020 2020 2069 6e6b 7363  y="0".     inksc
+00000420: 6170 653a 7769 6e64 6f77 2d6d 6178 696d  ape:window-maxim
+00000430: 697a 6564 3d22 3122 0a20 2020 2020 696e  ized="1".     in
+00000440: 6b73 6361 7065 3a63 7572 7265 6e74 2d6c  kscape:current-l
+00000450: 6179 6572 3d22 6c61 7965 7231 2220 2f3e  ayer="layer1" />
+00000460: 0a20 203c 6465 6673 0a20 2020 2020 6964  .  <defs.     id
+00000470: 3d22 6465 6673 3222 202f 3e0a 2020 3c67  ="defs2" />.  <g
+00000480: 0a20 2020 2020 696e 6b73 6361 7065 3a6c  .     inkscape:l
+00000490: 6162 656c 3d22 4361 6c71 7565 2031 220a  abel="Calque 1".
+000004a0: 2020 2020 2069 6e6b 7363 6170 653a 6772       inkscape:gr
+000004b0: 6f75 706d 6f64 653d 226c 6179 6572 220a  oupmode="layer".
+000004c0: 2020 2020 2069 643d 226c 6179 6572 3122       id="layer1"
+000004d0: 0a20 2020 2020 7472 616e 7366 6f72 6d3d  .     transform=
+000004e0: 2274 7261 6e73 6c61 7465 282d 3235 2e33  "translate(-25.3
+000004f0: 3939 3939 382c 2d32 352e 3339 3939 3938  99998,-25.399998
+00000500: 2922 3e0a 2020 2020 3c63 6972 636c 650a  )">.    <circle.
+00000510: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00000520: 6c6c 3a23 6666 6666 6666 3b73 7472 6f6b  ll:#ffffff;strok
+00000530: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
+00000540: 6474 683a 302e 3034 3732 3136 373b 7374  dth:0.0472167;st
+00000550: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
+00000560: 6e64 3b73 7472 6f6b 652d 6c69 6e65 6a6f  nd;stroke-linejo
+00000570: 696e 3a62 6576 656c 220a 2020 2020 2020  in:bevel".      
+00000580: 2069 643d 2270 6174 6832 3334 220a 2020   id="path234".  
+00000590: 2020 2020 2063 783d 2233 312e 3734 3939       cx="31.7499
+000005a0: 3938 220a 2020 2020 2020 2063 793d 2233  98".       cy="3
+000005b0: 312e 3734 3939 3938 220a 2020 2020 2020  1.749998".      
+000005c0: 2072 3d22 362e 3334 3939 3939 3922 202f   r="6.3499999" /
+000005d0: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/island-96-white.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/island-96.svg`

 * *Files 9% similar despite different names*

```diff
@@ -2,93 +2,94 @@
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
-00000080: 2231 322e 376d 6d22 0a20 2020 6865 6967  "12.7mm".   heig
-00000090: 6874 3d22 3132 2e37 6d6d 220a 2020 2076  ht="12.7mm".   v
-000000a0: 6965 7742 6f78 3d22 3020 3020 3132 2e37  iewBox="0 0 12.7
-000000b0: 2031 322e 3722 0a20 2020 7665 7273 696f   12.7".   versio
-000000c0: 6e3d 2231 2e31 220a 2020 2069 643d 2273  n="1.1".   id="s
-000000d0: 7667 3522 0a20 2020 696e 6b73 6361 7065  vg5".   inkscape
-000000e0: 3a76 6572 7369 6f6e 3d22 312e 322e 3220  :version="1.2.2 
-000000f0: 2862 3061 3834 3836 3534 312c 2032 3032  (b0a8486541, 202
-00000100: 322d 3132 2d30 3129 220a 2020 2073 6f64  2-12-01)".   sod
-00000110: 6970 6f64 693a 646f 636e 616d 653d 2269  ipodi:docname="i
-00000120: 736c 616e 642d 3936 2d77 6869 7465 2e73  sland-96-white.s
-00000130: 7667 220a 2020 2078 6d6c 6e73 3a69 6e6b  vg".   xmlns:ink
-00000140: 7363 6170 653d 2268 7474 703a 2f2f 7777  scape="http://ww
-00000150: 772e 696e 6b73 6361 7065 2e6f 7267 2f6e  w.inkscape.org/n
-00000160: 616d 6573 7061 6365 732f 696e 6b73 6361  amespaces/inksca
-00000170: 7065 220a 2020 2078 6d6c 6e73 3a73 6f64  pe".   xmlns:sod
-00000180: 6970 6f64 693d 2268 7474 703a 2f2f 736f  ipodi="http://so
-00000190: 6469 706f 6469 2e73 6f75 7263 6566 6f72  dipodi.sourcefor
-000001a0: 6765 2e6e 6574 2f44 5444 2f73 6f64 6970  ge.net/DTD/sodip
-000001b0: 6f64 692d 302e 6474 6422 0a20 2020 786d  odi-0.dtd".   xm
-000001c0: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
-000001d0: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
-000001e0: 0a20 2020 786d 6c6e 733a 7376 673d 2268  .   xmlns:svg="h
-000001f0: 7474 703a 2f2f 7777 772e 7733 2e6f 7267  ttp://www.w3.org
-00000200: 2f32 3030 302f 7376 6722 3e0a 2020 3c73  /2000/svg">.  <s
-00000210: 6f64 6970 6f64 693a 6e61 6d65 6476 6965  odipodi:namedvie
-00000220: 770a 2020 2020 2069 643d 226e 616d 6564  w.     id="named
-00000230: 7669 6577 3722 0a20 2020 2020 7061 6765  view7".     page
-00000240: 636f 6c6f 723d 2223 6666 6666 6666 220a  color="#ffffff".
-00000250: 2020 2020 2062 6f72 6465 7263 6f6c 6f72       bordercolor
-00000260: 3d22 2336 3636 3636 3622 0a20 2020 2020  ="#666666".     
-00000270: 626f 7264 6572 6f70 6163 6974 793d 2231  borderopacity="1
-00000280: 2e30 220a 2020 2020 2069 6e6b 7363 6170  .0".     inkscap
-00000290: 653a 7368 6f77 7061 6765 7368 6164 6f77  e:showpageshadow
-000002a0: 3d22 3222 0a20 2020 2020 696e 6b73 6361  ="2".     inksca
-000002b0: 7065 3a70 6167 656f 7061 6369 7479 3d22  pe:pageopacity="
-000002c0: 302e 3022 0a20 2020 2020 696e 6b73 6361  0.0".     inksca
-000002d0: 7065 3a70 6167 6563 6865 636b 6572 626f  pe:pagecheckerbo
-000002e0: 6172 643d 2230 220a 2020 2020 2069 6e6b  ard="0".     ink
-000002f0: 7363 6170 653a 6465 736b 636f 6c6f 723d  scape:deskcolor=
-00000300: 2223 6431 6431 6431 220a 2020 2020 2069  "#d1d1d1".     i
-00000310: 6e6b 7363 6170 653a 646f 6375 6d65 6e74  nkscape:document
-00000320: 2d75 6e69 7473 3d22 6d6d 220a 2020 2020  -units="mm".    
-00000330: 2073 686f 7767 7269 643d 2266 616c 7365   showgrid="false
-00000340: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000350: 7a6f 6f6d 3d22 322e 3139 3436 3639 3822  zoom="2.1946698"
-00000360: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
-00000370: 783d 2239 382e 3634 3830 3937 220a 2020  x="98.648097".  
-00000380: 2020 2069 6e6b 7363 6170 653a 6379 3d22     inkscape:cy="
-00000390: 3636 2e39 3830 3436 3322 0a20 2020 2020  66.980463".     
-000003a0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-000003b0: 7769 6474 683d 2231 3932 3022 0a20 2020  width="1920".   
-000003c0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-000003d0: 772d 6865 6967 6874 3d22 3130 3139 220a  w-height="1019".
-000003e0: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
-000003f0: 6e64 6f77 2d78 3d22 3022 0a20 2020 2020  ndow-x="0".     
-00000400: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-00000410: 793d 2230 220a 2020 2020 2069 6e6b 7363  y="0".     inksc
-00000420: 6170 653a 7769 6e64 6f77 2d6d 6178 696d  ape:window-maxim
-00000430: 697a 6564 3d22 3122 0a20 2020 2020 696e  ized="1".     in
-00000440: 6b73 6361 7065 3a63 7572 7265 6e74 2d6c  kscape:current-l
-00000450: 6179 6572 3d22 6c61 7965 7231 2220 2f3e  ayer="layer1" />
-00000460: 0a20 203c 6465 6673 0a20 2020 2020 6964  .  <defs.     id
-00000470: 3d22 6465 6673 3222 202f 3e0a 2020 3c67  ="defs2" />.  <g
-00000480: 0a20 2020 2020 696e 6b73 6361 7065 3a6c  .     inkscape:l
-00000490: 6162 656c 3d22 4361 6c71 7565 2031 220a  abel="Calque 1".
-000004a0: 2020 2020 2069 6e6b 7363 6170 653a 6772       inkscape:gr
-000004b0: 6f75 706d 6f64 653d 226c 6179 6572 220a  oupmode="layer".
-000004c0: 2020 2020 2069 643d 226c 6179 6572 3122       id="layer1"
-000004d0: 0a20 2020 2020 7472 616e 7366 6f72 6d3d  .     transform=
-000004e0: 2274 7261 6e73 6c61 7465 282d 3235 2e33  "translate(-25.3
-000004f0: 3939 3939 382c 2d32 352e 3339 3939 3938  99998,-25.399998
-00000500: 2922 3e0a 2020 2020 3c63 6972 636c 650a  )">.    <circle.
-00000510: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00000520: 6c6c 3a23 6666 6666 6666 3b73 7472 6f6b  ll:#ffffff;strok
-00000530: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00000540: 6474 683a 302e 3034 3732 3136 373b 7374  dth:0.0472167;st
-00000550: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
-00000560: 6e64 3b73 7472 6f6b 652d 6c69 6e65 6a6f  nd;stroke-linejo
-00000570: 696e 3a62 6576 656c 220a 2020 2020 2020  in:bevel".      
-00000580: 2069 643d 2270 6174 6832 3334 220a 2020   id="path234".  
-00000590: 2020 2020 2063 783d 2233 312e 3734 3939       cx="31.7499
-000005a0: 3938 220a 2020 2020 2020 2063 793d 2233  98".       cy="3
-000005b0: 312e 3734 3939 3938 220a 2020 2020 2020  1.749998".      
-000005c0: 2072 3d22 362e 3334 3939 3939 3922 202f   r="6.3499999" /
-000005d0: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
+00000080: 2236 2e39 3336 3038 3333 6d6d 220a 2020  "6.9360833mm".  
+00000090: 2068 6569 6768 743d 2236 2e39 3336 3038   height="6.93608
+000000a0: 3333 6d6d 220a 2020 2076 6965 7742 6f78  33mm".   viewBox
+000000b0: 3d22 3020 3020 362e 3933 3630 3833 3420  ="0 0 6.9360834 
+000000c0: 362e 3933 3630 3833 3422 0a20 2020 7665  6.9360834".   ve
+000000d0: 7273 696f 6e3d 2231 2e31 220a 2020 2069  rsion="1.1".   i
+000000e0: 643d 2273 7667 3522 0a20 2020 696e 6b73  d="svg5".   inks
+000000f0: 6361 7065 3a76 6572 7369 6f6e 3d22 312e  cape:version="1.
+00000100: 322e 3220 2862 3061 3834 3836 3534 312c  2.2 (b0a8486541,
+00000110: 2032 3032 322d 3132 2d30 3129 220a 2020   2022-12-01)".  
+00000120: 2073 6f64 6970 6f64 693a 646f 636e 616d   sodipodi:docnam
+00000130: 653d 2269 736c 616e 642d 3936 2e73 7667  e="island-96.svg
+00000140: 220a 2020 2078 6d6c 6e73 3a69 6e6b 7363  ".   xmlns:inksc
+00000150: 6170 653d 2268 7474 703a 2f2f 7777 772e  ape="http://www.
+00000160: 696e 6b73 6361 7065 2e6f 7267 2f6e 616d  inkscape.org/nam
+00000170: 6573 7061 6365 732f 696e 6b73 6361 7065  espaces/inkscape
+00000180: 220a 2020 2078 6d6c 6e73 3a73 6f64 6970  ".   xmlns:sodip
+00000190: 6f64 693d 2268 7474 703a 2f2f 736f 6469  odi="http://sodi
+000001a0: 706f 6469 2e73 6f75 7263 6566 6f72 6765  podi.sourceforge
+000001b0: 2e6e 6574 2f44 5444 2f73 6f64 6970 6f64  .net/DTD/sodipod
+000001c0: 692d 302e 6474 6422 0a20 2020 786d 6c6e  i-0.dtd".   xmln
+000001d0: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
+000001e0: 2e6f 7267 2f32 3030 302f 7376 6722 0a20  .org/2000/svg". 
+000001f0: 2020 786d 6c6e 733a 7376 673d 2268 7474    xmlns:svg="htt
+00000200: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
+00000210: 3030 302f 7376 6722 3e0a 2020 3c73 6f64  000/svg">.  <sod
+00000220: 6970 6f64 693a 6e61 6d65 6476 6965 770a  ipodi:namedview.
+00000230: 2020 2020 2069 643d 226e 616d 6564 7669       id="namedvi
+00000240: 6577 3722 0a20 2020 2020 7061 6765 636f  ew7".     pageco
+00000250: 6c6f 723d 2223 6666 6666 6666 220a 2020  lor="#ffffff".  
+00000260: 2020 2062 6f72 6465 7263 6f6c 6f72 3d22     bordercolor="
+00000270: 2336 3636 3636 3622 0a20 2020 2020 626f  #666666".     bo
+00000280: 7264 6572 6f70 6163 6974 793d 2231 2e30  rderopacity="1.0
+00000290: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+000002a0: 7368 6f77 7061 6765 7368 6164 6f77 3d22  showpageshadow="
+000002b0: 3222 0a20 2020 2020 696e 6b73 6361 7065  2".     inkscape
+000002c0: 3a70 6167 656f 7061 6369 7479 3d22 302e  :pageopacity="0.
+000002d0: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
+000002e0: 3a70 6167 6563 6865 636b 6572 626f 6172  :pagecheckerboar
+000002f0: 643d 2230 220a 2020 2020 2069 6e6b 7363  d="0".     inksc
+00000300: 6170 653a 6465 736b 636f 6c6f 723d 2223  ape:deskcolor="#
+00000310: 6431 6431 6431 220a 2020 2020 2069 6e6b  d1d1d1".     ink
+00000320: 7363 6170 653a 646f 6375 6d65 6e74 2d75  scape:document-u
+00000330: 6e69 7473 3d22 6d6d 220a 2020 2020 2073  nits="mm".     s
+00000340: 686f 7767 7269 643d 2266 616c 7365 220a  howgrid="false".
+00000350: 2020 2020 2069 6e6b 7363 6170 653a 7a6f       inkscape:zo
+00000360: 6f6d 3d22 362e 3230 3734 3633 3622 0a20  om="6.2074636". 
+00000370: 2020 2020 696e 6b73 6361 7065 3a63 783d      inkscape:cx=
+00000380: 2233 362e 3430 3737 3835 220a 2020 2020  "36.407785".    
+00000390: 2069 6e6b 7363 6170 653a 6379 3d22 3139   inkscape:cy="19
+000003a0: 2e31 3730 3437 3122 0a20 2020 2020 696e  .170471".     in
+000003b0: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
+000003c0: 6474 683d 2231 3932 3022 0a20 2020 2020  dth="1920".     
+000003d0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+000003e0: 6865 6967 6874 3d22 3130 3139 220a 2020  height="1019".  
+000003f0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+00000400: 6f77 2d78 3d22 3022 0a20 2020 2020 696e  ow-x="0".     in
+00000410: 6b73 6361 7065 3a77 696e 646f 772d 793d  kscape:window-y=
+00000420: 2230 220a 2020 2020 2069 6e6b 7363 6170  "0".     inkscap
+00000430: 653a 7769 6e64 6f77 2d6d 6178 696d 697a  e:window-maximiz
+00000440: 6564 3d22 3122 0a20 2020 2020 696e 6b73  ed="1".     inks
+00000450: 6361 7065 3a63 7572 7265 6e74 2d6c 6179  cape:current-lay
+00000460: 6572 3d22 6c61 7965 7231 2220 2f3e 0a20  er="layer1" />. 
+00000470: 203c 6465 6673 0a20 2020 2020 6964 3d22   <defs.     id="
+00000480: 6465 6673 3222 202f 3e0a 2020 3c67 0a20  defs2" />.  <g. 
+00000490: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
+000004a0: 656c 3d22 4361 6c71 7565 2031 220a 2020  el="Calque 1".  
+000004b0: 2020 2069 6e6b 7363 6170 653a 6772 6f75     inkscape:grou
+000004c0: 706d 6f64 653d 226c 6179 6572 220a 2020  pmode="layer".  
+000004d0: 2020 2069 643d 226c 6179 6572 3122 0a20     id="layer1". 
+000004e0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
+000004f0: 7261 6e73 6c61 7465 282d 3236 2e31 3635  ranslate(-26.165
+00000500: 3239 2c2d 3236 2e31 3635 3239 2922 3e0a  29,-26.16529)">.
+00000510: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
+00000520: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00000530: 3030 3030 3030 3b73 7472 6f6b 653a 6e6f  000000;stroke:no
+00000540: 6e65 3b73 7472 6f6b 652d 7769 6474 683a  ne;stroke-width:
+00000550: 302e 3032 3537 3837 343b 7374 726f 6b65  0.0257874;stroke
+00000560: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
+00000570: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a62  troke-linejoin:b
+00000580: 6576 656c 220a 2020 2020 2020 2069 643d  evel".       id=
+00000590: 2270 6174 6832 3334 220a 2020 2020 2020  "path234".      
+000005a0: 2063 783d 2232 392e 3633 3333 3331 220a   cx="29.633331".
+000005b0: 2020 2020 2020 2063 793d 2232 392e 3633         cy="29.63
+000005c0: 3333 3331 220a 2020 2020 2020 2072 3d22  3331".       r="
+000005d0: 332e 3436 3830 3431 3722 202f 3e0a 2020  3.4680417" />.  
+000005e0: 3c2f 673e 0a3c 2f73 7667 3e0a            </g>.</svg>.
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/island-96.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/island-300.svg`

 * *Files 12% similar despite different names*

```diff
@@ -2,94 +2,94 @@
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
-00000080: 2238 2e34 3636 3636 3632 6d6d 220a 2020  "8.4666662mm".  
-00000090: 2068 6569 6768 743d 2238 2e34 3636 3636   height="8.46666
-000000a0: 3632 6d6d 220a 2020 2076 6965 7742 6f78  62mm".   viewBox
-000000b0: 3d22 3020 3020 382e 3436 3636 3636 3320  ="0 0 8.4666663 
-000000c0: 382e 3436 3636 3636 3322 0a20 2020 7665  8.4666663".   ve
+00000080: 2232 312e 3330 3838 3436 6d6d 220a 2020  "21.308846mm".  
+00000090: 2068 6569 6768 743d 2232 312e 3330 3838   height="21.3088
+000000a0: 3436 6d6d 220a 2020 2076 6965 7742 6f78  46mm".   viewBox
+000000b0: 3d22 3020 3020 3231 2e33 3038 3834 3620  ="0 0 21.308846 
+000000c0: 3231 2e33 3038 3834 3622 0a20 2020 7665  21.308846".   ve
 000000d0: 7273 696f 6e3d 2231 2e31 220a 2020 2069  rsion="1.1".   i
 000000e0: 643d 2273 7667 3522 0a20 2020 696e 6b73  d="svg5".   inks
 000000f0: 6361 7065 3a76 6572 7369 6f6e 3d22 312e  cape:version="1.
 00000100: 322e 3220 2862 3061 3834 3836 3534 312c  2.2 (b0a8486541,
 00000110: 2032 3032 322d 3132 2d30 3129 220a 2020   2022-12-01)".  
 00000120: 2073 6f64 6970 6f64 693a 646f 636e 616d   sodipodi:docnam
-00000130: 653d 2269 736c 616e 642d 3936 2e73 7667  e="island-96.svg
-00000140: 220a 2020 2078 6d6c 6e73 3a69 6e6b 7363  ".   xmlns:inksc
-00000150: 6170 653d 2268 7474 703a 2f2f 7777 772e  ape="http://www.
-00000160: 696e 6b73 6361 7065 2e6f 7267 2f6e 616d  inkscape.org/nam
-00000170: 6573 7061 6365 732f 696e 6b73 6361 7065  espaces/inkscape
-00000180: 220a 2020 2078 6d6c 6e73 3a73 6f64 6970  ".   xmlns:sodip
-00000190: 6f64 693d 2268 7474 703a 2f2f 736f 6469  odi="http://sodi
-000001a0: 706f 6469 2e73 6f75 7263 6566 6f72 6765  podi.sourceforge
-000001b0: 2e6e 6574 2f44 5444 2f73 6f64 6970 6f64  .net/DTD/sodipod
-000001c0: 692d 302e 6474 6422 0a20 2020 786d 6c6e  i-0.dtd".   xmln
-000001d0: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-000001e0: 2e6f 7267 2f32 3030 302f 7376 6722 0a20  .org/2000/svg". 
-000001f0: 2020 786d 6c6e 733a 7376 673d 2268 7474    xmlns:svg="htt
-00000200: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
-00000210: 3030 302f 7376 6722 3e0a 2020 3c73 6f64  000/svg">.  <sod
-00000220: 6970 6f64 693a 6e61 6d65 6476 6965 770a  ipodi:namedview.
-00000230: 2020 2020 2069 643d 226e 616d 6564 7669       id="namedvi
-00000240: 6577 3722 0a20 2020 2020 7061 6765 636f  ew7".     pageco
-00000250: 6c6f 723d 2223 6666 6666 6666 220a 2020  lor="#ffffff".  
-00000260: 2020 2062 6f72 6465 7263 6f6c 6f72 3d22     bordercolor="
-00000270: 2336 3636 3636 3622 0a20 2020 2020 626f  #666666".     bo
-00000280: 7264 6572 6f70 6163 6974 793d 2231 2e30  rderopacity="1.0
-00000290: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000002a0: 7368 6f77 7061 6765 7368 6164 6f77 3d22  showpageshadow="
-000002b0: 3222 0a20 2020 2020 696e 6b73 6361 7065  2".     inkscape
-000002c0: 3a70 6167 656f 7061 6369 7479 3d22 302e  :pageopacity="0.
-000002d0: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
-000002e0: 3a70 6167 6563 6865 636b 6572 626f 6172  :pagecheckerboar
-000002f0: 643d 2230 220a 2020 2020 2069 6e6b 7363  d="0".     inksc
-00000300: 6170 653a 6465 736b 636f 6c6f 723d 2223  ape:deskcolor="#
-00000310: 6431 6431 6431 220a 2020 2020 2069 6e6b  d1d1d1".     ink
-00000320: 7363 6170 653a 646f 6375 6d65 6e74 2d75  scape:document-u
-00000330: 6e69 7473 3d22 6d6d 220a 2020 2020 2073  nits="mm".     s
-00000340: 686f 7767 7269 643d 2266 616c 7365 220a  howgrid="false".
-00000350: 2020 2020 2069 6e6b 7363 6170 653a 7a6f       inkscape:zo
-00000360: 6f6d 3d22 322e 3139 3436 3639 3822 0a20  om="2.1946698". 
-00000370: 2020 2020 696e 6b73 6361 7065 3a63 783d      inkscape:cx=
-00000380: 2231 3236 2e32 3134 3839 220a 2020 2020  "126.21489".    
-00000390: 2069 6e6b 7363 6170 653a 6379 3d22 3335   inkscape:cy="35
-000003a0: 2e39 3936 3330 3322 0a20 2020 2020 696e  .996303".     in
-000003b0: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
-000003c0: 6474 683d 2231 3932 3022 0a20 2020 2020  dth="1920".     
-000003d0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-000003e0: 6865 6967 6874 3d22 3130 3139 220a 2020  height="1019".  
-000003f0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-00000400: 6f77 2d78 3d22 3022 0a20 2020 2020 696e  ow-x="0".     in
-00000410: 6b73 6361 7065 3a77 696e 646f 772d 793d  kscape:window-y=
-00000420: 2230 220a 2020 2020 2069 6e6b 7363 6170  "0".     inkscap
-00000430: 653a 7769 6e64 6f77 2d6d 6178 696d 697a  e:window-maximiz
-00000440: 6564 3d22 3122 0a20 2020 2020 696e 6b73  ed="1".     inks
-00000450: 6361 7065 3a63 7572 7265 6e74 2d6c 6179  cape:current-lay
-00000460: 6572 3d22 6c61 7965 7231 2220 2f3e 0a20  er="layer1" />. 
-00000470: 203c 6465 6673 0a20 2020 2020 6964 3d22   <defs.     id="
-00000480: 6465 6673 3222 202f 3e0a 2020 3c67 0a20  defs2" />.  <g. 
-00000490: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
-000004a0: 656c 3d22 4361 6c71 7565 2031 220a 2020  el="Calque 1".  
-000004b0: 2020 2069 6e6b 7363 6170 653a 6772 6f75     inkscape:grou
-000004c0: 706d 6f64 653d 226c 6179 6572 220a 2020  pmode="layer".  
-000004d0: 2020 2069 643d 226c 6179 6572 3122 0a20     id="layer1". 
-000004e0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
-000004f0: 7261 6e73 6c61 7465 282d 3235 2e33 3939  ranslate(-25.399
-00000500: 3939 382c 2d32 352e 3339 3939 3938 2922  998,-25.399998)"
-00000510: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
-00000520: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00000530: 3a23 3030 3030 3030 3b73 7472 6f6b 653a  :#000000;stroke:
-00000540: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
-00000550: 683a 302e 3033 3134 3737 393b 7374 726f  h:0.0314779;stro
-00000560: 6b65 2d6c 696e 6563 6170 3a72 6f75 6e64  ke-linecap:round
-00000570: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00000580: 3a62 6576 656c 220a 2020 2020 2020 2069  :bevel".       i
-00000590: 643d 2270 6174 6832 3334 220a 2020 2020  d="path234".    
-000005a0: 2020 2063 783d 2232 392e 3633 3333 3331     cx="29.633331
-000005b0: 220a 2020 2020 2020 2063 793d 2232 392e  ".       cy="29.
-000005c0: 3633 3333 3331 220a 2020 2020 2020 2072  633331".       r
-000005d0: 3d22 342e 3233 3333 3333 3122 202f 3e0a  ="4.2333331" />.
-000005e0: 2020 3c2f 673e 0a3c 2f73 7667 3e0a         </g>.</svg>.
+00000130: 653d 2269 736c 616e 642d 3330 302e 7376  e="island-300.sv
+00000140: 6722 0a20 2020 786d 6c6e 733a 696e 6b73  g".   xmlns:inks
+00000150: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
+00000160: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
+00000170: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
+00000180: 6522 0a20 2020 786d 6c6e 733a 736f 6469  e".   xmlns:sodi
+00000190: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
+000001a0: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
+000001b0: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
+000001c0: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
+000001d0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+000001e0: 332e 6f72 672f 3230 3030 2f73 7667 220a  3.org/2000/svg".
+000001f0: 2020 2078 6d6c 6e73 3a73 7667 3d22 6874     xmlns:svg="ht
+00000200: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000210: 3230 3030 2f73 7667 223e 0a20 203c 736f  2000/svg">.  <so
+00000220: 6469 706f 6469 3a6e 616d 6564 7669 6577  dipodi:namedview
+00000230: 0a20 2020 2020 6964 3d22 6e61 6d65 6476  .     id="namedv
+00000240: 6965 7737 220a 2020 2020 2070 6167 6563  iew7".     pagec
+00000250: 6f6c 6f72 3d22 2366 6666 6666 6622 0a20  olor="#ffffff". 
+00000260: 2020 2020 626f 7264 6572 636f 6c6f 723d      bordercolor=
+00000270: 2223 3636 3636 3636 220a 2020 2020 2062  "#666666".     b
+00000280: 6f72 6465 726f 7061 6369 7479 3d22 312e  orderopacity="1.
+00000290: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
+000002a0: 3a73 686f 7770 6167 6573 6861 646f 773d  :showpageshadow=
+000002b0: 2232 220a 2020 2020 2069 6e6b 7363 6170  "2".     inkscap
+000002c0: 653a 7061 6765 6f70 6163 6974 793d 2230  e:pageopacity="0
+000002d0: 2e30 220a 2020 2020 2069 6e6b 7363 6170  .0".     inkscap
+000002e0: 653a 7061 6765 6368 6563 6b65 7262 6f61  e:pagecheckerboa
+000002f0: 7264 3d22 3022 0a20 2020 2020 696e 6b73  rd="0".     inks
+00000300: 6361 7065 3a64 6573 6b63 6f6c 6f72 3d22  cape:deskcolor="
+00000310: 2364 3164 3164 3122 0a20 2020 2020 696e  #d1d1d1".     in
+00000320: 6b73 6361 7065 3a64 6f63 756d 656e 742d  kscape:document-
+00000330: 756e 6974 733d 226d 6d22 0a20 2020 2020  units="mm".     
+00000340: 7368 6f77 6772 6964 3d22 6661 6c73 6522  showgrid="false"
+00000350: 0a20 2020 2020 696e 6b73 6361 7065 3a7a  .     inkscape:z
+00000360: 6f6f 6d3d 2232 2e31 3934 3636 3938 220a  oom="2.1946698".
+00000370: 2020 2020 2069 6e6b 7363 6170 653a 6378       inkscape:cx
+00000380: 3d22 3832 2e34 3732 3534 3322 0a20 2020  ="82.472543".   
+00000390: 2020 696e 6b73 6361 7065 3a63 793d 2232    inkscape:cy="2
+000003a0: 382e 3235 3032 3633 220a 2020 2020 2069  8.250263".     i
+000003b0: 6e6b 7363 6170 653a 7769 6e64 6f77 2d77  nkscape:window-w
+000003c0: 6964 7468 3d22 3139 3230 220a 2020 2020  idth="1920".    
+000003d0: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+000003e0: 2d68 6569 6768 743d 2231 3031 3922 0a20  -height="1019". 
+000003f0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
+00000400: 646f 772d 783d 2230 220a 2020 2020 2069  dow-x="0".     i
+00000410: 6e6b 7363 6170 653a 7769 6e64 6f77 2d79  nkscape:window-y
+00000420: 3d22 3022 0a20 2020 2020 696e 6b73 6361  ="0".     inksca
+00000430: 7065 3a77 696e 646f 772d 6d61 7869 6d69  pe:window-maximi
+00000440: 7a65 643d 2231 220a 2020 2020 2069 6e6b  zed="1".     ink
+00000450: 7363 6170 653a 6375 7272 656e 742d 6c61  scape:current-la
+00000460: 7965 723d 226c 6179 6572 3122 202f 3e0a  yer="layer1" />.
+00000470: 2020 3c64 6566 730a 2020 2020 2069 643d    <defs.     id=
+00000480: 2264 6566 7332 2220 2f3e 0a20 203c 670a  "defs2" />.  <g.
+00000490: 2020 2020 2069 6e6b 7363 6170 653a 6c61       inkscape:la
+000004a0: 6265 6c3d 2243 616c 7175 6520 3122 0a20  bel="Calque 1". 
+000004b0: 2020 2020 696e 6b73 6361 7065 3a67 726f      inkscape:gro
+000004c0: 7570 6d6f 6465 3d22 6c61 7965 7222 0a20  upmode="layer". 
+000004d0: 2020 2020 6964 3d22 6c61 7965 7231 220a      id="layer1".
+000004e0: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
+000004f0: 7472 616e 736c 6174 6528 2d32 372e 3434  translate(-27.44
+00000500: 3535 3736 2c2d 3237 2e34 3435 3537 3629  5576,-27.445576)
+00000510: 223e 0a20 2020 203c 6369 7263 6c65 0a20  ">.    <circle. 
+00000520: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00000530: 6c3a 2330 3030 3030 303b 7374 726f 6b65  l:#000000;stroke
+00000540: 3a6e 6f6e 653b 7374 726f 6b65 2d77 6964  :none;stroke-wid
+00000550: 7468 3a30 2e30 3739 3232 3334 3b73 7472  th:0.0792234;str
+00000560: 6f6b 652d 6c69 6e65 6361 703a 726f 756e  oke-linecap:roun
+00000570: 643b 7374 726f 6b65 2d6c 696e 656a 6f69  d;stroke-linejoi
+00000580: 6e3a 6265 7665 6c22 0a20 2020 2020 2020  n:bevel".       
+00000590: 6964 3d22 7061 7468 3233 3422 0a20 2020  id="path234".   
+000005a0: 2020 2020 6378 3d22 3338 2e30 3939 3939      cx="38.09999
+000005b0: 3822 0a20 2020 2020 2020 6379 3d22 3338  8".       cy="38
+000005c0: 2e30 3939 3939 3822 0a20 2020 2020 2020  .099998".       
+000005d0: 723d 2231 302e 3635 3434 3233 2220 2f3e  r="10.654423" />
+000005e0: 0a20 203c 2f67 3e0a 3c2f 7376 673e 0a    .  </g>.</svg>.
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/point-300.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/point-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/point-96.svg` & `crossroads-schematization-0.2.8/crschem/resources/500/point-96.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/style-300.xml` & `crossroads-schematization-0.2.8/crschem/resources/500/style-300.xml`

 * *Files 3% similar despite different names*

#### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/style-300.xml` & `crossroads-schematization-0.2.8/crschem/resources/500/style-300.xml`

```diff
@@ -5,14 +5,19 @@
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
       <PolygonPatternSymbolizer file="point-300.svg"/>
     </Rule>
   </Style>
+  <Style name="outer">
+    <Rule>
+      <PolygonSymbolizer fill="#fff"/>
+    </Rule>
+  </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
       <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="sidewalks">
@@ -72,14 +77,21 @@
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-outer.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/style-96.xml` & `crossroads-schematization-0.2.8/crschem/resources/500/style-96.xml`

 * *Files 1% similar despite different names*

#### Comparing `crossroads-schematization-0.2.7/crschem/resources/500/style-96.xml` & `crossroads-schematization-0.2.8/crschem/resources/500/style-96.xml`

```diff
@@ -5,14 +5,19 @@
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
       <PolygonPatternSymbolizer file="point-96.svg"/>
     </Rule>
   </Style>
+  <Style name="outer">
+    <Rule>
+      <PolygonSymbolizer fill="#fff"/>
+    </Rule>
+  </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
       <LineSymbolizer stroke="#fff" stroke-width="16" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
   </Style>
   <Style name="sidewalks">
@@ -72,14 +77,21 @@
     <StyleName>crossings</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-crossings.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
+    <StyleName>outer</StyleName>
+    <Datasource>
+      <Parameter name="file">crossroad-outer.shp</Parameter>
+      <Parameter name="type">shape</Parameter>
+    </Datasource>
+  </Layer>
+  <Layer>
     <StyleName>sidewalks</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-sidewalks.shp</Parameter>
       <Parameter name="type">shape</Parameter>
     </Datasource>
   </Layer>
   <Layer>
```

### Comparing `crossroads-schematization-0.2.7/crschem/utils.py` & `crossroads-schematization-0.2.8/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.7/setup.py` & `crossroads-schematization-0.2.8/setup.py`

 * *Files identical despite different names*


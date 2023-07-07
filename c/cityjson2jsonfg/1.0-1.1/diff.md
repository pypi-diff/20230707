# Comparing `tmp/cityjson2jsonfg-1.0.tar.gz` & `tmp/cityjson2jsonfg-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cityjson2jsonfg-1.0.tar", last modified: Tue Aug 30 11:19:17 2022, max compression
+gzip compressed data, was "cityjson2jsonfg-1.1.tar", last modified: Fri Jul  7 16:24:02 2023, max compression
```

## Comparing `cityjson2jsonfg-1.0.tar` & `cityjson2jsonfg-1.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 11:19:17.150552 cityjson2jsonfg-1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-30 11:19:04.000000 cityjson2jsonfg-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6632 2022-08-30 11:19:17.150552 cityjson2jsonfg-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6129 2022-08-30 11:19:04.000000 cityjson2jsonfg-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 11:19:17.150552 cityjson2jsonfg-1.0/cityjson2jsonfg/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 11:19:04.000000 cityjson2jsonfg-1.0/cityjson2jsonfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-08-30 11:19:04.000000 cityjson2jsonfg-1.0/cityjson2jsonfg/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-08-30 11:19:04.000000 cityjson2jsonfg-1.0/cityjson2jsonfg/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 11:19:17.150552 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6632 2022-08-30 11:19:17.000000 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-08-30 11:19:17.000000 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 11:19:17.000000 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-30 11:19:17.000000 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-08-30 11:19:17.000000 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-30 11:19:17.000000 cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-08-30 11:19:04.000000 cityjson2jsonfg-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-30 11:19:17.150552 cityjson2jsonfg-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:24:02.298099 cityjson2jsonfg-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-07 16:24:02.298099 cityjson2jsonfg-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:24:02.294099 cityjson2jsonfg-1.1/cityjson2jsonfg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/cityjson2jsonfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/cityjson2jsonfg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/cityjson2jsonfg/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:24:02.298099 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-07-07 16:24:02.000000 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-07 16:24:02.000000 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:24:02.000000 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 16:24:02.000000 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 16:24:02.000000 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 16:24:02.000000 cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 16:24:02.298099 cityjson2jsonfg-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:24:02.298099 cityjson2jsonfg-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 16:23:51.000000 cityjson2jsonfg-1.1/tests/test_convert.py
```

### Comparing `cityjson2jsonfg-1.0/LICENSE` & `cityjson2jsonfg-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cityjson2jsonfg-1.0/PKG-INFO` & `cityjson2jsonfg-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cityjson2jsonfg
-Version: 1.0
+Version: 1.1
 Summary: Convert CityJSON files to JSON-FG format
 Author-email: 3DGI <info@3dgi.nl>
 License: Apache-2.0 License
 Project-URL: github, https://github.com/3DGI/cityjson2jsonfg
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,15 +40,15 @@
 ```
 
 ## Usage
 
 Convert a single CityJSON file to JSON-FG.
 
 ```shell
-cityjson2jsonfg <input.city.json> <output.jsonfg>
+cityjson2jsonfg <input.city.json> <output.fg.json>
 ```
 
 See the help menu and the tool version
 
 ```shell
 cityjson2jsonfg --help
 cityjson2jsonfg --version
@@ -58,15 +58,15 @@
 
 [cjio]() is a CLI tool for manipulating 3D city models that are stored in CityJSON files.
 You can pipe cjio's output directly into *cityjson2jsonfg* without saving an intermedate file.
 This is particularly useful if you want to modify the citymodel before the conversion.
 For instance, upgrade the CityJSON file to v1.1 and then convert it to JSON-FG.
 
 ```shell
-cjio --suppress_msg <input.city.json> upgrade save stdout | cityjson2jsonfg - <output.jsonfg>
+cjio --suppress_msg <input.city.json> upgrade save stdout | cityjson2jsonfg - <output.fg.json>
 ```
 
 ## Limitations
 
 Version 1.0 was primarily developed to convert CityJSON files of the Dutch [3D BAG](https://3dbag.nl/en/viewer) and [3D Basisvoorziening](https://www.pdok.nl/introductie/-/article/3d-basisvoorziening-1) data sets.
 Conversion from other data sets might not work.
```

### Comparing `cityjson2jsonfg-1.0/README.md` & `cityjson2jsonfg-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ```
 
 ## Usage
 
 Convert a single CityJSON file to JSON-FG.
 
 ```shell
-cityjson2jsonfg <input.city.json> <output.jsonfg>
+cityjson2jsonfg <input.city.json> <output.fg.json>
 ```
 
 See the help menu and the tool version
 
 ```shell
 cityjson2jsonfg --help
 cityjson2jsonfg --version
@@ -43,15 +43,15 @@
 
 [cjio]() is a CLI tool for manipulating 3D city models that are stored in CityJSON files.
 You can pipe cjio's output directly into *cityjson2jsonfg* without saving an intermedate file.
 This is particularly useful if you want to modify the citymodel before the conversion.
 For instance, upgrade the CityJSON file to v1.1 and then convert it to JSON-FG.
 
 ```shell
-cjio --suppress_msg <input.city.json> upgrade save stdout | cityjson2jsonfg - <output.jsonfg>
+cjio --suppress_msg <input.city.json> upgrade save stdout | cityjson2jsonfg - <output.fg.json>
 ```
 
 ## Limitations
 
 Version 1.0 was primarily developed to convert CityJSON files of the Dutch [3D BAG](https://3dbag.nl/en/viewer) and [3D Basisvoorziening](https://www.pdok.nl/introductie/-/article/3d-basisvoorziening-1) data sets.
 Conversion from other data sets might not work.
```

### Comparing `cityjson2jsonfg-1.0/cityjson2jsonfg/cli.py` & `cityjson2jsonfg-1.1/cityjson2jsonfg/cli.py`

 * *Files identical despite different names*

### Comparing `cityjson2jsonfg-1.0/cityjson2jsonfg/convert.py` & `cityjson2jsonfg-1.1/cityjson2jsonfg/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 limitations under the License.
 """
 
 from io import StringIO
 import json
 from copy import deepcopy
 
+import cjio.models
 from pyproj import CRS
+from click import echo
 
 
 def to_jsonfg_str(collection):
     out = StringIO()
     out.write(json.dumps(collection, separators=(',', ':')))
     return out
 
@@ -115,25 +117,49 @@
     :type geomdim: set
     """
     max_lod = max(g.lod for g in co.geometry)
     for geom in co.geometry:
         if geom.lod < "0.2":
             crs_to = CRS("OGC:CRS84")
             boundaries_crs84 = geom.reproject(cm.get_epsg(), crs_to=crs_to)
-            feature["geometry"] = {"coordinates": boundaries_crs84}
+            geom.boundaries = boundaries_crs84
+            coordinates = geometry_to_coordinates(geom)
+            feature["geometry"] = {"coordinates": coordinates}
             if geom.type == "MultiSurface":
                 feature["geometry"]["type"] = "MultiPolygon"
                 geomdim.add(2)
             elif geom.type == "MultiPoint":
                 feature["geometry"]["type"] = "MultiPoint"
                 geomdim.add(0)
             elif geom.type == "MultiLineString":
                 feature["geometry"]["type"] = "MultiLineString"
                 geomdim.add(1)
+            else:
+                echo(
+                    f"Invalid CityJSON Geometry type {geom.type} for converting to JSON-FG 'geometry', skipping geometry.")
         # We only convert the highest LoD to "place"
         elif geom.lod == max_lod:
-            feature["place"] = {"coordinates": geom.boundaries}
+            coordinates = geometry_to_coordinates(geom)
+            feature["place"] = {"coordinates": coordinates}
             geomdim.add(3)
             if geom.type == "Solid":
                 feature["place"]["type"] = "Polyhedron"
             elif geom.type == "MultiSurface":
                 feature["place"]["type"] = "MultiPolygon"
+            else:
+                echo(f"CityJSON Geometry type {geom.type} is not supported for converting to JSON-FG 'place', skipping geometry.")
+
+
+def geometry_to_coordinates(geometry: cjio.models.Geometry) -> list:
+    """Convert a CityJSON Geometry to JSON-FG coordinates."""
+    if geometry.type == "Solid":
+        return [
+            [ [ring + [ring[0], ] for ring in surface] for surface in shell ]
+            for shell in geometry.boundaries
+        ]
+    elif geometry.type == "MultiSurface":
+        return [
+            [ring + [ring[0], ] for ring in surface]
+            for surface in geometry.boundaries
+        ]
+    elif geometry.type == "MultiPoint" or geometry.type == "MultiLineString":
+        return geometry.boundaries
```

### Comparing `cityjson2jsonfg-1.0/cityjson2jsonfg.egg-info/PKG-INFO` & `cityjson2jsonfg-1.1/cityjson2jsonfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cityjson2jsonfg
-Version: 1.0
+Version: 1.1
 Summary: Convert CityJSON files to JSON-FG format
 Author-email: 3DGI <info@3dgi.nl>
 License: Apache-2.0 License
 Project-URL: github, https://github.com/3DGI/cityjson2jsonfg
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,15 +40,15 @@
 ```
 
 ## Usage
 
 Convert a single CityJSON file to JSON-FG.
 
 ```shell
-cityjson2jsonfg <input.city.json> <output.jsonfg>
+cityjson2jsonfg <input.city.json> <output.fg.json>
 ```
 
 See the help menu and the tool version
 
 ```shell
 cityjson2jsonfg --help
 cityjson2jsonfg --version
@@ -58,15 +58,15 @@
 
 [cjio]() is a CLI tool for manipulating 3D city models that are stored in CityJSON files.
 You can pipe cjio's output directly into *cityjson2jsonfg* without saving an intermedate file.
 This is particularly useful if you want to modify the citymodel before the conversion.
 For instance, upgrade the CityJSON file to v1.1 and then convert it to JSON-FG.
 
 ```shell
-cjio --suppress_msg <input.city.json> upgrade save stdout | cityjson2jsonfg - <output.jsonfg>
+cjio --suppress_msg <input.city.json> upgrade save stdout | cityjson2jsonfg - <output.fg.json>
 ```
 
 ## Limitations
 
 Version 1.0 was primarily developed to convert CityJSON files of the Dutch [3D BAG](https://3dbag.nl/en/viewer) and [3D Basisvoorziening](https://www.pdok.nl/introductie/-/article/3d-basisvoorziening-1) data sets.
 Conversion from other data sets might not work.
```

### Comparing `cityjson2jsonfg-1.0/pyproject.toml` & `cityjson2jsonfg-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cityjson2jsonfg"
-version = "1.0"
+version = "1.1"
 description = "Convert CityJSON files to JSON-FG format"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache-2.0 License" }
 authors = [
     { name = "3DGI", email = "info@3dgi.nl" }
 ]
```


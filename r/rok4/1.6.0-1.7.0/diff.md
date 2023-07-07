# Comparing `tmp/rok4-1.6.0.tar.gz` & `tmp/rok4-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rok4-1.6.0.tar", last modified: Mon Mar 20 13:55:48 2023, max compression
+gzip compressed data, was "rok4-1.7.0.tar", last modified: Fri Jul  7 15:08:49 2023, max compression
```

## Comparing `rok4-1.6.0.tar` & `rok4-1.7.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:55:48.643482 rok4-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)    21865 2023-03-20 13:54:22.000000 rok4-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)    28081 2023-03-20 13:55:48.643482 rok4-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-03-20 13:54:22.000000 rok4-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      994 2023-03-20 13:54:22.000000 rok4-1.6.0/README.pypi.md
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-03-20 13:55:10.000000 rok4-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-20 13:55:48.643482 rok4-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-03-20 13:54:22.000000 rok4-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:55:48.639482 rok4-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:55:48.643482 rok4-1.6.0/src/rok4/
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/Layer.py
--rw-r--r--   0 runner    (1001) docker     (122)    34821 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/Pyramid.py
--rw-r--r--   0 runner    (1001) docker     (122)    27740 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/Storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     8376 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/TileMatrixSet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/Utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5881 2023-03-20 13:54:22.000000 rok4-1.6.0/src/rok4/Vector.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-20 13:55:10.000000 rok4-1.6.0/src/rok4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:55:48.643482 rok4-1.6.0/src/rok4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28081 2023-03-20 13:55:48.000000 rok4-1.6.0/src/rok4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-03-20 13:55:48.000000 rok4-1.6.0/src/rok4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 13:55:48.000000 rok4-1.6.0/src/rok4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-03-20 13:55:48.000000 rok4-1.6.0/src/rok4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-20 13:55:48.000000 rok4-1.6.0/src/rok4.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 13:55:48.643482 rok4-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6483 2023-03-20 13:54:22.000000 rok4-1.6.0/tests/test_Layer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10928 2023-03-20 13:54:22.000000 rok4-1.6.0/tests/test_Pyramid.py
--rw-r--r--   0 runner    (1001) docker     (122)    24499 2023-03-20 13:54:22.000000 rok4-1.6.0/tests/test_Storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     9198 2023-03-20 13:54:22.000000 rok4-1.6.0/tests/test_TileMatrixSet.py
--rw-r--r--   0 runner    (1001) docker     (122)     2217 2023-03-20 13:54:22.000000 rok4-1.6.0/tests/test_Utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5308 2023-03-20 13:54:22.000000 rok4-1.6.0/tests/test_Vector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:08:49.854428 rok4-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    21863 2023-07-07 15:07:49.000000 rok4-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    27900 2023-07-07 15:08:49.854428 rok4-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-07-07 15:07:49.000000 rok4-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-07-07 15:07:49.000000 rok4-1.7.0/README.pypi.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-07-07 15:08:23.000000 rok4-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 15:08:49.854428 rok4-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 15:07:49.000000 rok4-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:08:49.850428 rok4-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:08:49.854428 rok4-1.7.0/src/rok4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11178 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46620 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12383 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33990 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/TileMatrixSet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9275 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8648 2023-07-07 15:07:49.000000 rok4-1.7.0/src/rok4/Vector.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-07 15:08:23.000000 rok4-1.7.0/src/rok4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:08:49.854428 rok4-1.7.0/src/rok4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    27900 2023-07-07 15:08:49.000000 rok4-1.7.0/src/rok4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-07 15:08:49.000000 rok4-1.7.0/src/rok4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 15:08:49.000000 rok4-1.7.0/src/rok4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-07 15:08:49.000000 rok4-1.7.0/src/rok4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-07 15:08:49.000000 rok4-1.7.0/src/rok4.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 15:08:49.854428 rok4-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     6569 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_Layer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12473 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_Pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23528 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_Raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31490 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_Storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9565 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_TileMatrixSet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13825 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_Utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5046 2023-07-07 15:07:49.000000 rok4-1.7.0/tests/test_Vector.py
```

### Comparing `rok4-1.6.0/LICENSE.txt` & `rok4-1.7.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 
     Article 2 - PURPOSE
 
 The purpose of the Agreement is the grant by the Licensor to the
 Licensee of a non-exclusive, transferable and worldwide license for the
 Software as set forth in Article 5 hereinafter for the whole term of the
-protection granted by the rights over said Software. 
+protection granted by the rights over said Software.
 
 
     Article 3 - ACCEPTANCE
 
 3.1 The Licensee shall be deemed as having accepted the terms and
 conditions of this Agreement upon the occurrence of the first of the
 following events:
@@ -264,15 +264,15 @@
 
         5.3.3 DISTRIBUTION OF DERIVATIVE SOFTWARE
 
 When the Licensee creates Derivative Software, this Derivative Software
 may be distributed under a license agreement other than this Agreement,
 subject to compliance with the requirement to include a notice
 concerning the rights over the Software as defined in Article 6.4.
-In the event the creation of the Derivative Software required modification 
+In the event the creation of the Derivative Software required modification
 of the Source Code, the Licensee undertakes that:
 
    1. the resulting Modified Software will be governed by this Agreement,
    2. the Integrated Contributions in the resulting Modified Software
       will be clearly identified and documented,
    3. the Licensee will allow effective access to the source code of the
       Modified Software, at a minimum during the entire period of
```

### Comparing `rok4-1.6.0/PKG-INFO` & `rok4-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rok4
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python core libraries for ROK4 project
 Author-email: Géoportail IGN Developers <tout_rdev@ign.fr>
 License: 
         CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
@@ -123,15 +123,15 @@
         
         
             Article 2 - PURPOSE
         
         The purpose of the Agreement is the grant by the Licensor to the
         Licensee of a non-exclusive, transferable and worldwide license for the
         Software as set forth in Article 5 hereinafter for the whole term of the
-        protection granted by the rights over said Software. 
+        protection granted by the rights over said Software.
         
         
             Article 3 - ACCEPTANCE
         
         3.1 The Licensee shall be deemed as having accepted the terms and
         conditions of this Agreement upon the occurrence of the first of the
         following events:
@@ -269,15 +269,15 @@
         
                 5.3.3 DISTRIBUTION OF DERIVATIVE SOFTWARE
         
         When the Licensee creates Derivative Software, this Derivative Software
         may be distributed under a license agreement other than this Agreement,
         subject to compliance with the requirement to include a notice
         concerning the rights over the Software as defined in Article 6.4.
-        In the event the creation of the Derivative Software required modification 
+        In the event the creation of the Derivative Software required modification
         of the Source Code, the Licensee undertakes that:
         
            1. the resulting Modified Software will be governed by this Agreement,
            2. the Integrated Contributions in the resulting Modified Software
               will be clearly identified and documented,
            3. the Licensee will allow effective access to the source code of the
               Modified Software, at a minimum during the entire period of
@@ -533,16 +533,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE.txt
 
 # ROK4 Python libraries
 
 ![ROK4 Logo](https://rok4.github.io/assets/images/rok4.png)
 
 The `rok4` package help to use [ROK4 project](https://rok4.github.io/) concepts, like Tile Matrix Sets, data pyramids or layers.
@@ -556,17 +557,15 @@
 * [PyPI](https://pypi.org/project/rok4/) : `pip install rok4`
 * [GitHub](https://github.com/rok4/core-python/releases/) : `pip install https://github.com/rok4/core-python/releases/download/<version>/rok4-<version>-py3-none-any.whl`
 
 ## Usage
 
 ```python
 from rok4.TileMatrixSet import TileMatrixSet
-from rok4.Vector import Vector
 
 try:
     tms = TileMatrixSet("file:///path/to/tms.json")
-    vector = Vector("file:///path/to/vector.shp")
-    vector_csv1 = Vector("file:///path/to/vector.csv", delimiter, column_x, column_y)
-    vector_csv1 = Vector("file:///path/to/vector.csv", delimiter, column_WKT)
 except Exception as exc:
     print(exc)
 ```
+
+More examples in the developer documentation
```

### Comparing `rok4-1.6.0/pyproject.toml` & `rok4-1.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "rok4"
-version = "1.6.0"
+version = "1.7.0"
 
 description = "Python core libraries for ROK4 project"
 readme = "README.pypi.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 
 keywords = ["ROK4", "library", "pyramid", "tile matrix set", "storage"]
@@ -34,27 +34,37 @@
   "boto3 >= 1.26.54",
   "pillow >= 9.4.0",
   "numpy >= 1.24.2",
   "mapbox-vector-tile >= 2.0.1"
 ]
 
 [project.optional-dependencies]
+doc = [
+  "pdoc3 >= 0.10.0"
+]
+
+dev = [
+  "black",
+  "pre-commit >3,<4"
+]
+
 test = [
   "pytest >= 7.1.2",
   "coverage >= 7.0.5"
 ]
-doc = [
-  "pdoc3 >= 0.10.0"
-]
 
 [project.urls]
 "Homepage" = "https://rok4.github.io/core-python"
 "Bug Reports" = "https://github.com/rok4/core-python/issues"
 "Changelog" = "https://github.com/rok4/core-python/releases"
 "Source" = "https://github.com/rok4/core-python"
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.black]
+line-length = 100
+target-version = ['py38']
+
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `rok4-1.6.0/src/rok4/Exceptions.py` & `rok4-1.7.0/src/rok4/Exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,36 @@
     """
 
     def __init__(self, path, missing):
         self.path = path
         self.missing = missing
         super().__init__(f"Missing attribute {missing} in '{path}'")
 
+
 class MissingEnvironmentError(Exception):
     """
     Exception raised when a needed environment variable is not defined
     """
 
     def __init__(self, missing):
         self.missing = missing
         super().__init__(f"Missing environment variable {missing}")
 
+
 class StorageError(Exception):
     """
     Exception raised when an issue occured when using a storage
     """
 
     def __init__(self, type, issue):
         self.type = type
         self.issue = issue
         super().__init__(f"Issue occured using a {type} storage : {issue}")
 
+
 class FormatError(Exception):
     """
     Exception raised when a format is expected but not respected
     """
 
     def __init__(self, expected_format, content, issue):
         self.expected_format = expected_format
```

### Comparing `rok4-1.6.0/src/rok4/Layer.py` & `rok4-1.7.0/src/rok4/Layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from rok4.Exceptions import *
 from rok4.Pyramid import Pyramid, PyramidType
 from rok4.TileMatrixSet import TileMatrixSet
 from rok4.Storage import *
 from rok4.Utils import *
 
+
 class Layer:
     """A data layer, raster or vector
 
     Attributes:
         __name (str): layer's technical name
         __pyramids (Dict[str, Union[rok4.Pyramid.Pyramid,str,str]]): used pyramids
         __format (str): pyramid's list path
@@ -30,80 +31,83 @@
         __best_level (rok4.Pyramid.Level): Used pyramids best level
         __resampling (str): Interpolation to use fot resampling
         __bbox (Tuple[float, float, float, float]): data bounding box, TMS coordinates system
         __geobbox (Tuple[float, float, float, float]): data bounding box, EPSG:4326
     """
 
     @classmethod
-    def from_descriptor(cls, descriptor: str) -> 'Layer':
+    def from_descriptor(cls, descriptor: str) -> "Layer":
         """Create a layer from its descriptor
 
         Args:
             descriptor (str): layer's descriptor path
 
         Raises:
             FormatError: Provided path is not a well formed JSON
             MissingAttributeError: Attribute is missing in the content
             StorageError: Storage read issue (layer descriptor)
             MissingEnvironmentError: Missing object storage informations
 
         Returns:
             Layer: a Layer instance
-        """        
+        """
         try:
             data = json.loads(get_data_str(descriptor))
 
         except JSONDecodeError as e:
             raise FormatError("JSON", descriptor, e)
 
         layer = cls()
 
         storage_type, path, root, base_name = get_infos_from_path(descriptor)
-        layer.__name = base_name[:-5] # on supprime l'extension.json
+        layer.__name = base_name[:-5]  # on supprime l'extension.json
 
         try:
             # Attributs communs
             layer.__title = data["title"]
             layer.__abstract = data["abstract"]
             layer.__load_pyramids(data["pyramids"])
 
             # Paramètres optionnels
             if "keywords" in data:
                 for k in data["keywords"]:
                     layer.__keywords.append(k)
 
-
-            if layer.type == PyramidType.RASTER: 
+            if layer.type == PyramidType.RASTER:
                 if "resampling" in data:
                     layer.__resampling = data["resampling"]
 
                 if "styles" in data:
                     layer.__styles = data["styles"]
                 else:
                     layer.__styles = ["normal"]
 
             # Les bbox, native et géographique
             if "bbox" in data:
-                layer.__geobbox = (data["bbox"]["south"], data["bbox"]["west"], data["bbox"]["north"], data["bbox"]["east"])
+                layer.__geobbox = (
+                    data["bbox"]["south"],
+                    data["bbox"]["west"],
+                    data["bbox"]["north"],
+                    data["bbox"]["east"],
+                )
                 layer.__bbox = reproject_bbox(layer.__geobbox, "EPSG:4326", layer.__tms.srs, 5)
                 # On force l'emprise de la couche, on recalcule donc les tuiles limites correspondantes pour chaque niveau
                 for l in layer.__levels.values():
                     l.set_limits_from_bbox(layer.__bbox)
             else:
                 layer.__bbox = layer.__best_level.bbox
                 layer.__geobbox = reproject_bbox(layer.__bbox, layer.__tms.srs, "EPSG:4326", 5)
 
         except KeyError as e:
             raise MissingAttributeError(descriptor, e)
 
-
         return layer
 
     @classmethod
-    def from_parameters(cls, pyramids: List[Dict[str, str]], name: str, **kwargs) -> 'Layer':
+    def from_parameters(cls, pyramids: List[Dict[str, str]], name: str, **kwargs) -> "Layer":
         """Create a default layer from parameters
 
         Args:
             pyramids (List[Dict[str, str]]): pyramids to use and extrem levels, bottom and top
             name (str): layer's technical name
             **title (str): Layer's title (will be equal to name if not provided)
             **abstract (str): Layer's abstract (will be equal to name if not provided)
@@ -117,15 +121,17 @@
             Layer: a Layer instance
         """
 
         layer = cls()
 
         # Informations obligatoires
         if not re.match("^[A-Za-z0-9_-]*$", name):
-            raise Exception(f"Layer's name have to contain only letters, number, hyphen and underscore, to be URL and storage compliant ({name})")
+            raise Exception(
+                f"Layer's name have to contain only letters, number, hyphen and underscore, to be URL and storage compliant ({name})"
+            )
 
         layer.__name = name
         layer.__load_pyramids(pyramids)
 
         # Les bbox, native et géographique
         layer.__bbox = layer.__best_level.bbox
         layer.__geobbox = reproject_bbox(layer.__bbox, layer.__tms.srs, "EPSG:4326", 5)
@@ -141,154 +147,148 @@
             layer.__title = name
 
         if "abstract" in kwargs and kwargs["abstract"] is not None:
             layer.__abstract = kwargs["abstract"]
         else:
             layer.__abstract = name
 
-        if layer.type == PyramidType.RASTER: 
+        if layer.type == PyramidType.RASTER:
             if "styles" in kwargs and kwargs["styles"] is not None and len(kwargs["styles"]) > 0:
                 layer.__styles = kwargs["styles"]
             else:
                 layer.__styles = ["normal"]
 
             if "resampling" in kwargs and kwargs["resampling"] is not None:
                 layer.__resampling = kwargs["resampling"]
 
         return layer
 
-
     def __init__(self) -> None:
         self.__format = None
         self.__tms = None
         self.__best_level = None
-        self.__levels = dict()
+        self.__levels = {}
         self.__keywords = []
         self.__pyramids = []
 
     def __load_pyramids(self, pyramids: List[Dict[str, str]]) -> None:
         """Load and check pyramids
 
         Args:
             pyramids (List[Dict[str, str]]): List of descriptors' paths and optionnaly top and bottom levels
 
         Raises:
             Exception: Pyramids' do not all own the same format
             Exception: Pyramids' do not all own the same TMS
             Exception: Pyramids' do not all own the same channels number
             Exception: Overlapping in usage pyramids' levels
-        """        
+        """
 
         ## Toutes les pyramides doivent avoir les même caractéristiques
         channels = None
         for p in pyramids:
-
             pyramid = Pyramid.from_descriptor(p["path"])
             bottom_level = p.get("bottom_level", None)
             top_level = p.get("top_level", None)
 
             if bottom_level is None:
                 bottom_level = pyramid.bottom_level.id
 
             if top_level is None:
                 top_level = pyramid.top_level.id
 
             if self.__format is not None and self.__format != pyramid.format:
-                raise Exception(f"Used pyramids have to own the same format : {self.__format} != {pyramid.format}")
+                raise Exception(
+                    f"Used pyramids have to own the same format : {self.__format} != {pyramid.format}"
+                )
             else:
                 self.__format = pyramid.format
 
             if self.__tms is not None and self.__tms.id != pyramid.tms.id:
-                raise Exception(f"Used pyramids have to use the same TMS : {self.__tms.id} != {pyramid.tms.id}")
+                raise Exception(
+                    f"Used pyramids have to use the same TMS : {self.__tms.id} != {pyramid.tms.id}"
+                )
             else:
                 self.__tms = pyramid.tms
 
             if self.type == PyramidType.RASTER:
                 if channels is not None and channels != pyramid.raster_specifications["channels"]:
-                    raise Exception(f"Used RASTER pyramids have to own the same number of channels : {channels} != {pyramid.raster_specifications['channels']}")
+                    raise Exception(
+                        f"Used RASTER pyramids have to own the same number of channels : {channels} != {pyramid.raster_specifications['channels']}"
+                    )
                 else:
                     channels = pyramid.raster_specifications["channels"]
                 self.__resampling = pyramid.raster_specifications["interpolation"]
 
             levels = pyramid.get_levels(bottom_level, top_level)
             for l in levels:
                 if l.id in self.__levels:
                     raise Exception(f"Level {l.id} is present in two used pyramids")
                 self.__levels[l.id] = l
 
-            self.__pyramids.append({
-                "pyramid": pyramid,
-                "bottom_level": bottom_level,
-                "top_level": top_level
-            })
+            self.__pyramids.append(
+                {"pyramid": pyramid, "bottom_level": bottom_level, "top_level": top_level}
+            )
 
         self.__best_level = sorted(self.__levels.values(), key=lambda l: l.resolution)[0]
 
     def __str__(self) -> str:
         return f"{self.type.name} layer '{self.__name}'"
 
     @property
-    def serializable(self) -> Dict: 
+    def serializable(self) -> Dict:
         """Get the dict version of the layer object, descriptor compliant
 
         Returns:
             Dict: descriptor structured object description
-        """        
+        """
         serialization = {
             "title": self.__title,
             "abstract": self.__abstract,
             "keywords": self.__keywords,
-            "wmts": {
-                "authorized": True
-            },
-            "tms": {
-                "authorized": True
-            },
+            "wmts": {"authorized": True},
+            "tms": {"authorized": True},
             "bbox": {
                 "south": self.__geobbox[0],
                 "west": self.__geobbox[1],
                 "north": self.__geobbox[2],
-                "east": self.__geobbox[3]
+                "east": self.__geobbox[3],
             },
-            "pyramids": []
+            "pyramids": [],
         }
 
         for p in self.__pyramids:
-            serialization["pyramids"].append({
-                "bottom_level" : p["bottom_level"],
-                "top_level" : p["top_level"],
-                "path" : p["pyramid"].descriptor
-            })
+            serialization["pyramids"].append(
+                {
+                    "bottom_level": p["bottom_level"],
+                    "top_level": p["top_level"],
+                    "path": p["pyramid"].descriptor,
+                }
+            )
 
         if self.type == PyramidType.RASTER:
             serialization["wms"] = {
                 "authorized": True,
-                "crs": [
-                    "CRS:84",
-                    "IGNF:WGS84G",
-                    "EPSG:3857",
-                    "EPSG:4258",
-                    "EPSG:4326"
-                ]
+                "crs": ["CRS:84", "IGNF:WGS84G", "EPSG:3857", "EPSG:4258", "EPSG:4326"],
             }
 
             if self.__tms.srs.upper() not in serialization["wms"]["crs"]:
                 serialization["wms"]["crs"].append(self.__tms.srs.upper())
-            
+
             serialization["styles"] = self.__styles
             serialization["resampling"] = self.__resampling
 
         return serialization
 
     def write_descriptor(self, directory: str = None) -> None:
         """Print layer's descriptor as JSON
 
         Args:
             directory (str, optional): Directory (file or object) where to print the layer's descriptor, called <layer's name>.json. Defaults to None, JSON is printed to standard output.
-        """        
+        """
         content = json.dumps(self.serializable)
 
         if directory is None:
             print(content)
         else:
             put_data_str(content, os.path.join(directory, f"{self.__name}.json"))
 
@@ -302,8 +302,7 @@
     @property
     def bbox(self) -> Tuple[float, float, float, float]:
         return self.__bbox
 
     @property
     def geobbox(self) -> Tuple[float, float, float, float]:
         return self.__geobbox
-
```

### Comparing `rok4-1.6.0/src/rok4/Pyramid.py` & `rok4-1.7.0/src/rok4/Pyramid.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The module contains the following classes:
 
 - `Pyramid` - Data container
 - `Level` - Level of a pyramid
 """
 
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Tuple, Union, Iterator
 import json
 from json.decoder import JSONDecodeError
 import os
 import re
 import numpy
 import zlib
 import io
@@ -18,70 +18,83 @@
 from PIL import Image
 
 from rok4.Exceptions import *
 from rok4.TileMatrixSet import TileMatrixSet, TileMatrix
 from rok4.Storage import *
 from rok4.Utils import *
 
+
 class PyramidType(Enum):
+    """Pyramid's data type"""
+
     RASTER = "RASTER"
     VECTOR = "VECTOR"
 
+
 class SlabType(Enum):
-    DATA = "DATA"
-    MASK = "MASK"
+    """Slab's type"""
+
+    DATA = "DATA"  # Slab of data, raster or vector
+    MASK = "MASK"  # Slab of mask, only for raster pyramid, image with one band : 0 is nodata, other values are data
+
+
+ROK4_IMAGE_HEADER_SIZE = 2048
+"""Slab's header size, 2048 bytes"""
+
 
 def b36_number_encode(number: int) -> str:
     """Convert base-10 number to base-36
 
     Used alphabet is '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
     Args:
         number (int): base-10 number
 
     Returns:
         str: base-36 number
     """
 
-    alphabet='0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ'
+    alphabet = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 
-    base36 = ''
+    base36 = ""
 
     if 0 <= number < len(alphabet):
         return alphabet[number]
 
     while number != 0:
         number, i = divmod(number, len(alphabet))
         base36 = alphabet[i] + base36
 
     return base36
 
+
 def b36_number_decode(number: str) -> int:
     """Convert base-36 number to base-10
 
     Args:
         number (str): base-36 number
 
     Returns:
         int: base-10 number
     """
     return int(number, 36)
 
+
 def b36_path_decode(path: str) -> Tuple[int, int]:
     """Get slab's column and row from a base-36 based path
 
     Args:
         path (str): slab's path
 
     Returns:
         Tuple[int, int]: slab's column and row
-    """    
+    """
 
-    path = path.replace('/', '')
-    path = re.sub(r'(\.TIFF?)', "", path.upper())
+    path = path.replace("/", "")
+    path = re.sub(r"(\.TIFF?)", "", path.upper())
 
     b36_column = ""
     b36_row = ""
 
     while len(path) > 0:
         b36_column += path[0]
         b36_row += path[1]
@@ -96,15 +109,15 @@
     Args:
         column (int): slab's column
         row (int): slab's row
         slashs (int): slashs' number (to split path)
 
     Returns:
         str: base-36 based path
-    """    
+    """
 
     b36_column = b36_number_encode(column)
     b36_row = b36_number_encode(row)
 
     max_len = max(slashs + 1, len(b36_column), len(b36_row))
 
     b36_column = b36_column.rjust(max_len, "0")
@@ -121,78 +134,88 @@
 
         if slashs > 0:
             b36_path = "/" + b36_path
             slashs -= 1
 
     return f"{b36_path}.tif"
 
+
 class Level:
     """A pyramid's level, raster or vector
 
     Attributes:
         __id (str): level's identifier. have to exist in the pyramid's used TMS
         __tile_limits (Dict[str, int]): minimum and maximum tiles' columns and rows of pyramid's content
         __slab_size (Tuple[int, int]): number of tile in a slab, widthwise and heightwise
         __tables (List[Dict]): for a VECTOR pyramid, description of vector content, tables and attributes
     """
 
     @classmethod
-    def from_descriptor(cls, data: Dict, pyramid: 'Pyramid') -> 'Level':
+    def from_descriptor(cls, data: Dict, pyramid: "Pyramid") -> "Level":
         """Create a pyramid's level from the pyramid's descriptor levels element
 
         Args:
             data (Dict): level's information from the pyramid's descriptor
             pyramid (Pyramid): pyramid containing the level to create
 
         Raises:
             Exception: different storage or masks presence between the level and the pyramid
             MissingAttributeError: Attribute is missing in the content
 
         Returns:
             Pyramid: a Level instance
-        """    
+        """
         level = cls()
 
         level.__pyramid = pyramid
 
         # Attributs communs
         try:
             level.__id = data["id"]
             level.__tile_limits = data["tile_limits"]
-            level.__slab_size = (data["tiles_per_width"], data["tiles_per_height"],)
+            level.__slab_size = (
+                data["tiles_per_width"],
+                data["tiles_per_height"],
+            )
 
             # Informations sur le stockage : on les valide et stocke dans la pyramide
             if pyramid.storage_type.name != data["storage"]["type"]:
-                raise Exception(f"Pyramid {pyramid.descriptor} owns levels using different storage types ({ data['storage']['type'] }) than its one ({pyramid.storage_type.name})")
+                raise Exception(
+                    f"Pyramid {pyramid.descriptor} owns levels using different storage types ({ data['storage']['type'] }) than its one ({pyramid.storage_type.name})"
+                )
+
+            if pyramid.storage_type == StorageType.FILE:
+                pyramid.storage_depth = data["storage"]["path_depth"]
 
-            if pyramid.storage_type == StorageType.FILE:                    
-                pyramid.storage_depth = data["storage"]["path_depth"]   
-            
             if "mask_directory" in data["storage"] or "mask_prefix" in data["storage"]:
                 if not pyramid.own_masks:
-                    raise Exception(f"Pyramid {pyramid.__descriptor} does not define a mask format but level {level.__id} define mask storage informations")
+                    raise Exception(
+                        f"Pyramid {pyramid.__descriptor} does not define a mask format but level {level.__id} define mask storage informations"
+                    )
             else:
                 if pyramid.own_masks:
-                    raise Exception(f"Pyramid {pyramid.__descriptor} define a mask format but level {level.__id} does not define mask storage informations")
+                    raise Exception(
+                        f"Pyramid {pyramid.__descriptor} define a mask format but level {level.__id} does not define mask storage informations"
+                    )
 
         except KeyError as e:
             raise MissingAttributeError(pyramid.descriptor, f"levels[].{e}")
 
         # Attributs dans le cas d'un niveau vecteur
-        if level.__pyramid.type == PyramidType.VECTOR :
+        if level.__pyramid.type == PyramidType.VECTOR:
             try:
                 level.__tables = data["tables"]
 
             except KeyError as e:
                 raise MissingAttributeError(pyramid.descriptor, f"levels[].{e}")
 
         return level
 
     @classmethod
-    def from_other(cls, other: 'Level', pyramid: 'Pyramid') -> 'Level':
+    def from_other(cls, other: "Level", pyramid: "Pyramid") -> "Level":
         """Create a pyramid's level from another one
 
         Args:
             other (Level): level to clone
             pyramid (Pyramid): new pyramid containing the new level
 
         Raises:
@@ -208,129 +231,140 @@
         # Attributs communs
         level.__id = other.__id
         level.__pyramid = pyramid
         level.__tile_limits = other.__tile_limits
         level.__slab_size = other.__slab_size
 
         # Attributs dans le cas d'un niveau vecteur
-        if level.__pyramid.type == PyramidType.VECTOR :
+        if level.__pyramid.type == PyramidType.VECTOR:
             level.__tables = other.__tables
 
         return level
 
     def __str__(self) -> str:
         return f"{self.__pyramid.type.name} pyramid's level '{self.__id}' ({self.__pyramid.storage_type.name} storage)"
 
-
     @property
-    def serializable(self) -> Dict: 
+    def serializable(self) -> Dict:
         """Get the dict version of the pyramid object, pyramid's descriptor compliant
 
         Returns:
             Dict: pyramid's descriptor structured object description
-        """   
+        """
         serialization = {
             "id": self.__id,
             "tiles_per_width": self.__slab_size[0],
             "tiles_per_height": self.__slab_size[1],
-            "tile_limits": self.__tile_limits
+            "tile_limits": self.__tile_limits,
         }
 
         if self.__pyramid.type == PyramidType.VECTOR:
             serialization["tables"] = self.__tables
 
         if self.__pyramid.storage_type == StorageType.FILE:
             serialization["storage"] = {
                 "type": "FILE",
                 "image_directory": f"{self.__pyramid.name}/DATA/{self.__id}",
-                "path_depth": self.__pyramid.storage_depth
+                "path_depth": self.__pyramid.storage_depth,
             }
             if self.__pyramid.own_masks:
-                serialization["storage"]["mask_directory"] = f"{self.__pyramid.name}/MASK/{self.__id}"
+                serialization["storage"][
+                    "mask_directory"
+                ] = f"{self.__pyramid.name}/MASK/{self.__id}"
 
         elif self.__pyramid.storage_type == StorageType.CEPH:
             serialization["storage"] = {
                 "type": "CEPH",
                 "image_prefix": f"{self.__pyramid.name}/DATA_{self.__id}",
-                "pool_name": self.__pyramid.storage_root
+                "pool_name": self.__pyramid.storage_root,
             }
             if self.__pyramid.own_masks:
                 serialization["storage"]["mask_prefix"] = f"{self.__pyramid.name}/MASK_{self.__id}"
 
         elif self.__pyramid.storage_type == StorageType.S3:
             serialization["storage"] = {
                 "type": "S3",
                 "image_prefix": f"{self.__pyramid.name}/DATA_{self.__id}",
-                "bucket_name": self.__pyramid.storage_root
+                "bucket_name": self.__pyramid.storage_root,
             }
             if self.__pyramid.own_masks:
                 serialization["storage"]["mask_prefix"] = f"{self.__pyramid.name}/MASK_{self.__id}"
 
         return serialization
 
     @property
-    def id(self) -> str: 
+    def id(self) -> str:
         return self.__id
 
     @property
-    def bbox(self) -> Tuple[float, float, float, float]: 
+    def bbox(self) -> Tuple[float, float, float, float]:
         """Return level extent, based on tile limits
 
         Returns:
             Tuple[float, float, float, float]: level terrain extent (xmin, ymin, xmax, ymax)
-        """        
-        min_bbox = self.__pyramid.tms.get_level(self.__id).tile_to_bbox(self.__tile_limits["min_col"], self.__tile_limits["max_row"])
-        print(min_bbox)
-        max_bbox = self.__pyramid.tms.get_level(self.__id).tile_to_bbox(self.__tile_limits["max_col"], self.__tile_limits["min_row"])
-        print(max_bbox)
+        """
+
+        min_bbox = self.__pyramid.tms.get_level(self.__id).tile_to_bbox(
+            self.__tile_limits["min_col"], self.__tile_limits["max_row"]
+        )
+        max_bbox = self.__pyramid.tms.get_level(self.__id).tile_to_bbox(
+            self.__tile_limits["max_col"], self.__tile_limits["min_row"]
+        )
 
         return (min_bbox[0], min_bbox[1], max_bbox[2], max_bbox[3])
 
     @property
-    def resolution(self) -> str: 
+    def resolution(self) -> str:
         return self.__pyramid.tms.get_level(self.__id).resolution
 
     @property
-    def tile_matrix(self) -> TileMatrix: 
+    def tile_matrix(self) -> TileMatrix:
         return self.__pyramid.tms.get_level(self.__id)
 
     @property
-    def slab_width(self) -> int: 
+    def slab_width(self) -> int:
         return self.__slab_size[0]
 
     @property
-    def slab_height(self) -> int: 
+    def slab_height(self) -> int:
         return self.__slab_size[1]
 
     def is_in_limits(self, column: int, row: int) -> bool:
         """Is the tile indices in limits ?
 
         Args:
             column (int): tile's column
             row (int): tile's row
 
         Returns:
             bool: True if tiles' limits contain the provided tile's indices
         """
-        return self.__tile_limits["min_row"] <= row and self.__tile_limits["max_row"] >= row and self.__tile_limits["min_col"] <= column and self.__tile_limits["max_col"] >= column
+        return (
+            self.__tile_limits["min_row"] <= row
+            and self.__tile_limits["max_row"] >= row
+            and self.__tile_limits["min_col"] <= column
+            and self.__tile_limits["max_col"] >= column
+        )
 
     def set_limits_from_bbox(self, bbox: Tuple[float, float, float, float]) -> None:
         """Set tile limits, based on provided bounding box
 
         Args:
             bbox (Tuple[float, float, float, float]): terrain extent (xmin, ymin, xmax, ymax), in TMS coordinates system
 
         """
-        
-        col_min, row_min, col_max, row_max = self.__pyramid.tms.get_level(self.__id).bbox_to_tiles(bbox)
+
+        col_min, row_min, col_max, row_max = self.__pyramid.tms.get_level(self.__id).bbox_to_tiles(
+            bbox
+        )
         self.__tile_limits = {
             "min_row": row_min,
             "max_col": col_max,
             "max_row": row_max,
-            "min_col": col_min
+            "min_col": col_min,
         }
 
 
 class Pyramid:
 
     """A data pyramid, raster or vector
 
@@ -339,79 +373,110 @@
         __descriptor (str): pyramid's descriptor path
         __list (str): pyramid's list path
         __tms (rok4.TileMatrixSet.TileMatrixSet): Used grid
         __levels (Dict[str, Level]): Pyramid's levels
         __format (str): Data format
         __storage (Dict[str, Union[rok4.Storage.StorageType,str,int]]): Pyramid's storage informations (type, root and depth if FILE storage)
         __raster_specifications (Dict): If raster pyramid, raster specifications
+        __content (Dict): Loading status (loaded) and list content (cache).
+
+            Example (S3 storage):
+
+                {
+                    'cache': {
+                        (<SlabType.DATA: 'DATA'>, '18', 5424, 7526): {
+                            'link': False,
+                            'md5': None,
+                            'root': 'pyramids@localhost:9000/LIMADM',
+                            'slab': 'DATA_18_5424_7526'
+                        }
+                    },
+                    'loaded': True
+                }
     """
 
     @classmethod
-    def from_descriptor(cls, descriptor: str) -> 'Pyramid':
+    def from_descriptor(cls, descriptor: str) -> "Pyramid":
         """Create a pyramid from its descriptor
 
         Args:
             descriptor (str): pyramid's descriptor path
 
         Raises:
             FormatError: Provided path or the TMS is not a well formed JSON
             Exception: Level issue : no one in the pyramid or the used TMS, or level ID not defined in the TMS
             MissingAttributeError: Attribute is missing in the content
             StorageError: Storage read issue (pyramid descriptor or TMS)
             MissingEnvironmentError: Missing object storage informations or TMS root directory
 
+        Examples:
+
+            S3 stored descriptor
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://bucket_name/path/to/descriptor.json")
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor")
+
         Returns:
             Pyramid: a Pyramid instance
-        """        
+        """
         try:
             data = json.loads(get_data_str(descriptor))
 
         except JSONDecodeError as e:
             raise FormatError("JSON", descriptor, e)
 
-
         pyramid = cls()
 
-        pyramid.__storage["type"], path, pyramid.__storage["root"], base_name = get_infos_from_path(descriptor)
-        pyramid.__name = base_name[:-5] # on supprime l'extension.json
+        pyramid.__storage["type"], path, pyramid.__storage["root"], base_name = get_infos_from_path(
+            descriptor
+        )
+        pyramid.__name = base_name[:-5]  # on supprime l'extension.json
         pyramid.__descriptor = descriptor
-        pyramid.__list = get_path_from_infos(pyramid.__storage["type"], pyramid.__storage["root"], f"{pyramid.__name}.list")
+        pyramid.__list = get_path_from_infos(
+            pyramid.__storage["type"], pyramid.__storage["root"], f"{pyramid.__name}.list"
+        )
 
         try:
             # Attributs communs
             pyramid.__tms = TileMatrixSet(data["tile_matrix_set"])
             pyramid.__format = data["format"]
 
             # Attributs d'une pyramide raster
-            if pyramid.type == PyramidType.RASTER :
+            if pyramid.type == PyramidType.RASTER:
                 pyramid.__raster_specifications = data["raster_specifications"]
 
                 if "mask_format" in data:
                     pyramid.__masks = True
                 else:
                     pyramid.__masks = False
 
             # Niveaux
             for l in data["levels"]:
                 lev = Level.from_descriptor(l, pyramid)
                 pyramid.__levels[lev.id] = lev
 
                 if pyramid.__tms.get_level(lev.id) is None:
-                    raise Exception(f"Pyramid {descriptor} owns a level with the ID '{lev.id}', not defined in the TMS '{pyramid.tms.name}'")
+                    raise Exception(
+                        f"Pyramid {descriptor} owns a level with the ID '{lev.id}', not defined in the TMS '{pyramid.tms.name}'"
+                    )
 
         except KeyError as e:
             raise MissingAttributeError(descriptor, e)
 
         if len(pyramid.__levels.keys()) == 0:
             raise Exception(f"Pyramid '{descriptor}' has no level")
 
         return pyramid
 
     @classmethod
-    def from_other(cls, other: 'Pyramid', name: str, storage: Dict) -> 'Pyramid':
+    def from_other(cls, other: "Pyramid", name: str, storage: Dict) -> "Pyramid":
         """Create a pyramid from another one
 
         Args:
             other (Pyramid): pyramid to clone
             name (str): new pyramid's name
             storage (Dict[str, Union[str, int]]): new pyramid's storage informations
 
@@ -432,57 +497,63 @@
 
             if storage["type"] == StorageType.FILE and "depth" not in storage:
                 storage["depth"] = 2
 
             pyramid = cls()
 
             # Attributs communs
-            pyramid.__name = name 
+            pyramid.__name = name
             pyramid.__storage = storage
             pyramid.__masks = other.__masks
 
-            pyramid.__descriptor = get_path_from_infos(pyramid.__storage["type"], pyramid.__storage["root"], f"{pyramid.__name}.json")
-            pyramid.__list = get_path_from_infos(pyramid.__storage["type"], pyramid.__storage["root"], f"{pyramid.__name}.list")
+            pyramid.__descriptor = get_path_from_infos(
+                pyramid.__storage["type"], pyramid.__storage["root"], f"{pyramid.__name}.json"
+            )
+            pyramid.__list = get_path_from_infos(
+                pyramid.__storage["type"], pyramid.__storage["root"], f"{pyramid.__name}.list"
+            )
             pyramid.__tms = other.__tms
             pyramid.__format = other.__format
 
             # Attributs d'une pyramide raster
-            if pyramid.type == PyramidType.RASTER :
+            if pyramid.type == PyramidType.RASTER:
                 if other.own_masks:
                     pyramid.__masks = True
                 else:
                     pyramid.__masks = False
                 pyramid.__raster_specifications = other.__raster_specifications
 
             # Niveaux
             for l in other.__levels.values():
                 lev = Level.from_other(l, pyramid)
                 pyramid.__levels[lev.id] = lev
 
-
         except KeyError as e:
             raise MissingAttributeError(descriptor, e)
 
         return pyramid
 
     def __init__(self) -> None:
-        self.__storage = dict()
-        self.__levels = dict()
+        self.__storage = {}
+        self.__levels = {}
         self.__masks = None
 
+        self.__content = {"loaded": False, "cache": {}}
+
     def __str__(self) -> str:
         return f"{self.type.name} pyramid '{self.__name}' ({self.__storage['type'].name} storage)"
 
     @property
-    def serializable(self) -> Dict: 
+    def serializable(self) -> Dict:
         """Get the dict version of the pyramid object, descriptor compliant
 
         Returns:
             Dict: descriptor structured object description
-        """        
+        """
+        
         serialization = {
             "tile_matrix_set": self.__tms.name,
             "format": self.__format
         }
 
         serialization["levels"] = []
         sorted_levels = sorted(self.__levels.values(), key=lambda l: l.resolution, reverse=True)
@@ -509,163 +580,319 @@
     @property
     def name(self) -> str:
         return self.__name
 
     @property
     def tms(self) -> TileMatrixSet:
         return self.__tms
-        
+
     @property
     def raster_specifications(self) -> Dict:
         """Get raster specifications for a RASTER pyramid
 
         Example:
             {
                 "channels": 3,
                 "nodata": "255,0,0",
                 "photometric": "rgb",
                 "interpolation": "bicubic"
             }
-        
+
         Returns:
             Dict: Raster specifications, None if VECTOR pyramid
-        """        
+        """
         return self.__raster_specifications
 
     @property
-    def storage_type(self) -> StorageType: 
+    def storage_type(self) -> StorageType:
         """Get the storage type
 
         Returns:
             StorageType: FILE, S3 or CEPH
-        """        
+        """
         return self.__storage["type"]
 
     @property
-    def storage_root(self) -> str: 
+    def storage_root(self) -> str:
         """Get the pyramid's storage root.
 
         If storage is S3, the used cluster is removed.
 
         Returns:
             str: Pyramid's storage root
-        """        
-        return self.__storage["root"].split("@", 1)[0] # Suppression de l'éventuel hôte de spécification du cluster S3
+        """
+        
+        return self.__storage["root"].split("@", 1)[
+            0
+        ]  # Suppression de l'éventuel hôte de spécification du cluster S3
 
     @property
-    def storage_depth(self) -> int: 
+    def storage_depth(self) -> int:
         return self.__storage.get("depth", None)
 
-
     @property
     def storage_s3_cluster(self) -> str:
         """Get the pyramid's storage S3 cluster (host name)
 
         Returns:
             str: the host if known, None if the default one have to be used or if storage is not S3
-        """        
+        """
         if self.__storage["type"] == StorageType.S3:
             try:
                 return self.__storage["root"].split("@")[1]
             except IndexError:
                 return None
         else:
             return None
 
-
     @storage_depth.setter
     def storage_depth(self, d: int) -> None:
         """Set the tree depth for a FILE storage
 
         Args:
             d (int): file storage depth
 
         Raises:
             Exception: the depth is not equal to the already known depth
-        """        
+        """
         if "depth" in self.__storage and self.__storage["depth"] != d:
-            raise Exception(f"Pyramid {pyramid.__descriptor} owns levels with different path depths")
+            raise Exception(
+                f"Pyramid {pyramid.__descriptor} owns levels with different path depths"
+            )
         self.__storage["depth"] = d
 
     @property
     def own_masks(self) -> bool:
         return self.__masks
 
     @property
-    def format(self) -> str: 
+    def format(self) -> str:
         return self.__format
 
     @property
-    def bottom_level(self) -> 'Level': 
+    def tile_extension(self) -> str:
+
+        if self.__format in [
+            "TIFF_RAW_UINT8",
+            "TIFF_LZW_UINT8",
+            "TIFF_ZIP_UINT8",
+            "TIFF_PKB_UINT8",
+            "TIFF_RAW_FLOAT32",
+            "TIFF_LZW_FLOAT32",
+            "TIFF_ZIP_FLOAT32",
+            "TIFF_PKB_FLOAT32",
+        ]:
+            return "tif"
+        elif self.__format in ["TIFF_JPG_UINT8", "TIFF_JPG90_UINT8"]:
+            return "jpg"
+        elif self.__format == "TIFF_PNG_UINT8":
+            return "png"
+        elif self.__format == "TIFF_PBF_MVT":
+            return "pbf"
+        else:
+            raise Exception(
+                f"Unknown pyramid's format ({self.__format}), cannot return the tile extension"
+            )
+
+    @property
+    def bottom_level(self) -> "Level":
         """Get the best resolution level in the pyramid
 
         Returns:
             Level: the bottom level
-        """   
+        """
         return sorted(self.__levels.values(), key=lambda l: l.resolution)[0]
 
     @property
-    def top_level(self) -> 'Level':
+    def top_level(self) -> "Level":
         """Get the low resolution level in the pyramid
 
         Returns:
             Level: the top level
-        """        
+        """
         return sorted(self.__levels.values(), key=lambda l: l.resolution)[-1]
 
     @property
     def type(self) -> PyramidType:
         """Get the pyramid's type (RASTER or VECTOR) from its format
 
         Returns:
             PyramidType: RASTER or VECTOR
-        """        
+        """
         if self.__format == "TIFF_PBF_MVT":
             return PyramidType.VECTOR
         else:
             return PyramidType.RASTER
 
-    def get_level(self, level_id: str) -> 'Level':
+    def load_list(self) -> None:
+        """Load list content and cache it
+
+        If list is already loaded, nothing done
+        """
+        if self.__content["loaded"]:
+            return
+
+        for slab, infos in self.list_generator():
+            self.__content["cache"][slab] = infos
+
+        self.__content["loaded"] = True
+
+    def list_generator(self) -> Iterator[Tuple[Tuple[SlabType, str, int, int], Dict]]:
+        """Get list content
+
+        List is copied as temporary file, roots are read and informations about each slab is returned. If list is already loaded, we yield the cached content
+
+        Examples:
+
+            S3 stored descriptor
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://bucket_name/path/to/descriptor.json")
+
+                    for (slab_type, level, column, row), infos in pyramid.list_generator():
+                        print(infos)
+
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor and read the list")
+
+        Yields:
+            Iterator[Tuple[Tuple[SlabType,str,int,int], Dict]]: Slab indices and storage informations
+
+            Value example:
+
+                (
+                    (<SlabType.DATA: 'DATA'>, '18', 5424, 7526),
+                    {
+                        'link': False,
+                        'md5': None,
+                        'root': 'pyramids@localhost:9000/LIMADM',
+                        'slab': 'DATA_18_5424_7526'
+                    }
+                )
+
+        """
+        if self.__content["loaded"]:
+            for slab, infos in self.__content["cache"].items():
+                yield slab, infos
+        else:
+            # Copie de la liste dans un fichier temporaire (cette liste peut être un objet)
+            list_obj = tempfile.NamedTemporaryFile(mode="r", delete=False)
+            list_file = list_obj.name
+            copy(self.__list, f"file://{list_file}")
+            list_obj.close()
+
+            roots = {}
+            s3_cluster = self.storage_s3_cluster
+
+            with open(list_file, "r") as listin:
+                # Lecture des racines
+                for line in listin:
+                    line = line.rstrip()
+
+                    if line == "#":
+                        break
+
+                    root_id, root_path = line.split("=", 1)
+
+                    if s3_cluster is None:
+                        roots[root_id] = root_path
+                    else:
+                        # On a un nom de cluster S3, on l'ajoute au nom du bucket dans les racines
+                        root_bucket, root_path = root_path.split("/", 1)
+                        roots[root_id] = f"{root_bucket}@{s3_cluster}/{root_path}"
+
+                # Lecture des dalles
+                for line in listin:
+                    line = line.rstrip()
+
+                    parts = line.split(" ", 1)
+                    slab_path = parts[0]
+                    slab_md5 = None
+                    if len(parts) == 2:
+                        slab_md5 = parts[1]
+
+                    root_id, slab_path = slab_path.split("/", 1)
+
+                    slab_type, level, column, row = self.get_infos_from_slab_path(slab_path)
+                    infos = {
+                        "root": roots[root_id],
+                        "link": root_id != "0",
+                        "slab": slab_path,
+                        "md5": slab_md5,
+                    }
+
+                    yield ((slab_type, level, column, row), infos)
+
+            remove(f"file://{list_file}")
+
+    def get_level(self, level_id: str) -> "Level":
         """Get one level according to its identifier
 
         Args:
             level_id: Level identifier
 
         Returns:
             The corresponding pyramid's level, None if not present
         """
-      
+        
         return self.__levels.get(level_id, None)
 
-
     def get_levels(self, bottom_id: str = None, top_id: str = None) -> List[Level]:
-        """Get sorted levels from bottom and top provided
+        """Get sorted levels in the provided range from bottom to top
 
         Args:
-            bottom_id (str): optionnal specific bottom level id. Defaults to None.
-            top_id (str): optionnal specific top level id. Defaults to None.
+            bottom_id (str, optionnal): specific bottom level id. Defaults to None.
+            top_id (str, optionnal): specific top level id. Defaults to None.
 
         Raises:
             Exception: Provided levels are not consistent (bottom > top or not in the pyramid)
 
+        Examples:
+
+            All levels
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://bucket_name/path/to/descriptor.json")
+                    levels = pyramid.get_levels()
+
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor and get levels")
+
+            From pyramid's bottom to provided top (level 5)
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://bucket_name/path/to/descriptor.json")
+                    levels = pyramid.get_levels(None, "5")
+
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor and get levels")
+
         Returns:
             List[Level]: asked sorted levels
         """
 
         sorted_levels = sorted(self.__levels.values(), key=lambda l: l.resolution)
-        
+
         levels = []
 
         begin = False
         if bottom_id is None:
             # Pas de niveau du bas fourni, on commence tout en bas
             begin = True
         else:
             if self.get_level(bottom_id) is None:
-                raise Exception(f"Pyramid {self.name} does not contain the provided bottom level {bottom_id}")
+                raise Exception(
+                    f"Pyramid {self.name} does not contain the provided bottom level {bottom_id}"
+                )
 
         if top_id is not None and self.get_level(top_id) is None:
             raise Exception(f"Pyramid {self.name} does not contain the provided top level {top_id}")
 
         end = False
 
         for l in sorted_levels:
@@ -675,57 +902,83 @@
             if begin:
                 levels.append(l)
                 if top_id is not None and l.id == top_id:
                     end = True
                     break
                 else:
                     continue
-        
+
         if top_id is None:
             # Pas de niveau du haut fourni, on a été jusqu'en haut et c'est normal
             end = True
 
         if not begin or not end:
-            raise Exception(f"Provided levels ids are not consistent to extract levels from the pyramid {self.name}")
-      
+            raise Exception(
+                f"Provided levels ids are not consistent to extract levels from the pyramid {self.name}"
+            )
+
         return levels
 
     def write_descriptor(self) -> None:
-        """Write the pyramid's descriptor to the final location (in the pyramid's storage root)
-        """        
+        """Write the pyramid's descriptor to the final location (in the pyramid's storage root)"""
+
         content = json.dumps(self.serializable)
         put_data_str(content, self.__descriptor)
 
     def get_infos_from_slab_path(self, path: str) -> Tuple[SlabType, str, int, int]:
         """Get the slab's indices from its storage path
 
         Args:
             path (str): Slab's storage path
 
+        Examples:
+
+            FILE stored pyramid
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("/path/to/descriptor.json")
+                    slab_type, level, column, row = self.get_infos_from_slab_path("DATA/12/00/4A/F7.tif")
+                    # (SlabType.DATA, "12", 159, 367)
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor and convert a slab path")
+
+            S3 stored pyramid
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://bucket_name/path/to/pyramid.json")
+                    slab_type, level, column, row = self.get_infos_from_slab_path("s3://bucket_name/path/to/pyramid/MASK_15_9164_5846")
+                    # (SlabType.MASK, "15", 9164, 5846)
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor and convert a slab path")
+
         Returns:
             Tuple[SlabType, str, int, int]: Slab's type (DATA or MASK), level identifier, slab's column and slab's row
-        """        
+        """
         if self.__storage["type"] == StorageType.FILE:
             parts = path.split("/")
 
             # Le partie du chemin qui contient la colonne et ligne de la dalle est à la fin, en fonction de la profondeur choisie
             # depth = 2 -> on doit utiliser les 3 dernières parties pour la conversion
-            column, row = b36_path_decode('/'.join(parts[-(self.__storage["depth"]+1):]))
-            level = parts[-(self.__storage["depth"]+2)]
-            raw_slab_type = parts[-(self.__storage["depth"]+3)]
+            column, row = b36_path_decode("/".join(parts[-(self.__storage["depth"] + 1) :]))
+            level = parts[-(self.__storage["depth"] + 2)]
+            raw_slab_type = parts[-(self.__storage["depth"] + 3)]
 
             # Pour être retro compatible avec l'ancien nommage
             if raw_slab_type == "IMAGE":
                 raw_slab_type = "DATA"
 
             slab_type = SlabType[raw_slab_type]
 
             return slab_type, level, column, row
         else:
-            parts = re.split(r'[/_]', path)
+            parts = re.split(r"[/_]", path)
             column = parts[-2]
             row = parts[-1]
             level = parts[-3]
             raw_slab_type = parts[-4]
 
             # Pour être retro compatible avec l'ancien nommage
             if raw_slab_type == "IMG":
@@ -733,66 +986,94 @@
             elif raw_slab_type == "MSK":
                 raw_slab_type = "MASK"
 
             slab_type = SlabType[raw_slab_type]
 
             return slab_type, level, int(column), int(row)
 
-    def get_slab_path_from_infos(self, slab_type: SlabType, level: str, column: int, row: int, full: bool = True) -> str:
+    def get_slab_path_from_infos(
+        self, slab_type: SlabType, level: str, column: int, row: int, full: bool = True
+    ) -> str:
         """Get slab's storage path from the indices
 
         Args:
             slab_type (SlabType): DATA or MASK
             level (str): Level identifier
             column (int): Slab's column
             row (int): Slab's row
             full (bool, optional): Full path or just relative path from pyramid storage root. Defaults to True.
 
         Returns:
             str: Absolute or relative slab's storage path
-        """        
+        """
         if self.__storage["type"] == StorageType.FILE:
-            slab_path = os.path.join(slab_type.value, level, b36_path_encode(column, row, self.__storage["depth"]))
+            slab_path = os.path.join(
+                slab_type.value, level, b36_path_encode(column, row, self.__storage["depth"])
+            )
         else:
             slab_path = f"{slab_type.value}_{level}_{column}_{row}"
-        
+
         if full:
-            return get_path_from_infos(self.__storage["type"], self.__storage["root"], self.__name, slab_path )
+            return get_path_from_infos(
+                self.__storage["type"], self.__storage["root"], self.__name, slab_path
+            )
         else:
             return slab_path
-        
+
 
     def get_tile_data_binary(self, level: str, column: int, row: int) -> str:
         """Get a pyramid's tile as binary string
 
         To get a tile, 3 steps :
-            * calculate slab path from tile indice
+            * calculate slab path from tile index
             * read slab index to get offsets and sizes of slab's tiles
             * read the tile into the slab
 
         Args:
             level (str): Tile's level
             column (int): Tile's column
             row (int): Tile's row
 
         Limitations:
             Pyramids with one-tile slab are not handled
 
+        Examples:
+
+            FILE stored raster pyramid, to extract a tile containing a point and save it as independent image
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("/data/pyramids/SCAN1000.json")
+                    level, col, row, pcol, prow = pyramid.get_tile_indices(992904.46, 6733643.15, "9", srs = "IGNF:LAMB93")
+                    data = pyramid.get_tile_data_binary(level, col, row)
+
+                    if data is None:
+                        print("No data")
+                    else:
+                        tile_name = f"tile_{level}_{col}_{row}.{pyramid.tile_extension}"
+                        with open(tile_name, "wb") as image:
+                            image.write(data)
+                        print (f"Tile written in {tile_name}")
+
+                except Exception as e:
+                    print("Cannot save a pyramid's tile : {e}")
+
         Raises:
             Exception: Level not found in the pyramid
             NotImplementedError: Pyramid owns one-tile slabs
             MissingEnvironmentError: Missing object storage informations
             StorageError: Storage read issue
 
         Returns:
             str: data, as binary string, None if no data
         """
 
         level_object = self.get_level(level)
-        
+
         if level_object is None:
             raise Exception(f"No level {level} in the pyramid")
 
         if level_object.slab_width == 1 and level_object.slab_height == 1:
             raise NotImplementedError(f"One-tile slab pyramid is not handled")
 
         if not level_object.is_in_limits(column, row):
@@ -809,33 +1090,39 @@
         # Numéro de la tuile dans le header
         tile_index = relative_tile_row * level_object.slab_width + relative_tile_column
 
         # Calcul du chemin de la dalle contenant la tuile voulue
         slab_path = self.get_slab_path_from_infos(SlabType.DATA, level, slab_column, slab_row)
 
         # Récupération des offset et tailles des tuiles dans la dalle
-        # Une dalle ROK4 a une en-tête fixe de 2048 octets, 
+        # Une dalle ROK4 a une en-tête fixe de 2048 octets,
         # puis sont stockés les offsets (chacun sur 4 octets)
         # puis les tailles (chacune sur 4 octets)
         try:
-            binary_index = get_data_binary(slab_path, (2048, 2 * 4 * level_object.slab_width * level_object.slab_height))
+            binary_index = get_data_binary(
+                slab_path,
+                (
+                    ROK4_IMAGE_HEADER_SIZE,
+                    2 * 4 * level_object.slab_width * level_object.slab_height,
+                ),
+            )
         except FileNotFoundError as e:
             # L'absence de la dalle est gérée comme simplement une absence de données
             return None
 
         offsets = numpy.frombuffer(
             binary_index,
-            dtype = numpy.dtype('uint32'),
-            count = level_object.slab_width * level_object.slab_height
+            dtype=numpy.dtype("uint32"),
+            count=level_object.slab_width * level_object.slab_height,
         )
         sizes = numpy.frombuffer(
             binary_index,
-            dtype = numpy.dtype('uint32'),
-            offset = 4 * level_object.slab_width * level_object.slab_height,
-            count = level_object.slab_width * level_object.slab_height
+            dtype=numpy.dtype("uint32"),
+            offset=4 * level_object.slab_width * level_object.slab_height,
+            count=level_object.slab_width * level_object.slab_height,
         )
 
         if sizes[tile_index] == 0:
             return None
 
         return get_data_binary(slab_path, (offsets[tile_index], sizes[tile_index]))
 
@@ -857,81 +1144,103 @@
             Exception: Level not found in the pyramid
             NotImplementedError: Pyramid owns one-tile slabs
             NotImplementedError: Raster pyramid format not handled
             MissingEnvironmentError: Missing object storage informations
             StorageError: Storage read issue
             FormatError: Cannot decode tile
 
+        Examples:
+
+            FILE stored DTM (raster) pyramid, to get the altitude value at a point in the best level
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("/data/pyramids/RGEALTI.json")
+                    level, col, row, pcol, prow = pyramid.get_tile_indices(44, 5, srs = "EPSG:4326")
+                    data = pyramid.get_tile_data_raster(level, col, row)
+
+                    if data is None:
+                        print("No data")
+                    else:
+                        print(data[prow][pcol])
+
+                except Exception as e:
+                    print("Cannot get a pyramid's pixel value : {e}")
+
         Returns:
             str: data, as numpy array, None if no data
         """
 
         if self.type == PyramidType.VECTOR:
             raise Exception("Cannot get tile as raster data : it's a vector pyramid")
 
         binary_tile = self.get_tile_data_binary(level, column, row)
 
         if binary_tile is None:
             return None
 
         level_object = self.get_level(level)
 
-
         if self.__format == "TIFF_JPG_UINT8" or self.__format == "TIFF_JPG90_UINT8":
-            
+
             try:
                 img = Image.open(io.BytesIO(binary_tile))
             except Exception as e:
                 raise FormatError("JPEG", "binary tile", e)
-            
+
             data = numpy.asarray(img)
 
         elif self.__format == "TIFF_RAW_UINT8":
-            data = numpy.frombuffer(
-                binary_tile,
-                dtype = numpy.dtype('uint8')
+            data = numpy.frombuffer(binary_tile, dtype=numpy.dtype("uint8"))
+            data.shape = (
+                level_object.tile_matrix.tile_size[0],
+                level_object.tile_matrix.tile_size[1],
+                self.__raster_specifications["channels"],
             )
-            data.shape = (level_object.tile_matrix.tile_size[0], level_object.tile_matrix.tile_size[1], self.__raster_specifications["channels"]) 
 
         elif self.__format == "TIFF_PNG_UINT8":
             try:
                 img = Image.open(io.BytesIO(binary_tile))
             except Exception as e:
                 raise FormatError("PNG", "binary tile", e)
-            
+
             data = numpy.asarray(img)
 
         elif self.__format == "TIFF_ZIP_UINT8":
             try:
-                data = numpy.frombuffer(
-                    zlib.decompress( binary_tile ),
-                    dtype = numpy.dtype('uint8')
-                )
+                data = numpy.frombuffer(zlib.decompress(binary_tile), dtype=numpy.dtype("uint8"))
             except Exception as e:
                 raise FormatError("ZIP", "binary tile", e)
 
-            data.shape = (level_object.tile_matrix.tile_size[0], level_object.tile_matrix.tile_size[1], self.__raster_specifications["channels"]) 
+            data.shape = (
+                level_object.tile_matrix.tile_size[0],
+                level_object.tile_matrix.tile_size[1],
+                self.__raster_specifications["channels"],
+            )
 
         elif self.__format == "TIFF_ZIP_FLOAT32":
             try:
-                data = numpy.frombuffer(
-                    zlib.decompress( binary_tile ),
-                    dtype = numpy.dtype('float32')
-                )
+                data = numpy.frombuffer(zlib.decompress(binary_tile), dtype=numpy.dtype("float32"))
             except Exception as e:
                 raise FormatError("ZIP", "binary tile", e)
 
-            data.shape = (level_object.tile_matrix.tile_size[0], level_object.tile_matrix.tile_size[1], self.__raster_specifications["channels"]) 
+            data.shape = (
+                level_object.tile_matrix.tile_size[0],
+                level_object.tile_matrix.tile_size[1],
+                self.__raster_specifications["channels"],
+            )
 
         elif self.__format == "TIFF_RAW_FLOAT32":
-            data = numpy.frombuffer(
-                binary_tile,
-                dtype = numpy.dtype('float32')
+            data = numpy.frombuffer(binary_tile, dtype=numpy.dtype("float32"))
+            data.shape = (
+                level_object.tile_matrix.tile_size[0],
+                level_object.tile_matrix.tile_size[1],
+                self.__raster_specifications["channels"],
             )
-            data.shape = (level_object.tile_matrix.tile_size[0], level_object.tile_matrix.tile_size[1], self.__raster_specifications["channels"]) 
 
         else:
             raise NotImplementedError(f"Cannot get tile as raster data for format {self.__format}")
 
         return data
 
     def get_tile_data_vector(self, level: str, column: int, row: int) -> Dict:
@@ -947,14 +1256,34 @@
             Exception: Level not found in the pyramid
             NotImplementedError: Pyramid owns one-tile slabs
             NotImplementedError: Vector pyramid format not handled
             MissingEnvironmentError: Missing object storage informations
             StorageError: Storage read issue
             FormatError: Cannot decode tile
 
+        Examples:
+
+            S3 stored vector pyramid, to print a tile as GeoJSON
+
+                from rok4.Pyramid import Pyramid
+                import json
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://pyramids/vectors/BDTOPO.json")
+                    level, col, row, pcol, prow = pyramid.get_tile_indices(40.325, 3.123, srs = "EPSG:4326")
+                    data = pyramid.get_tile_data_vector(level, col, row)
+
+                    if data is None:
+                        print("No data")
+                    else:
+                        print(json.dumps(data))
+
+                except Exception as e:
+                    print("Cannot print a vector pyramid's tile as GeoJSON : {e}")
+
         Returns:
             str: data, as GeoJSON dictionnary. None if no data
         """
 
         if self.type == PyramidType.RASTER:
             raise Exception("Cannot get tile as vector data : it's a raster pyramid")
 
@@ -971,38 +1300,85 @@
             except Exception as e:
                 raise FormatError("PBF (MVT)", "binary tile", e)
         else:
             raise NotImplementedError(f"Cannot get tile as vector data for format {self.__format}")
 
         return data
 
-    def get_tile_indices(self, x: float, y: float, level: str = None, **kwargs) -> Tuple[str, int, int, int, int]:
+    def get_tile_indices(
+        self, x: float, y: float, level: str = None, **kwargs
+    ) -> Tuple[str, int, int, int, int]:
         """Get pyramid's tile and pixel indices from point's coordinates
 
-        Used coordinates system have to be the pyramide one. If EPSG:4326, x is latitude and y longitude.
+        Used coordinates system have to be the pyramid one. If EPSG:4326, x is latitude and y longitude.
 
         Args:
             x (float): point's x
             y (float): point's y
             level (str, optional): Pyramid's level to take into account, the bottom one if None . Defaults to None.
             **srs (string): spatial reference system of provided coordinates, with authority and code (same as the pyramid's one if not provided)
 
         Raises:
             Exception: Cannot find level to calculate indices
             RuntimeError: Provided SRS is invalid for OSR
 
+        Examples:
+
+            FILE stored DTM (raster) pyramid, to get the altitude value at a point in the best level
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("/data/pyramids/RGEALTI.json")
+                    level, col, row, pcol, prow = pyramid.get_tile_indices(44, 5, srs = "EPSG:4326")
+                    data = pyramid.get_tile_data_raster(level, col, row)
+
+                    if data is None:
+                        print("No data")
+                    else:
+                        print(data[prow][pcol])
+
+                except Exception as e:
+                    print("Cannot get a pyramid's pixel value : {e}")
+
         Returns:
             Tuple[str, int, int, int, int]: Level identifier, tile's column, tile's row, pixel's (in the tile) column, pixel's row
         """
 
         level_object = self.bottom_level
         if level is not None:
             level_object = self.get_level(level)
-        
+
         if level_object is None:
             raise Exception(f"Cannot found the level to calculate indices")
 
-        if "srs" in kwargs and kwargs["srs"] is not None and kwargs["srs"].upper() != self.__tms.srs.upper():
+        if (
+            "srs" in kwargs
+            and kwargs["srs"] is not None
+            and kwargs["srs"].upper() != self.__tms.srs.upper()
+        ):
             sr = srs_to_spatialreference(kwargs["srs"])
-            x, y = reproject_point((x, y), sr, self.__tms.sr )
+            x, y = reproject_point((x, y), sr, self.__tms.sr)
 
         return (level_object.id,) + level_object.tile_matrix.point_to_indices(x, y)
+
+    @property
+    def size(self) -> int:
+        """Get the size of the pyramid
+
+        Examples:
+
+                from rok4.Pyramid import Pyramid
+
+                try:
+                    pyramid = Pyramid.from_descriptor("s3://bucket_name/path/to/descriptor.json")
+                    size = pyramid.size()
+
+                except Exception as e:
+                    print("Cannot load the pyramid from its descriptor and get his size")
+
+        Returns:
+            int: size of the pyramid
+        """
+        if not hasattr(self,"_Pyramid__size") :
+            self.__size = size_path(get_path_from_infos(self.__storage["type"], self.__storage["root"], self.__name))
+        return self.__size
```

### Comparing `rok4-1.6.0/src/rok4/Storage.py` & `rok4-1.7.0/src/rok4/Storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Provide functions to use read or write
 
 Available storage types are :
 - S3 (path are preffixed with `s3://`)
-- CEPH (path are preffixed with `ceph://`)
-- FILE (path are preffixed with `file://`, but it is the default paths' interpretation)
+- CEPH (path are prefixed with `ceph://`)
+- FILE (path are prefixed with `file://`, but it is the default paths' interpretation)
+- HTTP (path are prefixed with `http://`)
+- HTTPS (path are prefixed with `https://`)
 
 According to functions, all storage types are not necessarily available.
 
 Using CEPH storage requires environment variables :
 - ROK4_CEPH_CONFFILE
 - ROK4_CEPH_USERNAME
 - ROK4_CEPH_CLUSTERNAME
@@ -31,163 +33,178 @@
 import boto3
 import botocore.exceptions
 import tempfile
 import re
 import os
 import rados
 import hashlib
+import requests
 from typing import Dict, List, Tuple, Union
 from enum import Enum
 from shutil import copyfile
 from osgeo import gdal
 
 gdal.UseExceptions()
 
 from rok4.Exceptions import *
 
+
 class StorageType(Enum):
     FILE = "file://"
     S3 = "s3://"
     CEPH = "ceph://"
+    HTTP = "http://"
+    HTTPS = "https://"
+
 
-__S3_CLIENTS = dict()
+__S3_CLIENTS = {}
 __S3_DEFAULT_CLIENT = None
-def __get_s3_client(bucket_name: str) -> Tuple[Dict[str, Union['boto3.client',str]], str, str]:
+
+
+def __get_s3_client(bucket_name: str) -> Tuple[Dict[str, Union["boto3.client", str]], str, str]:
     """Get the S3 client
 
     Create it if not already done
 
     Args:
         bucket_name (str): S3 bucket name. Could be just the bucket name, or <bucket name>@<cluster host>
 
     Raises:
         MissingEnvironmentError: Missing S3 storage informations
         StorageError: S3 client configuration issue
 
     Returns:
         Tuple[Dict[str, Union['boto3.client',str]], str, str]: the S3 informations (client, host, key, secret) and the simple bucket name
-    """    
+    """
+    
     global __S3_CLIENTS, __S3_DEFAULT_CLIENT
 
     if not __S3_CLIENTS:
         # C'est la première fois qu'on cherche à utiliser le stockage S3, chargeons les informations depuis les variables d'environnement
         try:
             keys = os.environ["ROK4_S3_KEY"].split(",")
             secret_keys = os.environ["ROK4_S3_SECRETKEY"].split(",")
             urls = os.environ["ROK4_S3_URL"].split(",")
 
             if len(keys) != len(secret_keys) or len(keys) != len(urls):
-                raise StorageError("S3", "S3 informations in environment variables are inconsistent : same number of element in each list is required")
+                raise StorageError(
+                    "S3",
+                    "S3 informations in environment variables are inconsistent : same number of element in each list is required",
+                )
 
             for i in range(len(keys)):
-
                 h = re.sub("https?://", "", urls[i])
 
                 if h in __S3_CLIENTS:
                     raise StorageError("S3", "A S3 cluster is defined twice (based on URL)")
 
                 __S3_CLIENTS[h] = {
                     "client": boto3.client(
-                        's3',
-                        aws_access_key_id = keys[i],
-                        aws_secret_access_key = secret_keys[i],
-                        endpoint_url = urls[i]
+                        "s3",
+                        aws_access_key_id=keys[i],
+                        aws_secret_access_key=secret_keys[i],
+                        endpoint_url=urls[i],
                     ),
                     "key": keys[i],
                     "secret_key": secret_keys[i],
                     "url": urls[i],
-                    "host": h
+                    "host": h,
                 }
 
                 if i == 0:
                     # Le premier cluster est celui par défaut
                     __S3_DEFAULT_CLIENT = h
 
         except KeyError as e:
             raise MissingEnvironmentError(e)
         except Exception as e:
             raise StorageError("S3", e)
 
-
     try:
         host = bucket_name.split("@")[1]
     except IndexError:
         host = __S3_DEFAULT_CLIENT
 
     bucket_name = bucket_name.split("@")[0]
 
     if host not in __S3_CLIENTS:
         raise StorageError("S3", f"Unknown S3 cluster, according to host '{host}'")
 
     return __S3_CLIENTS[host], bucket_name
 
+
 def disconnect_s3_clients() -> None:
-    """Clean S3 clients
-    """    
+    """Clean S3 clients"""
+  
     global __S3_CLIENTS, __S3_DEFAULT_CLIENT
-    __S3_CLIENTS = dict()
+    __S3_CLIENTS = {}
     __S3_DEFAULT_CLIENT = None
 
+
 __CEPH_CLIENT = None
-__CEPH_IOCTXS = dict()
-def __get_ceph_ioctx(pool: str) -> 'rados.Ioctx':
+__CEPH_IOCTXS = {}
+
+
+def __get_ceph_ioctx(pool: str) -> "rados.Ioctx":
     """Get the CEPH IO context
 
     Create it (client and context) if not already done
 
     Args:
         pool (str): CEPH pool's name
 
     Raises:
         MissingEnvironmentError: Missing CEPH storage informations
         StorageError: CEPH IO context configuration issue
 
     Returns:
         rados.Ioctx: IO ceph context
-    """    
+    """
     global __CEPH_CLIENT, __CEPH_IOCTXS
 
     if __CEPH_CLIENT is None:
         try:
             __CEPH_CLIENT = rados.Rados(
-                conffile = os.environ["ROK4_CEPH_CONFFILE"],
-                clustername = os.environ["ROK4_CEPH_CLUSTERNAME"],
-                name = os.environ["ROK4_CEPH_USERNAME"]
+                conffile=os.environ["ROK4_CEPH_CONFFILE"],
+                clustername=os.environ["ROK4_CEPH_CLUSTERNAME"],
+                name=os.environ["ROK4_CEPH_USERNAME"],
             )
 
             __CEPH_CLIENT.connect()
-            
+
         except KeyError as e:
             raise MissingEnvironmentError(e)
         except Exception as e:
             raise StorageError("CEPH", e)
 
     if pool not in __CEPH_IOCTXS:
         try:
             __CEPH_IOCTXS[pool] = __CEPH_CLIENT.open_ioctx(pool)
         except Exception as e:
             raise StorageError("CEPH", e)
-    
+
     return __CEPH_IOCTXS[pool]
 
+
 def disconnect_ceph_clients() -> None:
-    """Clean CEPH clients
-    """    
+    """Clean CEPH clients"""
     global __CEPH_CLIENT, __CEPH_IOCTXS
     __CEPH_CLIENT = None
-    __CEPH_IOCTXS = dict()
+    __CEPH_IOCTXS = {}
+
 
 __OBJECT_SYMLINK_SIGNATURE = "SYMLINK#"
 
+
 def get_infos_from_path(path: str) -> Tuple[StorageType, str, str, str]:
     """Extract storage type, the unprefixed path, the container and the basename from path (Default: FILE storage)
 
     For a FILE storage, the tray is the directory and the basename is the file name.
-    
-    For an object storage (CEPH or S3), the tray is the bucket or the pool and the basename is the object name. 
+
+    For an object storage (CEPH or S3), the tray is the bucket or the pool and the basename is the object name.
     For a S3 bucket, format can be <bucket name>@<cluster name> to use several clusters. Cluster name is the host (without protocol)
 
     Args:
         path (str): path to analyse
 
     Returns:
         Tuple[StorageType, str, str, str]: storage type, unprefixed path, the container and the basename
@@ -197,29 +214,33 @@
         bucket_name, object_name = path[5:].split("/", 1)
         return StorageType.S3, path[5:], bucket_name, object_name
     elif path.startswith("ceph://"):
         pool_name, object_name = path[7:].split("/", 1)
         return StorageType.CEPH, path[7:], pool_name, object_name
     elif path.startswith("file://"):
         return StorageType.FILE, path[7:], os.path.dirname(path[7:]), os.path.basename(path[7:])
+    elif path.startswith("http://"):
+        return StorageType.HTTP, path[7:], os.path.dirname(path[7:]), os.path.basename(path[7:])
+    elif path.startswith("https://"):
+        return StorageType.HTTPS, path[8:], os.path.dirname(path[8:]), os.path.basename(path[8:])
     else:
         return StorageType.FILE, path, os.path.dirname(path), os.path.basename(path)
 
 
 def get_path_from_infos(storage_type: StorageType, *args) -> str:
     """Write full path from elements
 
     Prefixed wih storage's type, elements are joined with a slash
 
     Args:
         storage_type (StorageType): Storage's type for path
 
     Returns:
         str: Full path
-    """    
+    """
     return f"{storage_type.value}{os.path.join(*args)}"
 
 
 def hash_file(path: str) -> str:
     """Process MD5 sum of the provided file
 
     Args:
@@ -227,22 +248,23 @@
 
     Returns:
         str: hexadeimal MD5 sum
     """
 
     checker = hashlib.md5()
 
-    with open(path,'rb') as file:
+    with open(path, "rb") as file:
         chunk = 0
-        while chunk != b'':
+        while chunk != b"":
             chunk = file.read(65536)
             checker.update(chunk)
 
     return checker.hexdigest()
 
+
 def get_data_str(path: str) -> str:
     """Load full data into a string
 
     Args:
         path (str): path to data
 
     Raises:
@@ -250,63 +272,68 @@
         StorageError: Storage read issue
         FileNotFoundError: File or object does not exist
 
     Returns:
         str: Data content
     """
 
-    return get_data_binary(path).decode('utf-8')
+    return get_data_binary(path).decode("utf-8")
 
 
-def get_data_binary(path: str, range: Tuple[int, int] = None) -> str: 
+def get_data_binary(path: str, range: Tuple[int, int] = None) -> str:
     """Load data into a binary string
 
     Args:
         path (str): path to data
         range (Tuple[int, int], optional): offset and size, to make a partial read. Defaults to None.
 
     Raises:
         MissingEnvironmentError: Missing object storage informations
         StorageError: Storage read issue
         FileNotFoundError: File or object does not exist
 
     Returns:
         str: Data binary content
     """
-
-    storage_type, path, tray_name, base_name  = get_infos_from_path(path)        
+    storage_type, path, tray_name, base_name = get_infos_from_path(path)
 
     if storage_type == StorageType.S3:
-        
         s3_client, bucket_name = __get_s3_client(tray_name)
 
         try:
             if range is None:
-                data = s3_client["client"].get_object(
-                    Bucket=bucket_name,
-                    Key=base_name,
-                )['Body'].read()
+                data = (
+                    s3_client["client"]
+                    .get_object(
+                        Bucket=bucket_name,
+                        Key=base_name,
+                    )["Body"]
+                    .read()
+                )
             else:
-                data = s3_client["client"].get_object(
-                    Bucket=bucket_name,
-                    Key=base_name,
-                    Range=f"bytes={range[0]}-{range[0] + range[1] - 1}"
-                )['Body'].read()
+                data = (
+                    s3_client["client"]
+                    .get_object(
+                        Bucket=bucket_name,
+                        Key=base_name,
+                        Range=f"bytes={range[0]}-{range[0] + range[1] - 1}",
+                    )["Body"]
+                    .read()
+                )
 
         except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == "404":
+            if e.response["Error"]["Code"] == "404":
                 raise FileNotFoundError(f"{storage_type.value}{path}")
             else:
                 raise StorageError("S3", e)
 
         except Exception as e:
             raise StorageError("S3", e)
 
     elif storage_type == StorageType.CEPH:
-        
         ioctx = __get_ceph_ioctx(tray_name)
 
         try:
             if range is None:
                 size, mtime = ioctx.stat(base_name)
                 data = ioctx.read(base_name, size)
             else:
@@ -315,78 +342,86 @@
         except rados.ObjectNotFound as e:
             raise FileNotFoundError(f"{storage_type.value}{path}")
 
         except Exception as e:
             raise StorageError("CEPH", e)
 
     elif storage_type == StorageType.FILE:
-
         try:
-            f = open(path, 'rb')
+            f = open(path, "rb")
             if range is None:
                 data = f.read()
             else:
                 f.seek(range[0])
                 data = f.read(range[1])
-            
+
             f.close()
 
         except FileNotFoundError as e:
             raise FileNotFoundError(f"{storage_type.value}{path}")
 
         except Exception as e:
             raise StorageError("FILE", e)
 
+    elif storage_type == StorageType.HTTP or storage_type == StorageType.HTTPS:
+
+        if range is None :
+            try:
+                reponse = requests.get(f"{storage_type.value}{path}", stream=True)
+                data = reponse.content
+                if reponse.status_code == 404 :
+                    raise FileNotFoundError(f"{storage_type.value}{path}")
+            except Exception as e:
+                raise StorageError(storage_type.name, e)
+        else :
+            raise NotImplementedError
+
     else:
         raise StorageError("UNKNOWN", "Unhandled storage type to read binary data")
 
     return data
 
+
 def put_data_str(data: str, path: str) -> None:
     """Store string data into a file or an object
 
     UTF-8 encoding is used for bytes conversion
 
     Args:
         data (str): data to write
         path (str): destination path, where to write data
 
     Raises:
         MissingEnvironmentError: Missing object storage informations
         StorageError: Storage write issue
     """
 
-    storage_type, path, tray_name, base_name  = get_infos_from_path(path)
+    storage_type, path, tray_name, base_name = get_infos_from_path(path)
 
     if storage_type == StorageType.S3:
-        
         s3_client, bucket_name = __get_s3_client(tray_name)
 
         try:
             s3_client["client"].put_object(
-                Body = data.encode('utf-8'),
-                Bucket = bucket_name,
-                Key = base_name
+                Body=data.encode("utf-8"), Bucket=bucket_name, Key=base_name
             )
         except Exception as e:
             raise StorageError("S3", e)
 
     elif storage_type == StorageType.CEPH:
-        
         ioctx = __get_ceph_ioctx(tray_name)
 
         try:
-            ioctx.write_full(base_name, data.encode('utf-8'))
+            ioctx.write_full(base_name, data.encode("utf-8"))
         except Exception as e:
             raise StorageError("CEPH", e)
 
     elif storage_type == StorageType.FILE:
-
         try:
-            f = open(path, 'w')
+            f = open(path, "w")
             f.write(data)
             f.close()
         except Exception as e:
             raise StorageError("FILE", e)
 
     else:
         raise StorageError("UNKNOWN", "Unhandled storage type to write string data")
@@ -402,44 +437,52 @@
         MissingEnvironmentError: Missing object storage informations
         StorageError: Storage read issue
 
     Returns:
         int: file/object size, in bytes
     """
 
-    storage_type, path, tray_name, base_name  = get_infos_from_path(path)
+    storage_type, path, tray_name, base_name = get_infos_from_path(path)
 
     if storage_type == StorageType.S3:
-
         s3_client, bucket_name = __get_s3_client(tray_name)
 
         try:
-            size = s3_client["client"].head_object(Bucket=bucket_name, Key=base_name)["ContentLength"].strip('"')
+            size = s3_client["client"].head_object(Bucket=bucket_name, Key=base_name)[
+                "ContentLength"
+            ]
             return int(size)
         except Exception as e:
             raise StorageError("S3", e)
 
     elif storage_type == StorageType.CEPH:
-
         ioctx = __get_ceph_ioctx(tray_name)
 
         try:
             size, mtime = ioctx.stat(base_name)
             return size
         except Exception as e:
             raise StorageError("CEPH", e)
 
     elif storage_type == StorageType.FILE:
-
         try:
             file_stats = os.stat(path)
             return file_stats.st_size
         except Exception as e:
             raise StorageError("FILE", e)
 
+    elif storage_type == StorageType.HTTP or storage_type == StorageType.HTTPS:
+
+        try:
+            # Le stream=True permet de ne télécharger que le header initialement
+            reponse = requests.get(storage_type.value + path, stream=True).headers["content-length"]
+            return reponse
+        except Exception as e:
+            raise StorageError(storage_type.name, e)
+
     else:
         raise StorageError("UNKNOWN", "Unhandled storage type to get size")
 
 
 def exists(path: str) -> bool:
     """Do the file or object exist ?
 
@@ -450,200 +493,217 @@
         MissingEnvironmentError: Missing object storage informations
         StorageError: Storage read issue
 
     Returns:
         bool: file/object existing status
     """
 
-    storage_type, path, tray_name, base_name  = get_infos_from_path(path)
+    storage_type, path, tray_name, base_name = get_infos_from_path(path)
 
     if storage_type == StorageType.S3:
-
         s3_client, bucket_name = __get_s3_client(tray_name)
 
         try:
             s3_client["client"].head_object(Bucket=bucket_name, Key=base_name)
             return True
         except botocore.exceptions.ClientError as e:
-            if e.response['Error']['Code'] == "404":
+            if e.response["Error"]["Code"] == "404":
                 return False
             else:
                 raise StorageError("S3", e)
 
     elif storage_type == StorageType.CEPH:
-
         ioctx = __get_ceph_ioctx(tray_name)
 
         try:
             ioctx.stat(base_name)
             return True
         except rados.ObjectNotFound as e:
             return False
         except Exception as e:
             raise StorageError("CEPH", e)
 
     elif storage_type == StorageType.FILE:
-
         return os.path.exists(path)
 
+    elif storage_type == StorageType.HTTP or storage_type == StorageType.HTTPS:
+
+        try:
+            response = requests.get(storage_type.value + path, stream=True)
+            if response.status_code == 200 :
+                return True
+            else :
+                return False
+        except Exception as e:
+            raise StorageError(storage_type.name, e)
+
     else:
         raise StorageError("UNKNOWN", "Unhandled storage type to test if exists")
 
+
 def remove(path: str) -> None:
     """Remove the file/object
 
     Args:
         path (str): path of file/object to remove
 
     Raises:
         MissingEnvironmentError: Missing object storage informations
         StorageError: Storage removal issue
     """
-    storage_type, path, tray_name, base_name  = get_infos_from_path(path)
+    storage_type, path, tray_name, base_name = get_infos_from_path(path)
 
     if storage_type == StorageType.S3:
-
         s3_client, bucket_name = __get_s3_client(tray_name)
 
         try:
-            s3_client["client"].delete_object(
-                Bucket=bucket_name,
-                Key=base_name
-            )
+            s3_client["client"].delete_object(Bucket=bucket_name, Key=base_name)
         except Exception as e:
             raise StorageError("S3", e)
 
     elif storage_type == StorageType.CEPH:
-
         ioctx = __get_ceph_ioctx(tray_name)
 
         try:
             ioctx.remove_object(base_name)
         except rados.ObjectNotFound as e:
             pass
         except Exception as e:
             raise StorageError("CEPH", e)
 
     elif storage_type == StorageType.FILE:
-
         try:
             os.remove(path)
         except FileNotFoundError as e:
             pass
         except Exception as e:
             raise StorageError("FILE", e)
 
     else:
         raise StorageError("UNKNOWN", "Unhandled storage type to remove things")
 
+
 def copy(from_path: str, to_path: str, from_md5: str = None) -> None:
     """Copy a file or object to a file or object place. If MD5 sum is provided, it is compared to sum after the copy.
 
     Args:
         from_path (str): source file/object path, to copy
         to_path (str): destination file/object path
         from_md5 (str, optional): MD5 sum, re-processed after copy and controlled. Defaults to None.
 
     Raises:
         StorageError: Unhandled copy or copy issue
         MissingEnvironmentError: Missing object storage informations
     """
 
-    from_type, from_path, from_tray, from_base_name  = get_infos_from_path(from_path)
-    to_type, to_path, to_tray, to_base_name  = get_infos_from_path(to_path)
+    from_type, from_path, from_tray, from_base_name = get_infos_from_path(from_path)
+    to_type, to_path, to_tray, to_base_name = get_infos_from_path(to_path)
 
     # Réalisation de la copie, selon les types de stockage
-    if from_type == StorageType.FILE and to_type == StorageType.FILE :
-        
+    if from_type == StorageType.FILE and to_type == StorageType.FILE:
         try:
             if to_tray != "":
                 os.makedirs(to_tray, exist_ok=True)
 
             copyfile(from_path, to_path)
 
-            if from_md5 is not None :
+            if from_md5 is not None:
                 to_md5 = hash_file(to_path)
                 if to_md5 != from_md5:
-                    raise StorageError(f"FILE", f"Invalid MD5 sum control for copy file {from_path} to {to_path} : {from_md5} != {to_md5}")
+                    raise StorageError(
+                        f"FILE",
+                        f"Invalid MD5 sum control for copy file {from_path} to {to_path} : {from_md5} != {to_md5}",
+                    )
 
         except Exception as e:
             raise StorageError(f"FILE", f"Cannot copy file {from_path} to {to_path} : {e}")
 
-    elif from_type == StorageType.S3 and to_type == StorageType.FILE :
-        
+    elif from_type == StorageType.S3 and to_type == StorageType.FILE:
         s3_client, from_bucket = __get_s3_client(from_tray)
 
         try:
             if to_tray != "":
                 os.makedirs(to_tray, exist_ok=True)
-            
+
             s3_client["client"].download_file(from_bucket, from_base_name, to_path)
 
-            if from_md5 is not None :
+            if from_md5 is not None:
                 to_md5 = hash_file(to_path)
                 if to_md5 != from_md5:
-                    raise StorageError("S3 and FILE", f"Invalid MD5 sum control for copy S3 object {from_path} to file {to_path} : {from_md5} != {to_md5}")
+                    raise StorageError(
+                        "S3 and FILE",
+                        f"Invalid MD5 sum control for copy S3 object {from_path} to file {to_path} : {from_md5} != {to_md5}",
+                    )
 
         except Exception as e:
-            raise StorageError(f"S3 and FILE", f"Cannot copy S3 object {from_path} to file {to_path} : {e}")
-
-    elif from_type == StorageType.FILE and to_type == StorageType.S3 :
+            raise StorageError(
+                f"S3 and FILE", f"Cannot copy S3 object {from_path} to file {to_path} : {e}"
+            )
 
+    elif from_type == StorageType.FILE and to_type == StorageType.S3:
         s3_client, to_bucket = __get_s3_client(to_tray)
-        
+
         try:
             s3_client["client"].upload_file(from_path, to_bucket, to_base_name)
 
-            if from_md5 is not None :
-                to_md5 = s3_client["client"].head_object(Bucket=to_bucket, Key=to_base_name)["ETag"].strip('"')
+            if from_md5 is not None:
+                to_md5 = (
+                    s3_client["client"]
+                    .head_object(Bucket=to_bucket, Key=to_base_name)["ETag"]
+                    .strip('"')
+                )
                 if to_md5 != from_md5:
-                    raise StorageError(f"FILE and S3", f"Invalid MD5 sum control for copy file {from_path} to S3 object {to_path} : {from_md5} != {to_md5}")
+                    raise StorageError(
+                        f"FILE and S3",
+                        f"Invalid MD5 sum control for copy file {from_path} to S3 object {to_path} : {from_md5} != {to_md5}",
+                    )
         except Exception as e:
-            raise StorageError(f"FILE and S3", f"Cannot copy file {from_path} to S3 object {to_path} : {e}")
-
-    elif from_type == StorageType.S3 and to_type == StorageType.S3 :
+            raise StorageError(
+                f"FILE and S3", f"Cannot copy file {from_path} to S3 object {to_path} : {e}"
+            )
 
+    elif from_type == StorageType.S3 and to_type == StorageType.S3:
         from_s3_client, from_bucket = __get_s3_client(from_tray)
         to_s3_client, to_bucket = __get_s3_client(to_tray)
 
         try:
             if to_s3_client["host"] == from_s3_client["host"]:
                 to_s3_client["client"].copy(
-                    {
-                        'Bucket': from_bucket,
-                        'Key': from_base_name
-                    }, 
-                    to_bucket, to_base_name
+                    {"Bucket": from_bucket, "Key": from_base_name}, to_bucket, to_base_name
                 )
             else:
                 with tempfile.NamedTemporaryFile("w+b") as f:
                     from_s3_client["client"].download_fileobj(from_bucket, from_base_name, f)
                     to_s3_client["client"].upload_file(f.name, to_bucket, to_base_name)
 
-            if from_md5 is not None :
-                to_md5 = to_s3_client["client"].head_object(Bucket=to_bucket, Key=to_base_name)["ETag"].strip('"')
+            if from_md5 is not None:
+                to_md5 = (
+                    to_s3_client["client"]
+                    .head_object(Bucket=to_bucket, Key=to_base_name)["ETag"]
+                    .strip('"')
+                )
                 if to_md5 != from_md5:
-                    raise StorageError(f"S3", f"Invalid MD5 sum control for copy S3 object {from_path} to {to_path} : {from_md5} != {to_md5}")
+                    raise StorageError(
+                        f"S3",
+                        f"Invalid MD5 sum control for copy S3 object {from_path} to {to_path} : {from_md5} != {to_md5}",
+                    )
 
         except Exception as e:
             raise StorageError(f"S3", f"Cannot copy S3 object {from_path} to {to_path} : {e}")
-        
-
-    elif from_type == StorageType.CEPH and to_type == StorageType.FILE :
 
+    elif from_type == StorageType.CEPH and to_type == StorageType.FILE:
         ioctx = __get_ceph_ioctx(from_tray)
 
         if from_md5 is not None:
             checker = hashlib.md5()
 
         try:
-
             if to_tray != "":
                 os.makedirs(to_tray, exist_ok=True)
-            f = open(to_path, 'wb')
+            f = open(to_path, "wb")
 
             offset = 0
             size = 0
 
             while True:
                 chunk = ioctx.read(from_base_name, 65536, offset)
                 size = len(chunk)
@@ -655,65 +715,69 @@
 
                 if size < 65536:
                     break
 
             f.close()
 
             if from_md5 is not None and from_md5 != checker.hexdigest():
-                raise StorageError(f"CEPH and FILE", f"Invalid MD5 sum control for copy CEPH object {from_path} to file {to_path} : {from_md5} != {checker.hexdigest()}")
+                raise StorageError(
+                    f"CEPH and FILE",
+                    f"Invalid MD5 sum control for copy CEPH object {from_path} to file {to_path} : {from_md5} != {checker.hexdigest()}",
+                )
 
         except Exception as e:
-            raise StorageError(f"CEPH and FILE", f"Cannot copy CEPH object {from_path} to file {to_path} : {e}")
-
-
-    elif from_type == StorageType.FILE and to_type == StorageType.CEPH :
+            raise StorageError(
+                f"CEPH and FILE", f"Cannot copy CEPH object {from_path} to file {to_path} : {e}"
+            )
 
+    elif from_type == StorageType.FILE and to_type == StorageType.CEPH:
         ioctx = __get_ceph_ioctx(to_tray)
-        
+
         if from_md5 is not None:
             checker = hashlib.md5()
 
         try:
-            f = open(from_path, 'rb')
+            f = open(from_path, "rb")
 
             offset = 0
             size = 0
 
             while True:
-
                 chunk = f.read(65536)
                 size = len(chunk)
                 ioctx.write(to_base_name, chunk, offset)
                 offset += size
 
                 if from_md5 is not None:
                     checker.update(chunk)
 
                 if size < 65536:
                     break
 
             f.close()
 
             if from_md5 is not None and from_md5 != checker.hexdigest():
-                raise StorageError(f"FILE and CEPH", f"Invalid MD5 sum control for copy file {from_path} to CEPH object {to_path} : {from_md5} != {checker.hexdigest()}")
+                raise StorageError(
+                    f"FILE and CEPH",
+                    f"Invalid MD5 sum control for copy file {from_path} to CEPH object {to_path} : {from_md5} != {checker.hexdigest()}",
+                )
 
         except Exception as e:
-            raise StorageError(f"FILE and CEPH", f"Cannot copy file {from_path} to CEPH object {to_path} : {e}")
-
-
-    elif from_type == StorageType.CEPH and to_type == StorageType.CEPH :
+            raise StorageError(
+                f"FILE and CEPH", f"Cannot copy file {from_path} to CEPH object {to_path} : {e}"
+            )
 
+    elif from_type == StorageType.CEPH and to_type == StorageType.CEPH:
         from_ioctx = __get_ceph_ioctx(from_tray)
         to_ioctx = __get_ceph_ioctx(to_tray)
 
         if from_md5 is not None:
             checker = hashlib.md5()
 
         try:
-
             offset = 0
             size = 0
 
             while True:
                 chunk = from_ioctx.read(from_base_name, 65536, offset)
                 size = len(chunk)
                 to_ioctx.write(to_base_name, chunk, offset)
@@ -722,33 +786,35 @@
                 if from_md5 is not None:
                     checker.update(chunk)
 
                 if size < 65536:
                     break
 
             if from_md5 is not None and from_md5 != checker.hexdigest():
-                raise StorageError(f"FILE and CEPH", f"Invalid MD5 sum control for copy CEPH object {from_path} to {to_path} : {from_md5} != {checker.hexdigest()}")
+                raise StorageError(
+                    f"FILE and CEPH",
+                    f"Invalid MD5 sum control for copy CEPH object {from_path} to {to_path} : {from_md5} != {checker.hexdigest()}",
+                )
 
         except Exception as e:
             raise StorageError(f"CEPH", f"Cannot copy CEPH object {from_path} to {to_path} : {e}")
-            
-    elif from_type == StorageType.CEPH and to_type == StorageType.S3 :
 
+    elif from_type == StorageType.CEPH and to_type == StorageType.S3:
         from_ioctx = __get_ceph_ioctx(from_tray)
 
         s3_client, to_bucket = __get_s3_client(to_tray)
 
         if from_md5 is not None:
             checker = hashlib.md5()
 
         try:
             offset = 0
             size = 0
 
-            with tempfile.NamedTemporaryFile("w+b",delete=False) as f:
+            with tempfile.NamedTemporaryFile("w+b", delete=False) as f:
                 name_tmp = f.name
                 while True:
                     chunk = from_ioctx.read(from_base_name, 65536, offset)
                     size = len(chunk)
                     offset += size
                     f.write(chunk)
 
@@ -759,22 +825,76 @@
                         break
 
             s3_client["client"].upload_file(name_tmp, to_bucket, to_base_name)
 
             os.remove(name_tmp)
 
             if from_md5 is not None and from_md5 != checker.hexdigest():
-                raise StorageError(f"CEPH and S3", f"Invalid MD5 sum control for copy CEPH object {from_path} to S3 object {to_path} : {from_md5} != {checker.hexdigest()}")
+                raise StorageError(
+                    f"CEPH and S3",
+                    f"Invalid MD5 sum control for copy CEPH object {from_path} to S3 object {to_path} : {from_md5} != {checker.hexdigest()}",
+                )
 
         except Exception as e:
-            raise StorageError(f"CEPH and S3", f"Cannot copy CEPH object {from_path} to S3 object {to_path} : {e}")
+            raise StorageError(
+                f"CEPH and S3", f"Cannot copy CEPH object {from_path} to S3 object {to_path} : {e}"
+            )
 
-    else:
-        raise StorageError(f"{from_type.name} and {to_type.name}", f"Cannot copy from {from_type.name} to {to_type.name}")
+    elif (from_type == StorageType.HTTP or from_type == StorageType.HTTPS) and to_type == StorageType.FILE :
+
+        try:
+            response = requests.get(from_type.value + from_path, stream = True)
+            with open(to_path, "wb") as f:
+                for chunk in response.iter_content(chunk_size=65536) :
+                    if chunk:
+                        f.write(chunk)
+
+        except Exception as e:
+            raise StorageError(f"HTTP(S) and FILE", f"Cannot copy HTTP(S) object {from_path} to FILE object {to_path} : {e}")
+
+    elif (from_type == StorageType.HTTP or from_type == StorageType.HTTPS) and to_type == StorageType.CEPH :
+
+        to_ioctx = __get_ceph_ioctx(to_tray)
+
+        try:
+            response = requests.get(from_type.value + from_path, stream = True)
+            offset = 0
+            for chunk in response.iter_content(chunk_size=65536) :
+                if chunk:
+                    size = len(chunk)
+                    to_ioctx.write(to_base_name, chunk, offset)
+                    offset += size
+
+        except Exception as e:
+            raise StorageError(f"HTTP(S) and CEPH", f"Cannot copy HTTP(S) object {from_path} to CEPH object {to_path} : {e}")
+
+    elif (from_type == StorageType.HTTP or from_type == StorageType.HTTPS) and to_type == StorageType.S3 :
+
+        to_s3_client, to_bucket = __get_s3_client(to_tray)
+
+        try:
+            response = requests.get(from_type.value + from_path, stream = True)
+            with tempfile.NamedTemporaryFile("w+b",delete=False) as f:
+                name_fich = f.name
+                for chunk in response.iter_content(chunk_size=65536) :
+                    if chunk:
+                        f.write(chunk)
+
+            to_s3_client["client"].upload_file(name_fich, to_tray, to_base_name)
 
+            os.remove(name_fich)
+
+        except Exception as e:
+            raise StorageError(f"HTTP(S) and S3", f"Cannot copy HTTP(S) object {from_path} to S3 object {to_path} : {e}")
+
+    else:
+        raise StorageError(
+            f"{from_type.name} and {to_type.name}",
+            f"Cannot copy from {from_type.name} to {to_type.name}",
+        )
 
 
 def link(target_path: str, link_path: str, hard: bool = False) -> None:
     """Create a symbolic link
 
     Args:
         target_path (str): file/object to link
@@ -782,63 +902,71 @@
         hard (bool, optional): hard link rather than symbolic. Only for FILE storage. Defaults to False.
 
     Raises:
         StorageError: Unhandled link or link issue
         MissingEnvironmentError: Missing object storage informations
     """
 
-    target_type, target_path, target_tray, target_base_name  = get_infos_from_path(target_path)
-    link_type, link_path, link_tray, link_base_name  = get_infos_from_path(link_path)
+    target_type, target_path, target_tray, target_base_name = get_infos_from_path(target_path)
+    link_type, link_path, link_tray, link_base_name = get_infos_from_path(link_path)
 
     if target_type != link_type:
-        raise StorageError(f"{target_type.name} and {link_type.name}", f"Cannot make link between two different storage types")
+        raise StorageError(
+            f"{target_type.name} and {link_type.name}",
+            f"Cannot make link between two different storage types",
+        )
 
     if hard and target_type != StorageType.FILE:
         raise StorageError(target_type.name, "Hard link is available only for FILE storage")
 
     # Réalisation du lien, selon les types de stockage
     if target_type == StorageType.S3:
-
         target_s3_client, target_bucket = __get_s3_client(target_tray)
         link_s3_client, link_bucket = __get_s3_client(link_tray)
 
         if target_s3_client["host"] != link_s3_client["host"]:
-            raise StorageError(f"S3", f"Cannot make link {link_path} -> {target_path} : link works only on the same S3 cluster")
+            raise StorageError(
+                f"S3",
+                f"Cannot make link {link_path} -> {target_path} : link works only on the same S3 cluster",
+            )
 
         try:
             target_s3_client["client"].put_object(
-                Body = f"{__OBJECT_SYMLINK_SIGNATURE}{target_bucket}/{target_base_name}".encode('utf-8'),
-                Bucket = link_bucket,
-                Key = link_base_name
+                Body=f"{__OBJECT_SYMLINK_SIGNATURE}{target_bucket}/{target_base_name}".encode(
+                    "utf-8"
+                ),
+                Bucket=link_bucket,
+                Key=link_base_name,
             )
         except Exception as e:
             raise StorageError("S3", e)
 
     elif target_type == StorageType.CEPH:
-        
         ioctx = __get_ceph_ioctx(link_tray)
 
         try:
-            ioctx.write_full(link_base_name, f"{__OBJECT_SYMLINK_SIGNATURE}{target_path}".encode('utf-8'))
+            ioctx.write_full(
+                link_base_name, f"{__OBJECT_SYMLINK_SIGNATURE}{target_path}".encode("utf-8")
+            )
         except Exception as e:
             raise StorageError("CEPH", e)
 
     elif target_type == StorageType.FILE:
-
         try:
             if hard:
                 os.link(target_path, link_path)
             else:
                 os.symlink(target_path, link_path)
         except Exception as e:
             raise StorageError("FILE", e)
 
     else:
         raise StorageError("UNKNOWN", "Unhandled storage type to make link")
 
+
 def get_osgeo_path(path: str) -> str:
     """Return GDAL/OGR Open compliant path and configure storage access
 
     For a S3 input path, endpoint, access and secret keys are set and path is built with "/vsis3" root.
 
     For a FILE input path, only storage prefix is removed
 
@@ -846,28 +974,82 @@
         path (str): Source path
 
     Raises:
         NotImplementedError: Storage type not handled
 
     Returns:
         str: GDAL/OGR Open compliant path
-    """    
-
-    storage_type, unprefixed_path, tray_name, base_name  = get_infos_from_path(path)
+    """
 
+    storage_type, unprefixed_path, tray_name, base_name = get_infos_from_path(path)
 
     if storage_type == StorageType.S3:
-
         s3_client, bucket_name = __get_s3_client(tray_name)
 
-        gdal.SetConfigOption('AWS_SECRET_ACCESS_KEY', s3_client["secret_key"])
-        gdal.SetConfigOption('AWS_ACCESS_KEY_ID', s3_client["key"])
-        gdal.SetConfigOption('AWS_S3_ENDPOINT', s3_client["host"])
-        gdal.SetConfigOption('AWS_VIRTUAL_HOSTING', 'FALSE')
+        gdal.SetConfigOption("AWS_SECRET_ACCESS_KEY", s3_client["secret_key"])
+        gdal.SetConfigOption("AWS_ACCESS_KEY_ID", s3_client["key"])
+        gdal.SetConfigOption("AWS_S3_ENDPOINT", s3_client["host"])
+        gdal.SetConfigOption("AWS_VIRTUAL_HOSTING", "FALSE")
 
         return f"/vsis3/{bucket_name}/{base_name}"
 
     elif storage_type == StorageType.FILE:
         return unprefixed_path
 
     else:
         raise NotImplementedError(f"Cannot get a GDAL/OGR compliant path from {path}")
+
+def size_path(path: str) -> int :
+    """Return the size of the path given (or, for the CEPH, the sum of the size of each object of the .list)
+
+    Args:
+        path (str): Source path
+
+    Raises:
+        StorageError: Unhandled link or link issue
+        MissingEnvironmentError: Missing object storage informations
+
+    Returns:
+        int: size of the path
+    """
+    storage_type, unprefixed_path, tray_name, base_name  = get_infos_from_path(path)
+
+    if storage_type == StorageType.FILE:
+        try :
+            total = 0
+            with os.scandir(unprefixed_path) as it:
+                for entry in it:
+                    if entry.is_file():
+                        total += entry.stat().st_size
+                    elif entry.is_dir():
+                        total += size_path(entry.path)
+
+        except Exception as e:
+            raise StorageError("FILE", e)
+
+    elif storage_type == StorageType.S3:
+        s3_client, bucket_name = __get_s3_client(tray_name)
+
+        try :
+            paginator = s3_client["client"].get_paginator('list_objects_v2')
+            pages = paginator.paginate(
+                Bucket=bucket_name,
+                Prefix=base_name+"/",
+                PaginationConfig={
+                    'PageSize': 10000,
+                }
+            )
+            total = 0
+            for page in pages:
+                for key in page['Contents']:
+                    total += key['Size']
+
+        except Exception as e:
+            raise StorageError("S3", e)
+
+
+    elif storage_type == StorageType.CEPH:
+        raise NotImplementedError
+    else:
+        raise StorageError("UNKNOWN", "Unhandled storage type to calculate size")
+
+    return total
```

### Comparing `rok4-1.6.0/src/rok4/TileMatrixSet.py` & `rok4-1.7.0/src/rok4/TileMatrixSet.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,47 +14,61 @@
 from rok4.Utils import *
 
 from typing import Dict, List, Tuple
 from json.decoder import JSONDecodeError
 import json
 import os
 
+
 class TileMatrix:
     """A tile matrix is a tile matrix set's level.
 
     Attributes:
         id (str): TM identifiant (no underscore).
         tms (TileMatrixSet): TMS to whom it belong
         resolution (float): Ground size of a pixel, using unity of the TMS's coordinate system.
         origin (Tuple[float, float]): X,Y coordinates of the upper left corner for the level, the grid's origin.
         tile_size (Tuple[int, int]): Pixel width and height of a tile.
         matrix_size (Tuple[int, int]): Number of tile in the level, widthwise and heightwise.
     """
 
-    def __init__(self, level: Dict, tms: 'TileMatrixSet') -> None:
+    def __init__(self, level: Dict, tms: "TileMatrixSet") -> None:
         """Constructor method
 
         Args:
             level: Level attributes, according to JSON structure
             tms: TMS object containing the level to create
 
         Raises:
             MissingAttributeError: Attribute is missing in the content
         """
 
         self.tms = tms
         try:
             self.id = level["id"]
             if self.id.find("_") != -1:
-                raise Exception(f"TMS {tms.path} owns a level whom id contains an underscore ({self.id})")
+                raise Exception(
+                    f"TMS {tms.path} owns a level whom id contains an underscore ({self.id})"
+                )
             self.resolution = level["cellSize"]
-            self.origin = (level["pointOfOrigin"][0], level["pointOfOrigin"][1],)
-            self.tile_size = (level["tileWidth"], level["tileHeight"],)
-            self.matrix_size = (level["matrixWidth"], level["matrixHeight"],)
-            self.__latlon = (self.tms.sr.EPSGTreatsAsLatLong() or self.tms.sr.EPSGTreatsAsNorthingEasting())
+            self.origin = (
+                level["pointOfOrigin"][0],
+                level["pointOfOrigin"][1],
+            )
+            self.tile_size = (
+                level["tileWidth"],
+                level["tileHeight"],
+            )
+            self.matrix_size = (
+                level["matrixWidth"],
+                level["matrixHeight"],
+            )
+            self.__latlon = (
+                self.tms.sr.EPSGTreatsAsLatLong() or self.tms.sr.EPSGTreatsAsNorthingEasting()
+            )
         except KeyError as e:
             raise MissingAttributeError(tms.path, f"tileMatrices[].{e}")
 
     def x_to_column(self, x: float) -> int:
         """Convert west-east coordinate to tile's column
 
         Args:
@@ -72,15 +86,15 @@
             y (float): north-south coordinate (TMS coordinates system)
 
         Returns:
             int: tile's row
         """
         return int((self.origin[1] - y) / (self.resolution * self.tile_size[1]))
 
-    def tile_to_bbox(self, tile_col: int, tile_row: int) -> Tuple[float, float, float, float]:    
+    def tile_to_bbox(self, tile_col: int, tile_row: int) -> Tuple[float, float, float, float]:
         """Get tile terrain extent (xmin, ymin, xmax, ymax), in TMS coordinates system
 
         TMS spatial reference is Lat / Lon case is handled.
 
         Args:
             tile_col (int): column indice
             tile_row (int): row indice
@@ -89,25 +103,25 @@
             Tuple[float, float, float, float]: terrain extent (xmin, ymin, xmax, ymax)
         """
         if self.__latlon:
             return (
                 self.origin[1] - self.resolution * (tile_row + 1) * self.tile_size[1],
                 self.origin[0] + self.resolution * tile_col * self.tile_size[0],
                 self.origin[1] - self.resolution * tile_row * self.tile_size[1],
-                self.origin[0] + self.resolution * (tile_col + 1) * self.tile_size[0]
+                self.origin[0] + self.resolution * (tile_col + 1) * self.tile_size[0],
             )
         else:
             return (
                 self.origin[0] + self.resolution * tile_col * self.tile_size[0],
                 self.origin[1] - self.resolution * (tile_row + 1) * self.tile_size[1],
                 self.origin[0] + self.resolution * (tile_col + 1) * self.tile_size[0],
-                self.origin[1] - self.resolution * tile_row * self.tile_size[1]
+                self.origin[1] - self.resolution * tile_row * self.tile_size[1],
             )
 
-    def bbox_to_tiles(self, bbox: Tuple[float, float, float, float]) -> Tuple[int, int, int, int]:    
+    def bbox_to_tiles(self, bbox: Tuple[float, float, float, float]) -> Tuple[int, int, int, int]:
         """Get extrems tile columns and rows corresponding to provided bounding box
 
         TMS spatial reference is Lat / Lon case is handled.
 
         Args:
             bbox (Tuple[float, float, float, float]): bounding box (xmin, ymin, xmax, ymax), in TMS coordinates system
 
@@ -116,45 +130,51 @@
         """
 
         if self.__latlon:
             return (
                 self.x_to_column(bbox[1]),
                 self.y_to_row(bbox[2]),
                 self.x_to_column(bbox[3]),
-                self.y_to_row(bbox[0])
+                self.y_to_row(bbox[0]),
             )
         else:
             return (
                 self.x_to_column(bbox[0]),
                 self.y_to_row(bbox[3]),
                 self.x_to_column(bbox[2]),
-                self.y_to_row(bbox[1])
+                self.y_to_row(bbox[1]),
             )
 
     def point_to_indices(self, x: float, y: float) -> Tuple[int, int, int, int]:
         """Get pyramid's tile and pixel indices from point's coordinates
 
         TMS spatial reference with Lat / Lon order is handled.
 
         Args:
             x (float): point's x
             y (float): point's y
 
         Returns:
             Tuple[int, int, int, int]: tile's column, tile's row, pixel's (in the tile) column, pixel's row
-        """        
-        
+        """
+
         if self.__latlon:
             absolute_pixel_column = int((y - self.origin[0]) / self.resolution)
             absolute_pixel_row = int((self.origin[1] - x) / self.resolution)
         else:
             absolute_pixel_column = int((x - self.origin[0]) / self.resolution)
             absolute_pixel_row = int((self.origin[1] - y) / self.resolution)
 
-        return absolute_pixel_column // self.tile_size[0], absolute_pixel_row // self.tile_size[1], absolute_pixel_column % self.tile_size[0], absolute_pixel_row % self.tile_size[1]
+        return (
+            absolute_pixel_column // self.tile_size[0],
+            absolute_pixel_row // self.tile_size[1],
+            absolute_pixel_column % self.tile_size[0],
+            absolute_pixel_row % self.tile_size[1],
+        )
+
 
 class TileMatrixSet:
     """A tile matrix set is multi levels grid definition
 
     Attributes:
         name (str): TMS's name
         path (str): TMS origin path (JSON)
@@ -177,15 +197,15 @@
             FormatError: Provided path is not a well formed JSON
             MissingAttributeError: Attribute is missing in the content
         """
 
         self.name = name
 
         try:
-            self.path = os.path.join(os.environ["ROK4_TMS_DIRECTORY"], f"{self.name}.json");
+            self.path = os.path.join(os.environ["ROK4_TMS_DIRECTORY"], f"{self.name}.json")
         except KeyError as e:
             raise MissingEnvironmentError(e)
 
         try:
             data = json.loads(get_data_str(self.path))
 
             self.id = data["id"]
@@ -196,34 +216,37 @@
                 lev = TileMatrix(l, self)
                 self.levels[lev.id] = lev
 
             if len(self.levels.keys()) == 0:
                 raise Exception(f"TMS '{self.path}' has no level")
 
             if data["orderedAxes"] != ["X", "Y"] and data["orderedAxes"] != ["Lon", "Lat"]:
-                raise Exception(f"TMS '{self.path}' own invalid axes order : only X/Y or Lon/Lat are handled")
+                raise Exception(
+                    f"TMS '{self.path}' own invalid axes order : only X/Y or Lon/Lat are handled"
+                )
 
         except JSONDecodeError as e:
             raise FormatError("JSON", self.path, e)
 
         except KeyError as e:
             raise MissingAttributeError(self.path, e)
 
         except RuntimeError as e:
-            raise Exception(f"Wrong attribute 'crs' ('{self.srs}') in '{self.path}', not recognize by OSR")
+            raise Exception(
+                f"Wrong attribute 'crs' ('{self.srs}') in '{self.path}', not recognize by OSR"
+            )
 
-    def get_level(self, level_id: str) -> 'TileMatrix':
+    def get_level(self, level_id: str) -> "TileMatrix":
         """Get one level according to its identifier
 
         Args:
             level_id: Level identifier
 
         Returns:
             The corresponding tile matrix, None if not present
         """
-      
+
         return self.levels.get(level_id, None)
 
     @property
-    def sorted_levels(self) -> List[TileMatrix]: 
+    def sorted_levels(self) -> List[TileMatrix]:
         return sorted(self.levels.values(), key=lambda l: l.resolution)
-
```

### Comparing `rok4-1.6.0/src/rok4.egg-info/PKG-INFO` & `rok4-1.7.0/src/rok4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rok4
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python core libraries for ROK4 project
 Author-email: Géoportail IGN Developers <tout_rdev@ign.fr>
 License: 
         CeCILL-C FREE SOFTWARE LICENSE AGREEMENT
         
         
             Notice
@@ -123,15 +123,15 @@
         
         
             Article 2 - PURPOSE
         
         The purpose of the Agreement is the grant by the Licensor to the
         Licensee of a non-exclusive, transferable and worldwide license for the
         Software as set forth in Article 5 hereinafter for the whole term of the
-        protection granted by the rights over said Software. 
+        protection granted by the rights over said Software.
         
         
             Article 3 - ACCEPTANCE
         
         3.1 The Licensee shall be deemed as having accepted the terms and
         conditions of this Agreement upon the occurrence of the first of the
         following events:
@@ -269,15 +269,15 @@
         
                 5.3.3 DISTRIBUTION OF DERIVATIVE SOFTWARE
         
         When the Licensee creates Derivative Software, this Derivative Software
         may be distributed under a license agreement other than this Agreement,
         subject to compliance with the requirement to include a notice
         concerning the rights over the Software as defined in Article 6.4.
-        In the event the creation of the Derivative Software required modification 
+        In the event the creation of the Derivative Software required modification
         of the Source Code, the Licensee undertakes that:
         
            1. the resulting Modified Software will be governed by this Agreement,
            2. the Integrated Contributions in the resulting Modified Software
               will be clearly identified and documented,
            3. the Licensee will allow effective access to the source code of the
               Modified Software, at a minimum during the entire period of
@@ -533,16 +533,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE.txt
 
 # ROK4 Python libraries
 
 ![ROK4 Logo](https://rok4.github.io/assets/images/rok4.png)
 
 The `rok4` package help to use [ROK4 project](https://rok4.github.io/) concepts, like Tile Matrix Sets, data pyramids or layers.
@@ -556,17 +557,15 @@
 * [PyPI](https://pypi.org/project/rok4/) : `pip install rok4`
 * [GitHub](https://github.com/rok4/core-python/releases/) : `pip install https://github.com/rok4/core-python/releases/download/<version>/rok4-<version>-py3-none-any.whl`
 
 ## Usage
 
 ```python
 from rok4.TileMatrixSet import TileMatrixSet
-from rok4.Vector import Vector
 
 try:
     tms = TileMatrixSet("file:///path/to/tms.json")
-    vector = Vector("file:///path/to/vector.shp")
-    vector_csv1 = Vector("file:///path/to/vector.csv", delimiter, column_x, column_y)
-    vector_csv1 = Vector("file:///path/to/vector.csv", delimiter, column_WKT)
 except Exception as exc:
     print(exc)
 ```
+
+More examples in the developer documentation
```

### Comparing `rok4-1.6.0/src/rok4.egg-info/SOURCES.txt` & `rok4-1.7.0/src/rok4.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 README.md
 README.pypi.md
 pyproject.toml
 setup.py
 src/rok4/Exceptions.py
 src/rok4/Layer.py
 src/rok4/Pyramid.py
+src/rok4/Raster.py
 src/rok4/Storage.py
 src/rok4/TileMatrixSet.py
 src/rok4/Utils.py
 src/rok4/Vector.py
 src/rok4/__init__.py
 src/rok4.egg-info/PKG-INFO
 src/rok4.egg-info/SOURCES.txt
 src/rok4.egg-info/dependency_links.txt
 src/rok4.egg-info/requires.txt
 src/rok4.egg-info/top_level.txt
 tests/test_Layer.py
 tests/test_Pyramid.py
+tests/test_Raster.py
 tests/test_Storage.py
 tests/test_TileMatrixSet.py
 tests/test_Utils.py
 tests/test_Vector.py
```

### Comparing `rok4-1.6.0/tests/test_Layer.py` & `rok4-1.7.0/tests/test_Layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,56 +4,63 @@
 
 import pytest
 import os
 
 from unittest.mock import *
 from unittest import mock
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Layer.get_data_str', return_value='{"pyramids" : [{"bottom_level" : "10","top_level" : "10","path" : "s3://pyramids/SCAN1000.json"}],"title" : "SCAN1000","bbox":{"east": 11.250000000000997,"west": -5.624999999999043,"north": 52.48278022207774,"south": 40.9798980696195},"styles" : ["normal","hypso"],"abstract" : "Diffusion de la donnée BDORTHO","resampling" : "linear","keywords" : ["PM","TIFF_JPG_UINT8"]}')
-@mock.patch('rok4.Layer.Pyramid.from_descriptor')
-@mock.patch('rok4.Layer.put_data_str', return_value=None)
+@mock.patch(
+    "rok4.Layer.get_data_str",
+    return_value='{"pyramids" : [{"bottom_level" : "10","top_level" : "10","path" : "s3://pyramids/SCAN1000.json"}],"title" : "SCAN1000","bbox":{"east": 11.250000000000997,"west": -5.624999999999043,"north": 52.48278022207774,"south": 40.9798980696195},"styles" : ["normal","hypso"],"abstract" : "Diffusion de la donnée BDORTHO","resampling" : "linear","keywords" : ["PM","TIFF_JPG_UINT8"]}',
+)
+@mock.patch("rok4.Layer.Pyramid.from_descriptor")
+@mock.patch("rok4.Layer.put_data_str", return_value=None)
 def test_descriptor_ok(mocked_put_data_str, mocked_pyramid_class, mocked_get_data_str):
-
     tms_instance = MagicMock()
     tms_instance.srs = "EPSG:3857"
 
     level_instance = MagicMock()
     level_instance.id = 10
     level_instance.resolution = 1
 
     pyramid_instance = MagicMock()
     pyramid_instance.raster_specifications = {
         "channels": 3,
         "nodata": "255,255,255",
         "photometric": "rgb",
-        "interpolation": "bicubic"
+        "interpolation": "bicubic",
     }
     pyramid_instance.format = "TIFF_JPG_UINT8"
     pyramid_instance.tms = tms_instance
     pyramid_instance.descriptor = "s3://pyramids/SCAN1000.json"
     pyramid_instance.get_levels.return_value = [level_instance]
     mocked_pyramid_class.return_value = pyramid_instance
 
     try:
         layer = Layer.from_descriptor("s3://layers/SCAN1000.json")
         assert layer.type == PyramidType.RASTER
-        mocked_get_data_str.assert_called_once_with('s3://layers/SCAN1000.json')
+        mocked_get_data_str.assert_called_once_with("s3://layers/SCAN1000.json")
 
         layer.write_descriptor("s3://layers_backup/")
-        mocked_put_data_str.assert_called_once_with('{"title": "SCAN1000", "abstract": "Diffusion de la donn\\u00e9e BDORTHO", "keywords": ["PM", "TIFF_JPG_UINT8"], "wmts": {"authorized": true}, "tms": {"authorized": true}, "bbox": {"south": 40.9798980696195, "west": -5.624999999999043, "north": 52.48278022207774, "east": 11.250000000000997}, "pyramids": [{"bottom_level": "10", "top_level": "10", "path": "s3://pyramids/SCAN1000.json"}], "wms": {"authorized": true, "crs": ["CRS:84", "IGNF:WGS84G", "EPSG:3857", "EPSG:4258", "EPSG:4326"]}, "styles": ["normal", "hypso"], "resampling": "linear"}', 's3://layers_backup/SCAN1000.json')
+        mocked_put_data_str.assert_called_once_with(
+            '{"title": "SCAN1000", "abstract": "Diffusion de la donn\\u00e9e BDORTHO", "keywords": ["PM", "TIFF_JPG_UINT8"], "wmts": {"authorized": true}, "tms": {"authorized": true}, "bbox": {"south": 40.9798980696195, "west": -5.624999999999043, "north": 52.48278022207774, "east": 11.250000000000997}, "pyramids": [{"bottom_level": "10", "top_level": "10", "path": "s3://pyramids/SCAN1000.json"}], "wms": {"authorized": true, "crs": ["CRS:84", "IGNF:WGS84G", "EPSG:3857", "EPSG:4258", "EPSG:4326"]}, "styles": ["normal", "hypso"], "resampling": "linear"}',
+            "s3://layers_backup/SCAN1000.json",
+        )
     except Exception as exc:
         assert False, f"Layer creation from descriptor raises an exception: {exc}"
 
 
-@mock.patch('rok4.Layer.Pyramid.from_descriptor')
-@mock.patch('rok4.Layer.reproject_bbox', return_value=(0, 0, 100, 100))
-@mock.patch('rok4.Layer.put_data_str', return_value=None)
-def test_parameters_vector_ok(mocked_put_data_str, mocked_utils_reproject_bbox, mocked_pyramid_class):
-
+@mock.patch("rok4.Layer.Pyramid.from_descriptor")
+@mock.patch("rok4.Layer.reproject_bbox", return_value=(0, 0, 100, 100))
+@mock.patch("rok4.Layer.put_data_str", return_value=None)
+def test_parameters_vector_ok(
+    mocked_put_data_str, mocked_utils_reproject_bbox, mocked_pyramid_class
+):
     tms_instance = MagicMock()
     tms_instance.srs = "EPSG:3857"
 
     level_instance = MagicMock()
     level_instance.id = 10
     level_instance.resolution = 1
     level_instance.bbox = (0, 0, 100000, 100000)
@@ -63,70 +70,76 @@
     pyramid_instance.tms = tms_instance
     pyramid_instance.descriptor = "file:///home/ign/pyramids/SCAN1000.json"
     pyramid_instance.get_levels.return_value = [level_instance]
     mocked_pyramid_class.return_value = pyramid_instance
 
     try:
         layer = Layer.from_parameters(
-            [{
-                "path": "file:///home/ign/pyramids/SCAN1000.json",
-                "bottom_level": "10",
-                "top_level": "10"
-            }],
+            [
+                {
+                    "path": "file:///home/ign/pyramids/SCAN1000.json",
+                    "bottom_level": "10",
+                    "top_level": "10",
+                }
+            ],
             "layername",
-            title = "title",
-            abstract = "abstract"
+            title="title",
+            abstract="abstract",
         )
         assert layer.type == PyramidType.VECTOR
         assert layer.geobbox == (0, 0, 100, 100)
         layer.write_descriptor("file:///home/ign/layers/")
-        mocked_put_data_str.assert_called_once_with('{"title": "title", "abstract": "abstract", "keywords": ["VECTOR", "layername"], "wmts": {"authorized": true}, "tms": {"authorized": true}, "bbox": {"south": 0, "west": 0, "north": 100, "east": 100}, "pyramids": [{"bottom_level": "10", "top_level": "10", "path": "file:///home/ign/pyramids/SCAN1000.json"}]}', 'file:///home/ign/layers/layername.json')
+        mocked_put_data_str.assert_called_once_with(
+            '{"title": "title", "abstract": "abstract", "keywords": ["VECTOR", "layername"], "wmts": {"authorized": true}, "tms": {"authorized": true}, "bbox": {"south": 0, "west": 0, "north": 100, "east": 100}, "pyramids": [{"bottom_level": "10", "top_level": "10", "path": "file:///home/ign/pyramids/SCAN1000.json"}]}',
+            "file:///home/ign/layers/layername.json",
+        )
 
     except Exception as exc:
         assert False, f"Layer creation from parameters raises an exception: {exc}"
 
 
-@mock.patch('rok4.Layer.Pyramid.from_descriptor')
-@mock.patch('rok4.Layer.reproject_bbox', return_value=(0, 0, 100, 100))
-@mock.patch('rok4.Layer.put_data_str', return_value=None)
-def test_parameters_raster_ok(mocked_put_data_str, mocked_utils_reproject_bbox, mocked_pyramid_class):
-
+@mock.patch("rok4.Layer.Pyramid.from_descriptor")
+@mock.patch("rok4.Layer.reproject_bbox", return_value=(0, 0, 100, 100))
+@mock.patch("rok4.Layer.put_data_str", return_value=None)
+def test_parameters_raster_ok(
+    mocked_put_data_str, mocked_utils_reproject_bbox, mocked_pyramid_class
+):
     tms_instance = MagicMock()
     tms_instance.srs = "EPSG:3857"
 
     level_instance = MagicMock()
     level_instance.id = 10
     level_instance.resolution = 1
     level_instance.bbox = (0, 0, 100000, 100000)
 
     pyramid_instance = MagicMock()
     pyramid_instance.format = "TIFF_ZIP_FLOAT32"
     pyramid_instance.raster_specifications = {
         "channels": 1,
         "nodata": "-99999",
         "photometric": "gray",
-        "interpolation": "nn"
+        "interpolation": "nn",
     }
     pyramid_instance.tms = tms_instance
     pyramid_instance.bottom_level.id = "10"
     pyramid_instance.top_level.id = "10"
     pyramid_instance.descriptor = "file:///home/ign/pyramids/RGEALTI.json"
     pyramid_instance.get_levels.return_value = [level_instance]
     mocked_pyramid_class.return_value = pyramid_instance
 
     try:
         layer = Layer.from_parameters(
-            [{
-                "path": "file:///home/ign/pyramids/RGEALTI.json"
-            }],
+            [{"path": "file:///home/ign/pyramids/RGEALTI.json"}],
             "layername",
-            title = "title",
-            abstract = "abstract"
+            title="title",
+            abstract="abstract",
         )
         assert layer.type == PyramidType.RASTER
         assert layer.geobbox == (0, 0, 100, 100)
         layer.write_descriptor("file:///home/ign/layers/")
-        mocked_put_data_str.assert_called_once_with('{"title": "title", "abstract": "abstract", "keywords": ["RASTER", "layername"], "wmts": {"authorized": true}, "tms": {"authorized": true}, "bbox": {"south": 0, "west": 0, "north": 100, "east": 100}, "pyramids": [{"bottom_level": "10", "top_level": "10", "path": "file:///home/ign/pyramids/RGEALTI.json"}], "wms": {"authorized": true, "crs": ["CRS:84", "IGNF:WGS84G", "EPSG:3857", "EPSG:4258", "EPSG:4326"]}, "styles": ["normal"], "resampling": "nn"}', 'file:///home/ign/layers/layername.json')
-                                                     
+        mocked_put_data_str.assert_called_once_with(
+            '{"title": "title", "abstract": "abstract", "keywords": ["RASTER", "layername"], "wmts": {"authorized": true}, "tms": {"authorized": true}, "bbox": {"south": 0, "west": 0, "north": 100, "east": 100}, "pyramids": [{"bottom_level": "10", "top_level": "10", "path": "file:///home/ign/pyramids/RGEALTI.json"}], "wms": {"authorized": true, "crs": ["CRS:84", "IGNF:WGS84G", "EPSG:3857", "EPSG:4258", "EPSG:4326"]}, "styles": ["normal"], "resampling": "nn"}',
+            "file:///home/ign/layers/layername.json",
+        )
 
     except Exception as exc:
-        assert False, f"Layer creation from parameters raises an exception: {exc}"
+        assert False, f"Layer creation from parameters raises an exception: {exc}"
```

### Comparing `rok4-1.6.0/tests/test_Pyramid.py` & `rok4-1.7.0/tests/test_Pyramid.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,199 +5,234 @@
 from rok4.Exceptions import *
 
 import pytest
 import os
 from unittest.mock import *
 from unittest import mock
 
-@mock.patch('rok4.Pyramid.get_data_str', side_effect=StorageError('FILE', 'Not found'))
+
+@mock.patch("rok4.Pyramid.get_data_str", side_effect=StorageError("FILE", "Not found"))
 def test_wrong_file(mocked_get_data_str):
     with pytest.raises(StorageError):
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
 
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"format": "TIFF_PBF_MVT","levels":[{"id": "100","tables":')
+
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"format": "TIFF_PBF_MVT","levels":[{"id": "100","tables":',
+)
 def test_bad_json(mocked_get_data_str):
     with pytest.raises(FormatError) as exc:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
 
-    assert str(exc.value) == "Expected format JSON to read 'file:///pyramid.json' : Expecting value: line 1 column 59 (char 58)"
-    mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
+    assert (
+        str(exc.value)
+        == "Expected format JSON to read 'file:///pyramid.json' : Expecting value: line 1 column 59 (char 58)"
+    )
+    mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
+
 
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"format": "TIFF_PBF_MVT","levels":[]}')
+@mock.patch("rok4.Pyramid.get_data_str", return_value='{"format": "TIFF_PBF_MVT","levels":[]}')
 def test_missing_tms(mocked_get_data_str):
     with pytest.raises(MissingAttributeError) as exc:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
 
     assert str(exc.value) == "Missing attribute 'tile_matrix_set' in 'file:///pyramid.json'"
-    mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
+    mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"format": "TIFF_PBF_MVT","levels":[{}], "tile_matrix_set": "PM"}')
-@mock.patch('rok4.Pyramid.TileMatrixSet', side_effect=StorageError('FILE', 'TMS not found'))
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"format": "TIFF_PBF_MVT","levels":[{}], "tile_matrix_set": "PM"}',
+)
+@mock.patch("rok4.Pyramid.TileMatrixSet", side_effect=StorageError("FILE", "TMS not found"))
 def test_wrong_tms(mocked_tms_constructor, mocked_get_data_str):
     with pytest.raises(StorageError) as exc:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
 
     assert str(exc.value) == "Issue occured using a FILE storage : TMS not found"
-    mocked_tms_constructor.assert_called_once_with('PM')
-    mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
+    mocked_tms_constructor.assert_called_once_with("PM")
+    mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
+
 
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"format": "TIFF_JPG_UINT8","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"0"}], "tile_matrix_set": "PM"}')
-@mock.patch('rok4.Pyramid.TileMatrixSet')
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"format": "TIFF_JPG_UINT8","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"0"}], "tile_matrix_set": "PM"}',
+)
+@mock.patch("rok4.Pyramid.TileMatrixSet")
 def test_raster_missing_raster_specifications(mocked_tms_class, mocked_get_data_str):
-
     with pytest.raises(MissingAttributeError) as exc:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
 
     assert str(exc.value) == "Missing attribute 'raster_specifications' in 'file:///pyramid.json'"
-    mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
+    mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"raster_specifications":{"channels":3,"nodata":"255,0,0","photometric":"rgb","interpolation":"bicubic"}, "format": "TIFF_JPG_UINT8","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"unknown"}], "tile_matrix_set": "PM"}')
-@mock.patch('rok4.Pyramid.TileMatrixSet')
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"raster_specifications":{"channels":3,"nodata":"255,0,0","photometric":"rgb","interpolation":"bicubic"}, "format": "TIFF_JPG_UINT8","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"unknown"}], "tile_matrix_set": "PM"}',
+)
+@mock.patch("rok4.Pyramid.TileMatrixSet")
 def test_wrong_level(mocked_tms_class, mocked_get_data_str):
-    
     tms_instance = MagicMock()
     tms_instance.get_level.return_value = None
     tms_instance.name = "PM"
     mocked_tms_class.return_value = tms_instance
 
     with pytest.raises(Exception) as exc:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
-    
-    mocked_tms_class.assert_called_once_with('PM')
-    mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
-    tms_instance.get_level.assert_called_once_with('unknown')
-    assert str(exc.value) == "Pyramid file:///pyramid.json owns a level with the ID 'unknown', not defined in the TMS 'PM'"
+
+    mocked_tms_class.assert_called_once_with("PM")
+    mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
+    tms_instance.get_level.assert_called_once_with("unknown")
+    assert (
+        str(exc.value)
+        == "Pyramid file:///pyramid.json owns a level with the ID 'unknown', not defined in the TMS 'PM'"
+    )
+
 
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"format": "TIFF_PBF_MVT","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"0"}], "tile_matrix_set": "PM"}')
-@mock.patch('rok4.Pyramid.TileMatrixSet', autospec=True)
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"format": "TIFF_PBF_MVT","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"0"}], "tile_matrix_set": "PM"}',
+)
+@mock.patch("rok4.Pyramid.TileMatrixSet", autospec=True)
 def test_vector_missing_tables(mocked_tms_class, mocked_get_data_str):
-
     with pytest.raises(MissingAttributeError) as exc:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
 
     assert str(exc.value) == "Missing attribute levels[].'tables' in 'file:///pyramid.json'"
-    mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
+    mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
+
 
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"raster_specifications":{"channels":3,"nodata":"255,0,0","photometric":"rgb","interpolation":"bicubic"}, "format": "TIFF_JPG_UINT8","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_prefix":"SCAN1000/DATA_0","pool_name":"pool1","type":"CEPH"},"tiles_per_width":16,"id":"0"}], "tile_matrix_set": "PM"}')
-@mock.patch('rok4.Pyramid.TileMatrixSet')
-@mock.patch('rok4.Pyramid.put_data_str', return_value=None)
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"raster_specifications":{"channels":3,"nodata":"255,0,0","photometric":"rgb","interpolation":"bicubic"}, "format": "TIFF_JPG_UINT8","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_prefix":"SCAN1000/DATA_0","pool_name":"pool1","type":"CEPH"},"tiles_per_width":16,"id":"0"}], "tile_matrix_set": "PM"}',
+)
+@mock.patch("rok4.Pyramid.TileMatrixSet")
+@mock.patch("rok4.Pyramid.put_data_str", return_value=None)
 def test_raster_ok(mocked_put_data_str, mocked_tms_class, mocked_get_data_str):
-
     tms_instance = MagicMock()
     tms_instance.name = "PM"
     tms_instance.srs = "EPSG:3857"
     tms_instance.sr = sr_src = srs_to_spatialreference("EPSG:3857")
 
     tm_instance = MagicMock()
     tm_instance.id = "0"
     tm_instance.resolution = 1
-    tm_instance.point_to_indices.return_value = (0,0,128,157)
+    tm_instance.point_to_indices.return_value = (0, 0, 128, 157)
 
     tms_instance.get_level.return_value = tm_instance
 
     mocked_tms_class.return_value = tms_instance
 
     try:
         pyramid = Pyramid.from_descriptor("ceph://pool1/sub/pyramid.json")
         assert pyramid.get_level("0") is not None
         assert pyramid.get_level("4") is None
         assert pyramid.name == "sub/pyramid"
         assert pyramid.storage_type == StorageType.CEPH
         assert pyramid.storage_root == "pool1"
-        mocked_get_data_str.assert_called_once_with('ceph://pool1/sub/pyramid.json')
+        mocked_get_data_str.assert_called_once_with("ceph://pool1/sub/pyramid.json")
 
         clone = Pyramid.from_other(pyramid, "titi", {"type": "FILE", "root": "/data/ign"})
         assert clone.name == "titi"
         assert clone.storage_type == StorageType.FILE
         assert clone.storage_root == "/data/ign"
+        assert clone.tile_extension == "jpg"
         assert clone.get_level("0") is not None
         assert clone.get_level("4") is None
-        assert clone.get_infos_from_slab_path("IMAGE/12/00/00/00.tif") == (SlabType.DATA, "12", 0, 0)
-        assert clone.get_tile_indices(102458, 6548125, srs = "EPSG:3857") == ("0",0,0,128,157)
-        assert clone.get_tile_indices(43, 2, srs = "EPSG:4326") == ("0",0,0,128,157)
-
+        assert clone.get_infos_from_slab_path("/data/ign/titi/IMAGE/12/00/4A/F7.tif") == (
+            SlabType.DATA,
+            "12",
+            159,
+            367,
+        )
+        assert clone.get_tile_indices(102458, 6548125, srs="EPSG:3857") == ("0", 0, 0, 128, 157)
+        assert clone.get_tile_indices(43, 2, srs="EPSG:4326") == ("0", 0, 0, 128, 157)
 
         assert len(clone.get_levels()) == 1
 
         clone.write_descriptor()
-        mocked_put_data_str.assert_called_once_with('{"tile_matrix_set": "PM", "format": "TIFF_JPG_UINT8", "levels": [{"id": "0", "tiles_per_width": 16, "tiles_per_height": 16, "tile_limits": {"min_col": 0, "max_row": 15, "max_col": 15, "min_row": 0}, "storage": {"type": "FILE", "image_directory": "titi/DATA/0", "path_depth": 2}}], "raster_specifications": {"channels": 3, "nodata": "255,0,0", "photometric": "rgb", "interpolation": "bicubic"}}', 'file:///data/ign/titi.json')
+        mocked_put_data_str.assert_called_once_with(
+            '{"tile_matrix_set": "PM", "format": "TIFF_JPG_UINT8", "levels": [{"id": "0", "tiles_per_width": 16, "tiles_per_height": 16, "tile_limits": {"min_col": 0, "max_row": 15, "max_col": 15, "min_row": 0}, "storage": {"type": "FILE", "image_directory": "titi/DATA/0", "path_depth": 2}}], "raster_specifications": {"channels": 3, "nodata": "255,0,0", "photometric": "rgb", "interpolation": "bicubic"}}',
+            "file:///data/ign/titi.json",
+        )
     except Exception as exc:
         assert False, f"Pyramid creation raises an exception: {exc}"
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.get_data_str', return_value='{"format": "TIFF_PBF_MVT","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"0","tables":[{"name":"table","geometry":"POINT","attributes":[{"type":"bigint","name":"fid","count":1531}]}]}], "tile_matrix_set": "PM"}')
-@mock.patch('rok4.Pyramid.TileMatrixSet')
+@mock.patch(
+    "rok4.Pyramid.get_data_str",
+    return_value='{"format": "TIFF_PBF_MVT","levels":[{"tiles_per_height":16,"tile_limits":{"min_col":0,"max_row":15,"max_col":15,"min_row":0},"storage":{"image_directory":"SCAN1000/DATA/0","path_depth":2,"type":"FILE"},"tiles_per_width":16,"id":"0","tables":[{"name":"table","geometry":"POINT","attributes":[{"type":"bigint","name":"fid","count":1531}]}]}], "tile_matrix_set": "PM"}',
+)
+@mock.patch("rok4.Pyramid.TileMatrixSet")
 def test_vector_ok(mocked_tms_class, mocked_get_data_str):
-
     try:
         pyramid = Pyramid.from_descriptor("file:///pyramid.json")
         assert pyramid.get_level("0") is not None
         assert pyramid.get_level("4") is None
         assert pyramid.name == "pyramid"
         assert pyramid.storage_depth == 2
         assert pyramid.storage_type == StorageType.FILE
-        mocked_get_data_str.assert_called_once_with('file:///pyramid.json')
+        mocked_get_data_str.assert_called_once_with("file:///pyramid.json")
 
         clone = Pyramid.from_other(pyramid, "toto", {"type": "S3", "root": "bucket"})
         assert clone.name == "toto"
+        assert clone.tile_extension == "pbf"
         assert clone.storage_type == StorageType.S3
         assert clone.get_level("0") is not None
         assert clone.get_level("4") is None
     except Exception as exc:
         assert False, f"Pyramid creation raises an exception: {exc}"
 
     with pytest.raises(Exception) as exc:
         pyramid.get_tile_data_raster("12", 5, 6)
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.TileMatrixSet')
+@mock.patch("rok4.Pyramid.TileMatrixSet")
 def test_tile_read_raster(mocked_tms_class):
-
     tms_instance = MagicMock()
     tms_instance.name = "UTM20W84MART_1M_MNT"
     tms_instance.srs = "IGNF:UTM20W84MART"
-    
+
     tm_instance = MagicMock()
     tm_instance.id = "8"
-    tm_instance.tile_size = (256,256)
+    tm_instance.tile_size = (256, 256)
 
     tms_instance.get_level.return_value = tm_instance
 
     mocked_tms_class.return_value = tms_instance
 
     try:
         pyramid = Pyramid.from_descriptor("file://tests/fixtures/TIFF_ZIP_FLOAT32.json")
-        data = pyramid.get_tile_data_raster("8",2748,40537)
+        data = pyramid.get_tile_data_raster("8", 2748, 40537)
 
-        assert data.shape == (256,256,1)
+        assert data.shape == (256, 256, 1)
         assert data[128][128][0] == 447.25
     except Exception as exc:
         assert False, f"Pyramid raster tile read raises an exception: {exc}"
 
 
-
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('rok4.Pyramid.TileMatrixSet')
+@mock.patch("rok4.Pyramid.TileMatrixSet")
 def test_tile_read_vector(mocked_tms_class):
-
     tms_instance = MagicMock()
     tms_instance.name = "PM"
     tms_instance.srs = "EPSG:3857"
-    
+
     tm_instance = MagicMock()
     tm_instance.id = "4"
-    tm_instance.tile_size = (256,256)
+    tm_instance.tile_size = (256, 256)
 
     tms_instance.get_level.return_value = tm_instance
 
     mocked_tms_class.return_value = tms_instance
 
     try:
         pyramid = Pyramid.from_descriptor("file://tests/fixtures/TIFF_PBF_MVT.json")
@@ -207,15 +242,61 @@
 
         data = pyramid.get_tile_data_vector("4", 8, 5)
         assert type(data) is dict
         assert "ecoregions_3857" in data
     except Exception as exc:
         assert False, f"Pyramid vector tile read raises an exception: {exc}"
 
+
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("rok4.Pyramid.TileMatrixSet")
+def test_list_read(mocked_tms_class):
+    tms_instance = MagicMock()
+    tms_instance.name = "PM"
+    tms_instance.srs = "EPSG:3857"
+
+    tm_instance = MagicMock()
+    tm_instance.id = "4"
+    tm_instance.tile_size = (256, 256)
+
+    tms_instance.get_level.return_value = tm_instance
+
+    mocked_tms_class.return_value = tms_instance
+
+    try:
+        pyramid = Pyramid.from_descriptor("file://tests/fixtures/TIFF_PBF_MVT.json")
+        pyramid.load_list()
+        pyramid.load_list()  # on passe par la détection d'une liste déjà chrargée ainsi
+        for (slab_type, level, column, row), infos in pyramid.list_generator():
+            assert slab_type == SlabType.DATA
+            assert level == "4"
+            assert column == 2
+            assert row == 1
+            assert infos == {
+                "link": False,
+                "md5": None,
+                "root": "TIFF_PBF_MVT",
+                "slab": "DATA/4/00/00/21.tif",
+            }
+
+    except Exception as exc:
+        assert False, f"Pyramid vector list read raises an exception: {exc}"
+
+
 def test_b36_path_decode():
-    assert b36_path_decode("3E/42/01.tif") == (4032, 18217,)
-    assert b36_path_decode("3E/42/01.TIFF") == (4032, 18217,)
-    assert b36_path_decode("3E/42/01") == (4032, 18217,)
+    assert b36_path_decode("3E/42/01.tif") == (
+        4032,
+        18217,
+    )
+    assert b36_path_decode("3E/42/01.TIFF") == (
+        4032,
+        18217,
+    )
+    assert b36_path_decode("3E/42/01") == (
+        4032,
+        18217,
+    )
+
 
 def test_b36_path_encode():
     assert b36_path_encode(4032, 18217, 2) == "3E/42/01.tif"
-    assert b36_path_encode(14, 18217, 1) == "0E02/E1.tif"
+    assert b36_path_encode(14, 18217, 1) == "0E02/E1.tif"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rok4-1.6.0/tests/test_Storage.py` & `rok4-1.7.0/tests/test_Storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,512 +6,728 @@
 
 import botocore.exceptions
 from rados import ObjectNotFound
 
 from unittest import mock
 from unittest.mock import *
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
 @patch("builtins.open", new_callable=mock_open, read_data=b"data")
 def test_hash_file_ok(mock_file):
     try:
         md5 = hash_file("/path/to/file.ext")
-        mock_file.assert_called_with("/path/to/file.ext", 'rb')
+        mock_file.assert_called_with("/path/to/file.ext", "rb")
         assert md5 == "8d777f385d3dfec8815d20f7496026dc"
     except Exception as exc:
         assert False, f"FILE md5 sum raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {}, clear=True)  
+@mock.patch.dict(os.environ, {}, clear=True)
 def test_get_infos_from_path():
     assert (StorageType.S3, "toto/titi", "toto", "titi") == get_infos_from_path("s3://toto/titi")
-    assert (StorageType.FILE, "/toto/titi/tutu.json", "/toto/titi", "tutu.json") == get_infos_from_path("file:///toto/titi/tutu.json")
-    assert (StorageType.CEPH, "toto/titi/tutu", "toto", "titi/tutu") == get_infos_from_path("ceph://toto/titi/tutu")
-    assert (StorageType.FILE, "wrong://toto/titi", "wrong://toto", "titi") == get_infos_from_path("wrong://toto/titi")
+    assert (
+        StorageType.FILE,
+        "/toto/titi/tutu.json",
+        "/toto/titi",
+        "tutu.json",
+    ) == get_infos_from_path("file:///toto/titi/tutu.json")
+    assert (StorageType.CEPH, "toto/titi/tutu", "toto", "titi/tutu") == get_infos_from_path(
+        "ceph://toto/titi/tutu"
+    )
+    assert (StorageType.FILE, "wrong://toto/titi", "wrong://toto", "titi") == get_infos_from_path(
+        "wrong://toto/titi"
+    )
 
 
-@mock.patch.dict(os.environ, {}, clear=True)  
+@mock.patch.dict(os.environ, {}, clear=True)
 def test_get_path_from_infos():
     assert get_path_from_infos(StorageType.S3, "toto", "toto/titi") == "s3://toto/toto/titi"
-    assert get_path_from_infos(StorageType.FILE, "/toto/titi", "tutu.json") == "file:///toto/titi/tutu.json"
+    assert (
+        get_path_from_infos(StorageType.FILE, "/toto/titi", "tutu.json")
+        == "file:///toto/titi/tutu.json"
+    )
     assert get_path_from_infos(StorageType.CEPH, "toto", "titi/tutu") == "ceph://toto/titi/tutu"
 
+
 ############ get_data_str
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_s3_missing_env():
     with pytest.raises(MissingEnvironmentError):
         data = get_data_str("s3://bucket/path/to/object")
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_ceph_missing_env():
     with pytest.raises(MissingEnvironmentError):
         data = get_data_str("ceph://bucket/path/to/object")
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "a,b", "ROK4_S3_SECRETKEY": "b,c", "ROK4_S3_KEY": "c,d,e"}, clear=True)
+
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "a,b", "ROK4_S3_SECRETKEY": "b,c", "ROK4_S3_KEY": "c,d,e"},
+    clear=True,
+)
 def test_s3_invalid_envs():
     with pytest.raises(StorageError):
         data = get_data_str("s3://bucket/path/to/object")
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "a", "ROK4_S3_SECRETKEY": "b", "ROK4_S3_KEY": "c"}, clear=True)
-@mock.patch('rok4.Storage.boto3.client')
+
+@mock.patch.dict(
+    os.environ, {"ROK4_S3_URL": "a", "ROK4_S3_SECRETKEY": "b", "ROK4_S3_KEY": "c"}, clear=True
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_s3_invalid_endpoint(mocked_s3_client):
     s3_instance = MagicMock()
-    mocked_s3_client.side_effect = Exception('Invalid URL')
+    mocked_s3_client.side_effect = Exception("Invalid URL")
     with pytest.raises(StorageError):
         data = get_data_str("s3://bucket/path/to/object")
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
 @mock.patch("builtins.open", side_effect=FileNotFoundError("not_found"))
 def test_file_read_error(mock_file):
     with pytest.raises(FileNotFoundError):
         data = get_data_str("file:///path/to/file.ext")
-    
+
     mock_file.assert_called_with("/path/to/file.ext", "rb")
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
 @patch("builtins.open", new_callable=mock_open, read_data=b"data")
 def test_file_read_ok(mock_file):
     try:
         data = get_data_str("file:///path/to/file.ext")
         mock_file.assert_called_with("/path/to/file.ext", "rb")
         assert data == "data"
     except Exception as exc:
         assert False, f"FILE read raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_s3_read_nok(mocked_s3_client):
     disconnect_s3_clients()
     s3_instance = MagicMock()
-    s3_instance.get_object.side_effect = Exception('Bucket or object not found')
+    s3_instance.get_object.side_effect = Exception("Bucket or object not found")
     mocked_s3_client.return_value = s3_instance
     with pytest.raises(StorageError):
         data = get_data_str("s3://bucket/path/to/object")
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_s3_read_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_body = MagicMock()
     s3_body.read.return_value = b"data"
-    s3_instance.get_object.return_value = {
-        "Body": s3_body
-    }
+    s3_instance.get_object.return_value = {"Body": s3_body}
     mocked_s3_client.return_value = s3_instance
 
     try:
         data = get_data_str("s3://bucket/path/to/object")
         assert data == "data"
     except Exception as exc:
         assert False, f"S3 read raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 def test_ceph_read_ok(mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.stat.return_value = (4, "date")
     ioctx_instance.read.return_value = b"data"
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
         data = get_data_str("ceph://pool/path/to/object")
         assert data == "data"
     except Exception as exc:
         assert False, f"CEPH read raises an exception: {exc}"
 
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("requests.get", side_effect={"status_code":404})
+def test_http_read_error(mock_http):
+    with pytest.raises(StorageError):
+        requests_instance = MagicMock()
+        requests_instance.content = "NULL"
+        requests_instance.status_code = 404
+        mock_http.return_value = requests_instance
+        data = get_data_str("http://path/to/file.ext")
+
+    mock_http.assert_called_with("http://path/to/file.ext", stream=True)
+
+@mock.patch.dict(os.environ, {}, clear=True)
+def test_http_read_range_error():
+    with pytest.raises(NotImplementedError):
+        data = get_data_binary("http://path/to/file.ext", (0,100))
+
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("requests.get")
+def test_http_read_ok(mock_http):
+    try :
+        requests_instance = MagicMock()
+        requests_instance.content = b'data'
+        mock_http.return_value = requests_instance
+
+        data = get_data_str("http://path/to/file.ext")
+        mock_http.assert_called_with("http://path/to/file.ext", stream=True)
+        assert data == 'data'
+    except Exception as exc:
+        assert False, f"HTTP read raises an exception: {exc}"
+
 
 ############ put_data_str
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_s3_write_nok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
-    s3_instance.put_object.side_effect = Exception('Cannot write S3 object')
+    s3_instance.put_object.side_effect = Exception("Cannot write S3 object")
     mocked_s3_client.return_value = s3_instance
 
     with pytest.raises(StorageError):
         put_data_str("data", "s3://bucket/path/to/object")
 
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_s3_write_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.put_object.return_value = None
     mocked_s3_client.return_value = s3_instance
     try:
         put_data_str("data", "s3://bucket/path/to/object")
     except Exception as exc:
         assert False, f"S3 write raises an exception: {exc}"
 
-
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 def test_ceph_write_ok(mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.write_full.return_value = None
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
         put_data_str("data", "ceph://pool/path/to/object")
     except Exception as exc:
         assert False, f"CEPH write raises an exception: {exc}"
 
+
 ############ copy
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
-@mock.patch('os.makedirs', return_value=None)
-@mock.patch('rok4.Storage.copyfile', return_value=None)
-@mock.patch('rok4.Storage.hash_file', return_value="toto")
+@mock.patch("os.makedirs", return_value=None)
+@mock.patch("rok4.Storage.copyfile", return_value=None)
+@mock.patch("rok4.Storage.hash_file", return_value="toto")
 def test_copy_file_file_ok(mock_hash_file, mock_copyfile, mock_makedirs):
     try:
         copy("file:///path/to/source.ext", "file:///path/to/destination.ext", "toto")
         mock_copyfile.assert_called_once_with("/path/to/source.ext", "/path/to/destination.ext")
         mock_hash_file.assert_called_once_with("/path/to/destination.ext")
         mock_makedirs.assert_called_once_with("/path/to", exist_ok=True)
     except Exception as exc:
         assert False, f"FILE -> FILE copy raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
-@mock.patch('os.makedirs', return_value=None)
-@mock.patch('rok4.Storage.hash_file', return_value="toto")
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
+@mock.patch("os.makedirs", return_value=None)
+@mock.patch("rok4.Storage.hash_file", return_value="toto")
 def test_copy_s3_file_ok(mock_hash_file, mock_makedirs, mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.download_file.return_value = None
     mocked_s3_client.return_value = s3_instance
 
     try:
-
         copy("s3://bucket/source.ext", "file:///path/to/destination.ext", "toto")
         mock_hash_file.assert_called_once_with("/path/to/destination.ext")
         mock_makedirs.assert_called_once_with("/path/to", exist_ok=True)
     except Exception as exc:
         assert False, f"S3 -> FILE copy raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
-@mock.patch('os.makedirs', return_value=None)
-@mock.patch('rok4.Storage.hash_file', return_value="toto")
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
+@mock.patch("os.makedirs", return_value=None)
+@mock.patch("rok4.Storage.hash_file", return_value="toto")
 def test_copy_s3_file_nok(mock_hash_file, mock_makedirs, mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
-    s3_instance.download_file.side_effect = Exception('Cannot download S3 object')
+    s3_instance.download_file.side_effect = Exception("Cannot download S3 object")
     mocked_s3_client.return_value = s3_instance
 
     with pytest.raises(StorageError):
         copy("s3://bucket/source.ext", "file:///path/to/destination.ext", "toto")
         mock_makedirs.assert_called_once_with("/path/to", exist_ok=True)
 
-
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_copy_file_s3_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.upload_file.return_value = None
     s3_instance.head_object.return_value = {"ETag": "toto"}
     mocked_s3_client.return_value = s3_instance
 
     try:
         copy("file:///path/to/source.ext", "s3://bucket/destination.ext", "toto")
     except Exception as exc:
         assert False, f"FILE -> S3 copy raises an exception: {exc}"
 
-
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_copy_s3_s3_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.copy.return_value = None
     s3_instance.head_object.return_value = {"ETag": "toto"}
     mocked_s3_client.return_value = s3_instance
 
     try:
         copy("s3://bucket/source.ext", "s3://bucket/destination.ext", "toto")
     except Exception as exc:
         assert False, f"S3 -> S3 copy raises an exception: {exc}"
 
-
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_copy_s3_s3_intercluster_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.copy.return_value = None
     s3_instance.head_object.return_value = {"ETag": "toto"}
     mocked_s3_client.return_value = s3_instance
 
     try:
         copy("s3://bucket@a/source.ext", "s3://bucket@b/destination.ext", "toto")
     except Exception as exc:
         assert False, f"S3 -> S3 inter cluster copy raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_copy_s3_s3_intercluster_nok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.copy.return_value = None
     s3_instance.head_object.return_value = {"ETag": "toto"}
     mocked_s3_client.return_value = s3_instance
 
     with pytest.raises(StorageError):
         copy("s3://bucket@a/source.ext", "s3://bucket@c/destination.ext", "toto")
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
-@mock.patch('os.makedirs', return_value=None)
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
+@mock.patch("os.makedirs", return_value=None)
 @patch("builtins.open", new_callable=mock_open)
 def test_copy_ceph_file_ok(mock_file, mock_makedirs, mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.read.return_value = b"data"
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
-        copy("ceph://pool/source.ext", "file:///path/to/destination.ext", "8d777f385d3dfec8815d20f7496026dc")
+        copy(
+            "ceph://pool/source.ext",
+            "file:///path/to/destination.ext",
+            "8d777f385d3dfec8815d20f7496026dc",
+        )
         mock_makedirs.assert_called_once_with("/path/to", exist_ok=True)
     except Exception as exc:
         assert False, f"CEPH -> FILE copy raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 @patch("builtins.open", new_callable=mock_open, read_data=b"data")
 def test_copy_file_ceph_ok(mock_file, mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.write.return_value = None
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
-        copy("file:///path/to/source.ext", "ceph://pool/destination.ext", "8d777f385d3dfec8815d20f7496026dc")
+        copy(
+            "file:///path/to/source.ext",
+            "ceph://pool/destination.ext",
+            "8d777f385d3dfec8815d20f7496026dc",
+        )
     except Exception as exc:
         assert False, f"FILE -> CEPH copy raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 @patch("builtins.open", new_callable=mock_open, read_data=b"data")
 def test_copy_ceph_ceph_ok(mock_file, mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.read.return_value = b"data"
     ioctx_instance.write.return_value = None
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
-        copy("ceph://pool1/source.ext", "ceph://pool2/destination.ext", "8d777f385d3dfec8815d20f7496026dc")
+        copy(
+            "ceph://pool1/source.ext",
+            "ceph://pool2/destination.ext",
+            "8d777f385d3dfec8815d20f7496026dc",
+        )
     except Exception as exc:
         assert False, f"CEPH -> CEPH copy raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c", "ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {
+        "ROK4_CEPH_CONFFILE": "a",
+        "ROK4_CEPH_CLUSTERNAME": "b",
+        "ROK4_CEPH_USERNAME": "c",
+        "ROK4_S3_URL": "https://a,https://b",
+        "ROK4_S3_SECRETKEY": "a,b",
+        "ROK4_S3_KEY": "a,b",
+    },
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
+@mock.patch("rok4.Storage.boto3.client")
 @patch("builtins.open", new_callable=mock_open, read_data=b"data")
 def test_copy_ceph_s3_ok(mock_file, mocked_s3_client, mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.read.return_value = b"data"
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.upload_file.return_value = None
     s3_instance.head_object.return_value = {"ETag": "8d777f385d3dfec8815d20f7496026dc"}
     mocked_s3_client.return_value = s3_instance
 
     try:
-        copy("ceph://pool1/source.ext", "s3://bucket/destination.ext", "8d777f385d3dfec8815d20f7496026dc")
+        copy(
+            "ceph://pool1/source.ext",
+            "s3://bucket/destination.ext",
+            "8d777f385d3dfec8815d20f7496026dc",
+        )
     except Exception as exc:
         assert False, f"CEPH -> S3 copy raises an exception: {exc}"
 
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch('requests.get')
+@patch('builtins.open', new_callable=mock_open)
+def test_copy_http_file_ok(mock_open, mock_requests):
+    try:
+
+        http_instance = MagicMock()
+        http_instance.iter_content.return_value = ["data","data2"]
+        mock_requests.return_value = http_instance
+
+        copy("http://path/to/source.ext", "file:///path/to/destination.ext")
+        mock_requests.assert_called_once_with("http://path/to/source.ext", stream=True)
+        mock_open.assert_called_once_with("/path/to/destination.ext", "wb")
+    except Exception as exc:
+        assert False, f"HTTP -> FILE copy raises an exception: {exc}"
+
+@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)
+@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch('requests.get')
+def test_copy_http_ceph_ok(mock_requests, mocked_rados_client):
+    try:
+
+        http_instance = MagicMock()
+        http_instance.iter_content.return_value = ["data","data2"]
+        mock_requests.return_value = http_instance
+
+
+        disconnect_ceph_clients()
+        ioctx_instance = MagicMock()
+        ioctx_instance.write.return_value = None
+        ceph_instance = MagicMock()
+        ceph_instance.open_ioctx.return_value = ioctx_instance
+        mocked_rados_client.return_value = ceph_instance
+
+        copy("http://path/to/source.ext", "ceph://pool1/source.ext")
+        mock_requests.assert_called_once_with("http://path/to/source.ext", stream=True)
+    except Exception as exc:
+        assert False, f"HTTP -> CEPH copy raises an exception: {exc}"
+
+@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)
+@mock.patch('rok4.Storage.boto3.client')
+@mock.patch('requests.get')
+@patch('tempfile.NamedTemporaryFile', new_callable=mock_open)
+@mock.patch('os.remove')
+def test_copy_http_s3_ok(mock_remove, mock_tempfile, mock_requests, mocked_s3_client):
+    try:
+
+        http_instance = MagicMock()
+        http_instance.iter_content.return_value = ["data","data2"]
+        mock_requests.return_value = http_instance
+
+        disconnect_s3_clients()
+        s3_instance = MagicMock()
+        s3_instance.upload_file.return_value = None
+        s3_instance.head_object.return_value = {"ETag": "8d777f385d3dfec8815d20f7496026dc"}
+        mocked_s3_client.return_value = s3_instance
+
+        copy("http://path/to/source.ext", "s3://bucket/destination.ext")
+        mock_requests.assert_called_once_with("http://path/to/source.ext", stream=True)
+        mock_tempfile.assert_called_once_with("w+b",delete=False)
+    except Exception as exc:
+        assert False, f"HTTP -> CEPH copy raises an exception: {exc}"
 
 
 ############ link
 
+
 def test_link_type_nok():
     with pytest.raises(StorageError):
         link("ceph://pool1/target.ext", "file:///path/to/link.ext")
 
+
 def test_link_hard_nok():
     with pytest.raises(StorageError):
         link("ceph://pool1/source.ext", "ceph://pool2/destination.ext", True)
 
-@mock.patch.dict(os.environ, {}, clear=True)  
-@mock.patch('os.symlink', return_value=None)
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("os.symlink", return_value=None)
 def test_link_file_ok(mock_link):
     try:
         link("file:///path/to/target.ext", "file:///path/to/link.ext")
         mock_link.assert_called_once_with("/path/to/target.ext", "/path/to/link.ext")
     except Exception as exc:
         assert False, f"FILE link raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {}, clear=True)  
-@mock.patch('os.link', return_value=None)
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("os.link", return_value=None)
 def test_hlink_file_ok(mock_link):
     try:
         link("file:///path/to/target.ext", "file:///path/to/link.ext", True)
         mock_link.assert_called_once_with("/path/to/target.ext", "/path/to/link.ext")
     except Exception as exc:
         assert False, f"FILE hard link raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 def test_link_ceph_ok(mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.write.return_value = None
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
         link("ceph://pool1/target.ext", "ceph://pool2/link.ext")
     except Exception as exc:
         assert False, f"CEPH link raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_link_s3_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.put_object.return_value = None
     mocked_s3_client.return_value = s3_instance
 
     try:
         link("s3://bucket1/target.ext", "s3://bucket2/link.ext")
     except Exception as exc:
         assert False, f"S3 link raises an exception: {exc}"
 
-
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_link_s3_nok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.put_object.return_value = None
     mocked_s3_client.return_value = s3_instance
 
     with pytest.raises(StorageError):
         link("s3://bucket1@a/target.ext", "s3://bucket2@b/link.ext")
 
+
 ############ get_size
 
-@mock.patch.dict(os.environ, {}, clear=True)  
-@mock.patch('os.stat')
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("os.stat")
 def test_size_file_ok(mock_stat):
     mock_stat.return_value.st_size = 12
     try:
         size = get_size("file:///path/to/file.ext")
         assert size == 12
     except Exception as exc:
         assert False, f"FILE size raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 def test_size_ceph_ok(mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.stat.return_value = (12, "date")
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
     try:
         size = get_size("ceph://pool/object.ext")
         assert size == 12
     except Exception as exc:
         assert False, f"CEPH size raises an exception: {exc}"
 
-
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_size_s3_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
-    s3_instance.head_object.return_value = {"ContentLength": '"12"'}
+    s3_instance.head_object.return_value = {"ContentLength": 12}
     mocked_s3_client.return_value = s3_instance
 
     try:
         size = get_size("s3://bucket/object.ext")
         assert size == 12
     except Exception as exc:
         assert False, f"S3 size raises an exception: {exc}"
 
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch('requests.get')
+def test_size_http_ok(mock_requests):
+
+    http_instance = MagicMock()
+    http_instance.headers = {"content-length":12}
+    mock_requests.return_value = http_instance
+
+    try:
+        size = get_size("http://path/to/file.ext")
+        assert size == 12
+    except Exception as exc:
+        assert False, f"HTTP size raises an exception: {exc}"
+
 
 ############ exists
 
-@mock.patch.dict(os.environ, {}, clear=True)  
-@mock.patch('os.path.exists', return_value=True)
+
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("os.path.exists", return_value=True)
 def test_exists_file_ok(mock_exists):
     try:
         assert exists("file:///path/to/file.ext")
     except Exception as exc:
         assert False, f"FILE exists raises an exception: {exc}"
 
     mock_exists.return_value = False
     try:
         assert not exists("file:///path/to/file.ext")
     except Exception as exc:
         assert False, f"FILE not exists raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 def test_exists_ceph_ok(mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.stat.return_value = None
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
@@ -523,56 +739,85 @@
     ioctx_instance.stat.side_effect = rados.ObjectNotFound("error")
     try:
         assert not exists("ceph://pool/object.ext")
     except Exception as exc:
         assert False, f"CEPH not exists raises an exception: {exc}"
 
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_exists_s3_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.head_object.return_value = None
     mocked_s3_client.return_value = s3_instance
 
     try:
         assert exists("s3://bucket/object.ext")
     except Exception as exc:
         assert False, f"S3 exists raises an exception: {exc}"
 
-    s3_instance.head_object.side_effect = botocore.exceptions.ClientError(operation_name='InvalidKeyPair.Duplicate', error_response={"Error": {"Code": "404"}})
+    s3_instance.head_object.side_effect = botocore.exceptions.ClientError(
+        operation_name="InvalidKeyPair.Duplicate", error_response={"Error": {"Code": "404"}}
+    )
     try:
         assert not exists("s3://bucket/object.ext")
     except Exception as exc:
         assert False, f"CEPH not exists raises an exception: {exc}"
 
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch('requests.get')
+def test_exists_http_ok(mock_requests):
+
+    http_instance = MagicMock()
+    http_instance.status_code = 200
+    mock_requests.return_value = http_instance
+
+    try:
+        assert exists("http://path/to/file.ext")
+    except Exception as exc:
+        assert False, f"HTTP exists raises an exception: {exc}"
+
+    http_instance.status_code = 404
+    mock_requests.return_value = http_instance
+
+    try:
+        assert not exists("http://path/to/file.ext")
+    except Exception as exc:
+        assert False, f"HTTP exists raises an exception: {exc}"
+
 
 ############ remove
 
-@mock.patch.dict(os.environ, {}, clear=True)  
-@mock.patch('os.remove')
+@mock.patch.dict(os.environ, {}, clear=True)
+@mock.patch("os.remove")
 def test_remove_file_ok(mock_remove):
     mock_remove.return_value = None
     try:
         remove("file:///path/to/file.ext")
     except Exception as exc:
         assert False, f"FILE deletion raises an exception: {exc}"
 
     mock_remove.side_effect = FileNotFoundError("error")
     try:
         remove("file:///path/to/file.ext")
     except Exception as exc:
         assert False, f"FILE deletion (not found) raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)  
-@mock.patch('rok4.Storage.rados.Rados')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.rados.Rados")
 def test_remove_ceph_ok(mocked_rados_client):
-
     disconnect_ceph_clients()
     ioctx_instance = MagicMock()
     ioctx_instance.remove_object.return_value = None
     ceph_instance = MagicMock()
     ceph_instance.open_ioctx.return_value = ioctx_instance
     mocked_rados_client.return_value = ceph_instance
 
@@ -583,49 +828,92 @@
 
     ioctx_instance.stat.side_effect = rados.ObjectNotFound("error")
     try:
         Exception("ceph://pool/object.ext")
     except Exception as exc:
         assert False, f"CEPH deletion (not found) raises an exception: {exc}"
 
-
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)  
-@mock.patch('rok4.Storage.boto3.client')
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
+@mock.patch("rok4.Storage.boto3.client")
 def test_remove_s3_ok(mocked_s3_client):
-
     disconnect_s3_clients()
     s3_instance = MagicMock()
     s3_instance.delete_object.return_value = None
     mocked_s3_client.return_value = s3_instance
 
     try:
         remove("s3://bucket/object.ext")
     except Exception as exc:
         assert False, f"S3 deletion raises an exception: {exc}"
 
 
 ############ get_osgeo_path
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_get_osgeo_path_file_ok():
     try:
         path = get_osgeo_path("file:///path/to/file.ext")
         assert path == "/path/to/file.ext"
     except Exception as exc:
         assert False, f"FILE osgeo path raises an exception: {exc}"
 
-@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True) 
+@mock.patch.dict(
+    os.environ,
+    {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"},
+    clear=True,
+)
 def test_get_osgeo_path_s3_ok():
-
     disconnect_s3_clients()
-    
+
     try:
         path = get_osgeo_path("s3://bucket@b/to/object.ext")
         assert path == "/vsis3/bucket/to/object.ext"
     except Exception as exc:
         assert False, f"S3 osgeo path raises an exception: {exc}"
 
 
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_get_osgeo_path_nok():
     with pytest.raises(NotImplementedError):
-        get_osgeo_path("ceph://pool/data.ext")
+        get_osgeo_path("ceph://pool/data.ext")
+
+############ size_path
+def test_size_path_file_ok():
+    try:
+        size = size_path("file://tests/fixtures/TIFF_PBF_MVT")
+        assert size == 124838
+    except Exception as exc:
+        assert False, f"FILE size of the path raises an exception: {exc}"
+
+def test_size_file_nok():
+    with pytest.raises(StorageError) :
+        size = size_path("file://tests/fixtures/TIFF_PBF_M")
+
+@mock.patch.dict(os.environ, {"ROK4_CEPH_CONFFILE": "a", "ROK4_CEPH_CLUSTERNAME": "b", "ROK4_CEPH_USERNAME": "c"}, clear=True)
+def test_size_path_ceph_nok():
+
+    with pytest.raises(NotImplementedError):
+        size = size_path("ceph://pool/path")
+
+@mock.patch.dict(os.environ, {"ROK4_S3_URL": "https://a,https://b", "ROK4_S3_SECRETKEY": "a,b", "ROK4_S3_KEY": "a,b"}, clear=True)
+@mock.patch('rok4.Storage.boto3.client')
+def test_size_path_s3_ok(mocked_s3_client):
+
+    disconnect_s3_clients()
+    pages = [{"Contents" : [{"Size" : 10},{"Size" : 20}]}, {"Contents" : [{"Size" : 50}]}]
+    paginator = MagicMock()
+    paginator.paginate.return_value = pages
+    client = MagicMock()
+    client.get_paginator.return_value = paginator
+    mocked_s3_client.return_value = client
+
+    try:
+        size = size_path("s3://bucket/path")
+        assert size == 80
+    except Exception as exc:
+        assert False, f"S3 size of the path raises an exception: {exc}"
+
```

### Comparing `rok4-1.6.0/tests/test_TileMatrixSet.py` & `rok4-1.7.0/tests/test_TileMatrixSet.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,129 +2,199 @@
 from rok4.Exceptions import *
 
 import pytest
 import os
 from unittest.mock import *
 from unittest import mock
 
+
 @mock.patch.dict(os.environ, {}, clear=True)
 def test_missing_env():
     with pytest.raises(MissingEnvironmentError):
         tms = TileMatrixSet("tms")
 
+
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', side_effect=StorageError('FILE', 'Not found'))
+@mock.patch("rok4.TileMatrixSet.get_data_str", side_effect=StorageError("FILE", "Not found"))
 def test_wrong_file(mocked_get_data_str):
     with pytest.raises(StorageError):
         tms = TileMatrixSet("tms")
 
+
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_bad_json(mocked_get_data_str):
     with pytest.raises(FormatError) as exc:
         tms = TileMatrixSet("tms")
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"crs":"EPSG:3857","orderedAxes":["X","Y"]}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"crs":"EPSG:3857","orderedAxes":["X","Y"]}',
+)
 def test_missing_id(mocked_get_data_str):
     with pytest.raises(MissingAttributeError) as exc:
         tms = TileMatrixSet("tms")
     assert str(exc.value) == "Missing attribute 'id' in 'file:///path/to/tms.json'"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_missing_crs(mocked_get_data_str):
     with pytest.raises(MissingAttributeError) as exc:
         tms = TileMatrixSet("tms")
     assert str(exc.value) == "Missing attribute 'crs' in 'file:///path/to/tms.json'"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
 
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"crs":"epsg:123456","orderedAxes":["X","Y"],"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"crs":"epsg:123456","orderedAxes":["X","Y"],"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_wrong_crs(mocked_get_data_str):
     with pytest.raises(Exception) as exc:
         tms = TileMatrixSet("tms")
-    assert str(exc.value) == "Wrong attribute 'crs' ('epsg:123456') in 'file:///path/to/tms.json', not recognize by OSR"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    assert (
+        str(exc.value)
+        == "Wrong attribute 'crs' ('epsg:123456') in 'file:///path/to/tms.json', not recognize by OSR"
+    )
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"crs":"epsg:4326","orderedAxes":["Lat","Lon"],"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"crs":"epsg:4326","orderedAxes":["Lat","Lon"],"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"id":"PM"}',
+)
 def test_wrong_axes_order(mocked_get_data_str):
     with pytest.raises(Exception) as exc:
         tms = TileMatrixSet("tms")
-    assert str(exc.value) == "TMS 'file:///path/to/tms.json' own invalid axes order : only X/Y or Lon/Lat are handled"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    assert (
+        str(exc.value)
+        == "TMS 'file:///path/to/tms.json' own invalid axes order : only X/Y or Lon/Lat are handled"
+    )
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_missing_levels(mocked_get_data_str):
     with pytest.raises(MissingAttributeError) as exc:
         tms = TileMatrixSet("tms")
     assert str(exc.value) == "Missing attribute 'tileMatrices' in 'file:///path/to/tms.json'"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_no_levels(mocked_get_data_str):
     with pytest.raises(Exception) as exc:
         tms = TileMatrixSet("tms")
     assert str(exc.value) == "TMS 'file:///path/to/tms.json' has no level"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[{"tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"orderedAxes":["X","Y"],"id":"PM","crs":"EPSG:3857"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[{"tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"orderedAxes":["X","Y"],"id":"PM","crs":"EPSG:3857"}',
+)
 def test_wrong_level(mocked_get_data_str):
     with pytest.raises(MissingAttributeError) as exc:
         tms = TileMatrixSet("tms")
     assert str(exc.value) == "Missing attribute tileMatrices[].'id' in 'file:///path/to/tms.json'"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[{"id":"level_0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[{"id":"level_0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_wrong_level_id(mocked_get_data_str):
     with pytest.raises(Exception) as exc:
         tms = TileMatrixSet("tms")
 
-    assert str(exc.value) == "TMS file:///path/to/tms.json owns a level whom id contains an underscore (level_0)"
-    mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+    assert (
+        str(exc.value)
+        == "TMS file:///path/to/tms.json owns a level whom id contains an underscore (level_0)"
+    )
+    mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
+
 
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[{"id":"0","tileWidth":256,"scaleDenominator":559082264.028718,"matrixWidth":1,"cellSize":156543.033928041,"matrixHeight":1,"tileHeight":256,"pointOfOrigin":[-20037508.3427892,20037508.3427892]}],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_ok(mocked_get_data_str):
     try:
         tms = TileMatrixSet("tms")
         assert tms.get_level("0") is not None
         assert tms.get_level("4") is None
-        mocked_get_data_str.assert_called_once_with('file:///path/to/tms.json')
+        mocked_get_data_str.assert_called_once_with("file:///path/to/tms.json")
     except Exception as exc:
         assert False, f"'TileMatrixSet creation raises an exception: {exc}"
 
+
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"tileMatrices":[{"id":"17","cellSize":1.19432856695588,"matrixHeight":131072,"pointOfOrigin":[-20037508.3427892,20037508.3427892],"tileHeight":256,"tileWidth":256,"scaleDenominator":4265.45916769957,"matrixWidth":131072}],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"tileMatrices":[{"id":"17","cellSize":1.19432856695588,"matrixHeight":131072,"pointOfOrigin":[-20037508.3427892,20037508.3427892],"tileHeight":256,"tileWidth":256,"scaleDenominator":4265.45916769957,"matrixWidth":131072}],"crs":"EPSG:3857","orderedAxes":["X","Y"],"id":"PM"}',
+)
 def test_pm_conversions(mocked_get_data_str):
     try:
         tms = TileMatrixSet("tms")
         tm = tms.get_level("17")
         assert tm.x_to_column(670654.2832369965) == 67729
         assert tm.y_to_row(5980575.503117723) == 45975
-        assert tm.tile_to_bbox(67728, 45975) == (670199.864004489, 5980433.093032133, 670505.6121176295, 5980738.841145273)
-        assert tm.bbox_to_tiles((670034.4267107458, 5980565.948489188,670649.5059227281, 5980936.190344945)) == (67727, 45974,67729, 45975)
+        assert tm.tile_to_bbox(67728, 45975) == (
+            670199.864004489,
+            5980433.093032133,
+            670505.6121176295,
+            5980738.841145273,
+        )
+        assert tm.bbox_to_tiles(
+            (670034.4267107458, 5980565.948489188, 670649.5059227281, 5980936.190344945)
+        ) == (67727, 45974, 67729, 45975)
         assert tm.point_to_indices(670654.2832369965, 5980575.503117723) == (67729, 45975, 124, 136)
     except Exception as exc:
         assert False, f"'TileMatrixSet creation raises an exception: {exc}"
 
+
 @mock.patch.dict(os.environ, {"ROK4_TMS_DIRECTORY": "file:///path/to"}, clear=True)
-@mock.patch('rok4.TileMatrixSet.get_data_str', return_value='{"crs":"EPSG:4326","tileMatrices":[{"tileWidth":256,"scaleDenominator":1066.36480348451,"matrixWidth":524288,"cellSize":2.68220901489258e-06,"matrixHeight":262144,"pointOfOrigin":[-180,90],"tileHeight":256,"id":"18"}],"orderedAxes":["Lon","Lat"],"id":"4326"}')
+@mock.patch(
+    "rok4.TileMatrixSet.get_data_str",
+    return_value='{"crs":"EPSG:4326","tileMatrices":[{"tileWidth":256,"scaleDenominator":1066.36480348451,"matrixWidth":524288,"cellSize":2.68220901489258e-06,"matrixHeight":262144,"pointOfOrigin":[-180,90],"tileHeight":256,"id":"18"}],"orderedAxes":["Lon","Lat"],"id":"4326"}',
+)
 def test_4326_conversions(mocked_get_data_str):
     try:
         tms = TileMatrixSet("tms")
         tm = tms.get_level("18")
         assert tm.x_to_column(5) == 269425
         assert tm.y_to_row(45) == 65535
-        assert tm.tile_to_bbox(269425, 65535) == (44.99999999999997, 4.999465942382926, 45.000686645507784, 5.000152587890739)
-        assert tm.bbox_to_tiles((45,5,48,6)) == (269425,61166,270882,65535)
-        assert tm.point_to_indices(45,5) == (269425, 65535, 199, 255)
+        assert tm.tile_to_bbox(269425, 65535) == (
+            44.99999999999997,
+            4.999465942382926,
+            45.000686645507784,
+            5.000152587890739,
+        )
+        assert tm.bbox_to_tiles((45, 5, 48, 6)) == (269425, 61166, 270882, 65535)
+        assert tm.point_to_indices(45, 5) == (269425, 65535, 199, 255)
     except Exception as exc:
-        assert False, f"'TileMatrixSet creation raises an exception: {exc}"
+        assert False, f"'TileMatrixSet creation raises an exception: {exc}"
```


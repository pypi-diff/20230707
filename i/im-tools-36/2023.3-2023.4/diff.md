# Comparing `tmp/im-tools-36-2023.3.tar.gz` & `tmp/im-tools-36-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-tools-36-2023.3.tar", last modified: Wed Feb  8 14:40:30 2023, max compression
+gzip compressed data, was "im-tools-36-2023.4.tar", last modified: Fri Jul  7 14:11:39 2023, max compression
```

## Comparing `im-tools-36-2023.3.tar` & `im-tools-36-2023.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 im-tools-36-2023.3/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4286 2023-02-08 14:40:30.935883 im-tools-36-2023.3/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-02-07 12:37:54.000000 im-tools-36-2023.3/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 im-tools-36-2023.3/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     3475 2023-02-07 12:36:42.000000 im-tools-36-2023.3/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1867 2023-02-07 11:11:10.000000 im-tools-36-2023.3/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/im_tools_36/
--rw-r--r--   0 eric      (1000) users      (984)     1596 2023-02-07 11:00:53.000000 im-tools-36-2023.3/im_tools_36/__init__.py
--rw-r--r--   0 eric      (1000) users      (984)     3130 2023-02-06 11:19:53.000000 im-tools-36-2023.3/im_tools_36/combination.py
--rw-r--r--   0 eric      (1000) users      (984)     8060 2023-02-08 09:42:49.000000 im-tools-36-2023.3/im_tools_36/input.py
--rw-r--r--   0 eric      (1000) users      (984)     3807 2023-02-06 12:55:09.000000 im-tools-36-2023.3/im_tools_36/intensity.py
--rw-r--r--   0 eric      (1000) users      (984)     5639 2023-02-08 14:15:56.000000 im-tools-36-2023.3/im_tools_36/output.py
--rw-r--r--   0 eric      (1000) users      (984)     2199 2023-02-06 10:51:35.000000 im-tools-36-2023.3/im_tools_36/path.py
--rw-r--r--   0 eric      (1000) users      (984)     3164 2023-02-07 11:18:43.000000 im-tools-36-2023.3/im_tools_36/processing.py
--rw-r--r--   0 eric      (1000) users      (984)    15831 2023-02-06 12:55:59.000000 im-tools-36-2023.3/im_tools_36/shape.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/im_tools_36/test/
--rw-r--r--   0 eric      (1000) users      (984)     5559 2023-02-06 14:14:39.000000 im-tools-36-2023.3/im_tools_36/test/autocropped.py
--rw-r--r--   0 eric      (1000) users      (984)     2846 2023-02-08 09:34:57.000000 im-tools-36-2023.3/im_tools_36/test/input.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/im_tools_36/type/
--rw-r--r--   0 eric      (1000) users      (984)     1703 2023-02-06 11:28:07.000000 im-tools-36-2023.3/im_tools_36/type/image.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-02-08 14:16:29.000000 im-tools-36-2023.3/im_tools_36/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-02-08 14:40:30.935883 im-tools-36-2023.3/im_tools_36.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4286 2023-02-08 14:40:30.000000 im-tools-36-2023.3/im_tools_36.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      569 2023-02-08 14:40:30.000000 im-tools-36-2023.3/im_tools_36.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-02-08 14:40:30.000000 im-tools-36-2023.3/im_tools_36.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       12 2023-02-08 14:40:30.000000 im-tools-36-2023.3/im_tools_36.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 im-tools-36-2023.3/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-02-08 14:40:30.935883 im-tools-36-2023.3/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5398 2023-02-07 11:16:57.000000 im-tools-36-2023.3/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.013587 im-tools-36-2023.4/
+-rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 im-tools-36-2023.4/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4286 2023-07-07 14:11:39.013587 im-tools-36-2023.4/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      636 2023-02-07 12:37:54.000000 im-tools-36-2023.4/README-COPYRIGHT-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 im-tools-36-2023.4/README-LICENCE-utf8.txt
+-rw-r--r--   0 eric      (1000) users      (984)     3475 2023-02-07 12:36:42.000000 im-tools-36-2023.4/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.006920 im-tools-36-2023.4/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.010254 im-tools-36-2023.4/documentation/wiki/
+-rw-r--r--   0 eric      (1000) users      (984)     1867 2023-02-07 11:11:10.000000 im-tools-36-2023.4/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.010254 im-tools-36-2023.4/im_tools_36/
+-rw-r--r--   0 eric      (1000) users      (984)     1596 2023-02-07 11:00:53.000000 im-tools-36-2023.4/im_tools_36/__init__.py
+-rw-r--r--   0 eric      (1000) users      (984)     3130 2023-02-06 11:19:53.000000 im-tools-36-2023.4/im_tools_36/combination.py
+-rw-r--r--   0 eric      (1000) users      (984)     8955 2023-07-07 14:06:08.000000 im-tools-36-2023.4/im_tools_36/input.py
+-rw-r--r--   0 eric      (1000) users      (984)     3807 2023-02-06 12:55:09.000000 im-tools-36-2023.4/im_tools_36/intensity.py
+-rw-r--r--   0 eric      (1000) users      (984)     5639 2023-02-08 14:15:56.000000 im-tools-36-2023.4/im_tools_36/output.py
+-rw-r--r--   0 eric      (1000) users      (984)     2199 2023-02-06 10:51:35.000000 im-tools-36-2023.4/im_tools_36/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     3164 2023-02-07 11:18:43.000000 im-tools-36-2023.4/im_tools_36/processing.py
+-rw-r--r--   0 eric      (1000) users      (984)    15831 2023-02-06 12:55:59.000000 im-tools-36-2023.4/im_tools_36/shape.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.013587 im-tools-36-2023.4/im_tools_36/test/
+-rw-r--r--   0 eric      (1000) users      (984)     5559 2023-02-06 14:14:39.000000 im-tools-36-2023.4/im_tools_36/test/autocropped.py
+-rw-r--r--   0 eric      (1000) users      (984)     2993 2023-07-07 14:06:56.000000 im-tools-36-2023.4/im_tools_36/test/input.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.013587 im-tools-36-2023.4/im_tools_36/type/
+-rw-r--r--   0 eric      (1000) users      (984)     1703 2023-02-06 11:28:07.000000 im-tools-36-2023.4/im_tools_36/type/image.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2023-07-07 13:23:02.000000 im-tools-36-2023.4/im_tools_36/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-07-07 14:11:39.013587 im-tools-36-2023.4/im_tools_36.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4286 2023-07-07 14:11:39.000000 im-tools-36-2023.4/im_tools_36.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      569 2023-07-07 14:11:39.000000 im-tools-36-2023.4/im_tools_36.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2023-07-07 14:11:39.000000 im-tools-36-2023.4/im_tools_36.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       12 2023-07-07 14:11:39.000000 im-tools-36-2023.4/im_tools_36.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 im-tools-36-2023.4/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2023-07-07 14:11:39.013587 im-tools-36-2023.4/setup.cfg
+-rw-r--r--   0 eric      (1000) users      (984)     5398 2023-02-07 11:16:57.000000 im-tools-36-2023.4/setup.py
```

### Comparing `im-tools-36-2023.3/PKG-INFO` & `im-tools-36-2023.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-tools-36
-Version: 2023.3
+Version: 2023.4
 Summary: A Toolbox for n-Dimensional Images
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/im-tools-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/im-tools-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/im-tools-36/
```

### Comparing `im-tools-36-2023.3/README-COPYRIGHT-utf8.txt` & `im-tools-36-2023.4/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/README-LICENCE-utf8.txt` & `im-tools-36-2023.4/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/README.rst` & `im-tools-36-2023.4/README.rst`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/documentation/wiki/description.asciidoc` & `im-tools-36-2023.4/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/__init__.py` & `im-tools-36-2023.4/im_tools_36/__init__.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/combination.py` & `im-tools-36-2023.4/im_tools_36/combination.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/input.py` & `im-tools-36-2023.4/im_tools_36/input.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,20 +39,32 @@
 import imageio as mgio
 import numpy as nmpy
 from im_tools_36.path import path_h, path_t
 
 
 def _Module(name: str, /) -> module_t | None:
     """"""
-    try:
-        output = mprt.import_module(name)
-    except ModuleNotFoundError:
-        output = None
+    if name in sstm.modules:
+        return sstm.modules[name]
+
+    # https://docs.python.org/3/library/importlib.html#checking-if-a-module-can-be-imported
+    if (spec := mprt.util.find_spec(name)) is None:
+        return None
+
+    output = mprt.util.module_from_spec(spec)
+    sstm.modules[name] = output
+    spec.loader.exec_module(output)
 
     return output
+    # try:
+    #     output = mprt.import_module(name)
+    # except ModuleNotFoundError:
+    #     output = None
+    #
+    # return output
 
 
 # Using VTK seems too complicated. See
 # https://stackoverflow.com/questions/25230541/how-to-convert-a-vtkimage-into-a-numpy-array
 # for a 3-D example.
 aics = _Module("aicsimageio")
 pncv = _Module("cv2")
@@ -136,14 +148,15 @@
     path: path_h,
     /,
     *,
     should_squeeze: bool = True,
     expected_dim: int = None,
     expected_shape: Sequence[int | None] = None,
     with_module: str = None,
+    should_print_module: bool = False,
 ) -> array_t | Tuple[str, ...]:
     """"""
     # Potential outputs
     image = None
     issues = []
 
     if isinstance(path, str):
@@ -175,55 +188,67 @@
             reading_functions.append(FUNCTION_OF_MODULE[mrci])
         elif img_format in ("czi", "lif", "nd2"):
             reading_functions.append(FUNCTION_OF_MODULE[aics])
     elif with_module in MODULE_WITH_NAME:
         reading_functions = [FUNCTION_OF_MODULE[MODULE_WITH_NAME[with_module]]]
     else:
         return (
-            f"{with_module}: Invalid module. Expected={str(tuple(MODULE_WITH_NAME.keys()))[1:-1]}",
+            f"{with_module}: Invalid module. "
+            f"Expected={str(tuple(MODULE_WITH_NAME.keys()))[1:-1]}",
         )
 
+    failure = True
     for Read in reversed(reading_functions):
         if Read is None:
             continue
 
         try:
             image = Read(path_str)
-            break
+            # A module might return None, for example, in case of a failure instead of
+            # raising an exception. Hence the test below.
+            if isinstance(image, array_t):
+                failure = False
+                if should_print_module:
+                    print(f'{path_str}: Read with function "{Read.__name__}".')
+                break
         except Exception as exception:
             issues.append(str(exception))
 
-    if image is None:
-        return tuple(issues)
+    if failure:
+        if issues.__len__() > 0:
+            return tuple(issues)
+        return ("Silent Exception",)
 
     if should_squeeze:
         image = nmpy.squeeze(image)
 
     if (expected_dim is not None) and (image.ndim != expected_dim):
         return (
-            f"{image.ndim}: Invalid dimension (shape={image.shape}). Expected={expected_dim}",
+            f"{image.ndim}: Invalid dimension (shape={image.shape}). "
+            f"Expected={expected_dim}",
         )
     if expected_shape is None:
         return image
 
     shape = image.shape
-    if _ShapesMatch(shape, expected_shape):
+    if _ShapeMatches(shape, expected_shape):
         return image
 
     shape_as_array = nmpy.array(shape)
     for order in ittl.permutations(range(image.ndim)):
-        if _ShapesMatch(shape_as_array[nmpy.array(order)], expected_shape):
+        if _ShapeMatches(shape_as_array[nmpy.array(order)], expected_shape):
             return nmpy.moveaxis(image, order, range(image.ndim))
 
     return (
-        f"{shape}: Invalid shape. Expected={tuple(expected_shape)}, or a permutation of it",
+        f"{shape}: Invalid shape. "
+        f"Expected={tuple(expected_shape)}, or a permutation of it.",
     )
 
 
-def _ShapesMatch(
+def _ShapeMatches(
     actual: Tuple[int, ...] | array_t, expected: Sequence[int | None], /
 ) -> bool:
     """"""
     return all((_ctl == _xpt) or (_xpt is None) for _ctl, _xpt in zip(actual, expected))
 
 
 def AvailableModules(
```

### Comparing `im-tools-36-2023.3/im_tools_36/intensity.py` & `im-tools-36-2023.4/im_tools_36/intensity.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/output.py` & `im-tools-36-2023.4/im_tools_36/output.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/path.py` & `im-tools-36-2023.4/im_tools_36/path.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/processing.py` & `im-tools-36-2023.4/im_tools_36/processing.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/shape.py` & `im-tools-36-2023.4/im_tools_36/shape.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/test/autocropped.py` & `im-tools-36-2023.4/im_tools_36/test/autocropped.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/test/input.py` & `im-tools-36-2023.4/im_tools_36/test/input.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
+import textwrap as txtw
 from pathlib import Path as path_t
 from typing import Tuple
 
 from numpy import ndarray as array_t
 
 from im_tools_36.input import AvailableModules, ImageVolumeOrSequence
 
-
 PATH_JR = "/home/eric/Data/Videos/people/jeremie-roux"
 
 
 modules_details = AvailableModules()
 
 print("--- PYTHON MODULES")
 for module in AvailableModules(as_modules=True):
@@ -54,21 +54,24 @@
 
 def CheckImage(path: path_t, expected_shape: Tuple[int | None, ...], /) -> None:
     """"""
     print(f"--- {path}: {expected_shape}")
 
     for module_ in ((None,),) + modules_details:
         ivs = ImageVolumeOrSequence(
-            path, expected_shape=expected_shape, with_module=module_[0]
+            path,
+            expected_shape=expected_shape,
+            with_module=module_[0],
+            should_print_module=module_[0] is None,
         )
         if isinstance(ivs, array_t):
-            print(f"{module_[0]}: {ivs.shape}")
+            print(f"{module_[0]}: Success w/ shape {ivs.shape}")
         else:
-            print(f"!!! {module_[0]}")
-            print("\n".join(ivs))
+            print(f"!!! {module_[0]}: Failure")
+            print(txtw.indent("\n".join(ivs), "    "))
 
 
 channels = ("YFP", "mCherry", "POL")
 CheckImage(
     path_t(PATH_JR) / "p53" / "treat01_10_R3D.dv", (None, None, channels.__len__(), 433)
 )
```

### Comparing `im-tools-36-2023.3/im_tools_36/type/image.py` & `im-tools-36-2023.4/im_tools_36/type/image.py`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/im_tools_36/version.py` & `im-tools-36-2023.4/im_tools_36/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.3"
+__version__ = "2023.4"
```

### Comparing `im-tools-36-2023.3/im_tools_36.egg-info/PKG-INFO` & `im-tools-36-2023.4/im_tools_36.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-tools-36
-Version: 2023.3
+Version: 2023.4
 Summary: A Toolbox for n-Dimensional Images
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/im-tools-36/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/im-tools-36//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/im-tools-36/
```

### Comparing `im-tools-36-2023.3/im_tools_36.egg-info/SOURCES.txt` & `im-tools-36-2023.4/im_tools_36.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im-tools-36-2023.3/setup.py` & `im-tools-36-2023.4/setup.py`

 * *Files identical despite different names*


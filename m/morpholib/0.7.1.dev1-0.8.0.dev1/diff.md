# Comparing `tmp/morpholib-0.7.1.dev1.tar.gz` & `tmp/morpholib-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ksmall\Documents\Kenneth's stuff\Python\Morpho\pip\v0.7.1-test\dist\.tmp-zkv1ja08\morpholib-0.7.1.dev1.tar", last modified: Sat May 27 15:03:36 2023, max compression
+gzip compressed data, was "C:\Users\ksmall\Documents\Kenneth's stuff\Python\Morpho\pip\v080-test\dist\.tmp-53vsonz5\morpholib-0.8.0.dev1.tar", last modified: Fri Jul  7 19:30:24 2023, max compression
```

## Comparing `morpholib-0.7.1.dev1.tar` & `morpholib-0.8.0.dev1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/
--rw-rw-rw-   0        0        0     1091 2021-09-29 20:39:14.000000 morpholib-0.7.1.dev1/LICENSE
--rw-rw-rw-   0        0        0     4356 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     3967 2023-05-27 15:02:41.000000 morpholib-0.7.1.dev1/README.md
--rw-rw-rw-   0        0        0      110 2021-09-27 17:28:21.000000 morpholib-0.7.1.dev1/pyproject.toml
--rw-rw-rw-   0        0        0      665 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.785412 morpholib-0.7.1.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.847813 morpholib-0.7.1.dev1/src/morpholib/
--rw-rw-rw-   0        0        0      459 2022-12-26 17:15:37.000000 morpholib-0.7.1.dev1/src/morpholib/__init__.py
--rw-rw-rw-   0        0        0    10495 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/actions.py
--rw-rw-rw-   0        0        0   172890 2023-05-26 22:47:05.000000 morpholib-0.7.1.dev1/src/morpholib/anim.py
--rw-rw-rw-   0        0        0    28588 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/base.py
--rw-rw-rw-   0        0        0     4241 2023-03-12 21:13:07.000000 morpholib-0.7.1.dev1/src/morpholib/bezier.py
--rw-rw-rw-   0        0        0    29327 2023-03-09 16:23:34.000000 morpholib-0.7.1.dev1/src/morpholib/calculus.py
--rw-rw-rw-   0        0        0    36375 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/color.py
--rw-rw-rw-   0        0        0      512 2022-12-26 17:15:37.000000 morpholib-0.7.1.dev1/src/morpholib/combo.py
--rw-rw-rw-   0        0        0    86385 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/figure.py
--rw-rw-rw-   0        0        0    10763 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/gadgets.py
--rw-rw-rw-   0        0        0     2513 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/giffer.py
--rw-rw-rw-   0        0        0     9517 2023-05-26 22:47:05.000000 morpholib-0.7.1.dev1/src/morpholib/graph.py
--rw-rw-rw-   0        0        0    42139 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/graphics.py
--rw-rw-rw-   0        0        0   193540 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/grid.py
--rw-rw-rw-   0        0        0     6428 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/latex.py
--rw-rw-rw-   0        0        0    13144 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/matrix.py
--rw-rw-rw-   0        0        0      709 2022-08-01 17:17:30.000000 morpholib-0.7.1.dev1/src/morpholib/sample.py
--rw-rw-rw-   0        0        0   113081 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/shapes.py
--rw-rw-rw-   0        0        0    80385 2023-05-26 22:47:05.000000 morpholib-0.7.1.dev1/src/morpholib/text.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.894612 morpholib-0.7.1.dev1/src/morpholib/tools/
--rw-rw-rw-   0        0        0       72 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/__init__.py
--rw-rw-rw-   0        0        0        4 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/base.py
--rw-rw-rw-   0        0        0    11946 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/tools/basics.py
--rw-rw-rw-   0        0        0       31 2022-06-16 19:16:16.000000 morpholib-0.7.1.dev1/src/morpholib/tools/color.py
--rw-rw-rw-   0        0        0    12210 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/tools/dev.py
--rw-rw-rw-   0        0        0     2093 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/ktimer.py
--rw-rw-rw-   0        0        0     6348 2023-04-25 17:14:02.000000 morpholib-0.7.1.dev1/src/morpholib/tools/latex2svg.py
--rw-rw-rw-   0        0        0      811 2022-03-08 00:05:51.000000 morpholib-0.7.1.dev1/src/morpholib/tools/subimporter.py
--rw-rw-rw-   0        0        0     5370 2023-05-26 22:15:27.000000 morpholib-0.7.1.dev1/src/morpholib/transitions.py
--rw-rw-rw-   0        0        0     9128 2022-06-16 19:16:16.000000 morpholib-0.7.1.dev1/src/morpholib/video.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:03:36.863412 morpholib-0.7.1.dev1/src/morpholib.egg-info/
--rw-rw-rw-   0        0        0     4356 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-27 15:03:36.000000 morpholib-0.7.1.dev1/src/morpholib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 19:30:24.586043 morpholib-0.8.0.dev1/
+-rw-rw-rw-   0        0        0     1091 2021-09-29 20:39:14.000000 morpholib-0.8.0.dev1/LICENSE
+-rw-rw-rw-   0        0        0     4356 2023-07-07 19:30:24.588544 morpholib-0.8.0.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     3967 2023-05-27 15:02:41.000000 morpholib-0.8.0.dev1/README.md
+-rw-rw-rw-   0        0        0      110 2021-09-27 17:28:21.000000 morpholib-0.8.0.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0      665 2023-07-07 19:30:24.588544 morpholib-0.8.0.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-07 19:30:24.483542 morpholib-0.8.0.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 19:30:24.546043 morpholib-0.8.0.dev1/src/morpholib/
+-rw-rw-rw-   0        0        0      459 2022-12-26 17:15:37.000000 morpholib-0.8.0.dev1/src/morpholib/__init__.py
+-rw-rw-rw-   0        0        0    10589 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/actions.py
+-rw-rw-rw-   0        0        0   179308 2023-07-06 15:17:38.000000 morpholib-0.8.0.dev1/src/morpholib/anim.py
+-rw-rw-rw-   0        0        0    29333 2023-07-06 15:17:38.000000 morpholib-0.8.0.dev1/src/morpholib/base.py
+-rw-rw-rw-   0        0        0     4241 2023-03-12 21:13:07.000000 morpholib-0.8.0.dev1/src/morpholib/bezier.py
+-rw-rw-rw-   0        0        0    29327 2023-03-09 16:23:34.000000 morpholib-0.8.0.dev1/src/morpholib/calculus.py
+-rw-rw-rw-   0        0        0    36222 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/color.py
+-rw-rw-rw-   0        0        0      512 2022-12-26 17:15:37.000000 morpholib-0.8.0.dev1/src/morpholib/combo.py
+-rw-rw-rw-   0        0        0    90641 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/figure.py
+-rw-rw-rw-   0        0        0    10120 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/gadgets.py
+-rw-rw-rw-   0        0        0     2513 2022-03-08 00:05:51.000000 morpholib-0.8.0.dev1/src/morpholib/giffer.py
+-rw-rw-rw-   0        0        0     9907 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/graph.py
+-rw-rw-rw-   0        0        0    41881 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/graphics.py
+-rw-rw-rw-   0        0        0   191576 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/grid.py
+-rw-rw-rw-   0        0        0     6428 2023-05-27 15:37:00.000000 morpholib-0.8.0.dev1/src/morpholib/latex.py
+-rw-rw-rw-   0        0        0    13144 2023-05-27 15:37:00.000000 morpholib-0.8.0.dev1/src/morpholib/matrix.py
+-rw-rw-rw-   0        0        0      709 2022-08-01 17:17:30.000000 morpholib-0.8.0.dev1/src/morpholib/sample.py
+-rw-rw-rw-   0        0        0   114448 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/shapes.py
+-rw-rw-rw-   0        0        0    78063 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/text.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:30:24.586043 morpholib-0.8.0.dev1/src/morpholib/tools/
+-rw-rw-rw-   0        0        0       72 2022-03-08 00:05:51.000000 morpholib-0.8.0.dev1/src/morpholib/tools/__init__.py
+-rw-rw-rw-   0        0        0        4 2022-03-08 00:05:51.000000 morpholib-0.8.0.dev1/src/morpholib/tools/base.py
+-rw-rw-rw-   0        0        0    12383 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/tools/basics.py
+-rw-rw-rw-   0        0        0       31 2022-06-16 19:16:16.000000 morpholib-0.8.0.dev1/src/morpholib/tools/color.py
+-rw-rw-rw-   0        0        0    18127 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/tools/dev.py
+-rw-rw-rw-   0        0        0     2093 2022-03-08 00:05:51.000000 morpholib-0.8.0.dev1/src/morpholib/tools/ktimer.py
+-rw-rw-rw-   0        0        0     6348 2023-04-25 17:14:02.000000 morpholib-0.8.0.dev1/src/morpholib/tools/latex2svg.py
+-rw-rw-rw-   0        0        0      811 2022-03-08 00:05:51.000000 morpholib-0.8.0.dev1/src/morpholib/tools/subimporter.py
+-rw-rw-rw-   0        0        0     7137 2023-06-26 17:31:05.000000 morpholib-0.8.0.dev1/src/morpholib/transitions.py
+-rw-rw-rw-   0        0        0     9128 2022-06-16 19:16:16.000000 morpholib-0.8.0.dev1/src/morpholib/video.py
+drwxrwxrwx   0        0        0        0 2023-07-07 19:30:24.561043 morpholib-0.8.0.dev1/src/morpholib.egg-info/
+-rw-rw-rw-   0        0        0     4356 2023-07-07 19:30:24.000000 morpholib-0.8.0.dev1/src/morpholib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-07-07 19:30:24.000000 morpholib-0.8.0.dev1/src/morpholib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 19:30:24.000000 morpholib-0.8.0.dev1/src/morpholib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-07 19:30:24.000000 morpholib-0.8.0.dev1/src/morpholib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-07 19:30:24.000000 morpholib-0.8.0.dev1/src/morpholib.egg-info/top_level.txt
```

### Comparing `morpholib-0.7.1.dev1/LICENSE` & `morpholib-0.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/PKG-INFO` & `morpholib-0.8.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpholib
-Version: 0.7.1.dev1
+Version: 0.8.0.dev1
 Summary: A general-purpose programmatic animation tool
 Home-page: https://github.com/morpho-matters/morpholib
 Author: Kenneth Small
 Author-email: morpho.matters@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `morpholib-0.7.1.dev1/README.md` & `morpholib-0.8.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/setup.cfg` & `morpholib-0.8.0.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f72 7068 6f6c 6962 0d0a 7665   = morpholib..ve
-00000020: 7273 696f 6e20 3d20 302e 372e 312e 6465  rsion = 0.7.1.de
+00000020: 7273 696f 6e20 3d20 302e 382e 302e 6465  rsion = 0.8.0.de
 00000030: 7631 0d0a 6175 7468 6f72 203d 204b 656e  v1..author = Ken
 00000040: 6e65 7468 2053 6d61 6c6c 0d0a 6175 7468  neth Small..auth
 00000050: 6f72 5f65 6d61 696c 203d 206d 6f72 7068  or_email = morph
 00000060: 6f2e 6d61 7474 6572 7340 676d 6169 6c2e  o.matters@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2041 2067 656e 6572 616c 2d70 7572   = A general-pur
 00000090: 706f 7365 2070 726f 6772 616d 6d61 7469  pose programmati
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/actions.py` & `morpholib-0.8.0.dev1/src/morpholib/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,17 @@
 # versions of registered actor actions.
 # See "morpho.actions.action" for more info.
 class MultiActionSummoner(object):
     def __getattr__(self, actionName):
         def multiaction(actors, *args, atFrame=None, stagger=0, **kwargs):
             if isinstance(actors, morpho.Actor):
                 actors = [actors]
+            elif isinstance(actors, morpho.Layer):
+                actors = actors.actors
+
             if atFrame is None:
                 atFrame = max(actor.lastID() for actor in actors)
             for n,actor in enumerate(actors):
                 try:
                     action = getattr(actor, actionName)
                 except AttributeError:
                     raise AttributeError(f"'{actor.figureType.__name__}' does not implement action '{actionName}'")
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/anim.py` & `morpholib-0.8.0.dev1/src/morpholib/anim.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 cr = cairo
 
 import morpholib as morpho
 import morpholib.transitions, morpholib.giffer
 from morpholib.tools.basics import *
 from morpholib.tools.ktimer import tic, toc
 import morpholib.tools.dev
-from morpholib.tools.dev import BoundingBoxFigure, makesubcopies, listselect
+from morpholib.tools.dev import BoundingBoxFigure, makesubcopies, listselect, \
+    _SubAttributeManager, _InPlaceSubAttributeManager, AmbiguousValueError
 
 # Backward compatibility because these functions used to live in anim.py
 from morpholib import screenCoords, physicalCoords, \
     pixelWidth, physicalWidth, pixelHeight, physicalHeight, \
     setupContext, clearContext, cairoJointStyle, object_hasattr
 
 import math, cmath
 import numpy as np
 import os, shutil, tempfile, ctypes
 import subprocess as sp
 import pyperclip
 from warnings import warn
 from tempfile import TemporaryDirectory
+from collections.abc import Iterable
 
 # # Get location of the Morpho directory.
 # # pwd = os.sep.join(sys.argv[0].split(os.sep)[:-1])
 # pwd = os.sep.join(os.path.dirname(os.path.abspath(__file__)).split(os.sep)[:-1])
 # if os.sep not in pwd:
 #     pwd = os.curdir
 # # pwd += os.sep
@@ -68,134 +70,146 @@
 
 class LayerMergeError(MergeError):
     pass
 
 class MaskConfigurationError(Exception):
     pass
 
-class AmbiguousValueError(ValueError):
-    pass
-
-### CLASSES ###
 
-# Mainly for internal use.
-# Object created when the `sub` property is used in a Frame object.
-# Allows one to modify the attributes of the subfigures of a frame
-# all at once.
-class _SubAttributeManager(object):
-    # `frame` is the Frame on which `.all` is being called.
-    # `origframe` is the Frame that should be returned by
-    # the set() method. If unspecified, it defaults to the
-    # value of `frame`. This is useful when calling .select[]
-    # since the return value of set() will be the true original
-    # Frame including unselected subfigures.
-    def __init__(self, frame, origframe=None, /):
-        if origframe is None:
-            origframe = frame
-        # Bypass native setattr() because it's overridden below.
-        object.__setattr__(self, "_subattrman_frame", frame)
-        object.__setattr__(self, "_subattrman_origframe", origframe)
-
-    # Returns a function that when called will call the
-    # corresponding method across all subfigures in the
-    # Frame and collect their return values into a list
-    # which will then be returned.
-    def _subattrman_createSubmethod(self, name):
-        def submethod(*args, **kwargs):
-            outputs = []
-            for fig in self._subattrman_frame.figures:
-                outputs.append(getattr(fig, name)(*args, **kwargs))
-            return outputs
-        return submethod
+### CLASS DECORATORS ###
 
-    def __getattr__(self, name):
-        frame = self._subattrman_frame
+# Decorator for Frame tween methods that implements subfigure
+# tweening and splitting automatically for tween methods that
+# ignore the `figures` tweenable.
+def handleSubfigureTweening(tweenmethod):
+    def splitter(t, beg, mid, fin):
+        # First use the original splitter to split the tween method
+        if morpho.tweenSplittable(tweenmethod):
+            tweenmethod.splitter(t, beg, mid, fin)
+
+        # Split subfigure tween methods
+        for subbeg, submid, subfin in zip(beg.figures, mid.figures, fin.figures):
+            # Split the tween methods of corresponding subfigure triplets
+            if morpho.tweenSplittable(subbeg.tweenMethod):
+                subbeg.tweenMethod.splitter(t, subbeg, submid, subfin)
+
+    @morpho.TweenMethod(splitter=splitter)
+    def wrapper(self, other, t, *args, **kwargs):
+        # Apply original tween method and assume it doesn't
+        # affect the `figures` tweenable.
+        twfig = tweenmethod(self, other, t, *args, **kwargs)
+
+        # Tween subfigures
+        twfig_figures = twfig.figures  # Saves on tweenable getattr time
+        for n, (fig1, fig2) in enumerate(zip(self.figures, other.figures)):
+            # Skip any static subfigures
+            if fig1.static: continue
+            twfig_figures[n] = fig1.tweenMethod(fig1, fig2, t)
 
-        # Extract initial value for the attribute (if possible)
-        try:
-            commonValue = getattr(frame.figures[0], name)
-        except AttributeError:
-            raise AttributeError(f"Subfigures do not all possess attribute `{name}`")
-        except IndexError:
-            raise IndexError("Frame has no subfigures.")
-
-        commonValue_is_list_or_tuple = isinstance(commonValue, (list, tuple))
-
-        # Check if the attribute is common to all the
-        # subfigures and having the same value
-        for subfigure in frame.figures:
-            try:
-                value = getattr(subfigure, name)
-            except AttributeError:
-                raise AttributeError(f"Subfigures do not all possess attribute `{name}`")
+        return twfig
+    return wrapper
 
-            if commonValue_is_list_or_tuple and isinstance(value, (list, tuple)):
-                # Convert value to commonValue's type so that cross-container
-                # comparison with commonValue will work
-                value = type(commonValue)(value)
-            # Check if they are unequal
-            if not isequal(value, commonValue):  # isequal() handles np.arrays too
-                if callable(commonValue):
-                    return self._subattrman_createSubmethod(name)
-                raise AmbiguousValueError(f"Subfigures do not have a common value for attribute `{name}`")
-
-        return commonValue if not isinstance(commonValue, (list, np.ndarray)) else commonValue.copy()
-
-    def __setattr__(self, name, value):
-        # Handle ordinary attribute sets if self possesses
-        # the attribute.
-        if object_hasattr(self, name):
-            object.__setattr__(self, name, value)
+### CLASSES ###
 
-        # Set every subfigure attribute
-        frame = self._subattrman_frame
-        for subfigure in frame.figures:
-            setattr(subfigure, name, value)
+# Enables Frame-like figures to apply an action to its subfigures
+# via the syntax
+#   myfilm.subaction.myaction(..., substagger=5)
+# Note that this assumes `myaction` only needs access to the final
+# keyfigure of the actor, and only modifies the actor by appending
+# new keyfigures to the end of its timeline. Actions such as
+# fadeIn/Out() and growIn/shrinkOut(), but not rollback() (since it
+# needs access to the first keyfigure).
+class _SubactionSummoner(object):
+    def __init__(self, actor):
+        self.actor = actor
+
+    # Apply actor actions to subfigures in a Frame-like figure,
+    # along with a substagger option. A subset of subfigures can
+    # be selected by passing in indices/slices into the `select`
+    # keyword parameter.
+    @staticmethod
+    def subaction(action, film, duration=30, atFrame=None, *,
+        substagger=0, select=None, **kwargs):
+        if atFrame is None:
+            atFrame = film.lastID()
+
+        if select is None:
+            select = sel[:]
+        elif isinstance(select, Iterable):
+            select = tuple(select)
+
+        frame0 = film.last()
+        initframe = frame0.copy()
+
+        # Get a dict containing the selected indices
+        selectedIndices = listselect(initframe.figures, select)
+
+        subactors = []
+        for n,fig in enumerate(initframe.figures):
+            fig_orig = fig
+            fig = fig.copy()
+
+            subactor = morpho.Actor(fig)
+            if n in selectedIndices:
+                # Transition is set to uniform because transitions are ignored
+                # in frames and we want Actor.zip() to respect that.
+                fig.transition = morpho.transitions.uniform
+                if initframe.transition != morpho.transitions.uniform:
+                    fig.tweenMethod = morpho.transitions.incorporateTransition(initframe.transition, fig.tweenMethod)
+                # fig.static = False
+                action(subactor, duration=duration, **kwargs)
+                # Restore tween method and transition to original
+                # values for the final keyfigure in the subactor
+                subactor.last().set(
+                    tweenMethod=fig_orig.tweenMethod,
+                    transition=fig_orig.transition
+                    )
+            subactors.append(subactor)
+
+        for count, n in enumerate(selectedIndices):
+            subactors[n].shift(count*substagger)
+
+        if atFrame == film.lastID():
+            film.delkey(atFrame)
+        template = initframe.copy().set(figures=[])
+        zipped = morpho.Actor.zip(subactors, template=template)
+        film.insert(zipped, atFrame=atFrame)
 
-    def set(self, **kwargs):
-        for name, value in kwargs.items():
-            setattr(self, name, value)
-        return self._subattrman_origframe
-
-
-class _MetaArray(np.ndarray):
-    """Array with metadata.
-    Thanks to @Bertrand L on StackOverflow for this!
-    https://stackoverflow.com/a/34967782"""
-
-    def __new__(cls, array, dtype=None, order=None, **kwargs):
-        obj = np.asarray(array, dtype=dtype, order=order).view(cls)
-        obj.metadata = kwargs
-        return obj
-
-    def __array_finalize__(self, obj):
-        if obj is None: return
-        self.metadata = getattr(obj, 'metadata', None)
-
-# Special version of _SubAttributeManager which in the case of an
-# AmbiguousValueError, returns a MetaArray of the values across all
-# subfigures. Mainly used for enabling the .iall and .iselect
-# features for subfigure in-place operations.
-class _InPlaceSubAttributeManager(_SubAttributeManager):
     def __getattr__(self, name):
-        try:
-            return _SubAttributeManager.__getattr__(self, name)
-        except AmbiguousValueError:
-            # A MetaArray is used in order to distinguish these object arrays
-            # from regular numpy object arrays just in case a user is trying
-            # to update a value that is already natively an object array.
-            return _MetaArray([getattr(subfig, name) for subfig in self._subattrman_frame.figures], dtype=object)
+        action = getattr(morpho.action, name)
 
-    def __setattr__(self, name, value):
-        if isinstance(value, _MetaArray):
-            for subfig, subvalue in zip(self._subattrman_frame.figures, value.tolist()):
-                setattr(subfig, name, subvalue)
-        else:
-            _SubAttributeManager.__setattr__(self, name, value)
+        def subaction(*args, substagger=0, **kwargs):
+            return self.subaction(action, self.actor, *args, substagger=substagger, **kwargs)
 
+        return subaction
+
+    # The subaction property can be called by supplying
+    # an actor action and other args/kwargs. This allows
+    # one to use an unregistered action with `subaction`.
+    def __call__(self, action, *args, **kwargs):
+        return self.subaction(action, self.actor, *args, **kwargs)
+
+# Enables MultiFigures to apply an action to its subfigures
+# via the syntax
+#   myfilm.subaction.myaction(..., substagger=5)
+# Note that if substagger or select is used, the MultiFigure
+# will have its toplevel tween method set to Frame.tweenLinear
+# for the duration of the action.
+class _SubactionSummonerForMultiFigures(_SubactionSummoner):
+    @staticmethod
+    def subaction(action, film, *args, substagger=0, select=None, **kwargs):
+        if substagger == 0 and select is None:
+            _SubactionSummoner.subaction(action, film, *args,
+                substagger=0, select=select, **kwargs)
+        else:
+            origTweenMethod = film.last().tweenMethod
+            film.last().tweenMethod = Frame.tweenLinear
+            _SubactionSummoner.subaction(action, film, *args,
+                substagger=substagger, select=select, **kwargs)
+            film.last().tweenMethod = origTweenMethod
 
 # Frame class. Groups figures together for simultaneous drawing.
 # Syntax: myframe = Frame(list_of_figures, **kwargs)
 #
 # Note that arbitrary keyword arguments can be supplied to the
 # Frame constructor, in which case they will be interpreted as
 # name-subfigure pairs and will be appended to the end of the
@@ -233,15 +247,15 @@
     def __init__(self, figures=None, /, **kwargs):
         # By default, do what the superclass does.
         # morpho.Figure.__init__(self)
         super().__init__()
 
         if figures is None:
             figures = []
-        elif isinstance(figures, tuple):
+        elif not isinstance(figures, list):
             figures = list(figures)
         figures.extend(kwargs.values())
 
         self.Tweenable("figures", figures, tags=["figures", "notween"])
         self.Tweenable("origin", 0, tags=["complex", "nofimage"])
         # background = morpho.Tweenable(
         #     name="background", tags=["vector"], value=[0,0,0])
@@ -271,14 +285,24 @@
 
         # # Other (non-tweenable) attributes
         # self.delay = 0  # number of frames to delay at keyframe
 
         # self.defaultTween = Frame.tweenLinear
 
     @property
+    def figures(self):
+        return self._state["figures"].value
+
+    @figures.setter
+    def figures(self, value):
+        if not isinstance(value, list):
+            value = list(value)
+        self._state["figures"].value = value
+
+    @property
     def numfigs(self):
         return len(self.figures)
 
     # Modified because checking if the two figure lists are
     # equal via vanilla Python list equality will not work.
     # Instead, it goes thru the figure lists of self and other
     # and checks if all corresponding figures appear equal.
@@ -295,14 +319,20 @@
     # # Returns True iff the "stylistic" attributes of two frames match
     # # i.e. their views, indices, and defaultTweens match.
     # # This can be used as a criterion on whether or not merging two frames
     # # can be done without affecting the other frame.
     # def matchesStyle(self, other):
     #     return self.defaultTween==other.defaultTween
 
+    # Allows actor actions to be applied to subfigures with a
+    # substagger parameter.
+    @staticmethod
+    def subaction(actor):
+        return _SubactionSummoner(actor)
+
     # Append the figure list of other to self in place.
     # Also adds in the named subfigures of other into self's registry,
     # but skips any duplicate names so that self's names are
     # not overwritten.
     def merge(self, other):
         # if not self._names.keys().isdisjoint(other._names.keys()):
         #     raise MergeError("Frame to merge shares names with self.")
@@ -321,32 +351,49 @@
 
         # Extend the figure list
         self.figures.extend(other.figures)
         return self
 
     @property
     def all(self):
-        return _SubAttributeManager(self)
+        return _SubAttributeManager(self.figures, self)
 
     # Version of .all that is only meant to be used for in-place
     # operations like `+=`.
     # Example: myframe.iall[:3].pos += 2j
     @property
     def iall(self):
-        return _InPlaceSubAttributeManager(self)
+        return _InPlaceSubAttributeManager(self.figures, self)
 
     def _select(self, index, *, _asFrame=False, _iall=False):
-        selection = list(listselect(self.figures, index).values())
+        seldict = listselect(self.figures, index)
+        selection = list(seldict.values())
 
-        frm = type(self)(selection)
-        frm._updateFrom(self, ignore="figures")
+        # Do an empty initialization first followed by assigning
+        # to `figures` so that `select[]` does not assume anything
+        # about how type(self).__init__() works.
+        frm = type(self)()
+        frm.figures = selection
+        frm._updateFrom(self, ignore={"figures", "_names"})
         if _asFrame:
+            # If self has named subfigures, ensure the names transfer over
+            # to the returned subframe.
+            if len(self._names) > 0:
+                # Dict mapping selected indices in self to indices in the subframe.
+                # Eliminates the need to use list.index() which is slow.
+                subIDpositions = {subID : n for n, subID in enumerate(seldict.keys())}
+
+                # Go thru self's names dict and map names for subfigures
+                # that self has in common with the subframe
+                for name, subID in self._names.items():
+                    if subID in seldict:
+                        frm._names[name] = subIDpositions[subID]
             return frm
         else:
-            return _InPlaceSubAttributeManager(frm, self) if _iall else _SubAttributeManager(frm, self)
+            return _InPlaceSubAttributeManager(frm.figures, self) if _iall else _SubAttributeManager(frm.figures, self)
 
     def _iselect(self, *args, **kwargs):
         return self._select(*args, _iall=True, **kwargs)
 
     # Allows the modification of a subset of the subfigures
     # with the syntax:
     #   myframe.select[1:4].set(...)
@@ -361,15 +408,14 @@
     # Version of .select[] that is only meant to be used for in-place
     # operations like `+=`.
     # Example: myframe.iselect[:3].pos += 2j
     @property
     def iselect(self):
         return morpho.tools.dev.Slicer(getter=self._iselect)
 
-
     def _sub(self, index):
         return self._select(index, _asFrame=True).copy()
 
     # Extracts a subframe of subfigures from the Frame.
     # Subfigures can be selected either via slice notation
     #   subframe = myframe.sub[1:4]
     # Or by choice function:
@@ -386,14 +432,19 @@
         # in this case.
         subframe = self._select(index, _asFrame=True)
         figures = list(self.figures)
         for subfig in subframe.figures:
             while subfig in figures:
                 figures.remove(subfig)
         self.figures = figures
+
+        # Remove cut subfigure names from self's names dict
+        for name in subframe._names:
+            del self._names[name]
+
         return subframe
 
     # Basically the same as sub[], but it also removes the selected
     # subfigures from self's figure list. The selected subfiures
     # are NOT copied since they are removed from self's figure list.
     @property
     def cut(self):
@@ -409,17 +460,19 @@
     # in that order.
     #
     # Note that partition() will leave the original Frame figure
     # that called it unchanged, and will return a new Frame
     # of copies of the underlying subfigures per chunk.
     #
     # Subfigure names currently do not transfer.
-    def partition(self, indices):
+    def partition(self, *indices):
         if len(indices) == 0:
             return Frame([self.sub[:]])
+        if len(indices) == 1 and isinstance(indices[0], Iterable):
+            indices = indices[0]
 
         # Divide any negative indices mod len(self.figures)
         # so they will be in the correct order relative to
         # positive indices.
         for n, index in enumerate(indices):
             if index < 0:
                 indices[n] = index % len(self.figures)
@@ -462,24 +515,24 @@
     # frm.poly.fill = [1,1,0]
     #
     # When the Frame is turned into an actor, it enables subfigure
     # manipulation after creating new keyfigures:
     # frm.newendkey(30)
     # frm.last().pt.pos = 3+3j
     def setName(self, **kwargs):
-        for name, figure in kwargs.items():
-            if isinstance(figure, morpho.Figure):
+        for name, index in kwargs.items():
+            if isinstance(index, morpho.Figure):
                 try:
-                    figure = self.figures.index(figure)
+                    index = self.figures.index(index)
                 except ValueError:
                     raise ValueError("Given figure is not in the Frame's figure list.")
-            elif not isinstance(figure, int):
-                raise TypeError(f"`figure` must be Figure or int, not `{type(figure).__name__}`")
+            elif not isinstance(index, int):
+                raise TypeError(f"Value associated with name must be Figure or int, not `{type(index).__name__}`")
 
-            self._names[name] = figure
+            self._names[name] = index
 
     # Returns the subfigure of the given name.
     def getName(self, name):
         return self.figures[self._names[name]]
 
     def __getattr__(self, name):
         # First try using the superclass's built-in getattr()
@@ -560,16 +613,17 @@
         # Copy the tweenables, default tween method and transition.
         # new = morpho.Figure.copy(self)
         new = super().copy()
         # new = super().copy()
 
         # Make copies of all the underlying figures.
         if deep:
-            for i in range(len(new.figures)):
-                new.figures[i] = new.figures[i].copy()
+            new_figures = new.figures  # Saves on tweenable getattr time loss
+            for i, fig in enumerate(new_figures):
+                new_figures[i] = fig.copy()
         return new
 
     # Perform an fimage on all non-static figures that possess
     # a method with the name "fimage".
     # Returns a new frame object that is the result.
     def fimage(self, func):
         S = self
@@ -577,79 +631,113 @@
         fS = S.copy()
         for i in range(len(fS.figures)):
             fig = fS.figures[i]
             if not fig.static:
                 fS.figures[i] = fig.fimage(func)
         return fS
 
-    # Use the default tween method and transition to tween the frame.
-    # Also auto-tweens all of the figures in the figure list.
-    # Frame transition should only affect frame-specific tweenables.
-    # It should not transfer down to the figures it contains.
-    # Also note that tween() assumes the figure lists between
-    # self and other are compatible i.e. of the same lengths AND
-    # item-by-item having the same figure types. Trying to tween
-    # figures of different types may result in a crash or
-    # unpredictable behavior. So if you have two keyframes in an
-    # animation that are one after the other in the same layer,
-    # you should set the first keyframe to be static so that it
-    # doesn't tween.
-    def tween(self, other, t):
-        frm = self.defaultTween(self, other, self.transition(t))
-
-        # Now do stuff with the figures tweenable
-        # Tween each figure according to its default tween method.
-        for i in range(len(self.figures)):
-            fig = self.figures[i]
-            # Don't tween if the figure is static
-            if fig.static: continue
-
-            pig = other.figures[i]
-            twig = fig.tween(pig, t)
-            frm.figures[i] = twig
-        return frm
+    ### TWEEN METHODS ###
+
+    tweenLinear = handleSubfigureTweening(morpho.Figure.tweenLinear)
+    tweenSpiral = handleSubfigureTweening(morpho.Figure.tweenSpiral)
+
+    @classmethod
+    def tweenPivot(cls, angle=tau/2):
+        pivot = morpho.Figure.tweenPivot(angle)
+        # Enable splitting
+        pivot = morpho.pivotTweenMethod(cls.tweenPivot, angle)(pivot)
+        pivot = handleSubfigureTweening(pivot)
+
+        return pivot
 
 # Blank frame used by the Animation class.
 blankFrame = Frame()
 blankFrame.static = True
 
+# Special fadeIn() for Frame-like actors supports a `substagger`
+# parameter that applies a staggered fade in to the subfigures.
+#
+# Note: For substagger to work, the tween method of the latest
+# keyfigure must delegate subfigure tweening to the subfigures'
+# individual tween methods. This condition is always satisfied
+# if using one of the built-in tween methods, but if using a
+# custom one, make sure to decorate it with
+# @handleSubfigureTweening.
 @Frame.action
-def fadeIn(frame, duration=30, atFrame=None, jump=0, alpha=1):
+def fadeIn(film, duration=30, atFrame=None, jump=0, alpha=1, *, substagger=0):
+    lasttime = film.lastID()
     if atFrame is None:
-        atFrame = frame.lastID()
+        atFrame = lasttime
 
-    frame0 = frame.last()
-    frame0.visible = False
-    frame1 = frame.newkey(atFrame)
-    frame1.visible = True
-    frame2 = frame.newendkey(duration)
-
-    for n,fig in enumerate(frame1.figures):
-        fig.static = False
-        actor = morpho.Actor(fig)
-        actor.fadeIn(duration=duration, jump=jump, alpha=alpha)
-        frame1.figures[n] = actor.first()
-        frame2.figures[n] = actor.last()
+    frame0 = film.last()
+    frame0.visible = True
+    finalframe = frame0.copy()
+    frame0.all.static = False
+
+    if substagger == 0:
+        # Do traditional fade in action. The traditional way exists
+        # since using the subaction feature on MultiFigures incurs
+        # some drawbacks that I would like to not have to deal with
+        # if substagger is 0.
+        frame1 = film.newkey(atFrame)
+        frame1.visible = True
+        frame2 = film.newendkey(duration)
+
+        for n,fig in enumerate(frame1.figures):
+            # fig.static = False
+            actor = morpho.Actor(fig)
+            actor.fadeIn(duration=duration, jump=jump)
+            frame1.figures[n] = actor.first()
+            frame2.figures[n] = actor.last()
+    else:
+        film.subaction.fadeIn(duration, atFrame, jump=jump, alpha=alpha, substagger=substagger)
+
+    # Hide lingering initial keyfigure if it exists.
+    if atFrame > lasttime:
+        frame0.visible = False
+
+    # Ensure final frame really is the original final frame,
+    # but with adjusted alpha
+    film.fin = finalframe
+    film.fin.all.alpha = alpha
 
 @Frame.action
-def fadeOut(frame, duration=30, atFrame=None, jump=0):
-    if atFrame is None:
-        atFrame = frame.lastID()
-
-    frame0 = frame.last()
-    frame1 = frame.newkey(atFrame)
-    frame2 = frame.newendkey(duration)
-    frame2.visible = False
-
-    for n,fig in enumerate(frame1.figures):
-        fig.static = False
-        actor = morpho.Actor(fig)
-        actor.fadeOut(duration=duration, jump=jump)
-        frame1.figures[n] = actor.first()
-        frame2.figures[n] = actor.last()
+def fadeOut(film, duration=30, atFrame=None, jump=0, *, substagger=0):
+    # Record of who was static so we can restore this later
+    staticRecord = [fig.static for fig in film.last().figures]
+    film.last().all.static = False
+    if substagger == 0:
+        # Do traditional fade out action. The traditional way exists
+        # since using the subaction feature on MultiFigures incurs
+        # some drawbacks that I would like to not have to deal with
+        # if substagger is 0.
+        if atFrame is None:
+            atFrame = film.lastID()
+
+        frame0 = film.last()
+        frame1 = film.newkey(atFrame)
+        frame2 = film.newendkey(duration)
+        frame2.visible = False
+
+        for n,fig in enumerate(frame1.figures):
+            # fig.static = False
+            actor = morpho.Actor(fig)
+            actor.fadeOut(duration=duration, jump=jump)
+            frame1.figures[n] = actor.first()
+            frame2.figures[n] = actor.last()
+    else:
+        film.subaction.fadeOut(duration, atFrame, jump=jump, substagger=substagger)
+
+    film.last().visible = False
+
+    # Restore static attribute for subfigures that were originally
+    # static. This is helpful in case the user wants to use the
+    # Frame again after fade out is complete.
+    for fig, static in zip(film.last().figures, staticRecord):
+        fig.static = static
 
 @Frame.action
 def rollback(frame, duration=30, atFrame=None):
     if atFrame is None:
         atFrame = frame.lastID()
 
     frame1 = frame.newkey(atFrame)
@@ -711,14 +799,20 @@
         if isinstance(value, slice):
             value = range(self.numfigs)[value]
         self._subpool = value if type(value) is set else set(value)
 
     def _appearsEqual(self, other, *args, compareSubNonTweenables=True, **kwargs):
         return morpho.Frame._appearsEqual(self, other, *args, compareSubNonTweenables=compareSubNonTweenables, **kwargs)
 
+    # Allows actor actions to be applied to subfigures with a
+    # substagger parameter.
+    @staticmethod
+    def subaction(actor):
+        return _SubactionSummonerForMultiFigures(actor)
+
     # # NOT IMPLEMENTED!!!
     # # Returns a StateStruct encapsulating all the tweenables
     # # of all the figures in the MultiFigure.
     # # Main example use case:
     # # my_multifig.all().alpha = 0 changes all the subfigures'
     # # alpha attribute to 0.
     # # By default, the tweenables encapsulated are all the
@@ -733,14 +827,21 @@
     #     if tweenableNames is None:
     #         tweenableNames = list(self.figures[0]._state)
     #     if figures is None:
     #         figures = self.figures
 
     #     return StateStruct(tweenableNames, figures)
 
+    # Computes the bounding box of the entire MultiFigure,
+    # assuming all of its subfigures have implemented `box()`.
+    # Returned as [xmin, xmax, ymin, ymax].
+    # Additional arguments are passed to the box() methods
+    # of subfigures.
+    def box(self, *args, **kwargs):
+        return shiftBox(totalBox(subfig.box(*args, **kwargs) for subfig in self.figures), self.origin)
 
     # If attempted to access a non-existent attribute,
     # check if it's an attribute of the first figure in
     # the figure list and return that instead.
     def __getattr__(self, name):
         # First try using the superclass's built-in getattr()
         # which should grab any valid attribute returns in the
@@ -765,15 +866,15 @@
             # in the protected clause above. However, this time
             # I WANT the error to be thrown!
             # return super().__getattr__(name)
             return morpho.Frame.__getattr__(self, name)
 
         # Try to find the attribute in the first member figure
         # and if found, return it.
-        fig = self.figures[0]
+        # fig = self.figures[0]
         try:
             # return fig.__getattribute__(name)
             # return getattr(fig, name)
             return getattr(self.all, name)
         # This attribute is nowhere to be found anywhere. So give up.
         except AttributeError:
             # raise AttributeError("First member figure of type '"+type(fig)+"'' does not have attribute '"+name+"'")
@@ -813,15 +914,23 @@
             try:
                 # Get first component figure (if possible)
                 fig = self.figures[0]
 
                 # See if it already exists as an attribute
                 # of the first member figure.
                 # fig.__getattribute__(name)
-                getattr(fig, name)
+                try:
+                    getattr(fig, name)
+                except AmbiguousValueError:
+                    # Ignore AmbiguousValueError since it just
+                    # means the getattr() failed because of conflicting
+                    # values, but that's okay, because all we
+                    # are using getattr() for is to loosely check for
+                    # attribute existence!
+                    pass
 
                 # If you got here, we didn't get an attribute error,
                 # so it should be a real attribute! Go ahead and set it!
                 self.all.__setattr__(name, value)
                 # fig.__setattr__(name, value)
 
             # Got an attribute error, so the given attribute isn't
@@ -860,17 +969,17 @@
     #              modified. This method will be applied to the
     #              subfigures during a tween.
     # mainMethod = The corresponding method in the MultiFigure subclass.
     #              e.g. MultiFigure.tweenLinear. This method handles
     #              tweening all the "main" tweenables of the multifigure
     #              object itself (as opposed to subfigures), but it
     #              should NOT act on the `figures` tweenable!
-    #              Defaults to Frame.tweenLinear.
+    #              Defaults to Figure.tweenLinear.
     @staticmethod
-    def Multi(baseMethod, mainMethod=Frame.tweenLinear):
+    def Multi(baseMethod, mainMethod=morpho.Figure.tweenLinear):
 
         def wrapper(self, other, t, *args, **kwargs):
             # wrapper function for a MultiFigure tween method
 
             # Temporarily extend the figure list of self or other
             # so that both have exactly the same number of subfigures.
             len_self_figures = len(self.figures)
@@ -988,21 +1097,34 @@
     def _applyToSubfigures(basemethod):
         def modifiedMethod(self, *args, **kwargs):
             for fig in self.figures:
                 basemethod(fig, *args, **kwargs)
             return self
         return modifiedMethod
 
-
-    # This is needed because inherited tween() is Frame.tween()
-    # which is a modified version of default Figure.tween()
-    tween = morpho.Figure.tween
-
 Multifigure = MultiFigure
 
+@MultiFigure.action
+def fadeIn(actor, duration=30, atFrame=None, jump=0, alpha=1, *, substagger=0, **kwargs):
+    actor.last().visible = True
+    finalkey = actor.last().copy()
+    if substagger != 0:
+        actor.last().tweenMethod = Frame.tweenLinear
+    Frame.actions["fadeIn"](actor, duration, atFrame, jump, alpha, substagger=substagger, **kwargs)
+    actor.fin = finalkey
+    actor.fin.all.alpha = alpha
+
+@MultiFigure.action
+def fadeOut(actor, *args, substagger=0, **kwargs):
+    origTweenMethod = actor.last().tweenMethod
+    if substagger != 0:
+        actor.last().tweenMethod = Frame.tweenLinear
+    Frame.actions["fadeOut"](actor, *args, substagger=substagger, **kwargs)
+    actor.last().tweenMethod = origTweenMethod
+
 
 # Class encapsulates all the tweenables of a list of figures of common
 # type so that you can easily modify a single tweenable across all the
 # figures in a single line of code.
 # Mainly for internal use in the MultiFigure class and its derivatives.
 class StateStruct(object):
     def __init__(self, tweenableNames, figures):
@@ -1078,21 +1200,26 @@
 # the default primitives() method of SpaceFrame assumes each figure
 # it contains supports its own primitives() method.
 # If you want to include figures that lack a primitives()
 # method, you should just use an ordinary Frame instead.
 # However, most space figures support primitives(), so you probably
 # don't need to worry about this.
 class SpaceFrame(Frame):
-    def __init__(self, figures=None):
+    def __init__(self, figures=None, /, **kwargs):
         if isinstance(figures, Frame):
             # super().__init__(figures.figures)
             super().__init__()
             self._updateFrom(figures, common=True)
+            if not isinstance(self.figures, list):
+                self.figures = list(self.figures)
+
+            self.figures.extend(kwargs.values())
+            self.setName(**kwargs)
         else:
-            super().__init__(figures)
+            super().__init__(figures, **kwargs)
 
     # Space version of Frame.partition().
     def partition(self, *args, **kwargs):
         return SpaceFrame(Frame.partition(self, *args, **kwargs))
 
     # Only for frames consisting only of space figures
     # (i.e. figures possessing a primitives() method and a 5 input
@@ -1106,14 +1233,17 @@
             if fig.visible:
                 primlist.extend(fig.primitives(camera))
 
         return primlist
 
 # 3D version of the MultiFigure class. See "MultiFigure" for more info.
 class SpaceMultiFigure(SpaceFrame):
+    # Use MultiFigure's actions instead of SpaceFrame's
+    actions = MultiFigure.actions.copy()
+
     def __getattr__(self, name):
         return MultiFigure.__getattr__(self, name)
 
 SpaceMultifigure = Spacemultifigure = SpaceMultiFigure
 
 
 # Generates frame objects according to a time parameter.
@@ -1378,14 +1508,19 @@
     def width(self):
         return self.boxWidth()
 
     # Returns height of the viewbox: view[3] - view[2]
     def height(self):
         return self.boxHeight()
 
+    # Returns the dimensions of the viewbox as a tuple
+    # (width, height)
+    def dimensions(self):
+        return (self.width(), self.height())
+
     # Given a complex number "pos" representing a position, this method returns
     # a new complex number corresponding to this position had the camera's
     # view been the unit square [0,1] x [0,1].
     # In other words, returns the RELATIVE coordinates of a position with
     # respect to the this camera's viewbox.
     #
     # Usually used in conjunction with physicalCoords()
@@ -1421,17 +1556,26 @@
         y = Y*height + c
 
         return x + 1j*y
 
     # Converts position coordinates from one camera system to another.
     # Given complex position `pos`, this method returns the
     # corresponding complex position in the camera system of `other`.
+    # See also: convertCoordsFrom()
     def convertCoords(self, other, pos):
         return other.physicalCoords(self.normalizedCoords(pos))
 
+    # Converts position coordinates from one camera system to another.
+    # Given complex position `pos` in `other`'s coordinate system,
+    # this method returns the corresponding complex position in the
+    # self's camera system.
+    # Identical to convertCoords(), but self and `other` are swapped.
+    def convertCoordsFrom(self, other, pos):
+        return self.physicalCoords(other.normalizedCoords(pos))
+
     # Given a physical width, returns the corresponding width in the
     # normalized coordinate system.
     # See normalizeCoords() for more info.
     def normalizedWidth(self, width):
         a,b,c,d = self.view
         return width / (b-a)
 
@@ -1551,27 +1695,25 @@
 
     # Generates a modified version of the tweenZoom() tween method
     # that multiplies the zoom amount by the given multiplier function.
     # Syntax:
     #   mycamera.tweenMethod = mycamera.tweenZoomWithMultiplier(multfunc)
     @classmethod
     def tweenZoomWithMultiplier(cls, multiplierFunc):
-        def splitter(tmid):
+        def splitter(tmid, beg, mid, fin):
             one_minus_tmid = 1 - tmid
             M_tmid = multiplierFunc(tmid)
             def mult1(t):
                 return multiplierFunc(tmid*t) / M_tmid**t
 
             def mult2(t):
                 return multiplierFunc(tmid + one_minus_tmid*t)/M_tmid**(1-t)
 
-            multzoom1 = cls.tweenZoomWithMultiplier(mult1)
-            multzoom2 = cls.tweenZoomWithMultiplier(mult2)
-
-            return (multzoom1, multzoom2)
+            beg.tweenMethod = cls.tweenZoomWithMultiplier(mult1)
+            mid.tweenMethod = cls.tweenZoomWithMultiplier(mult2)
 
         @morpho.TweenMethod(splitter=splitter)
         def multzoom(self, other, t):
             return self.tweenZoom(other, t).zoomOut(multiplierFunc(t))
         return multzoom
 
     # Generates a modified version of the tweenZoom() tween method
@@ -2880,14 +3022,18 @@
     def delays(self):
         return self._delays
 
     @delays.setter
     def delays(self, value):
         self._delays = IntDict(value)
 
+    @property
+    def aspectRatioWH(self):
+        WIDTH, HEIGHT = self.windowShape
+        return WIDTH/HEIGHT
 
 
     # Returns a (deep-ish) copy of the animation.
     # If deep=False, then the animation will not make copies of the
     # underlying figures in the layers.
     # Note that copy will not copy over the window attribute, so you will
     # have to manually associate the window to the copied animation.
@@ -3449,19 +3595,22 @@
     # NOT IMPLEMENTED!
     # Moves the firstIndex to the previous key index.
     def prevkey(self):
         raise NotImplementedError
 
     # Convenience function makes the animation delay for the
     # given number of frames at whichever index is currently
-    # its lastID. Defaults to infinity.
-    # Optionally specify a timeOffset. Positive means after lastID,
-    # negative means before lastID.
-    def wait(self, f=oo, timeOffset=0):
-        end = self.lastID() + timeOffset
+    # its lastID. This can be overridden to any index by passing
+    # in the frame index into the optional keyword `atFrame`.
+    # By default, the delay duration is infinite.
+    # Optionally specify a timeOffset as well.
+    def wait(self, f=oo, timeOffset=0, *, atFrame=None):
+        if atFrame is None:
+            atFrame = self.lastID()
+        end = atFrame + timeOffset
         if end == -oo:
             raise IndexError("End of animation is undefined.")
         self.delays[end] = f
 
     @property
     def endDelay(self):
         return self.wait
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/base.py` & `morpholib-0.8.0.dev1/src/morpholib/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Ignore warnings by default.
 # This is mainly for the sake of the Spline class, which
 # uses some non-standard arithmetic intentionally.
 # filterwarnings("ignore")
 
 
-version = "0.7.1.dev1"  # Current public morpho version
+version = "0.8.0.dev1"  # Current public morpho version
 internalVersion = "2.4.1ip"  # Current internal morpho version
 subversion = ""
 DEBUG_MODE = False
 
 
 ### CLASSES ###
 
@@ -398,17 +398,26 @@
 # def my_tween_method(self, other, t)
 #
 # It automatically enforces the rule
 # that t=0 returns self.copy() and t=1 returns other.copy()
 #
 # Optionally, a splitter function can be assigned to the tween method
 # which enables the tween method to be split into two submethods at
-# a given t-value. It's a function that takes a t-value as input
-# and returns a tuple of two tween methods. Splitters are used to
-# create a new keyfigure seamlessly between two existing keyfigures.
+# a given t-value. Splitters are used to create a new keyfigure
+# seamlessly between two existing keyfigures. It's a function that
+# takes as input a t-value and three figures `beg`, `mid`, and `fin`
+# representing the three keyfigures involved in a split. The function
+# should then reassign new tween methods to those keyfigures (usually
+# just `beg` and `mid`) as well as perform any other needed
+# modifications to those keyfigures to make a seamless split.
+# The splitter function can alternatively be assigned afterward with
+# the @newSplitter decorator:
+#   @myNewTweenMethod.newSplitter
+#   def splitter(t):
+#       ...
 def tweenMethod(tween=None, *, splitter=None):
     # If no tween method to decorate, assume we're trying to
     # modify the default behavior of tweenMethod(), so return
     # the modified decorator.
     if tween is None:
         def decorator(tween):
             return tweenMethod(tween, splitter=splitter)
@@ -429,25 +438,34 @@
         elif t == 1:
             return other.copy()
         else:
             twfig = tween(self, other, t, *args, **kwargs)
             # twfig.visible = self.visible  # Inherits visibility of self
             return twfig
 
-    wrapper.splitter = splitter
+    # The unwrapped version of the given tween method.
+    wrapper.interpolator = tween
+
+    # Decorator that assigns the given function as the splitter
+    # of this tween method.
+    def newSplitter(splitter):
+        wrapper.splitter = splitter
+        return splitter
+    wrapper.newSplitter = newSplitter
+    wrapper.newSplitter(splitter)
+
     return wrapper
 
 TweenMethod = tweenMethod  # Initial letter can optionally be uppercase.
 
 # Returns boolean on whether the given tween method has
 # a splitter defined. It is equivalent to
 # hasattr(tweenMethod, "splitter") and tweenMethod.splitter is not None
 def tweenSplittable(tweenMethod):
-    return (hasattr(tweenMethod, "splitter") and \
-            tweenMethod.splitter is not None)
+    return (hasattr(tweenMethod, "splitter") and tweenMethod.splitter is not None)
 
 # Converts complex coordinates into screen pixel coordinates
 # according to the screen dimensions and the shape of the cairo
 # context target surface.
 # Instead of supplying a cairo context, ctx can optionally be a list/tuple
 # indicating the window dimensions in pixels (width, height)
 def screenCoords(z, view, ctx):
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/bezier.py` & `morpholib-0.8.0.dev1/src/morpholib/bezier.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/calculus.py` & `morpholib-0.8.0.dev1/src/morpholib/calculus.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/color.py` & `morpholib-0.8.0.dev1/src/morpholib/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,21 +155,17 @@
 # colormap should be used for programming purposes.
 colors = ["red", "green", "blue", "yellow", "cyan", "magenta",
     "orange", "violet", "brown", "white", "black"]
 
 # Transparently overlays the color A over the color B
 # using transparency alpha (default=0.5)
 def alphaOverlay(A, B, alpha=0.5):
-    if type(A) is list or type(A) is tuple:
-        result = [0,0,0]
-        for i in range(len(A)):
-            result[i] = alphaOverlay(A[i], B[i], alpha)
-        return tuple(result)
-    else:
-        return A*alpha + B*(1-alpha)
+    A = np.array(A)
+    B = np.array(B)
+    return (A*alpha + B*(1-alpha)).tolist()
 
 # Tweens two RGB colors represented by triples and returns
 # a new list with the tweened value.
 def colorTween(rgb1, rgb2, t, start=0, end=1):
     if rgb1 == rgb2: return rgb1
 
     R1, G1, B1 = rgb1
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/combo.py` & `morpholib-0.8.0.dev1/src/morpholib/combo.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/figure.py` & `morpholib-0.8.0.dev1/src/morpholib/figure.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 This can be done by avoiding names that are nothing but
 lowercase letters since convention has it that package
 names are all lowercase letters.
 '''
 
 
 import morpholib as morpho
-from morpholib.tools.basics import *
 import morpholib.matrix
 import morpholib.actions
+import morpholib.transitions
+from morpholib.tools.basics import *
 
 import math, cmath
 import numpy as np
 
 # Alias for `set` because the name gets overridden
 # in the Figure class
 pyset = set
@@ -553,15 +554,16 @@
 
                     # elif isinstance(a, function) or "function" in tweenable.tags:
                     elif callable(a) or "function" in tweenable.tags:
                         if a == b:
                             tw = a
                         else:
                             # Homotopy tween!!
-                            tw = lambda x, t=t: (1-t)*a(x) + t*b(x)
+                            def tw(*args, _tween_funcA=a, _tween_funcB=b, _tween_t=t, **kwargs):
+                                return (1-_tween_t)*_tween_funcA(*args, **kwargs) + _tween_t*_tween_funcB(*args, **kwargs)
 
                     else:
                         # Assume basic numeric type
                         tw = morpho.numTween(a, b, t)
                         if "integer" in tweenable.tags:
                             tw = round(tw)
                     newB[i] = tw
@@ -628,15 +630,16 @@
             # Data type is callable
             # elif isinstance(A, function) or "function" in tweenable.tags:
             elif callable(A) or "function" in tweenable.tags:
                 if A == B:
                     tw = A
                 else:
                     # Homotopy tween!!
-                    tw = lambda x, A=A, B=B, t=t: (1-t)*A(x) + t*B(x)
+                    def tw(*args, _tween_funcA=A, _tween_funcB=B, _tween_t=t, **kwargs):
+                        return (1-_tween_t)*_tween_funcA(*args, **kwargs) + _tween_t*_tween_funcB(*args, **kwargs)
 
             # All other types (assume it's a python numeric type)
             else:
                 tw = morpho.numTween(A,B,t)
                 if "integer" in tweenable.tags:
                     tw = round(tw)
 
@@ -1171,27 +1174,25 @@
 # passed to the methodGenerator as part of the splitter function.
 def pivotTweenMethod(methodGenerator, angle, *args, **kwargs):
     # This decorator will be returned and should be used to
     # decorate a custom angle-specific pivot tween method.
     def decorator(pivotTween):
         # This is the splitter function that will be attached
         # to the provided angle-specific pivot tween method.
-        def pivotSplitter(t):
+        def pivotSplitter(t, beg, mid, fin):
             # Split the angles
             angle1 = t*angle
             angle2 = (1-t)*angle
 
             # Generate the corresponding angle-specific
             # pivot tween methods specific to the provided
             # bound pivot tween method generator.
-            tween1 = methodGenerator(angle1, *args, **kwargs)
-            tween2 = methodGenerator(angle2, *args, **kwargs)
-
-            return (tween1, tween2)
-        pivotTween.splitter = pivotSplitter
+            beg.tweenMethod = methodGenerator(angle1, *args, **kwargs)
+            mid.tweenMethod = methodGenerator(angle2, *args, **kwargs)
+        pivotTween = morpho.TweenMethod(pivotTween, splitter=pivotSplitter)
         return pivotTween
     return decorator
 
 
 # A higher-level structure that collects figures of a common type and
 # places them into a timeline.
 #
@@ -1413,14 +1414,26 @@
     def timeof(self, keyfig):
         try:
             IDno = list(self.timeline.values()).index(keyfig)
             return list(self.timeline.keys())[IDno]
         except ValueError:
             raise ValueError("Given keyfigure is not in the timeline.")
 
+    # Splits tween method and transition to make inserting a new
+    # intermediate keyfigure seamless.
+    @staticmethod
+    def _splitTweenAndTransition(t, beg, mid, fin):
+        # Split the tween method
+        if morpho.tweenSplittable(beg.tweenMethod):
+            beg.tweenMethod.splitter(beg.transition(t), beg, mid, fin)
+        # Split the transition function
+        func1, func2 = morpho.transitions.split(beg.transition, t)
+        beg.transition = func1
+        mid.transition = func2
+
     # Creates a new keyfigure at index f and returns it.
     # If f is ahead of the last keyframe, the new keyfigure
     # will be a copy of the latest keyfigure. If f is before
     # the first keyfigure (or the timeline is empty), the
     # new keyfigure will be the default figure for the actor's
     # figure type. If f is between the first and last
     # keyframes, the new keyfigure will be determined by
@@ -1435,61 +1448,46 @@
     # two neighboring keyfigures. This behavior can be
     # disabled by passing in the keyword argument
     # `seamless=False`
     # Also note that this will only work for strictly increasing
     # transition functions.
     def newkey(self, f, figure=None, *, seamless=True):
         f = round(f)
-        if type(f) is not int:
-            raise TypeError("Index is NOT an int.")
 
         if figure is None:
             # Default new keyfigure is given by tweening.
-            figure = self.time(f)
-            # if f in self.timeline:
-            #     figure = self.time(f).copy()
-            # else:
-            #     figure = self.time(f)
+            figure = self.time(f, copykeys=True)
 
             # If tweening fails somehow, then new keyfigure
             # is a copy of the previous keyfigure if it exists,
             # else just use the default figure.
             if figure is None:
                 k = listfloor(self.keyIDs, f)
                 if k == -1:  # If before first keyfigure
                     figure = self.figureType()
                 else:  # Else use latest keyfigure
                     # keyID = self.keyIDs[k]
                     figure = self.key(k).copy()
-            else:  # In case time() returned a keyfig.
-                figure = figure.copy()
         elif type(figure) is not self.figureType:
             raise TypeError("Given figure is not of actor's figure type.")
         elif figure in self.timeline.values():
             # Copy the figure if it's already in the timeline.
             figure = figure.copy()
 
         # Adjust transition of previous keyfig so that the
         # insertion of a new keyfigure does not modify the playback
         # of the animation. But only do this if the index is a
         # genuinely new index that is in the middle of the timeline
         if seamless and self.firstID() < f < self.lastID() and f not in self.timeline:
             # raise NotImplementedError
             keyfig1 = self.prevkey(f)
+            keyfig2 = self.nextkey(f)
             a,b = self.prevkeyID(f), self.nextkeyID(f)
             t_split = (f-a)/(b-a)
-            # Split the tween method
-            if hasattr(keyfig1.tweenMethod, "splitter") and keyfig1.tweenMethod.splitter is not None:
-                tween1, tween2 = keyfig1.tweenMethod.splitter(keyfig1.transition(t_split))
-                keyfig1.tweenMethod = tween1
-                figure.tweenMethod = tween2
-            # Split the transition function
-            func1, func2 = morpho.transitions.split(keyfig1.transition, t_split)
-            keyfig1.transition = func1
-            figure.transition = func2
+            Actor._splitTweenAndTransition(t_split, keyfig1, figure, keyfig2)
 
         # Add the figure to the timeline
         self.timeline[f] = figure
         self.update()
 
         return figure
 
@@ -1839,14 +1837,98 @@
         start = actor.firstID()
         for keyID in actor.timeline:
             self.newkey(keyID-start+afterFrame+1, actor.timeline[keyID], seamless=False)
 
     # Alternate name for insert() is paste()
     # paste = insert
 
+    # For internal use only by Films (Frame Actors).
+    # Merges a given film into self IN PLACE.
+    # Note that the secondary film may get modified by this function.
+    def _mergeFilm(self, film):
+        # film = film.copy()
+
+        # Manually create a new initial keyframe. This is to
+        # prevent the default behavior of newkey() to create a
+        # default (i.e. blank) keyfigure if it occurs before
+        # the earliest keyframe in the timeline.
+        mintime = min([self.firstID(), film.firstID()])
+        self.newkey(mintime, self.first().copy())
+        film.newkey(mintime, film.first().copy())
+
+        # Sorting is useful to prevent unnecessary tween method
+        # splitting for later keyfigures.
+        keytimes = sorted(set(self.keyIDs).union(film.keyIDs))
+        # Seamlessly introduce new keyframes into secondary film
+        # corresponding to the keyframes of self. This
+        # way, the secondary film will still animate identically
+        # after being merged into the (possibly crowded) timeline
+        # of self.
+        for keytime in keytimes:
+            self.newkey(keytime)
+            film.newkey(keytime)
+        # Likewise, add new keyframes to self from those
+        # uniquely in film and then merge keyframes across the
+        # two films.
+        for keytime in keytimes:
+            self.time(keytime).merge(film.time(keytime))
+
+        return self
+
+    # Combines all the actors into a single Frame actor.
+    # Optional keyword `stagger` can be given an integer
+    # to offset each actor from the previous in the sequence by
+    # a certain number of frames.
+    # Optional keyword `template` is an empty Frame or Frame subtype
+    # that will be used to construct the Actor.
+    # Default: morpho.Frame()
+    @staticmethod
+    def zip(*actors, stagger=0, template=None):
+        if len(actors) == 0:
+            raise TypeError("No actors to zip.")
+        if isinstance(actors[0], (list, tuple)):
+            actors = actors[0]
+        if template is None:
+            template = morpho.Frame()
+
+        # Turn each individual actor into a singleton Frame Actor
+        # (aka "Film") before combining them all into a single Film.
+        films = []
+        for n, actor in enumerate(actors):
+            actor = actor.copy()
+            film = Actor(type(template))
+            for time, keyfig in actor.timeline.items():
+                # Incorporate non-uniform transitions into tween methods
+                # since Frame tweening ignores subfigure transitions.
+                if keyfig.transition != morpho.transitions.uniform:
+                    keyfig.tweenMethod = morpho.transitions.incorporateTransition(keyfig.transition, keyfig.tweenMethod)
+                    keyfig.transition = morpho.transitions.uniform
+                # Transitions are handled within the tween methods of
+                # subfigures, so the toplevel transition of the film
+                # should be uniform.
+                film.newkey(time+n*stagger, template.copy()).set(figures=[keyfig], transition=morpho.transitions.uniform)
+            films.append(film)
+
+        # Combine all the individual singleton films into
+        # a single film.
+        finalFilm = films[0]
+        for film in films[1:]:
+            finalFilm._mergeFilm(film)
+        # Ensure state of the subfigures of the final keyframe exactly
+        # matches the state of the final keys of the supplied actors.
+        # Also ensure other settings of the final keyframe matches the
+        # template.
+        finalFilm.fin = template.copy().set(figures=[actor.last().copy() for actor in actors])
+
+        return finalFilm
+
+    @property
+    def subaction(self):
+        return self.figureType.subaction(self)
+
     # NOT IMPLEMENTED!
     # Like insert(), except it overwrites the original actor
     # at the target frame going into the future.
     def overwrite(self, afterFrame=None):
         raise NotImplementedError
 
     # Returns the first keyID coming before or equal to the given index.
@@ -1945,14 +2027,20 @@
             currentIndex = self.owner.owner.currentIndex
         except AttributeError:
             raise TypeError("No global timeline to reference.")
 
         f = currentIndex - self.owner.timeOffset
         fig = self.time(f, copykeys=True)  # Make a copy in case it's a keyfigure
 
+        # Lie and say that self owns this figure so that methods like
+        # Text.box() work correctly. I think it's okay for it to lie here since
+        # the primary use case of now() is within Skit.makeFrame(), so this lie
+        # is unlikely to cause harm.
+        fig.owner = self
+
         return fig
 
     # Optimizes the Actor for playback by setting keyfigures to be
     # acutely static if it looks like there's no reason to tween
     # them e.g. the starting and ending keyfigures appear equal, or
     # the current keyfigure is invisible (whereby the tweened figure
     # will inherit the invisibility).
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/gadgets.py` & `morpholib-0.8.0.dev1/src/morpholib/gadgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 import morpholib as morpho
 import morpholib.anim
 import morpholib.grid
 from morpholib.tools.basics import *
+from morpholib.tools.dev import handleBoxTypecasting
 
 import math, cmath
 
-# Decorator for gadget functions that operate on a box.
-# Allows such a gadget function to accept a Figure type input
-# whereby it will attempt to infer a box by calling the
-# figure's `box()` method, assuming it exists.
-# If given an Actor object, it will use the latest keyfigure.
-def handleBoxTypecasting(gadgetfunc):
-    def wrapper(box, *args, **kwargs):
-        if isinstance(box, morpho.Actor):
-            box = box.last()
-        if isinstance(box, morpho.Figure):
-            if not hasattr(box, "box"):
-                raise TypeError(f"`{type(box).__name__}` type figure does not support box() method.")
-            box = box.box()
-        return gadgetfunc(box, *args, **kwargs)
-    return wrapper
-
 # DEPRECATED! Use crossout() or crossoutPath() instead.
 # Returns a layer which when animated makes a colored X cross
 # out the box you specify.
 # box = a 4-item list/tuple in the same fashion as the view box
 # time = duration for the animation
 # width = thickness of the lines
 # color = color of the lines
@@ -240,16 +225,17 @@
 
 enbox = enboxPath  # Synonym for emboxPath()
 
 # Same as enbox(), but it deboxes immediately afterward.
 # Useful for briefly highlighting something with a box.
 # An additional keyword-only input `pause` can be specified
 # to provide a delay between enboxing and deboxing.
-def enboxHighlight(*args, pause=0, **kwargs):
+def enboxFlourish(*args, pause=0, **kwargs):
     return enbox(*args, _debox=True, _pause=pause, **kwargs)
+enboxHighlight = enboxFlourish
 
 # Scales all the nodes of a path by the given factor about the given
 # centerpoint. If the center is unspecified, defaults to the center
 # of mass of all the path's nodes.
 def expandPath(path, factor, center=None):
     if center is None:
         center = sum(path.seq)/len(path.seq)
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/giffer.py` & `morpholib-0.8.0.dev1/src/morpholib/giffer.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/graph.py` & `morpholib-0.8.0.dev1/src/morpholib/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from morpholib.tools.basics import *
 import morpholib.transitions
 
 import pyglet as pg
 pyglet = pg
 from cmath import exp
 
+import numpy as np
+
 # Returns a Frame figure that defines axes over the given view.
 #
 # ARGUMENTS
 # xwidth = x-axis thickness (in pixels). Default: 5
 # ywidth = y-axis thickness (in pixels). Default: 5
 # xcolor = x-axis color (RGB list). Default: [0,0,0] (black)
 # ycolor = y-axis color (RGB list). Default: [0,0,0] (black)
@@ -128,14 +130,16 @@
 # stagger = Cycle offset between consecutive streamers.
 #           For example, stagger=0.25 means each consecutive streamer
 #           will be a quarter cycle offset from the previous one.
 #           Default: 0 (no stagger)
 # offset = Cycle position the first streamer should start in.
 #          Essentially, this advances all the initial streamers
 #          by the given amount. Default: 0 (no offset)
+#          Can also be a list of N values which will generate N-many
+#          copies of each streamer offset by each amount in the list.
 # sectorSize = Portion of the cycle that will be visible at any given
 #              moment. Default: 0.5 (display half a cycle)
 # transition = Transition function to use for each streamer.
 #              Default: Uniform transition
 # Any additional inputs will be passed to flowStreamer() for the
 # construction of each individual streamer.
 class FlowField(morpho.Layer):
@@ -152,24 +156,31 @@
     def streamers(self, value):
         self.actors = value
 
     @staticmethod
     def generateStreamers(points, *args, stagger=0, offset=0, sectorSize=0.5,
         transition=morpho.transitions.uniform, _3dmode=False, **kwargs):
 
+        if isinstance(offset, np.ndarray):
+            offset = offset.tolist()
+        elif not isinstance(offset, (list, tuple)):
+            offset = [offset]
+
         makeStreamer = flowStreamer3d if _3dmode else flowStreamer
         streamers = []
-        for n,z in enumerate(points):
-            streamer = makeStreamer(z, *args, **kwargs)
-            streamer.start = n*stagger + offset
-            streamer.end = streamer.start + sectorSize
-            streamer.transition = transition
 
-            streamer = morpho.Actor(streamer)
-            streamers.append(streamer)
+        for shift in offset:
+            for n,z in enumerate(points):
+                streamer = makeStreamer(z, *args, **kwargs)
+                streamer.start = n*stagger + shift
+                streamer.end = streamer.start + sectorSize
+                streamer.transition = transition
+
+                streamer = morpho.Actor(streamer)
+                streamers.append(streamer)
         return streamers
 
     # Returns a Frame-like object consisting of all the final
     # keyfigures for each streamer.
     # Note that these may not all correspond to exactly the same
     # time coordinate!
     def last(self):
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/graphics.py` & `morpholib-0.8.0.dev1/src/morpholib/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,81 +261,69 @@
         return self
 
     # Sets the "linked" attr to False
     def unlink(self):
         self.linked = False
         return self
 
-    # # Allows you to specify the origin using a scheme
-    # # similar to the Text class's anchor scheme
-    # def align(self, x=None, y=None):
-    #     if x is not None:
-    #         self.origin[0] = self.imageWidth*(x + 1)/2
-    #     if y is not None:
-    #         self.origin[1] = self.imageHeight*(y + 1)/2
-
     @property
     def imageOrigin(self):
         x,y = self.align
         return [self.imageWidth*(x+1)/2, self.imageHeight*(y+1)/2]
 
     @imageOrigin.setter
     def imageOrigin(self, value):
         X,Y = value
         self.align = [2*X/self.imageWidth-1, 2*Y/self.imageHeight-1]
 
-    # Returns the bounding box (with possible padding) of the image
-    # ignoring any transformations like rotation, transform, or scale
-    # Also assumes the image has physical set to True.
-    def box(self, pad=0):
-        align_x, align_y = self.align
-        # a = self.pos.real - self.scale_x*self.width/2*(align_x + 1)
-        # b = a + self.scale_x*self.width
-        # c = self.pos.imag - self.scale_y*self.height/2*(align_y + 1)
-        # d = c + self.scale_y*self.height
-
-        a = self.pos.real - self.width/2*(align_x + 1)
-        b = a + self.width
-        c = self.pos.imag - self.height/2*(align_y + 1)
-        d = c + self.height
-
-        return [a-pad, b+pad, c-pad, d+pad]
+    # Returns the bounding box (with possible padding) of the image.
+    # If keyword `raw` is set to True, it will ignore `rotation`,
+    # `transform`, and `scale` attributes.
+    # Also assumes the image has `physical` set to True.
+    def box(self, *args, **kwargs):
+        a,b,c,d = self.relbox(*args, **kwargs)
+        x,y = self.pos.real, self.pos.imag
+        return [a+x, b+x, c+y, d+y]
 
     # Same as box(), but the coordinates are relative to the image's
     # physical position.
-    def relbox(self, pad=0):
+    def relbox(self, pad=0, *, raw=False):
         align_x, align_y = self.align
         a = -self.width/2*(align_x + 1)
         b = a + self.width
         c = -self.height/2*(align_y + 1)
         d = c + self.height
 
-        return [a-pad, b+pad, c-pad, d+pad]
+        if not raw and not(self.rotation == 0 and self.scale_x == 1 and self.scale_y == 1 and np.array_equal(self._transform, I2)):
+            transform = self._transform @ morpho.matrix.scale2d(self.scale_x, self.scale_y)
+            return BoundingBoxFigure._transformedBox([a,b,c,d], 0, self.rotation, transform, pad)
+        else:
+            return [a-pad, b+pad, c-pad, d+pad]
 
     # Returns the four corners of the image's bounding box
     # plus any optional padding. The sequence of the corners is
     # NW, SW, SE, NE.
-    def corners(self, pad=0):
+    def corners(self, *args, **kwargs):
         # NOTE: This method should actually be removable
         # since its behavior should be identical to the corners()
         # method inherited from BoundingBoxFigure.
-        a,b,c,d = self.box(pad)
+        a,b,c,d = self.box(*args, **kwargs)
 
         NW = a + d*1j
         SW = a + c*1j
         SE = b + c*1j
         NE = b + d*1j
 
         return [NW,SW,SE,NE]
 
 
     # Same as corners(), but the coordinates are relative to wherever
     # the image's physical position is.
-    def relcorners(self, pad=0):
-        a,b,c,d = self.relbox(pad)
+    def relcorners(self, *args, **kwargs):
+        a,b,c,d = self.relbox(*args, **kwargs)
 
         NW = a + d*1j
         SW = a + c*1j
         SE = b + c*1j
         NE = b + d*1j
 
         return [NW,SW,SE,NE]
@@ -450,15 +438,15 @@
         areaMat[:,1] *= self.imageHeight
         if morpho.matrix.thinHeight2x2(areaMat) < 1:
             return
 
         if self.backAlpha > 0:
             # Construct background rectangle and draw it
             rectTransform = premat
-            box = self.relbox(pad=self.backPad)
+            box = self.relbox(pad=self.backPad, raw=True)
             if not self.physical:
                 w1 = morpho.physicalWidth(1, view, ctx)
                 h1 = morpho.physicalHeight(1, view, ctx)
                 a,b,c,d = box
                 box = [a*w1, b*w1, c*h1, d*h1]
 
                 # If in a non-square view, conjugate the premat
@@ -857,16 +845,14 @@
             fig = self.figures[n]
             if not isinstance(fig, Image):
                 newfig = fig.images[0].copy()
                 self.figures[n] = newfig
 
     # tween = morpho.Figure.tween
 
-    box = morpho.grid.MultiPath.box
-
     ### TWEEN METHODS ###
 
     tweenLinear = Multi(Image.tweenLinear, mainMethod=morpho.MultiFigure.tweenLinear)
     tweenSpiral = Multi(Image.tweenSpiral, mainMethod=morpho.MultiFigure.tweenSpiral)
 
     @classmethod
     def tweenPivot(cls, angle=tau/2, *args, **kwargs):
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/grid.py` & `morpholib-0.8.0.dev1/src/morpholib/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 import morpholib as morpho
 mo = morpho
-import morpholib.tools.color, morpholib.anim
+import morpholib.tools.color, morpholib.anim, morpholib.transitions
 from morpholib.matrix import mat
 from morpholib.anim import MultiFigure
 from morpholib.tools.basics import *
 from morpholib.tools.dev import drawOutOfBoundsStartEnd, BoundingBoxFigure, \
-    totalBox, shiftBox, translateArrayUnderTransforms
+    totalBox, shiftBox, translateArrayUnderTransforms, handleBoxTypecasting, \
+    AmbiguousValueError
 
 from morpholib import object_hasattr
 
 import pyglet as pg
 pyglet = pg
 import cairo
 cr = cairo
@@ -590,26 +591,26 @@
         self._transform = morpho.matrix.array(value)
 
     # Setting `tipSize` property sets both `headSize` and `tailSize
     # to the same value.
     @property
     def tipSize(self):
         if self.headSize != self.tailSize:
-            raise ValueError("headSize and tailSize are different!")
+            raise AmbiguousValueError("headSize and tailSize are different!")
         return self.headSize
 
     @tipSize.setter
     def tipSize(self, value):
         self.headSize = value
         self.tailSize = value
 
     @property
     def tipExternal(self):
         if self.headExternal != self.tailExternal:
-            raise ValueError("headExternal and tailExternal have different truth values.")
+            raise AmbiguousValueError("headExternal and tailExternal have different truth values.")
         return self.headExternal
 
     @tipExternal.setter
     def tipExternal(self, value):
         self.headExternal = value
         self.tailExternal = value
 
@@ -1649,14 +1650,22 @@
                     ctx.move_to(x,y)
                 else:
                     ctx.line_to(x,y)
 
                 # Update zn to z
                 zn = z
 
+            # Auto-close path if the path has the simplest possible settings
+            if self.seq[0] == self.seq[-1] and \
+                self.start == 0 and self.end == 1 and \
+                len(self.deadends) == 0 and \
+                self.headSize == 0 and self.tailSize == 0:
+
+                ctx.close_path()
+
             # Stroke and fill the path
             if self.width < 0:
                 # Draw stroke first, then fill
                 ctx.restore()
                 self._drawStroke(ctx, RGBA_start)
                 with morpho.pushPhysicalCoords(view, ctx):
                     self._drawFill(camera, ctx)
@@ -1709,14 +1718,15 @@
         self.seq += other.seq
         # if isinstance(self, PathPolar) and isinstance(other, PathPolar):
         #     self.windSeq += other.windSeq
         if not connectEnds:
             self.deadends.add(old_len-1)
 
         # Merge deadends from other into self
+        len_self = len(self.seq)
         for n in other.deadends:
             self.deadends.add(n+len_self)
 
         return self
 
         # return result
 
@@ -2113,15 +2123,16 @@
         return actor.morphFrom(combined, *args, **kwargs)
     else:
         return morpho.Figure.actions["morphFrom"](actor, source, *args, **kwargs)
 
 # Highlights the MultiPath actor
 @MultiPath.action
 def highlight(actor, duration=15, atFrame=None, *,
-    width=-3, fill=(1,1,0), color=(0,0,0), rescale=1, select=None):
+    width=-3, fill=(1,1,0), color=(0,0,0), rescale=1, select=None,
+    **kwargs):
 
     if atFrame is None:
         atFrame = actor.lastID()
 
     if select is None:
         select = sel[:]
     elif isinstance(select, Iterable):
@@ -2132,15 +2143,15 @@
     path2 = actor.newendkey(duration)
 
     # Assignment to subframe needs to happen because
     # if `select` is a choice function, modifying the
     # width/fill/color of the subpaths can change what
     # the choice function selects on the second call.
     subframe = path2.select[select]
-    subframe.set(width=width, fill=fill, color=color)
+    subframe.set(width=width, fill=fill, color=color, **kwargs)
     if rescale != 1:
         if select == sel[:]:
             path2.rescale(rescale)
         else:
             subframe.rescale(rescale)
 
 # Highlights then immediately de-highlights the MultiPath actor.
@@ -2156,14 +2167,67 @@
     path1 = actor.newkey(atFrame)
 
     actor.highlight(duration, atFrame, **kwargs)
     if pause > 0:
         actor.newendkey(pause)
     actor.newendkey(duration, path1.copy())
 
+# Draws in a MultiPath actor Manim-style.
+#
+# OPTIONAL KEYWORD-ONLY INPUTS
+# tempWidth = Temporary stroke width to use in the animation
+#       if the stroke width is 0. Default: 3
+# transition = Transition to use in the animation.
+#       Note that this only applies to the portion of the actor's
+#       timeline affected by this action. After the action
+#       concludes, the original transition of this actor will
+#       be used for future keyfigures. Default: uniform.
+@MultiPath.action
+def drawIn(actor, duration=30, atFrame=None, *,
+    tempWidth=3, transition=morpho.transitions.uniform,
+    overlap=0):
+
+    # (`overlap` is a currently unimplemented possible future feature
+    # that would control how much the animation of drawing in one
+    # subpath overlaps with the drawing in of the previous subpath.
+    # It's kind of like a reverse `stagger` parameter.)
+
+    if atFrame is None:
+        atFrame = actor.lastID()
+
+    mpath0 = actor.last()
+    # Save current final state of the actor which should be
+    # the same final state when this action is finished.
+    final = mpath0.copy()
+    mpath0.all.set(start=0, end=0, alphaFill=0, alphaEdge=1)
+    mpath0.transition = transition
+    for path in mpath0.figures:
+        # Give a temporary stroke width and color to the subpath
+        # if its width is 0
+        if path.width == 0:
+            path.width = tempWidth
+            if not isinstance(path.fill, morpho.color.GradientFill):
+                path.color = path.fill[:]
+
+    mpath1 = actor.newkey(atFrame)
+    mpath0.visible = False
+
+    tstart = atFrame
+    tend = atFrame + duration
+    numfigs = mpath1.numfigs
+    dt = duration / (numfigs + 1)
+    for n in range(numfigs):
+        time = tstart + (n+1)*dt
+        mpath_n = actor.newkey(time)
+        if n > 0:
+            mpath_n.figures[n-1] = final.figures[n-1].copy()
+        mpath_n.figures[n].set(start=final.figures[n].start, end=final.figures[n].end)
+    actor.newkey(tend, final)
+
+
 
 # 3D version of MultiPath meant to enable 2D MultiPaths to be
 # positionable and orientable in 3D space. This is NOT a full
 # SpaceMultiPath class, which would be a MultiFigure of
 # SpaceSplines! Rather, this is just a regular 2D MultiPath
 # which can be rendered in a 3D space like SpaceImage can.
 #
@@ -2282,23 +2346,14 @@
         # Set default tick width and color based on the
         # given values for path width and color
         if tickWidth is None:
             tickWidth = width/2
         if tickColor is None:
             tickColor = color[:]
 
-        # New tweenables
-        tickWidth = morpho.Tweenable("tickWidth", tickWidth, tags=["size"])
-        tickColor = morpho.Tweenable("tickColor", tickColor, tags=["color"])
-        tickAlpha = morpho.Tweenable("tickAlpha", tickAlpha, tags=["scalar"])
-        tickLength = morpho.Tweenable("tickLength", tickLength, tags=["scalar"])
-        tickGap = morpho.Tweenable("tickGap", tickGap, tags=["scalar"])
-        tickStart = morpho.Tweenable("tickStart", 0, tags=["scalar"])
-        tickEnd = morpho.Tweenable("tickEnd", 1, tags=["scalar"])
-
         if isinstance(seq, Path):
             path = seq
             super().__init__(path.seq[:], path.width, path.color, path.alpha)
             self.start = path.start
             self.end = path.end
             self.alphaEdge = path.alphaEdge
             self.fill = path.fill[:]
@@ -2320,32 +2375,40 @@
             # # Actually, maybe nevermind. This could conflict with
             # # any user-specified tickAlpha in the constructor.
             # tickAlpha.value = 0
 
         else:
             super().__init__(seq, width, color, alpha)
 
-        self.extendState(
-            [tickWidth, tickColor, tickAlpha,
-            tickLength, tickGap, tickStart, tickEnd]
-            )
+        # New tweenables
+        self.Tweenable("tickWidth", tickWidth, tags=["size"])
+        self.Tweenable("tickColor", tickColor, tags=["color"])
+        self.Tweenable("tickAlpha", tickAlpha, tags=["scalar"])
+        self.Tweenable("tickLength", tickLength, tags=["scalar"])
+        self.Tweenable("tickGap", tickGap, tags=["scalar"])
+        self.Tweenable("tickStart", 0, tags=["scalar"])
+        self.Tweenable("tickEnd", 1, tags=["scalar"])
+        self.Tweenable("tickOffset", 0, tags=["scalar"])
+
+
 
     # Generates the underlying path object which when drawn
     # makes the ticks appear.
     def makeTicks(self):
         backpath = Path(self.seq)
         backpath.color = self.tickColor
         backpath.alpha = self.tickAlpha*self.alphaEdge*self.alpha
         backpath.width = self.tickLength
         backpath.start = max(self.tickStart, self.start)
         backpath.end = min(self.tickEnd, self.end)
         # Prevent negative dash steps
         gap = self.tickGap-self.tickWidth
         if gap > 0:
             backpath.dash = [self.tickWidth, gap]
+            backpath.dashOffset = self.tickOffset
 
         backpath.origin = self.origin
         backpath.rotation = self.rotation
         backpath._transform = self._transform
 
         backpath.interp = self.interp
         backpath.deadends = self.deadends
@@ -2987,210 +3050,86 @@
 
         # Temporarily modify self.tickGap to the pixel value and use
         # Track.draw() to render it before reverting tickGap back to
         # its original value.
         # Also temporarily adjust some other attributes to handle
         # centering the tickmarks.
         origGap = self.tickGap
-        origOrigin = self.origin
-        origEnd = self.seq[1]
+        origTickOffset = self.tickOffset
         self.tickGap = self.tickGap*scale
-        shift = 0.5*self.tickWidth/scale*unit
-        self.origin = self.origin - shift
-        self.seq[1] = self.seq[1] + shift
+        self.tickOffset = self.tickOffset*scale + self.tickWidth/2
         Track.draw(self, camera, ctx)
         # Restore original values
         self.tickGap = origGap
-        self.origin = origOrigin
-        self.seq[1] = origEnd
+        self.tickOffset = origTickOffset
 
 
 # Mainly for internal use.
 # 3D version of the Axis class. See `Axis` for more info.
 class SpaceAxis(SpaceTrack):
     def primitives(self, camera):
         primitives = SpaceTrack.primitives(self, camera)
         if len(primitives) == 0: return []
         track = primitives[0]
         axis = Axis()
         axis._updateFrom(track, copy=True, common=True)
 
         # Scale tick spacing based on how much the axis has
         # shrunk due to foreshortening.
-        axis.tickGap *= abs(axis.seq[1]-axis.seq[0]) / np.linalg.norm(self.seq[1]-self.seq[0]).tolist()
+        scale = abs(axis.seq[1]-axis.seq[0]) / np.linalg.norm(self.seq[1]-self.seq[0]).tolist()
+        axis.tickGap *= scale
+        axis.tickOffset *= scale
 
         return [axis]
 
 
-# Mainly for internal use by the MathGrid class
-# to enable MathGrids to split their subpaths'
-# tween methods.
-# Special tween method splitter that returns two special
-# dictionaries containing t_split values for the subpaths
-# of a MathGrid object. When these dicts are assigned to
-# MathGrid's special `tweenMethod` property, the t_split
-# values are extracted and passed to the subfigures'
-# tween method splitters.
-def _gridSplitter(t):
-    tween1 = dict(t_split=t)
-    tween2 = dict(t_split=1-t)
-    return (tween1, tween2)
-
 # Special Frame figure for mathgrids
 class MathGrid(morpho.Frame):
-    def __init__(self, *args, **kwargs):
-        # Bypass Figure class special setattr() method to set the
-        # hidden `_transition` attribute so that the `transition`
-        # property works when super().__init__() is called.
-        object.__setattr__(self, "_transition", morpho.transition.default)
-        object.__setattr__(self, "_defaultTween", type(self).tweenLinear)
-        super().__init__(*args, **kwargs)
-        # This assigns the Frame's transition to all component figures.
-        self.transition = self._transition
-
-    # transition property makes it so that setting the transition
-    # of the MathGrid as a whole propagates it down to the component
-    # figures.
-    @property
-    def transition(self):
-        return self._transition
-
-    @transition.setter
-    def transition(self, value):
-        self._transition = value
-        # The try clause here is because the transition property
-        # may be set before the figures tweenable has been setup
-        # e.g. in __init__()
-        try:
-            for fig in self._state["figures"].value:
-                fig.transition = value
-        except KeyError:
-            pass
-
-    @property
-    def defaultTween(self):
-        return self._defaultTween
-
-    # Special setter for the defaultTween attribute
-    # enables MathGrids to split subfigure tween methods.
-    # It works as normal, but if a dict is assigned
-    # to the defaultTween/tweenMethod attribute instead of a
-    # function, it extracts the t-split value inside and passes
-    # it to the splitters of the subfigure tween methods.
-    # If the dict also contains a "tweenMethod" key, it will
-    # assign the value of that tweenMethod as the tween method
-    # of the MathGrid object.
-    @defaultTween.setter
-    def defaultTween(self, value):
-        # If value is callable, just treat it as an ordinary
-        # tween method and assign it normally.
-        if callable(value):
-            self._defaultTween = value
-        # If value is a dictionary, potentially do some subfigure
-        # tween method splitting.
-        elif isinstance(value, dict):
-            if "tweenMethod" in value:
-                self._defaultTween = value["tweenMethod"]
-            if "t_split" in value:
-                t_split = value["t_split"]
-                # Go thru the
-                # path list and split all the tween methods
-                # according to the given t_split value.
-                for fig in self.figures:
-                    if morpho.tweenSplittable(fig.tweenMethod):
-                        fig.tweenMethod = fig.tweenMethod.splitter(t_split)[0]
-        else:
-            raise TypeError(f"Invalid type `{type(value).__name__}` for tween method.")
 
     # Returns equivalent MultiPath figure of this MathGrid
     def toMultiPath(self):
         multipath = MultiPath(self.figures)
         return multipath
 
-    ### TWEEN METHODS ###
-
-    # This is a hack to enable MathGrids to split the
-    # tween methods of their component figures.
-    # The tween methods are assigned a special splitter that
-    # instead of returning two tween methods, returns
-    # two dicts containing t-split values. When MathGrid
-    # figures are assigned these dicts as tweenMethods,
-    # they will propagate the t-split values to the splitters
-    # of the subfigures while leaving the MathGrid tweenMethod
-    # attribute unchanged.
-    @morpho.TweenMethod(splitter=_gridSplitter)
-    def tweenLinear(self, *args, **kwargs):
-        return super().tweenLinear(*args, **kwargs)
-
-    @morpho.TweenMethod(splitter=_gridSplitter)
-    def tweenSpiral(self, *args, **kwargs):
-        return super().tweenSpiral(*args, **kwargs)
-
-    @classmethod
-    def tweenPivot(cls, *args, **kwargs):
-        pivot = super().tweenPivot(*args, **kwargs)
-
-        # This is another hack. The tween methods returned by
-        # the standard pivot splitter are packaged into a dict
-        # along with a special "t_split" key which the tweenMethod
-        # setter for the MathGrid class will pass on to the
-        # subfigures' tween method splitters.
-        basesplitter = pivot.splitter
-        def splitter(t):
-            tween1, tween2 = basesplitter(t)
-            tween1 = dict(tweenMethod=tween1, t_split=t)
-            tween2 = dict(tweenMethod=tween2, t_split=1-t)
-            return (tween1, tween2)
-
-        pivot = morpho.TweenMethod(pivot, splitter=splitter)
-        return pivot
-
-
-
 @MathGrid.action
-def growIn(grid, duration=30, atFrame=None, *, reverse=False):
+def growIn(grid, duration=30, atFrame=None, *, reverse=False, substagger=0):
+    lasttime = grid.lastID()
     if atFrame is None:
-        atFrame = grid.lastID()
+        atFrame = lasttime
 
     grid0 = grid.last()
-    grid1 = grid.newkey(atFrame)
-    grid2 = grid.newendkey(duration)
-
-    grid0.visible = False
-
-    for path in grid1.figures:
-        path.static = False
-        if reverse:
-            path.start = 1
-        else:
-            path.end = 0
-# MathGrid_growIn = growIn
+    gridfinal = grid0.copy().set(visible=True)
+    grid0.all.static = False
+    grid.subaction.growIn(duration, atFrame, reverse=reverse, substagger=substagger)
+
+    # Hide lingering initial keyfigure if it exists.
+    if atFrame > lasttime:
+        grid0.visible = False
+
+    # Ensure final keyfigure is really the original final figure.
+    # Also restores all formerly static subfigures to being static
+    # again.
+    grid.fin = gridfinal
 
 @MathGrid.action
-def shrinkOut(grid, duration=30, atFrame=None, *, reverse=False):
-    if atFrame is None:
-        atFrame = grid.lastID()
-
-    grid0 = grid.newkey(atFrame)
-    for path in grid0.figures:
-        path.static = False
-
-    grid1 = grid.newendkey(duration)
-    for path in grid1.figures:
-        path.set(headSize=0, tailSize=0, visible=False)
-        if reverse:
-            path.start = 1
-        else:
-            path.end = 0
+def shrinkOut(grid, *args, **kwargs):
+    # Remember who was static so we can restore later
+    staticRecord = [fig.static for fig in grid.last().figures]
+    grid.last().all.static = False
+    grid.subaction.shrinkOut(*args, **kwargs)
+    grid.last().visible = False
+    # Restore static attribute for subfigures that were originally
+    # static. This is helpful in case the user wants to use the
+    # grid again after shrink out is complete.
+    for fig, static in zip(grid.last().figures, staticRecord):
+        fig.static = static
 
 
 # Special SpaceFrame figure for 3D mathgrids
 class SpaceMathGrid(MathGrid, morpho.SpaceFrame):
-    # Copy over the actions defined for MathGrid
-    actions = MathGrid.actions.copy()
 
     ### TWEEN METHODS ###
 
     def tweenSpiral(self, other, t):
         raise NotImplementedError
 
     @classmethod
@@ -3244,28 +3183,31 @@
 #       Default: None (meaning it uses morpho.transition.default)
 def mathaxes(*,
     view=(-5,5, -5,5), axis="xy",
     xwidth=5, ywidth=5, width=None,
     xcolor=(1,1,1), ycolor=(1,1,1), color=None, alpha=1,
     xtickLength=0, ytickLength=0, tickLength=None,
     xtickWidth=None, ytickWidth=None, tickWidth=None,
+    xtickOffset=0, ytickOffset=0, tickOffset=None,
     dx=1, dy=1, spacing=None,
     tweenMethod=Axis.tweenLinear,
     transition=None):
 
     # Handle orientation-agnostic keyword inputs
     if spacing is not None:
         dx = dy = spacing
     if color is not None:
         xcolor = color[:]
         ycolor = color[:]
     if tickLength is not None:
         xtickLength = ytickLength = tickLength
     if tickWidth is not None:
         xtickWidth = ytickWidth = tickWidth
+    if tickOffset is not None:
+        xtickOffset = ytickOffset = tickOffset
     if width is not None:
         xwidth = ywidth = width
 
     if xtickWidth is None:
         xtickWidth = xwidth/2
     if ytickWidth is None:
         ytickWidth = ywidth/2
@@ -3277,26 +3219,26 @@
     frm = MathGrid()
 
     xmin, xmax, ymin, ymax = view
     if "x" in axis:
         xaxis = mo.grid.Axis([xmin, xmax]).set(
             width=xwidth, color=xcolor, alpha=alpha,
             tickLength=xtickLength, tickWidth=xtickWidth,
-            tickGap=dx, tickColor=xcolor[:],
+            tickGap=dx, tickColor=xcolor[:], tickOffset=xtickOffset,
             tweenMethod=tweenMethod,
             transition=transition
             )
         frm.figures.append(xaxis)
         frm.setName(xaxis=xaxis)
 
     if "y" in axis:
         yaxis = mo.grid.Axis([ymin*1j, ymax*1j]).set(
             width=ywidth, color=ycolor, alpha=alpha,
             tickLength=ytickLength, tickWidth=ytickWidth,
-            tickGap=dy, tickColor=ycolor[:],
+            tickGap=dy, tickColor=ycolor[:], tickOffset=ytickOffset,
             tweenMethod=tweenMethod,
             transition=transition
             )
         frm.figures.append(yaxis)
         frm.setName(yaxis=yaxis)
 
     frm.transition = transition
@@ -4535,14 +4477,15 @@
 
 # Helper function sets up a basic rectangular Quadmesh in the xy-plane, which
 # can then be manipulated with fimage().
 #
 # INPUTS
 # view = Bounding box of the quadmesh ([xmin,xmax,ymin,ymax]). Default: [-5,5, -5,5]
 # dx,dy = Horizontal or vertical spacing between vertices (physical units).
+#         You can also specify `spacing` to set both to the same value.
 #         Default: 1
 # width = Thickness of mesh lines (in pixels). Default: 3
 # color = Color of mesh lines (RGB list). Default (0,0,0) (black)
 # alphaEdge = Opacity of mesh lines. Default 1 (opaque)
 # fill = Quadmesh interior color (RGB list). Default (1,0,0) (red)
 #        Can also be a color function mapping (x,y,z) to RGB.
 # alphaFill = Quadmesh interior opacity. Default: 1 (opaque)
@@ -4553,21 +4496,25 @@
 # tweenMethod = Tween method to assign. Default: Quadmesh.tweenLinear
 # transition = Transition function to assign. Default: morpho.transition.default
 #
 # Any additional keyword inputs are set as attributes of the returned
 # Quadmesh.
 def quadgrid(*,
     view=(-5,5, -5,5),
-    dx=1, dy=1,
+    dx=1, dy=1, spacing=None,
     width=3,
     color=(0,0,0), alphaEdge=1,
     fill=(1,0,0), alphaFill=1, alpha=1, fill2=None,
     tweenMethod=Quadmesh.tweenLinear,
     transition=None, **kwargs):
 
+    # Handle orientation-agnostic keyword inputs
+    if spacing is not None:
+        dx = dy = spacing
+
     xmin, xmax, ymin, ymax = view
     xmax += 1.0e-6  # +epsilon to deal with floating point error
     ymax += 1.0e-6
 
     Nx = 1 + int((xmax-xmin) // dx)
     Ny = 1 + int((ymax-ymin) // dy)
     array = np.zeros((Nx, Ny, 3))
@@ -4966,14 +4913,15 @@
     return path
 
 # Return a generic polygon figure in the shape of the given box.
 # Box is specified as [xmin, xmax, ymin, ymax]
 #
 # If optional keyword input `relative` is set to True, the rect
 # will be centered using the `origin` attribute.
+@handleBoxTypecasting
 def rect(box, pad=0, *, relative=False):
     a,b,c,d = box
     a -= pad
     b += pad
     c -= pad
     d += pad
     SW = a + c*1j
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/latex.py` & `morpholib-0.8.0.dev1/src/morpholib/latex.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/matrix.py` & `morpholib-0.8.0.dev1/src/morpholib/matrix.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/sample.py` & `morpholib-0.8.0.dev1/src/morpholib/sample.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/shapes.py` & `morpholib-0.8.0.dev1/src/morpholib/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1386,14 +1386,25 @@
             #     q, qin, qout = self.nodeData(final-1)
             #     m0, m1, m2, m3 = morpho.bezier.bezierFirstSlice(p, pout, qin, q, end-(final-1))
             #     x2,y2 = m2.real, m2.imag
             #     x,y = m3.real, m3.imag
 
             #     ctx.curve_to(x1,y1, x2,y2, x,y)
 
+        # Auto-close path if the path has the simplest possible settings
+        if self.node(0) == self.node(-1) and \
+            self.start == 0 and self.end == 1 and \
+            len(self.deadends) == 0 and \
+            self.headSize == 0 and self.tailSize == 0:
+            # (checking for headSize and tailSize is technically unnecessary
+            # since splines don't have arrow support, BUT THEY MIGHT IN THE FUTURE,
+            # so that's why the checks are here)
+
+            ctx.close_path()
+
         # Stroke and fill the path
         rgba = list(self.color) + [self.alpha*self.alphaEdge]
         if self.width < 0:
             # Draw stroke first, then fill
             self._drawStroke(ctx, rgba)
             with morpho.pushPhysicalCoords(camera.view, ctx):
                 self._drawFill(camera, ctx)
@@ -2382,14 +2393,16 @@
         self.Tweenable("yradius", yradius, tags=["scalar"])
         self.Tweenable("strokeWeight", strokeWeight, tags=["scalar"])
         self.Tweenable("color", list(color), tags=["color"])
         self.Tweenable("fill", list(fill), tags=["color"])
         self.Tweenable("alphaEdge", alphaEdge, tags=["scalar"])
         self.Tweenable("alphaFill", alphaFill, tags=["scalar"])
         self.Tweenable("alpha", alpha, tags=["scalar"])
+        self.Tweenable("dash", [], tags=["scalar", "list"])
+        self.Tweenable("dashOffset", 0, tags=["scalar"])
         self.Tweenable("rotation", 0, tags=["scalar"])
         self.Tweenable("_transform", np.identity(2), tags=["nparray"])
 
 
     @property
     def transform(self):
         return self._transform
@@ -2488,15 +2501,42 @@
         ctx.set_source_rgba(*self.fill, self.alphaFill*self.alpha)
         ctx.fill_preserve()
         if self.strokeWeight < 0.5:  # Don't stroke if strokeWeight is too small
             ctx.new_path()
         else:
             ctx.set_source_rgba(*self.color, self.alphaEdge*self.alpha)
             ctx.set_line_width(self.strokeWeight)
+            ctx.set_dash(self.dash, self.dashOffset)
             ctx.stroke()
+            ctx.set_dash([])
+
+# Animates an Ellipse actor appearing by growing its
+# radii from zero.
+@Ellipse.action
+def popIn(ellipse, duration=30, atFrame=None):
+    if atFrame is None:
+        atFrame = ellipse.lastID()
+
+    ellipse0 = ellipse.last()
+    ellipse0.visible = False
+    ellipse1 = ellipse.newkey(atFrame)
+    ellipse1.visible = True
+    ellipse.newendkey(duration)
+    ellipse1.radius = 0
+
+# Animates an Ellipse actor disappearing by shrinking
+# its radii to zero.
+@Ellipse.action
+def popOut(ellipse, duration=30, atFrame=None):
+    if atFrame is None:
+        atFrame = ellipse.lastID()
+
+    ellipse.newkey(atFrame)
+    ellipse1 = ellipse.newendkey(duration)
+    ellipse1.set(radius=0, visible=False)
 
 
 # Creates an arc of an ellipse.
 # Angles should be interpreted as if the ellipse were a circle.
 # That is, angles refer to a circular arc BEFORE being stretched
 # into an ellipse. They are in units of radians.
 #
@@ -2530,14 +2570,17 @@
         theta1 = morpho.Tweenable("theta1", theta1, tags=["scalar"])
         strokeWeight = morpho.Tweenable("strokeWeight", strokeWeight, tags=["scalar"])
         color = morpho.Tweenable("color", list(color), tags=["color"])
         alpha = morpho.Tweenable("alpha", alpha, tags=["scalar"])
 
         self.extendState([pos, xradius, yradius, theta0, theta1, strokeWeight, color, alpha])
 
+        self.Tweenable("dash", [], tags=["scalar", "list"])
+        self.Tweenable("dashOffset", 0, tags=["scalar"])
+
     # Setting `radius` property sets both `xradius` and `yradius` to
     # the same value.
     @property
     def radius(self):
         if self.xradius != self.yradius:
             raise ValueError("xradius does not equal yradius. No common radius.")
         return self.xradius
@@ -2575,25 +2618,22 @@
         z1 = cmath.exp(theta1*1j)
         seq = [z0]
         for n in range(1, steps):
             seq.append(cmath.exp((theta0+n*dTheta)*1j))
         seq.append(z1)
 
         path = morpho.grid.Path(seq)
-        path.width = self.strokeWeight
-        path.color = self.color[:]
-        path.alpha = self.alpha
 
         # Stretch it into an ellipse and move it
         path = path.fimage(lambda z: mat(self.xradius,0,0,self.yradius)*z)
         # path = path.fimage(lambda z: z + self.pos)
-        path.origin = self.pos
 
-        # Update standard figure meta-settings
-        path._updateSettings(self)
+        path._updateFrom(self, common=True)
+        path.origin = self.pos
+        path.width = self.strokeWeight
 
         return path
 
 
     def draw(self, camera, ctx):
         view = camera.view
 
@@ -2620,15 +2660,17 @@
         ctx.restore()
 
         if self.strokeWeight < 0.5:  # Don't stroke if strokeWeight is too small
             ctx.new_path()
         else:
             ctx.set_source_rgba(*self.color, self.alpha)
             ctx.set_line_width(self.strokeWeight)
+            ctx.set_dash(self.dash, self.dashOffset)
             ctx.stroke()
+            ctx.set_dash([])
 
 # Animates an e-arc actor appearing by "growing in" from theta0
 # toward theta1 unless reverse=True whereby it will grow from
 # theta1 toward theta0.
 #
 # See also: morpho.actions.fadeIn()
 @EllipticalArc.action
@@ -2717,15 +2759,17 @@
         ctx.fill_preserve()
 
         if self.strokeWeight < 0.5:  # Don't stroke if strokeWeight is too small
             ctx.new_path()
         else:
             ctx.set_source_rgba(*self.color, self.alphaEdge*self.alpha)
             ctx.set_line_width(self.strokeWeight)
+            ctx.set_dash(self.dash, self.dashOffset)
             ctx.stroke()
+            ctx.set_dash([])
 
     # Converts the figure into an equivalent Path figure.
     # Optionally specify the angular steps (in rads).
     # Default: 2pi/72 (5 degrees)
     # NOTE: Arc center will be assigned using the `origin`
     # transformation attribute.
     # You will need to call commitTransforms() on the resulting
@@ -2776,29 +2820,21 @@
             innerSeq = [0]
 
         seq.extend(innerSeq)
 
         # Make the polygon
         poly = morpho.grid.Polygon(seq)
 
-        # Style parameters
-        poly.width = self.strokeWeight
-        poly.color = self.color[:]
-        poly.fill = self.fill[:]
-        poly.alphaEdge = self.alphaEdge
-        poly.alphaFill = self.alphaFill
-        poly.alpha = self.alpha
-
         # Stretch it into an ellipse and move it
         poly = poly.fimage(lambda z: mat(self.xradius,0,0,self.yradius)*z)
         # poly = poly.fimage(lambda z: z + self.pos)
-        poly.origin = self.pos
 
-        # Update standard figure meta-settings
-        poly._updateSettings(self)
+        poly._updateFrom(self, common=True)
+        poly.origin = self.pos
+        poly.width = self.strokeWeight
 
         return poly
 
 ### HELPERS ###
 
 # Parses a string of SVG data using svgelements.SVG.parse()
 # and returns the resulting SVG object.
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/text.py` & `morpholib-0.8.0.dev1/src/morpholib/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,78 +207,51 @@
         width = morpho.physicalWidth(WIDTH, view, ctx)
         height = morpho.physicalHeight(HEIGHT, view, ctx)
 
         return (width, height)
 
     # Returns bounding box of the text in physical units.
     # Mainly of use internally to draw the background box.
-    # Note: Ignores rotation and transform, but includes
-    # the prescale factors
-    @typecastViewCtx
-    def box(self, view, ctx, pad=0):
-        width, height = self.dimensions(view, ctx)
-        # Modify by prescale factors
-        width *= self.prescale_x
-        height *= self.prescale_y
-        align_x, align_y = self.anchor_x, self.anchor_y
-        a = self.pos.real - width/2*(align_x + 1)
-        b = a + width
-        c = self.pos.imag - height/2*(align_y + 1)
-        d = c + height
-
-        return [a-pad, b+pad, c-pad, d+pad]
+    def box(self, *args, **kwargs):
+        a,b,c,d = self.relbox(*args, **kwargs)
+        x,y = self.pos.real, self.pos.imag
+        return [a+x, b+x, c+y, d+y]
 
     # Same as box(), but the coordinates are relative to
     # the text's position.
     @typecastViewCtx
-    def relbox(self, view, ctx, pad=0):
+    def relbox(self, view, ctx, pad=0, *, raw=False):
         width, height = self.dimensions(view, ctx)
         # Modify by prescale factors
         width *= self.prescale_x
         height *= self.prescale_y
         align_x, align_y = self.anchor_x, self.anchor_y
         a = -width/2*(align_x + 1)
         b = a + width
         c = -height/2*(align_y + 1)
         d = c + height
 
-        return [a-pad, b+pad, c-pad, d+pad]
-
-    # Returns the four corners of the text's bounding box
-    # plus any optional padding. The sequence of the corners is
-    # NW, SW, SE, NE.
-    @typecastViewCtx
-    def corners(self, view, ctx, pad=0):
-        # NOTE: This method should actually be removable
-        # since its behavior should be identical to the corners()
-        # method inherited from BoundingBoxFigure.
-        a,b,c,d = self.box(view, ctx, pad)
-
-        NW = a + d*1j
-        SW = a + c*1j
-        SE = b + c*1j
-        NE = b + d*1j
-
-        return [NW,SW,SE,NE]
+        if not raw and not(self.rotation == 0 and np.array_equal(self._transform, I2)):
+            return BoundingBoxFigure._transformedBox([a,b,c,d], 0, self.rotation, self._transform, pad)
+        else:
+            return [a-pad, b+pad, c-pad, d+pad]
 
     # Same as corners(), but the coordinates are relative to wherever
     # the text's physical position is.
-    @typecastViewCtx
-    def relcorners(self, view, ctx, pad=0):
-        a,b,c,d = self.relbox(view, ctx, pad)
+    def relcorners(self, *args, **kwargs):
+        a,b,c,d = self.relbox(*args, **kwargs)
 
         NW = a + d*1j
         SW = a + c*1j
         SE = b + c*1j
         NE = b + d*1j
 
         return [NW,SW,SE,NE]
 
-    # Returns the visual centerpoint of the text, ignoring
-    # the transformation attributes.
+    # Returns the visual centerpoint of the text.
     @typecastViewCtx
     def center(self, view, ctx):
         return mean(self.corners(view, ctx))
 
     # Returns the width of the text in pixels.
     def pixelWidth(self):
         return self.pixelDimensions()[0]
@@ -366,15 +339,15 @@
         mat[:,0] *= textWidth*self.prescale_x
         mat[:,1] *= textHeight*self.prescale_y
         if morpho.matrix.thinHeight2x2(mat) < 1:
             return
 
         if self.backAlpha > 0:
             # Construct background rectangle and draw it
-            box = self.relbox(view, ctx, pad=self.backPad)
+            box = self.relbox(view, ctx, pad=self.backPad, raw=True)
             rect = morpho.grid.rect(box)
             rect.origin = self.pos
             rect.width = 0
             rect.fill = self.background
             rect.alpha = self.backAlpha*self.alpha
 
             # Do something special if the viewbox and window shape
@@ -578,62 +551,20 @@
     # `size` attribute in the 2D Text class) for this PText figure
     # given the viewbox and ctx/windowShape.
     @typecastViewCtx
     def fontsize(self, view, ctx):
         # return self._fontRatio*self.pixelHeight(view, ctx)
         return self._fontRatio*morpho.pixelHeight(self.size, view, ctx)
 
-    # Returns bounding box of the text in physical units.
-    # Mainly of use internally to draw the background box.
-    # Note: Ignores rotation and transform, but includes
-    # the prescale factors
-    def box(self, pad=0):
-        return Text.box(self, DUMMY, DUMMY, pad=pad)
-
     # Same as box(), but the coordinates are relative to
     # the text's position.
-    def relbox(self, pad=0):
-        return Text.relbox(self, DUMMY, DUMMY, pad=pad)
+    def relbox(self, pad=0, *, raw=False):
+        return Text.relbox(self, DUMMY, DUMMY, pad=pad, raw=raw)
 
-    # Returns the four corners of the text's bounding box
-    # plus any optional padding. The sequence of the corners is
-    # NW, SW, SE, NE.
-    #
-    # Note: Since the physical width is merely estimated,
-    # x-coordinates of the corners may be slightly off.
-    def corners(self, pad=0):
-        # NOTE: This method should actually be removable
-        # since its behavior should be identical to the corners()
-        # method inherited from BoundingBoxFigure.
-        a,b,c,d = self.box(pad)
-
-        NW = a + d*1j
-        SW = a + c*1j
-        SE = b + c*1j
-        NE = b + d*1j
-
-        return [NW,SW,SE,NE]
-
-    # Same as corners(), but the coordinates are relative to wherever
-    # the text's physical position is.
-    #
-    # Note: Since the physical width is merely estimated,
-    # x-coordinates of the corners may be slightly off.
-    def relcorners(self, pad=0):
-        a,b,c,d = self.relbox(pad)
-
-        NW = a + d*1j
-        SW = a + c*1j
-        SE = b + c*1j
-        NE = b + d*1j
-
-        return [NW,SW,SE,NE]
-
-    # Returns the visual centerpoint of the text, ignoring
-    # the transformation attributes.
+    # Returns the visual centerpoint of the text.
     def center(self):
         return mean(self.corners())
 
     # Returns the "M" physical width of the text.
     # That is, returns the physical width of the current text
     # if it only consisted of the single capital letter "M".
     # Mainly used to help define horizontal spacing relative
@@ -908,20 +839,22 @@
         # # if possible.
         # for n in range(len(self.figures)):
         #     fig = self.figures[n]
         #     if not isinstance(fig, Text):
         #         newfig = fig.images[0].copy()
         #         self.figures[n] = newfig
 
-    # Compute bounding box of the entire figure taking `origin`
-    # attribute into account, but no other transformation attributes.
-    # Returned as [xmin, xmax, ymin, ymax]
     @typecastViewCtx
-    def box(self, view, ctx, pad=0, *, raw=False):
-        return padbox(shiftBox(totalBox(path.box(view, ctx) for path in self.figures), self.origin if not raw else 0), pad)
+    def relbox(self, view, ctx, pad=0):
+        return padbox(totalBox(subfig.box(view, ctx) for subfig in self.figures), pad)
+
+    def box(self, *args, **kwargs):
+        return shiftBox(self.relbox(*args, **kwargs), self.origin)
+
+    relcorners = Text.relcorners
 
     ### TWEEN METHODS ###
 
     tweenLinear = Multi(Text.tweenLinear, morpho.MultiFigure.tweenLinear)
     tweenSpiral = Multi(Text.tweenSpiral, morpho.MultiFigure.tweenSpiral)
 
     @classmethod
@@ -937,15 +870,16 @@
         return pivot
 
 # Physical version of the MultiText class.
 # See MultiText and PText for more info.
 class MultiPText(MultiText):
     _baseFigure = PText
 
-    box = morpho.grid.MultiPath.box
+    def relbox(self, pad=0, *, raw=False):
+        return padbox(totalBox(subfig.box() for subfig in self.figures), pad)
 
     # EXPERIMENTAL! May be changed in a future version!
     # Converts the MultiPText figure into an equivalent MultiSpline.
     # The resulting MultiSpline will have its global origin set to the
     # position of the MultiPText's first component text figure's
     # position. All subsplines will have origin = 0.
     def toSpline(self):
@@ -1440,78 +1374,79 @@
                     raise AttributeError(f"Some component figures have `{name}` attribute and others don't!")
                 # The very first component figure failed to have `name` as
                 # an attribute, so assume `name` is a new attribute name
                 # intended for the main class object, self.
                 else:
                     morpho.Figure.__setattr__(self, name, value)
 
+    # General version of totalBox() that can be used to implement totalBox()
+    # for both FancyMultiText and FancyMultiPText.
+    def _totalBoxGeneral(self, viewctx=(), pad=0, *, raw=False, _verbose=False):
+        boxes = [fig.box(*viewctx, pad=0, raw=False) for fig in self.figures]
+        left = min(box[0] for box in boxes)
+        right = max(box[1] for box in boxes)
+        bottom = min(box[2] for box in boxes)
+        top = max(box[3] for box in boxes)
+        rawbox = [left, right, bottom, top]
+
+        if not raw and not(self.rotation == 0 and np.array_equal(self._transform, I2)):
+            bigbox = BoundingBoxFigure._transformedBox(rawbox, 0, self.rotation, self._transform, pad)
+        else:
+            bigbox = padbox(rawbox, pad)
+
+        if _verbose:
+            return dict(rawbox=rawbox, bigbox=bigbox)
+        return bigbox
+
     # Returns the physical bounding box of the entire text group as
     # [xmin, xmax, ymin, ymax]
     # Note that this is with respect to the group's LOCAL origin,
     # meaning this method does not take the `pos` attribute into
     # account.
     @typecastViewCtx
-    def totalBox(self, view, ctx, pad=0):
-        boxes = [fig.box(view, ctx, pad) for fig in self.figures]
-        left = min(box[0] for box in boxes)
-        right = max(box[1] for box in boxes)
-        bottom = min(box[2] for box in boxes)
-        top = max(box[3] for box in boxes)
-
-        return [left, right, bottom, top]
+    def totalBox(self, view, ctx, *args, **kwargs):
+        return self._totalBoxGeneral((view, ctx), *args, **kwargs)
 
     # Returns the center of the text group's bounding box.
-    @typecastViewCtx
-    def totalCenter(self, view, ctx):
-        box = self.totalBox(view, ctx)
+    def totalCenter(self, *args, **kwargs):
+        box = self.totalBox(*args, **kwargs)
         return mean(box[:2]) + 1j*mean(box[2:])
 
-    # Mainly for internal use by the box() method.
-    # Takes the box outputted by totalBox() and adjusts
-    # it according to the global position and alignment of the
-    # text group so that it now encloses the actual bounding
-    # box of the text group in absolute coordinates.
-    def _alignBox(self, box, *, pad=0):
-        left, right, bottom, top = box
+    # Returns the physical bounding box of the whole text group as
+    # [xmin, xmax, ymin, ymax].
+    def box(self, *args, **kwargs):
+        boxdata = self.totalBox(*args, _verbose=True, **kwargs)
+        rawbox = boxdata["rawbox"]
+        bigbox = boxdata["bigbox"]
+
+        left, right, bottom, top = rawbox
         width = right - left
         height = top - bottom
 
-        offset_x = self.pos.real - self.anchor_x*width/2
-        offset_y = self.pos.imag - self.anchor_y*height/2
-        left += offset_x
-        right += offset_x
-        bottom += offset_y
-        top += offset_y
-
-        return [left-pad, right+pad, bottom-pad, top+pad]
+        alignShift = complex(-self.anchor_x*width/2, -self.anchor_y*height/2)
+        alignShift = morpho.matrix.Mat(self._transform) * (cmath.exp(self.rotation*1j)*alignShift)
 
-    # Returns the physical bounding box of the whole text group as
-    # [xmin, xmax, ymin, ymax]
-    # and takes into account the global position and alignment
-    # properties, but ignores transformation properties.
-    @typecastViewCtx
-    def box(self, view, ctx, pad=0):
-        box = self.totalBox(view, ctx, pad=0)
-        return self._alignBox(box, pad=pad)
+        return shiftBox(bigbox, alignShift+self.pos+self.origin)
 
     corners = Text.corners
 
+    @typecastViewCtx
     def width(self, view, ctx):
-        a,b,c,d = self.box(view, ctx)
+        a,b,c,d = self.box(view, ctx, raw=True)
         return b - a
 
+    @typecastViewCtx
     def height(self, view, ctx):
-        a,b,c,d = self.box(view, ctx)
+        a,b,c,d = self.box(view, ctx, raw=True)
         return d - c
 
     # Moves the text group so that its total center is at the origin.
     # This makes it so the alignment respects the `pos` attribute.
-    @typecastViewCtx
-    def recenter(self, view, ctx):
-        center = self.totalCenter(view, ctx)
+    def recenter(self, *args, **kwargs):
+        center = self.totalCenter(*args, **kwargs)
         for fig in self.figures:
             fig.pos -= center
 
     def _makeFrameFromBoxes(self, boxes, *, ignoreBackground=False):
         left = min(box[0] for box in boxes)
         right = max(box[1] for box in boxes)
         bottom = min(box[2] for box in boxes)
@@ -1547,25 +1482,33 @@
                 )
             rect.origin = self.pos
             rect.width = 0
             rect.fill = self.background
             rect.alpha = self.backAlpha*self.alpha
             rect.rotation = self.rotation
             rect._transform = self._transform
-            return morpho.Frame([rect, MultiText(figs)])
+
+            frm = morpho.Frame([rect, MultiText(figs)])
+            frm.origin = self.origin
+            return frm
 
         return MultiText(figs)
 
-    def makeFrame(self, camera, ctx):
-        boxes = [fig.box(camera, ctx) for fig in self.figures]
+    def makeFrame(self, *args, **kwargs):
+        boxes = [fig.box(*args, **kwargs) for fig in self.figures]
 
         return self._makeFrameFromBoxes(boxes)
 
     def draw(self, camera, ctx):
-        self.makeFrame(camera, ctx).draw(camera, ctx)
+        # NOTE: I *think* `raw=True` can be removed here
+        # which would allow for correct rendering of background
+        # boxes for paragraphs that contain transformed subfigures.
+        # However, I'm not 100% sure yet it's safe to remove
+        # `raw=True`, so that's why it's still here.
+        self.makeFrame(camera, ctx, raw=True).draw(camera, ctx)
 
     ### TWEEN METHODS ###
 
     @morpho.TweenMethod
     def tweenLinear(self, other, t):
         tw = MultiText.tweenLinear(self, other, t)
         return tw
@@ -1606,74 +1549,52 @@
 # Fancy version of MultiPText.
 # See FancyMultiText and MultiPText for more info.
 class FancyMultiPText(FancyMultiText):
     _baseFigure = PText
 
     # Returns the physical bounding box of the entire text group as
     # [xmin, xmax, ymin, ymax]
-    def totalBox(self, pad=0):
-        boxes = [fig.box(pad) for fig in self.figures]
-        left = min(box[0] for box in boxes)
-        right = max(box[1] for box in boxes)
-        bottom = min(box[2] for box in boxes)
-        top = max(box[3] for box in boxes)
-
-        return [left, right, bottom, top]
-
-    # Returns the center of the text group's bounding box.
-    #
-    # The optional arguments `view` and `ctx` do nothing here,
-    # but they exist for internal implementation reasons.
-    def totalCenter(self, view=DUMMY, ctx=DUMMY):
-        box = self.totalBox()
-        return mean(box[:2]) + 1j*mean(box[2:])
-
-    # Returns the physical bounding box of the whole text group as
-    # [xmin, xmax, ymin, ymax]
-    # and takes into account the global position and alignment
-    # properties, but ignores transformation properties.
-    def box(self, pad=0):
-        box = self.totalBox(pad=0)
-        return self._alignBox(box, pad=pad)
+    def totalBox(self, *args, **kwargs):
+        return self._totalBoxGeneral((), *args, **kwargs)
 
     def width(self):
-        a,b,c,d = self.box()
+        a,b,c,d = self.box(raw=True)
         return b - a
 
     def height(self):
-        a,b,c,d = self.box()
+        a,b,c,d = self.box(raw=True)
         return d - c
 
     corners = PText.corners
 
-    # Moves the text group so that its total center is at the origin.
-    # This makes it so the alignment respects the `pos` attribute.
-    #
-    # The optional arguments `view` and `ctx` do nothing here,
-    # but they exist for internal implementation reasons.
-    def recenter(self, view=DUMMY, ctx=DUMMY):
-        FancyMultiText.recenter(self, DUMMY, DUMMY)
-
-    def makeFrame(self, camera=None, ctx=None, *, ignoreBackground=False):
-        boxes = [fig.box() for fig in self.figures]
+    def makeFrame(self, *args, ignoreBackground=False, **kwargs):
+        boxes = [fig.box(*args, **kwargs) for fig in self.figures]
 
         return self._makeFrameFromBoxes(boxes, ignoreBackground=ignoreBackground)
 
     # EXPERIMENTAL! May be changed in a future version!
     # Converts the text figure into an equivalent MultiSpline figure.
     # The origin attribute of the MultiSpline will match the pos
     # attribute of the text figure.
     def toSpline(self):
-        multispline = MultiPText(self.makeFrame(ignoreBackground=True).figures).toSpline()
+        multispline = MultiPText(self.makeFrame(raw=True, ignoreBackground=True).figures).toSpline()
         for spline in multispline.figures:
             spline.origin += multispline.origin - self.pos
             spline.commitTransforms()
         multispline.origin = self.pos
         return multispline
 
+    def draw(self, camera, ctx):
+        # NOTE: I *think* `raw=True` can be removed here
+        # which would allow for correct rendering of background
+        # boxes for paragraphs that contain transformed subfigures.
+        # However, I'm not 100% sure yet it's safe to remove
+        # `raw=True`, so that's why it's still here.
+        self.makeFrame(raw=True).draw(camera, ctx)
+
 FancyMultiPtext = FancyMultiPText
 
 
 # Special class used to render 3D paragraphs.
 # Mainly for internal use by the paragraph3d() function.
 class SpaceParagraph(FancyMultiText):
     _baseMultiFigure = FancyMultiText
@@ -2065,23 +1986,23 @@
     if align is not None:
         anchor_x, anchor_y = align
 
     # Calculate y-positions of all rows
     yPositions = [0]
     rowBoxes = []
     for i, row in enumerate(textarray[:-1]):
-        boxes = [fig.box(*camctx) for fig in row]
+        boxes = [fig.box(*camctx, raw=True) for fig in row]
         rowBoxes.append(boxes)
         rowHeight = max(box[-1]-box[-2] for box in boxes)
         yPositions.append(yPositions[-1]-ygaps[i]-rowHeight)
     adjust = -mean([yPositions[0], yPositions[-1]])
     yPositions = [y+adjust for y in yPositions]
 
     # Append final row of boxes
-    rowBoxes.append([fig.box(*camctx) for fig in textarray[-1]])
+    rowBoxes.append([fig.box(*camctx, raw=True) for fig in textarray[-1]])
 
     # Create rows
     rows = []
     for i, row in enumerate(textarray):
         rowWidth = sum(box[1]-box[0] for box in rowBoxes[i]) + rowgaps[i]
         rowPosition = -morpho.lerp(-rowWidth/2, rowWidth/2, flush, start=-1, end=1) + 1j*yPositions[i]
         if physical:
@@ -2102,15 +2023,15 @@
     parag.anchor_x = anchor_x
     parag.anchor_y = anchor_y
     parag.alpha = alpha
     parag.rotation = rotation
     parag.background = background
     parag.backAlpha = backAlpha
     parag.backPad = backPad
-    parag.recenter(*camctx)
+    parag.recenter(*camctx, raw=True)
 
     return parag
 
 
 # Physical version of paragraph().
 # See paragraph() for more info.
 # Note that this function will auto-convert any non-physical
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/tools/basics.py` & `morpholib-0.8.0.dev1/src/morpholib/tools/basics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,32 @@
 oo = inf = float("inf")
 nan = float("nan")
 # Basic unit vectors for 3D animations
 ihat = np.array([1,0,0], dtype=float)
 jhat = np.array([0,1,0], dtype=float)
 khat = np.array([0,0,1], dtype=float)
 
+### DECORATORS ###
+
+# Decorator for functions that operate on a box.
+# Allows such a function to accept a Figure type input
+# whereby it will attempt to infer a box by calling the
+# figure's `box()` method, assuming it exists.
+# If given an Actor object, it will use the latest keyfigure.
+def handleBoxTypecasting(func):
+    def wrapper(box, *args, **kwargs):
+        if isinstance(box, morpho.Actor):
+            box = box.last()
+        if isinstance(box, morpho.Figure):
+            if not hasattr(box, "box"):
+                raise TypeError(f"`{type(box).__name__}` type figure does not support box() method.")
+            box = box.box()
+        return func(box, *args, **kwargs)
+    return wrapper
+
 ### FUNCTIONS ###
 
 isbadnum_old = lambda x: math.isnan(abs(x)*0)
 
 # Detect infinite or nan (real or complex)
 def isbadnum(x):
     return cmath.isnan(x) or cmath.isinf(x)
@@ -276,14 +294,15 @@
 # returns the corners of the box as a list of complex numbers.
 # Useful for passing into a Path or Polygon figure's seq or vertices.
 # By default, it does so starting at the northwest corner and
 # going counter-clockwise, but this can be modified by altering
 # the "initCorner" and "CCW" parameters. By default:
 # initCorner = "NW"
 # CCW = True
+@handleBoxTypecasting
 def boxCorners(box, initCorner="NW", CCW=True):
     initCorner = initCorner.upper()
     dirs = ["NW", "SW", "SE", "NE"]
     if initCorner not in dirs:
         raise ValueError('initCorner must be "NW", "SW", "SE", or "NE".')
 
     left = box[0]
@@ -309,21 +328,16 @@
 # Pads a bounding box by the given pad amount.
 # Usage: padbox(box, pad) -> paddedBox
 # where `box` is a 4-tuple defining the bounding box in the format
 #       [xmin, xmax, ymin, ymax]
 # Optionally, a ypad value can be specified, allowing the box to be
 # padded differently vertically vs horizontally:
 #       padbox(box, xpad, ypad) -> paddedBox
+@handleBoxTypecasting
 def padbox(box, xpad, ypad=None, /):
-    # Typecast Actors/Figures to box
-    if isinstance(box, morpho.Actor):
-        box = box.last().box()
-    elif isinstance(box, morpho.Figure):
-        box = box.box()
-
     if ypad is None:
         ypad = xpad
 
     box = list(box)
     box[0] -= xpad
     box[1] += xpad
     box[2] -= ypad
@@ -331,21 +345,16 @@
 
     return box
 padBox = padbox  # Alias
 
 # Shifts a bounding box of the form [xmin,xmax,ymin,ymax]
 # by the given 2d vector `shift` expressed as a complex number.
 # Returns the modified box.
+@handleBoxTypecasting
 def shiftBox(box, shift):
-    # Typecast Actors/Figures to box
-    if isinstance(box, morpho.Actor):
-        box = box.last().box()
-    elif isinstance(box, morpho.Figure):
-        box = box.box()
-
     left, right, bottom, top = box
     # Adjust by origin
     left += shift.real
     right += shift.real
     bottom += shift.imag
     top += shift.imag
     return [left, right, bottom, top]
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/tools/dev.py` & `morpholib-0.8.0.dev1/src/morpholib/tools/dev.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,32 @@
 be used by the regular end-user.
 
 An assortment of useful functions and classes.
 '''
 
 import morpholib as morpho
 import morpholib.anim
+from morpholib.figure import object_hasattr
 from morpholib.tools.basics import *
 
 import numpy as np
 import math, cmath
 from collections.abc import Iterable
 
+### SPECIAL EXCEPTIONS ###
+
+# Exception that should be thrown if a dynamically
+# computed value cannot be given a single definite
+# value. For example, trying to get the attribute
+# `tipSize` for a Path whose headSize and tailSize
+# differ.
+class AmbiguousValueError(ValueError):
+    pass
+
+
 # Decorator allows a method to extract the needed
 # `view` and `ctx` parameters from Layer/Camera/Animation
 # inputs allowing for syntax like
 #   mytext.width(my_layer_or_camera, my_animation)
 # whereby `view` will be taken as the latest viewbox in the
 # layer and `windowShape` will be taken from the corresponding
 # attribute in the animation object.
@@ -194,14 +206,143 @@
             brect.set(
                 origin=origin, rotation=rotation,
                 _transform=transform,
                 width=0, fill=self.background, alpha=self.backAlpha*alpha
                 )
             brect.draw(camera, ctx)
 
+    # Returns the bounding box of a box that is being subjected
+    # to a shift, rotation, and transformation.
+    @staticmethod
+    def _transformedBox(box, shift=0, rotation=0, transform=np.eye(2), pad=0):
+        a,b,c,d = box
+        corners = [complex(x,y) for x in [a,b] for y in [c,d]]
+        rotator = cmath.exp(rotation*1j)
+        mat = morpho.matrix.Mat(transform)
+
+        newcorners = [mat*(rotator*z) + shift for z in corners]
+        A = min(z.real for z in newcorners)
+        B = max(z.real for z in newcorners)
+        C = min(z.imag for z in newcorners)
+        D = max(z.imag for z in newcorners)
+
+        return [A-pad, B+pad, C-pad, D+pad]
+
+
+# Mainly for internal use by the Frame class (and its derivatives)
+# for implementing the `all`, `select`, `sub`, and `cut` features.
+# Allows one to modify the attributes of a collection of objects
+# all at once.
+class _SubAttributeManager(object):
+    # `objects` is the sequence of objects whose attributes are
+    # getting accessed/modified en masse.
+    # `origCaller` is the original object that should be returned by
+    # the set() method (usually a Frame object).
+    def __init__(self, objects, origCaller, /):
+        # Bypass native setattr() because it's overridden below.
+        object.__setattr__(self, "_subattrman_objects", objects)
+        object.__setattr__(self, "_subattrman_origCaller", origCaller)
+
+    # Returns a function that when called will call the
+    # corresponding method across all subfigures in the
+    # Frame and collect their return values into a list
+    # which will then be returned.
+    def _subattrman_createSubmethod(self, name):
+        def submethod(*args, **kwargs):
+            outputs = []
+            for obj in self._subattrman_objects:
+                outputs.append(getattr(obj, name)(*args, **kwargs))
+            return outputs
+        return submethod
+
+    def __getattr__(self, name):
+        objects = self._subattrman_objects
+
+        # Extract initial value for the attribute (if possible)
+        try:
+            commonValue = getattr(objects[0], name)
+        except AttributeError:
+            raise AttributeError(f"Objects do not all possess attribute `{name}`")
+        except IndexError:
+            raise IndexError("No objects to find attributes for.")
+
+        commonValue_is_list_or_tuple = isinstance(commonValue, (list, tuple))
+
+        # Check if the attribute is common to all the
+        # objects and having the same value
+        for obj in objects:
+            try:
+                value = getattr(obj, name)
+            except AttributeError:
+                raise AttributeError(f"Objects do not all possess attribute `{name}`")
+
+            if commonValue_is_list_or_tuple and isinstance(value, (list, tuple)):
+                # Convert value to commonValue's type so that cross-container
+                # comparison with commonValue will work
+                value = type(commonValue)(value)
+            # Check if they are unequal
+            if not isequal(value, commonValue):  # isequal() handles np.arrays too
+                if callable(commonValue):
+                    return self._subattrman_createSubmethod(name)
+                raise AmbiguousValueError(f"Objects do not have a common value for attribute `{name}`")
+
+        return commonValue if not isinstance(commonValue, (list, np.ndarray)) else commonValue.copy()
+
+    def __setattr__(self, name, value):
+        # Handle ordinary attribute sets if self possesses
+        # the attribute.
+        if object_hasattr(self, name):
+            object.__setattr__(self, name, value)
+
+        # Set every attribute of the given objects
+        objects = self._subattrman_objects
+        for obj in objects:
+            setattr(obj, name, value)
+
+    def set(self, **kwargs):
+        for name, value in kwargs.items():
+            setattr(self, name, value)
+        return self._subattrman_origCaller
+
+
+class _MetaArray(np.ndarray):
+    """Array with metadata.
+    Thanks to @Bertrand L on StackOverflow for this!
+    https://stackoverflow.com/a/34967782"""
+
+    def __new__(cls, array, dtype=None, order=None, **kwargs):
+        obj = np.asarray(array, dtype=dtype, order=order).view(cls)
+        obj.metadata = kwargs
+        return obj
+
+    def __array_finalize__(self, obj):
+        if obj is None: return
+        self.metadata = getattr(obj, 'metadata', None)
+
+# Special version of _SubAttributeManager which in the case of an
+# AmbiguousValueError, returns a MetaArray of the values across all
+# subfigures. Mainly used for enabling the .iall and .iselect
+# features for subfigure in-place operations.
+class _InPlaceSubAttributeManager(_SubAttributeManager):
+    def __getattr__(self, name):
+        try:
+            return _SubAttributeManager.__getattr__(self, name)
+        except AmbiguousValueError:
+            # A MetaArray is used in order to distinguish these object arrays
+            # from regular numpy object arrays just in case a user is trying
+            # to update a value that is already natively an object array.
+            return _MetaArray([getattr(obj, name) for obj in self._subattrman_objects], dtype=object)
+
+    def __setattr__(self, name, value):
+        if isinstance(value, _MetaArray):
+            for obj, subvalue in zip(self._subattrman_objects, value.tolist()):
+                setattr(obj, name, subvalue)
+        else:
+            _SubAttributeManager.__setattr__(self, name, value)
+
 # Draw a figure whose start or end attribute is outside the interval
 # [0,1] according to the cyclic rules.
 def drawOutOfBoundsStartEnd(fig, camera, ctx):
     diff = fig.end - fig.start
     if diff <= 0:
         return
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/tools/ktimer.py` & `morpholib-0.8.0.dev1/src/morpholib/tools/ktimer.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/tools/latex2svg.py` & `morpholib-0.8.0.dev1/src/morpholib/tools/latex2svg.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/tools/subimporter.py` & `morpholib-0.8.0.dev1/src/morpholib/tools/subimporter.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib/transitions.py` & `morpholib-0.8.0.dev1/src/morpholib/transitions.py`

 * *Files 17% similar despite different names*

```diff
@@ -146,18 +146,55 @@
 default = uniform
 
 # Splits a strictly increasing transition function that maps
 # [0,1] onto [0,1] into two transition functions that are
 # normalized to work as regular transition functions.
 def split(func, t):
     if not(0 < t < 1):
-        raise ValueError("t must be strictly between 0 and 1.")
+        raise ValueError(f"t must be strictly between 0 and 1. Got t={t}")
 
     y = func(t)
 
     def func1(s):
         return func(morpho.lerp0(0,t, s))/y
 
     def func2(s):
         return (func(morpho.lerp0(t,1, s))-y)/(1-y)
 
     return func1, func2
+
+# Mainly for internal use by incorporateTransition().
+# Generates the splitter for the modified tween method
+# returned by incorporateTransition().
+def _generateTransitionSplitter(transition, tweenmethod):
+    def newSplitter(t, beg, mid, fin):
+        trans1, trans2 = split(transition, t)
+
+        if morpho.tweenSplittable(tweenmethod):
+            tweenmethod.splitter(transition(t), beg, mid, fin)
+            basetween1, basetween2 = beg.tweenMethod, mid.tweenMethod
+        else:
+            # Assume the tween method respects splitting
+            basetween1 = basetween2 = tweenmethod
+
+        @morpho.TweenMethod(splitter=_generateTransitionSplitter(trans1, basetween1))
+        def tween1(self, other, t, *args, **kwargs):
+            return basetween1(self, other, trans1(t), *args, **kwargs)
+
+        @morpho.TweenMethod(splitter=_generateTransitionSplitter(trans2, basetween2))
+        def tween2(self, other, t, *args, **kwargs):
+            return basetween2(self, other, trans2(t), *args, **kwargs)
+
+        beg.tweenMethod = tween1
+        mid.tweenMethod = tween2
+    return newSplitter
+
+# Incorporates the given transition function directly into the given
+# tween method, meaning using this tween method with a uniform
+# transition will produce the same effect as the original tween method
+# with the given transition function applied separately.
+# The modified tween method is returned and is not changed in place.
+def incorporateTransition(transition, tweenmethod):
+    @morpho.TweenMethod(splitter=_generateTransitionSplitter(transition, tweenmethod))
+    def newTween(self, other, t, *args, **kwargs):
+        return tweenmethod(self, other, transition(t), *args, **kwargs)
+    return newTween
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib/video.py` & `morpholib-0.8.0.dev1/src/morpholib/video.py`

 * *Files identical despite different names*

### Comparing `morpholib-0.7.1.dev1/src/morpholib.egg-info/PKG-INFO` & `morpholib-0.8.0.dev1/src/morpholib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morpholib
-Version: 0.7.1.dev1
+Version: 0.8.0.dev1
 Summary: A general-purpose programmatic animation tool
 Home-page: https://github.com/morpho-matters/morpholib
 Author: Kenneth Small
 Author-email: morpho.matters@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `morpholib-0.7.1.dev1/src/morpholib.egg-info/SOURCES.txt` & `morpholib-0.8.0.dev1/src/morpholib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


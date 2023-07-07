# Comparing `tmp/objtoolbox-0.0.1.tar.gz` & `tmp/objtoolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objtoolbox-0.0.1.tar", last modified: Mon Jul  3 08:33:02 2023, max compression
+gzip compressed data, was "objtoolbox-0.0.2.tar", last modified: Fri Jul  7 12:15:22 2023, max compression
```

## Comparing `objtoolbox-0.0.1.tar` & `objtoolbox-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-03 08:33:02.141326 objtoolbox-0.0.1/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 objtoolbox-0.0.1/LICENSE
--rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-03 08:33:02.141326 objtoolbox-0.0.1/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      212 2023-07-03 08:00:36.000000 objtoolbox-0.0.1/README.md
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      562 2023-07-03 08:26:33.000000 objtoolbox-0.0.1/pyproject.toml
--rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-07-03 08:33:02.141326 objtoolbox-0.0.1/setup.cfg
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-03 08:33:02.137326 objtoolbox-0.0.1/src/
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-03 08:33:02.137326 objtoolbox-0.0.1/src/objtoolbox/
--rw-r--r--   0 ruof      (1000) ruof      (1000)      128 2023-07-03 08:22:06.000000 objtoolbox-0.0.1/src/objtoolbox/__init__.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1737 2023-07-03 08:07:25.000000 objtoolbox-0.0.1/src/objtoolbox/merge.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)    12284 2023-07-03 08:26:22.000000 objtoolbox-0.0.1/src/objtoolbox/storage.py
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1668 2023-07-03 08:22:00.000000 objtoolbox-0.0.1/src/objtoolbox/utils.py
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-03 08:33:02.141326 objtoolbox-0.0.1/src/objtoolbox.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-03 08:33:02.000000 objtoolbox-0.0.1/src/objtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 ruof      (1000) ruof      (1000)      322 2023-07-03 08:33:02.000000 objtoolbox-0.0.1/src/objtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-07-03 08:33:02.000000 objtoolbox-0.0.1/src/objtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       25 2023-07-03 08:33:02.000000 objtoolbox-0.0.1/src/objtoolbox.egg-info/requires.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-07-03 08:33:02.000000 objtoolbox-0.0.1/src/objtoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 objtoolbox-0.0.2/LICENSE
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      212 2023-07-03 08:00:36.000000 objtoolbox-0.0.2/README.md
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      562 2023-07-07 09:38:49.000000 objtoolbox-0.0.2/pyproject.toml
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/setup.cfg
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/src/
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/src/objtoolbox/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      128 2023-07-03 08:22:06.000000 objtoolbox-0.0.2/src/objtoolbox/__init__.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1774 2023-07-06 15:29:36.000000 objtoolbox-0.0.2/src/objtoolbox/merge.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)    12284 2023-07-03 08:26:22.000000 objtoolbox-0.0.2/src/objtoolbox/storage.py
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2233 2023-07-07 12:14:09.000000 objtoolbox-0.0.2/src/objtoolbox/utils.py
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-07-07 12:15:22.257209 objtoolbox-0.0.2/src/objtoolbox.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      632 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      322 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       25 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/requires.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-07-07 12:15:22.000000 objtoolbox-0.0.2/src/objtoolbox.egg-info/top_level.txt
```

### Comparing `objtoolbox-0.0.1/LICENSE` & `objtoolbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `objtoolbox-0.0.1/PKG-INFO` & `objtoolbox-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtoolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Advanced utility functions for python objects
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/objtoolbox
 Project-URL: Bug Tracker, https://github.com/joruof/objtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `objtoolbox-0.0.1/pyproject.toml` & `objtoolbox-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "objtoolbox"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jona Ruof", email="jona.ruof@uni-ulm.de" },
 ]
 description = "Advanced utility functions for python objects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `objtoolbox-0.0.1/src/objtoolbox/merge.py` & `objtoolbox-0.0.2/src/objtoolbox/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import copy
 
+from objtoolbox import get_obj_dict
+
 
 def merge(dst, src):
     """
     For a given destination and source object this synchronizes both objects,
     by copying from the source into the destination object (in-place), while
     keeping the destination object structure unchanged.
     """
```

### Comparing `objtoolbox-0.0.1/src/objtoolbox/storage.py` & `objtoolbox-0.0.2/src/objtoolbox/storage.py`

 * *Files identical despite different names*

### Comparing `objtoolbox-0.0.1/src/objtoolbox/utils.py` & `objtoolbox-0.0.2/src/objtoolbox/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,42 @@
         if res is None:
             res = obj[p]
         obj = res
 
     return obj
 
 
+def set_value_by_path(obj, path, value):
+    """
+    This set a value in a given object, where the specific value
+    can be adressed by a path given as either
+
+    "/obj_list/0/sub_obj/value_a" or ["obj_list", 0, "sub_obj", "value_a"].
+    """
+
+    if type(path) == str:
+        path = to_path_list(path)
+
+    if path == []:
+        return
+
+    sub = get_value_by_path(obj, path[:-1])
+
+    p = path[-1]
+
+    if type(p) == str:
+        try:
+            setattr(sub, p, value)
+            return
+        except AttributeError:
+            pass
+
+    sub[p] = value
+
+
 def to_path_list(path):
     """
     This converts from a path string to a path list.
     """
 
     path = path.strip()
     pl = []
```

### Comparing `objtoolbox-0.0.1/src/objtoolbox.egg-info/PKG-INFO` & `objtoolbox-0.0.2/src/objtoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objtoolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Advanced utility functions for python objects
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/objtoolbox
 Project-URL: Bug Tracker, https://github.com/joruof/objtoolbox/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


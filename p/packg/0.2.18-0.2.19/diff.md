# Comparing `tmp/packg-0.2.18.tar.gz` & `tmp/packg-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.18.tar", last modified: Thu Jul  6 08:49:20 2023, max compression
+gzip compressed data, was "packg-0.2.19.tar", last modified: Fri Jul  7 08:51:04 2023, max compression
```

## Comparing `packg-0.2.18.tar` & `packg-0.2.19.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.366962 packg-0.2.18/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.18/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-06 08:49:20.366962 packg-0.2.18/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-06 08:46:49.000000 packg-0.2.18/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.18/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-06 08:46:49.000000 packg-0.2.18/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-06 08:49:20.366962 packg-0.2.18/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.242959 packg-0.2.18/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.302960 packg-0.2.18/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7270 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.362961 packg-0.2.18/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      592 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/compressed.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/gitmatcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5493 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/paths.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/strings.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-06 08:46:49.000000 packg-0.2.18/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-06 08:49:20.322960 packg-0.2.18/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      733 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-06 08:49:20.000000 packg-0.2.18/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.18/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 08:51:04.953815 packg-0.2.19/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.19/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-07 08:51:04.953815 packg-0.2.19/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-07 08:50:11.000000 packg-0.2.19/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.19/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 08:50:11.000000 packg-0.2.19/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-07 08:51:04.957815 packg-0.2.19/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 08:51:04.833812 packg-0.2.19/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 08:51:04.889813 packg-0.2.19/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8349 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 08:51:04.949814 packg-0.2.19/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      592 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/compressed.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3779 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5493 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/paths.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/strings.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-07 08:50:11.000000 packg-0.2.19/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-07 08:51:04.909814 packg-0.2.19/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-07 08:51:04.000000 packg-0.2.19/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      733 2023-07-07 08:51:04.000000 packg-0.2.19/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-07 08:51:04.000000 packg-0.2.19/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 08:51:04.000000 packg-0.2.19/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-07 08:51:04.000000 packg-0.2.19/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.19/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.18/LICENSE` & `packg-0.2.19/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/PKG-INFO` & `packg-0.2.19/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.18
+Version: 0.2.19
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.18 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.19 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.18/README.md` & `packg-0.2.19/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/pyproject.toml` & `packg-0.2.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/caching.py` & `packg-0.2.19/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/constclass.py` & `packg-0.2.19/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/debugging.py` & `packg-0.2.19/src/packg/debugging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/import_from_source.py` & `packg-0.2.19/src/packg/import_from_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,23 +24,31 @@
 
 
     @pytest.mark.parametrize("module", module_list)
     def test_imports_from_source(module: str) -> None:
         print(f"Importing: {module}")
         apply_visitor(module=module, visitor=ImportFromSourceChecker(module))
 
+Notes:
+    - Currently does not respect try/except blocks around the imports and throws errors anyway
+        - This functionality looks difficult to implement
+        - Workaround: pass the list of false positives like this:
+          ImportFromSourceChecker(module, module_list_to_ignore_not_found=["module.submodule"])
+          Then all ModuleNotFoundErrors where the module name starts with a module in this list
+          will be ignored.
+
 
 """
 import logging
 from ast import parse, NodeVisitor, ImportFrom
 from importlib import util as import_util, import_module
 from importlib.machinery import ModuleSpec
 from os import path
 from pkgutil import iter_modules
-from typing import Any, List, Iterator
+from typing import Any, List, Iterator, Optional
 
 
 def _is_test_module(module_name: str) -> bool:
     components = module_name.split(".")
 
     return len(components) >= 2 and components[1] == "tests"
 
@@ -67,22 +75,23 @@
                     packages_only=packages_only,
                 )
             elif not packages_only:
                 yield f"{module_name}.{child.name}"
 
 
 class _ImportFromSourceChecker(NodeVisitor):
-    def __init__(self, module: str):
+    def __init__(self, module: str, module_list_to_ignore_not_found: Optional[List] = None):
         module_spec = import_util.find_spec(module)
         is_pkg = (module_spec is not None
                   and module_spec.origin is not None
                   and module_spec.origin.endswith("__init__.py"))
 
         self._module = module if is_pkg else ".".join(module.split(".")[:-1])
         self._top_level_module = self._module.split(".")[0]
+        self._module_list_to_ignore_not_found = module_list_to_ignore_not_found
 
     def visit_ImportFrom(self, node: ImportFrom) -> Any:
         # Check that there are no relative imports that attempt to read from a parent module. We've found that there
         # generally is no good reason to have such imports.
         if node.level >= 2:
             raise ValueError(
                 f"Import in {self._module} attempts to import from parent module using relative import. Please "
@@ -102,15 +111,24 @@
             module_to_import = f"{self._module}.{node.module}"
 
         # We're only looking at imports of objects defined inside this top-level package
         if not module_to_import.startswith(self._top_level_module):
             return
 
         # Actually import the module and iterate through all the objects potentially exported by it.
-        module = import_module(module_to_import)
+        print(f"    Importing module: {module_to_import}")
+        try:
+            module = import_module(module_to_import)
+        except ModuleNotFoundError as e:
+            if self._module_list_to_ignore_not_found is not None:
+                for module_to_ignore_not_found in self._module_list_to_ignore_not_found:
+                    if module_to_import.startswith(module_to_ignore_not_found):
+                        print(f"        Ignore missing module: {module_to_import}")
+                        return
+            raise e
         for alias in node.names:
             # assert hasattr(module, alias.name), f"Imported {alias.name} from {module_to_import}, but this object does not exist. in {module}"
             if not hasattr(module, alias.name):
                 if alias.name == "*":
                     continue
                 attr = import_module(f"{module_to_import}.{alias.name}")
             else:
```

### Comparing `packg-0.2.18/src/packg/iotools/__init__.py` & `packg-0.2.19/src/packg/iotools/__init__.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/iotools/jsonext.py` & `packg-0.2.19/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.19/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/iotools/misc.py` & `packg-0.2.19/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/iotools/yamlext.py` & `packg-0.2.19/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/log.py` & `packg-0.2.19/src/packg/log.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/paths.py` & `packg-0.2.19/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/strings.py` & `packg-0.2.19/src/packg/strings.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/system.py` & `packg-0.2.19/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/tensors.py` & `packg-0.2.19/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg/typext.py` & `packg-0.2.19/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.18/src/packg.egg-info/PKG-INFO` & `packg-0.2.19/src/packg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.18
+Version: 0.2.19
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.18 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.19 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.18/src/packg.egg-info/SOURCES.txt` & `packg-0.2.19/src/packg.egg-info/SOURCES.txt`

 * *Files identical despite different names*


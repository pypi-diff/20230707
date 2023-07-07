# Comparing `tmp/ansys_mechanical_core-0.9.1.tar.gz` & `tmp/ansys_mechanical_core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_mechanical_core-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_mechanical_core-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_mechanical_core-0.9.1.tar` & `ansys_mechanical_core-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1089 2023-06-21 20:01:07.489448 ansys_mechanical_core-0.9.1/LICENSE
--rw-r--r--   0        0        0     5448 2023-06-21 20:01:07.489448 ansys_mechanical_core-0.9.1/README.rst
--rw-r--r--   0        0        0     4042 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1236 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      138 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     4266 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     3697 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     6761 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/__init__.py
--rw-r--r--   0        0        0     4603 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/environ.py
--rw-r--r--   0        0        0     4834 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/linux_api.py
--rw-r--r--   0        0        0      238 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/sinks.py
--rw-r--r--   0        0        0     4094 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/windows_api.py
--rw-r--r--   0        0        0      852 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2990 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    78531 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25279 2023-06-21 20:01:07.497448 ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-07 14:00:26.682650 ansys_mechanical_core-0.9.2/LICENSE
+-rw-r--r--   0        0        0     5448 2023-07-07 14:00:26.682650 ansys_mechanical_core-0.9.2/README.rst
+-rw-r--r--   0        0        0     4042 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      138 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     4793 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     6568 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     6761 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/__init__.py
+-rw-r--r--   0        0        0     4603 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/environ.py
+-rw-r--r--   0        0        0     4834 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/linux_api.py
+-rw-r--r--   0        0        0      238 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/sinks.py
+-rw-r--r--   0        0        0     4094 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/windows_api.py
+-rw-r--r--   0        0        0      852 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2990 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    78531 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25279 2023-07-07 14:00:26.694651 ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.2/PKG-INFO
```

### Comparing `ansys_mechanical_core-0.9.1/LICENSE` & `ansys_mechanical_core-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/README.rst` & `ansys_mechanical_core-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/pyproject.toml` & `ansys_mechanical_core-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.9.1"
+version = "0.9.2"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -44,33 +44,33 @@
 Documentation = "https://mechanical.docs.pyansys.com"
 Source = "https://github.com/ansys/pymechanical"
 Homepage = "https://github.com/ansys/pymechanical"
 Tracker = "https://github.com/ansys/pymechanical/issues"
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.3.2",
+    "pytest==7.4.0",
     "pytest-cov==4.1.0",
-    "pytest-print==0.3.2",
+    "pytest-print==0.3.3",
 ]
 doc = [
     "Sphinx==6.2.1", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
     "ansys-sphinx-theme==0.9.9",
-    "grpcio==1.54.2",
+    "grpcio==1.56.0",
     "imageio-ffmpeg==0.4.8",
     "imageio==2.31.1",
     "jupyter_sphinx==0.4.0",
     "jupyterlab>=3.2.8",
     "matplotlib==3.7.1",
     "numpydoc==1.5.0",
     "plotly==5.15.0",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
-    "pyvista==0.39.1",
+    "pyvista==0.40.0",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.0",
     "sphinx-copybutton==0.5.2",
     "sphinx_design==0.4.1",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
```

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/__init__.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/_version.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/app.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Main application class for embedded Mechanical."""
 import atexit
 import os
+import shutil
 
 from ansys.mechanical.core.embedding import initializer, runtime
 from ansys.mechanical.core.embedding.config import Configuration, configure
 
 
 def _get_default_configuration() -> Configuration:
     configuration = Configuration()
@@ -18,22 +19,30 @@
 
 def _dispose_embedded_app(instances):  # pragma: nocover
     if len(instances) > 0:
         instance = instances[0]
         instance._dispose()
 
 
+def _cleanup_private_appdata(folder):
+    shutil.rmtree(folder, ignore_errors=True)
+
+
 class App:
     """Mechanical embedding Application."""
 
-    def __init__(self, db_file=None, **kwargs):
+    def __init__(self, db_file=None, private_appdata=False, **kwargs):
         """Construct an instance of the mechanical Application.
 
         db_file is an optional path to a mechanical database file (.mechdat or .mechdb)
         you may set a version number with the `version` keyword argument.
+
+        private_appdata is an optional setting for a temporary AppData directory.
+        By default, private_appdata is False. This is beneficial for running parallel
+        instances of mechanical.
         """
         global INSTANCES
         from ansys.mechanical.core import BUILDING_GALLERY
 
         if BUILDING_GALLERY:
             if len(INSTANCES) != 0:
                 self._app = INSTANCES[0]
@@ -48,14 +57,20 @@
         import clr
 
         clr.AddReference("Ansys.Mechanical.Embedding")
         import Ansys
 
         configuration = kwargs.get("config", _get_default_configuration())
         configure(configuration)
+
+        if private_appdata:
+            self.pid = os.getpid()
+            self.tmp_dir = initializer.set_private_appdata(self.pid)
+            atexit.register(_cleanup_private_appdata, self.tmp_dir)
+
         self._app = Ansys.Mechanical.Embedding.Application(db_file)
         runtime.initialize(self._version)
         self._disposed = False
         atexit.register(_dispose_embedded_app, INSTANCES)
         INSTANCES.append(self)
 
     def __repr__(self):
```

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/config.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/imports.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/loader.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/__init__.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/environ.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/environ.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/linux_api.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/linux_api.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/logger/windows_api.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/logger/windows_api.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/resolver.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/runtime.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/embedding/shims.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/errors.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/examples/downloads.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/launcher.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/logging.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/mechanical.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/mechanical.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/misc.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/src/ansys/mechanical/core/pool.py` & `ansys_mechanical_core-0.9.2/src/ansys/mechanical/core/pool.py`

 * *Files identical despite different names*

### Comparing `ansys_mechanical_core-0.9.1/PKG-INFO` & `ansys_mechanical_core-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -22,37 +22,37 @@
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: protobuf>=3.12.2,<3.21.0
 Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: tqdm>=4.45.0
 Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
-Requires-Dist: grpcio==1.54.2 ; extra == "doc"
+Requires-Dist: grpcio==1.56.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: jupyterlab>=3.2.8 ; extra == "doc"
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: plotly==5.15.0 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pythreejs==2.4.2 ; extra == "doc"
-Requires-Dist: pyvista==0.39.1 ; extra == "doc"
+Requires-Dist: pyvista==0.40.0 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx_design==0.4.1 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
-Requires-Dist: pytest==7.3.2 ; extra == "tests"
+Requires-Dist: pytest==7.4.0 ; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
-Requires-Dist: pytest-print==0.3.2 ; extra == "tests"
+Requires-Dist: pytest-print==0.3.3 ; extra == "tests"
 Project-URL: Documentation, https://mechanical.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/pymechanical
 Project-URL: Source, https://github.com/ansys/pymechanical
 Project-URL: Tracker, https://github.com/ansys/pymechanical/issues
 Provides-Extra: doc
 Provides-Extra: tests
```


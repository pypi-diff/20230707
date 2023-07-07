# Comparing `tmp/edwh_pipcompile_plugin-0.2.1.tar.gz` & `tmp/edwh_pipcompile_plugin-0.2.2.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.2.1.tar` & `edwh_pipcompile_plugin-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/README.md
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/README.md
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.2/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.2.1/CHANGELOG.md` & `edwh_pipcompile_plugin-0.2.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.2 (2023-07-07)
+
+### Fix
+
+* `pip-compile` executable sometimes not found ([`50677e7`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/50677e7da3e049cc823af43dd93652b0a1ec5048))
+
 ## v0.2.1 (2023-05-31)
 
 
 ## v0.2.0 (2023-05-08)
 ### Feature
 * Import main tasks to __init__ so this plugin can be used as a library ([`61611cf`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/61611cf0f795221615e4e802bf8209280b1ef854))
```

### Comparing `edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.2.2/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,37 @@
 kunnen doen. Compile werkt hetzelfde, maar het is fijn om alle related commando's onder invoke pip.* te hebben.
 """
 
 import glob
 import typing
 from dataclasses import dataclass
 import re
+
+from edwh.meta import _python
 from invoke import run, task
 from pathlib import Path
 from difflib import unified_diff
 
 DEFAULT_SERVER = None  # pypi default
 
 
+def pip_compile_executable(python: str = None):
+    # python = '/home/eddie/.local/pipx/venvs/edwh/bin/python'
+    # -> /home/eddie/.local/pipx/venvs/edwh/bin/pip-compile
+    if python is None:
+        python = _python()
+
+    command_parts = python.split("/")
+    command_parts[-1] = "pip-compile"
+    return "/".join(command_parts)
+
+
+PIP_COMPILE = pip_compile_executable()
+
+
 # DEFAULT_SERVER = "https://devpi.edwh.nl/remco/dev/+simple"
 
 # DEFAULT_OUT = 'py4web_requirements.txt'
 
 
 class Color:
     """
@@ -172,15 +188,15 @@
 def _pip_compile(*args, **kwargs):
     """
     Execute pip-compile with positional and keyword args
     """
     if "resolver" not in kwargs:
         kwargs["resolver"] = "backtracking"
 
-    run("pip-compile " + " ".join(args) + kwargs_to_options(kwargs))
+    run(f"{PIP_COMPILE} " + " ".join(args) + kwargs_to_options(kwargs))
 
 
 def _find_infiles(directory: str | Path = None) -> typing.Iterator:
     """
     Iterate over files ending with .in (in the current directory)
     """
```

### Comparing `edwh_pipcompile_plugin-0.2.1/LICENSE.txt` & `edwh_pipcompile_plugin-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.2.1/README.md` & `edwh_pipcompile_plugin-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.2.1/pyproject.toml` & `edwh_pipcompile_plugin-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['invoke', "pip-tools"]
 
 [project.optional-dependencies]
 dev = [
+  "edwh",
   "hatch",
   # "python-semantic-release",
   "black",
 ]
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme"
```

### Comparing `edwh_pipcompile_plugin-0.2.1/PKG-INFO` & `edwh_pipcompile_plugin-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.2.1
+Version: 0.2.2
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: invoke
 Requires-Dist: pip-tools
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
+Requires-Dist: edwh; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-pipcompile-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
```


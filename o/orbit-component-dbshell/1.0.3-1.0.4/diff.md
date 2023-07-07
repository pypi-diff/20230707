# Comparing `tmp/orbit_component_dbshell-1.0.3.tar.gz` & `tmp/orbit_component_dbshell-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_dbshell-1.0.3.tar", max compression
+gzip compressed data, was "orbit_component_dbshell-1.0.4.tar", max compression
```

## Comparing `orbit_component_dbshell-1.0.3.tar` & `orbit_component_dbshell-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-17 16:50:03.098236 orbit_component_dbshell-1.0.3/LICENSE.md
--rw-r--r--   0        0        0        0 2023-06-21 15:30:58.376561 orbit_component_dbshell-1.0.3/README.md
--rw-r--r--   0        0        0       82 2023-06-21 12:41:11.901965 orbit_component_dbshell-1.0.3/orbit_component_dbshell/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-29 12:45:49.668149 orbit_component_dbshell-1.0.3/orbit_component_dbshell/plugin.py
--rw-r--r--   0        0        0     1253 2023-06-29 13:20:52.412275 orbit_component_dbshell-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 orbit_component_dbshell-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 16:50:03.098236 orbit_component_dbshell-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-06-21 15:30:58.376561 orbit_component_dbshell-1.0.4/README.md
+-rw-r--r--   0        0        0       82 2023-06-21 12:41:11.901965 orbit_component_dbshell-1.0.4/orbit_component_dbshell/__init__.py
+-rw-r--r--   0        0        0      515 2023-07-06 17:21:12.797206 orbit_component_dbshell-1.0.4/orbit_component_dbshell/plugin.py
+-rw-r--r--   0        0        0     1254 2023-07-07 15:12:03.390268 orbit_component_dbshell-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 orbit_component_dbshell-1.0.4/PKG-INFO
```

### Comparing `orbit_component_dbshell-1.0.3/pyproject.toml` & `orbit_component_dbshell-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-dbshell"
-version = "1.0.3"
+version = "1.0.4"
 description = "Orbit Database shell component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_dbshell"}]
 classifiers = [
@@ -21,16 +21,16 @@
 documentation = "https://gitlab.com/madpenguin/orbit-component-dbshell"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-component-dbshell"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-component-dbshell/-/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-orbit-database-shell = "^1.0.0"
+python = ">=3.10, <4"
+orbit-database-shell = "^1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `orbit_component_dbshell-1.0.3/PKG-INFO` & `orbit_component_dbshell-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: orbit-component-dbshell
-Version: 1.0.3
+Version: 1.0.4
 Summary: Orbit Database shell component
 Home-page: https://gitlab.com/madpenguin/orbit-component-dbshell
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: orbit-database-shell (>=1.0.0,<2.0.0)
+Requires-Dist: orbit-database-shell (>=1,<2)
 Project-URL: Documentation, https://gitlab.com/madpenguin/orbit-component-dbshell
 Project-URL: Repository, https://gitlab.com/madpenguin/orbit-component-dbshell
 Description-Content-Type: text/markdown
```


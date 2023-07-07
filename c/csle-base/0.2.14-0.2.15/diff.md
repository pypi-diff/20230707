# Comparing `tmp/csle_base-0.2.14.tar.gz` & `tmp/csle_base-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_base-0.2.14.tar", last modified: Sat Jun 10 14:00:35 2023, max compression
+gzip compressed data, was "csle_base-0.2.15.tar", last modified: Fri Jul  7 09:36:53 2023, max compression
```

## Comparing `csle_base-0.2.14.tar` & `csle_base-0.2.15.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-10 14:00:35.732807 csle_base-0.2.14/
--rw-rw-r--   0 kim       (1000) kim       (1000)      664 2023-06-10 14:00:35.732807 csle_base-0.2.14/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3888 2023-06-10 13:33:21.000000 csle_base-0.2.14/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      670 2023-06-10 13:33:21.000000 csle_base-0.2.14/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1173 2023-06-10 14:00:35.732807 csle_base-0.2.14/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_base-0.2.14/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-10 14:00:35.732807 csle_base-0.2.14/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-10 14:00:35.732807 csle_base-0.2.14/src/csle_base/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_base-0.2.14/src/csle_base/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       23 2023-06-10 14:00:30.000000 csle_base-0.2.14/src/csle_base/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1537 2023-06-10 13:41:34.000000 csle_base-0.2.14/src/csle_base/json_serializable.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-06-10 14:00:35.732807 csle_base-0.2.14/src/csle_base.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      664 2023-06-10 14:00:35.000000 csle_base-0.2.14/src/csle_base.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      353 2023-06-10 14:00:35.000000 csle_base-0.2.14/src/csle_base.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-10 14:00:35.000000 csle_base-0.2.14/src/csle_base.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-06-10 13:43:53.000000 csle_base-0.2.14/src/csle_base.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      158 2023-06-10 14:00:35.000000 csle_base-0.2.14/src/csle_base.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       10 2023-06-10 14:00:35.000000 csle_base-0.2.14/src/csle_base.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 09:36:53.835092 csle_base-0.2.15/
+-rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 09:36:53.835219 csle_base-0.2.15/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     3391 2023-06-28 07:40:45.000000 csle_base-0.2.15/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      670 2023-06-11 13:17:52.000000 csle_base-0.2.15/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1222 2023-07-07 09:36:53.835799 csle_base-0.2.15/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2023-06-11 13:17:52.000000 csle_base-0.2.15/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 09:36:53.826904 csle_base-0.2.15/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 09:36:53.832094 csle_base-0.2.15/src/csle_base/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2023-06-11 13:17:52.000000 csle_base-0.2.15/src/csle_base/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       23 2023-07-07 09:36:45.000000 csle_base-0.2.15/src/csle_base/__version__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      574 2023-06-16 06:45:51.000000 csle_base-0.2.15/src/csle_base/grpc_serializable.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1537 2023-06-11 13:17:52.000000 csle_base-0.2.15/src/csle_base/json_serializable.py
+-rw-r--r--   0 kimham     (501) staff       (20)      713 2023-06-16 06:45:51.000000 csle_base-0.2.15/src/csle_base/kafka_serializable.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-07-07 09:36:53.834843 csle_base-0.2.15/src/csle_base.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      664 2023-07-07 09:36:53.000000 csle_base-0.2.15/src/csle_base.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      424 2023-07-07 09:36:53.000000 csle_base-0.2.15/src/csle_base.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 09:36:53.000000 csle_base-0.2.15/src/csle_base.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-07-07 09:36:52.000000 csle_base-0.2.15/src/csle_base.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      204 2023-07-07 09:36:53.000000 csle_base-0.2.15/src/csle_base.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       10 2023-07-07 09:36:53.000000 csle_base-0.2.15/src/csle_base.egg-info/top_level.txt
```

### Comparing `csle_base-0.2.14/PKG-INFO` & `csle_base-0.2.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_base
-Version: 0.2.14
+Version: 0.2.15
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_base-0.2.14/README.md` & `csle_base-0.2.15/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,75 +16,46 @@
 - `tox` (for automated testing)
 - `pytest` (for unit tests)
 - `pytest-cov` (for unit test coverage)
 - `mypy` (for static typing)
 - `sphinx` (for API documentation)
 - `sphinxcontrib-napoleon` (for API documentation)
 - `sphinx-rtd-theme` (for API documentation)
+- `pytest-mock` (for mocking tests)
+- `pytest-grpc` (for grpc tests)
 
 ## Installation
 
 ```bash
 # install from pip
 pip install csle-base==<version>
 # local install from source
 $ pip install -e csle-base
 # or (equivalently):
 make install
 # force upgrade deps
 $ pip install -e csle-base --upgrade
-
 # git clone and install from source
 git clone https://github.com/Limmen/csle
 cd csle/simulation-system/libs/csle-base
 pip3 install -e .
+# Install development dependencies
+$ pip install -r requirements_dev.txt
 ```
 
 ### Development tools 
 
 Install all development tools at once:
 ```bash
 make install_dev
 ```
-
-Install the Python build tool
-```bash
-pip install -q build
-```
-
-Install `twine` for publishing the package to PyPi:
-```bash
-python3 -m pip install --upgrade twine
-```
-
-Install the `flake8` linter:
-```bash
-python -m pip install flake8
-```
-
-Install the mypy for static type checking:
+or
 ```bash
-python3 -m pip install -U mypy
+pip install -r requirements_dev.txt
 ```
-
-Install `pytest` and `mock` for unit tests:
-```bash
-pip install -U pytest mock pytest-mock pytest-cov
-```
-
-Install Sphinx to automatically generate API documentation from docstrings:
-```bash
-pip install sphinx sphinxcontrib-napoleon sphinx-rtd-theme
-```
-
-Install tox for automatically running tests in different python environments:
-```bash
-pip install tox
-```
-
 ## API documentation
 
 This section contains instructions for generating API documentation using `sphinx`.
 
 ### Latest Documentation
 
 The latest documentation is available at [https://limmen.dev/csle/docs/csle-base](https://limmen.dev/csle/docs/csle-base)
```

### Comparing `csle_base-0.2.14/pyproject.toml` & `csle_base-0.2.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.14/setup.cfg` & `csle_base-0.2.15/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,23 @@
 where = src
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
 	pytest-cov>=2.0
 	pytest-mock>=3.6.0
-	mypy>=0.910
+	pytest-grpc>=0.8.0
+	mypy>=1.3.0
 	flake8>=3.9
 	tox>=3.24
 	sphinx>=5.3.0
 	sphinxcontrib-napoleon>=0.7
 	sphinx-rtd-theme>=1.1.1
+	twine>=4.0.2
+	build>=0.10.0
 
 [options.package_data]
 csle_ryu = py.typed
 
 [flake8]
 max-line-length = 120
 exclude = .git,__pycache__,docs/source/conf.py,old,build,dist,*_pb2*,*init__*
```

### Comparing `csle_base-0.2.14/src/csle_base/json_serializable.py` & `csle_base-0.2.15/src/csle_base/json_serializable.py`

 * *Files identical despite different names*

### Comparing `csle_base-0.2.14/src/csle_base.egg-info/PKG-INFO` & `csle_base-0.2.15/src/csle_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-base
-Version: 0.2.14
+Version: 0.2.15
 Summary: Library with base classes and definitions for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```


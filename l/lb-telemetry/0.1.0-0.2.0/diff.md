# Comparing `tmp/lb-telemetry-0.1.0.tar.gz` & `tmp/lb-telemetry-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb-telemetry-0.1.0.tar", last modified: Wed Jul  5 14:24:36 2023, max compression
+gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-svmt_l_3/lb-telemetry-0.2.0.tar", last modified: Fri Jul  7 16:05:16 2023, max compression
```

## Comparing `lb-telemetry-0.1.0.tar` & `lb-telemetry-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.366642 lb-telemetry-0.1.0/
--rw-r--r--   0 cmcclymont   (501) staff       (20)     2191 2023-07-05 13:43:47.000000 lb-telemetry-0.1.0/.gitignore
--rw-r--r--   0 cmcclymont   (501) staff       (20)     2084 2023-07-05 13:55:01.000000 lb-telemetry-0.1.0/.gitlab-ci.yml
--rw-r--r--   0 cmcclymont   (501) staff       (20)       37 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/.mypy.ini
--rw-r--r--   0 cmcclymont   (501) staff       (20)      657 2023-07-05 13:58:55.000000 lb-telemetry-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 cmcclymont   (501) staff       (20)    18151 2023-06-22 14:51:29.000000 lb-telemetry-0.1.0/.pylintrc
--rw-r--r--   0 cmcclymont   (501) staff       (20)    35065 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/LICENSE
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1359 2023-07-05 14:24:36.366470 lb-telemetry-0.1.0/PKG-INFO
--rw-r--r--   0 cmcclymont   (501) staff       (20)      705 2023-06-26 11:09:24.000000 lb-telemetry-0.1.0/README.md
--rw-r--r--   0 cmcclymont   (501) staff       (20)      979 2023-07-05 14:22:15.000000 lb-telemetry-0.1.0/pyproject.toml
--rw-r--r--   0 cmcclymont   (501) staff       (20)      156 2023-07-05 13:51:18.000000 lb-telemetry-0.1.0/requirements.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)       38 2023-07-05 14:24:36.366687 lb-telemetry-0.1.0/setup.cfg
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.364670 lb-telemetry-0.1.0/src/
--rw-r--r--   0 cmcclymont   (501) staff       (20)        0 2023-06-26 11:25:27.000000 lb-telemetry-0.1.0/src/__init__.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.365282 lb-telemetry-0.1.0/src/lb_telemetry/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       21 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/src/lb_telemetry/__init__.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)       41 2023-06-27 12:07:56.000000 lb-telemetry-0.1.0/src/lb_telemetry/log_fetch_error.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)     5447 2023-07-05 12:56:41.000000 lb-telemetry-0.1.0/src/lb_telemetry/logger.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.366214 lb-telemetry-0.1.0/src/lb_telemetry/tests/
--rw-r--r--   0 cmcclymont   (501) staff       (20)       60 2023-06-22 14:51:30.000000 lb-telemetry-0.1.0/src/lb_telemetry/tests/__init__.py
--rw-r--r--   0 cmcclymont   (501) staff       (20)     5203 2023-07-05 13:32:53.000000 lb-telemetry-0.1.0/src/lb_telemetry/tests/test_logger.py
-drwxr-xr-x   0 cmcclymont   (501) staff       (20)        0 2023-07-05 14:24:36.365869 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/
--rw-r--r--   0 cmcclymont   (501) staff       (20)     1359 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 cmcclymont   (501) staff       (20)      460 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)        1 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 cmcclymont   (501) staff       (20)       22 2023-07-05 14:24:36.000000 lb-telemetry-0.1.0/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/src/lb_telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/src/lb_telemetry/log_fetch_error.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/src/lb_telemetry/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 16:05:16.000000 lb-telemetry-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-07-07 16:05:08.000000 lb-telemetry-0.2.0/tests/test_logger.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `lb-telemetry-0.1.0/.gitignore` & `lb-telemetry-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.1.0/.gitlab-ci.yml` & `lb-telemetry-0.2.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,52 +5,46 @@
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 
-image: gitlab-registry.cern.ch/ci-tools/ci-worker:cc7
+image: registry.cern.ch/docker.io/library/python:3.11
 
 stages:
   - lint
   - test
   - build
   - deploy
 
 before_script:
   - source /cvmfs/lhcb.cern.ch/lib/LbEnv
   - python -m venv .venv
   - source .venv/bin/activate
-  - pip install -r requirements.txt
-  - pip install -e .
+  - pip install -e .[dev]
 
 pre_commit:
   stage: lint
+  before_script:
+    - pip install pre-commit
   script:
     - pre-commit run --all-files
-  allow_failure: true
-
-ruff:
-  stage: lint
-  script:
-    - ruff check src/lb_telemetry --fix
-  allow_failure: true
 
 mypy:
   stage: lint
   script:
     - mypy src/lb_telemetry --explicit-package-bases
   allow_failure: true
 
 tests:
   stage: test
   needs: []
   script:
-    - python -m pytest src/lb_telemetry/tests/ -v
+    - python -m pytest tests/ -v
   coverage: '/TOTAL.*\s+(\d+%)$/'
 
 package:
   stage: build
   image: gitlab-registry.cern.ch/lhcb-docker/python-deployment:python-3.7
   script:
     - python -m build
```

### Comparing `lb-telemetry-0.1.0/.pre-commit-config.yaml` & `lb-telemetry-0.2.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,17 @@
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: no-commit-to-branch
         args: [--branch, master]
 
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: v0.0.277
     hooks:
       - id: ruff
+        args: ["--fix"]
```

### Comparing `lb-telemetry-0.1.0/.pylintrc` & `lb-telemetry-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.1.0/LICENSE` & `lb-telemetry-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.1.0/PKG-INFO` & `lb-telemetry-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.1.0
+Version: 0.2.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # lb-telemetry
 
 A utility for logging telemetry data about LHCb packages to [MONIT](https://monit.web.cern.ch/).
 Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46).
```

### Comparing `lb-telemetry-0.1.0/README.md` & `lb-telemetry-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.1.0/pyproject.toml` & `lb-telemetry-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 [project]
 name = "lb-telemetry"
-version = "0.1.0"
+#version = "0.1.0"
+dynamic = ["version"]
 authors = [
     {name="Cameron McClymont", email="cameron.duncan.mcclymont@cern.ch"},
     {name="Daniel Cervenkov", email="daniel.cervenkov@cern.ch"},
     {name="Chris Burr", email="christopher.burr@cern.ch"},
 ]
 description = "A utility for logging telemetry data from LHCb packages to MONIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "logzero",
+    "requests",
+]
+
+[tool.setuptools_scm]
 
 [project.urls]
 "Homepage" = "https://gitlab.cern.ch/lhcb/lb-telemetry"
 "Bug Tracker" = "https://gitlab.cern.ch/lhcb/lb-telemetry/issues"
 
 [build-system]
 requires = [
-    "setuptools >= 30.3.0",
+    "setuptools >= 61",
     "wheel",
-    "setuptools_scm[toml] >= 3.4"
+    "setuptools_scm[toml] >= 3.4",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = [
     "-ra",
     "-q",
     "--cov=src/lb_telemetry"
 ]
-testpaths = [
-    "src/lb_telemetry/tests",
+
+[project.optional-dependencies]
+dev = [
+    "mypy",
+    "mypy-extensions",
+    "pre-commit",
+    "pytest",
+    "pytest-cov",
+    "ruff",
+    "types-requests"
 ]
```

### Comparing `lb-telemetry-0.1.0/src/lb_telemetry/logger.py` & `lb-telemetry-0.2.0/src/lb_telemetry/logger.py`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.1.0/src/lb_telemetry/tests/test_logger.py` & `lb-telemetry-0.2.0/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import json
 import time
 from typing import Optional
 
 import requests
 from logzero import logger as logzero
 
-from src.lb_telemetry.log_fetch_error import LogFetchError
-from src.lb_telemetry.logger import INFLUXDB_LEGAL_TYPES, Logger
+from lb_telemetry.log_fetch_error import LogFetchError
+from lb_telemetry.logger import INFLUXDB_LEGAL_TYPES, Logger
 
 TEST_TABLE = "testing"
 TEST_DATA = {
     "test_field1": "test_value",
     "test_field2": False,
     "test_field3": 0,
     "test_field4": 3.5,
```

### Comparing `lb-telemetry-0.1.0/src/lb_telemetry.egg-info/PKG-INFO` & `lb-telemetry-0.2.0/src/lb_telemetry.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.1.0
+Version: 0.2.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # lb-telemetry
 
 A utility for logging telemetry data about LHCb packages to [MONIT](https://monit.web.cern.ch/).
 Usage data graphs specific to each package can be viewed on the [MONIT Grafana](https://monit-grafana.cern.ch/d/Q78h6E-nz/home?orgId=46).
```


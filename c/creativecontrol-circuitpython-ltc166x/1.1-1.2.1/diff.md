# Comparing `tmp/creativecontrol-circuitpython-ltc166x-1.1.tar.gz` & `tmp/creativecontrol-circuitpython-ltc166x-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.1.tar", last modified: Mon May 29 17:40:35 2023, max compression
+gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.2.1.tar", last modified: Fri Jul  7 02:37:00 2023, max compression
```

## Comparing `creativecontrol-circuitpython-ltc166x-1.1.tar` & `creativecontrol-circuitpython-ltc166x-1.2.1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/examples/creativecontrol_circuitpython_ltc166x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.718333 creativecontrol-circuitpython-ltc166x-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.718333 creativecontrol-circuitpython-ltc166x-1.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.718333 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:37:00.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_list_selective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_single_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_single_value_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-07 02:36:52.000000 creativecontrol-circuitpython-ltc166x-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 02:36:43.000000 creativecontrol-circuitpython-ltc166x-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:37:00.722333 creativecontrol-circuitpython-ltc166x-1.2.1/setup.cfg
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `creativecontrol-circuitpython-ltc166x-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_gh.yml` & `creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_pypi.yml` & `creativecontrol-circuitpython-ltc166x-1.2.1/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/.gitignore` & `creativecontrol-circuitpython-ltc166x-1.2.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -45,7 +45,10 @@
 # IDE-specific files
 .idea
 .vscode
 *~
 
 # PYPI Dist
 dist
+
+# VS Code Workspace
+*.code-workspace
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/.pre-commit-config.yaml` & `creativecontrol-circuitpython-ltc166x-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/.pylintrc` & `creativecontrol-circuitpython-ltc166x-1.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/CODE_OF_CONDUCT.md` & `creativecontrol-circuitpython-ltc166x-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/LICENSE` & `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/CC-BY-4.0.txt` & `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/MIT.txt` & `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/Unlicense.txt` & `creativecontrol-circuitpython-ltc166x-1.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 1.1
+Version: 1.2.1
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/README.rst` & `creativecontrol-circuitpython-ltc166x-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.2.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 1.1
+Version: 1.2.1
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/examples/creativecontrol_circuitpython_ltc166x_simpletest.py` & `creativecontrol-circuitpython-ltc166x-1.2.1/examples/creativecontrol_circuitpython_ltc166x_dac_value_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 # SPDX-FileCopyrightText: Copyright (c) 2023 Thadeus Frazier-Reed for creativecontrol
 #
 # SPDX-License-Identifier: Unlicense
 
+"""
+Write individual values to all DAC channels from a list.
+"""
+
 import time
 import board
 import creativecontrol_circuitpython_ltc166x
 
 ltc1665 = creativecontrol_circuitpython_ltc166x.LTC1665(
-    csld=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True
+    csel=board.GP1, sck=board.GP2, mosi=board.GP3, debug=True
 )
 
 dac_values = [1, 3, 7, 15, 31, 63, 127, 255]
 
 while True:
     print("writing dac values ", time.monotonic())
     ltc1665.write_dac_values(dac_values)
```

### Comparing `creativecontrol-circuitpython-ltc166x-1.1/pyproject.toml` & `creativecontrol-circuitpython-ltc166x-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "creativecontrol-circuitpython-ltc166x"
 description = "CircuitPython library for control of LTC166X 8-bit and 10-bit DACs."
-version = "01.1"
+version = "1.2.1"
 readme = "README.rst"
 authors = [
     {name = "creativecontrol", email = "t@creativecontrol.cc"}
 ]
 urls = {Homepage = "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X"}
 keywords = [
     "adafruit",
```


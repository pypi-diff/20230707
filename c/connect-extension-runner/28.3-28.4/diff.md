# Comparing `tmp/connect_extension_runner-28.3.tar.gz` & `tmp/connect_extension_runner-28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_extension_runner-28.3.tar", max compression
+gzip compressed data, was "connect_extension_runner-28.4.tar", max compression
```

## Comparing `connect_extension_runner-28.3.tar` & `connect_extension_runner-28.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/LICENSE
--rw-r--r--   0        0        0     1422 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/README.md
--rw-r--r--   0        0        0       55 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/dataclasses.py
--rw-r--r--   0        0        0      405 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/extension.py
--rw-r--r--   0        0        0      143 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/artworks/__init__.py
--rw-r--r--   0        0        0     9409 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/artworks/ansi_regular.flf
--rw-r--r--   0        0        0      950 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/artworks/banner.py
--rw-r--r--   0        0        0    11425 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/artworks/bloody.flf
--rw-r--r--   0        0        0     6483 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/config.py
--rw-r--r--   0        0        0     5708 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/constants.py
--rw-r--r--   0        0        0      320 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/handlers/__init__.py
--rw-r--r--   0        0        0     2692 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/handlers/anvil.py
--rw-r--r--   0        0        0     4391 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/handlers/base.py
--rw-r--r--   0        0        0     3751 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/handlers/events.py
--rw-r--r--   0        0        0     2444 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/handlers/transformations.py
--rw-r--r--   0        0        0     7175 2023-07-06 15:41:03.941961 connect_extension_runner-28.3/connect/eaas/runner/handlers/web.py
--rw-r--r--   0        0        0    18982 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/helpers.py
--rw-r--r--   0        0        0     1989 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/main.py
--rw-r--r--   0        0        0      340 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/__init__.py
--rw-r--r--   0        0        0     3190 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/background.py
--rw-r--r--   0        0        0     8100 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/base.py
--rw-r--r--   0        0        0     2225 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/interactive.py
--rw-r--r--   0        0        0     1931 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/scheduled.py
--rw-r--r--   0        0        0    20665 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/transformation.py
--rw-r--r--   0        0        0      533 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/managers/utils.py
--rw-r--r--   0        0        0     7917 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/master.py
--rw-r--r--   0        0        0        0 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/workers/__init__.py
--rw-r--r--   0        0        0     2549 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/workers/anvil.py
--rw-r--r--   0        0        0    11320 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/workers/base.py
--rw-r--r--   0        0        0     8834 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/workers/events.py
--rw-r--r--   0        0        0     6545 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/workers/transformations.py
--rw-r--r--   0        0        0     7038 2023-07-06 15:41:03.945962 connect_extension_runner-28.3/connect/eaas/runner/workers/web.py
--rw-r--r--   0        0        0     2870 2023-07-06 15:42:27.440713 connect_extension_runner-28.3/pyproject.toml
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 connect_extension_runner-28.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/LICENSE
+-rw-r--r--   0        0        0     1422 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/README.md
+-rw-r--r--   0        0        0       55 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/dataclasses.py
+-rw-r--r--   0        0        0      405 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/extension.py
+-rw-r--r--   0        0        0      143 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/artworks/__init__.py
+-rw-r--r--   0        0        0     9409 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/artworks/ansi_regular.flf
+-rw-r--r--   0        0        0      950 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/artworks/banner.py
+-rw-r--r--   0        0        0    11425 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/artworks/bloody.flf
+-rw-r--r--   0        0        0     6483 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/config.py
+-rw-r--r--   0        0        0     5708 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/constants.py
+-rw-r--r--   0        0        0      320 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/anvil.py
+-rw-r--r--   0        0        0     4391 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/base.py
+-rw-r--r--   0        0        0     3751 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/events.py
+-rw-r--r--   0        0        0     2444 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/transformations.py
+-rw-r--r--   0        0        0     7175 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/web.py
+-rw-r--r--   0        0        0    18982 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/helpers.py
+-rw-r--r--   0        0        0     1989 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/main.py
+-rw-r--r--   0        0        0      340 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/__init__.py
+-rw-r--r--   0        0        0     3190 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/background.py
+-rw-r--r--   0        0        0     8100 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/base.py
+-rw-r--r--   0        0        0     2225 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/interactive.py
+-rw-r--r--   0        0        0     1931 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/scheduled.py
+-rw-r--r--   0        0        0    20665 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/transformation.py
+-rw-r--r--   0        0        0      533 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/utils.py
+-rw-r--r--   0        0        0     7917 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/master.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/__init__.py
+-rw-r--r--   0        0        0     2549 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/anvil.py
+-rw-r--r--   0        0        0    11320 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/base.py
+-rw-r--r--   0        0        0     8834 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/events.py
+-rw-r--r--   0        0        0     6545 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/transformations.py
+-rw-r--r--   0        0        0     7038 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/web.py
+-rw-r--r--   0        0        0     2870 2023-07-07 07:59:44.431392 connect_extension_runner-28.4/pyproject.toml
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 connect_extension_runner-28.4/PKG-INFO
```

### Comparing `connect_extension_runner-28.3/LICENSE` & `connect_extension_runner-28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/README.md` & `connect_extension_runner-28.4/README.md`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/artworks/ansi_regular.flf` & `connect_extension_runner-28.4/connect/eaas/runner/artworks/ansi_regular.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/artworks/banner.py` & `connect_extension_runner-28.4/connect/eaas/runner/artworks/banner.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/artworks/bloody.flf` & `connect_extension_runner-28.4/connect/eaas/runner/artworks/bloody.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/config.py` & `connect_extension_runner-28.4/connect/eaas/runner/config.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/constants.py` & `connect_extension_runner-28.4/connect/eaas/runner/constants.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/handlers/anvil.py` & `connect_extension_runner-28.4/connect/eaas/runner/handlers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/handlers/base.py` & `connect_extension_runner-28.4/connect/eaas/runner/handlers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/handlers/events.py` & `connect_extension_runner-28.4/connect/eaas/runner/handlers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/handlers/transformations.py` & `connect_extension_runner-28.4/connect/eaas/runner/handlers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/handlers/web.py` & `connect_extension_runner-28.4/connect/eaas/runner/handlers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/helpers.py` & `connect_extension_runner-28.4/connect/eaas/runner/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/main.py` & `connect_extension_runner-28.4/connect/eaas/runner/main.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/managers/background.py` & `connect_extension_runner-28.4/connect/eaas/runner/managers/background.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/managers/base.py` & `connect_extension_runner-28.4/connect/eaas/runner/managers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/managers/interactive.py` & `connect_extension_runner-28.4/connect/eaas/runner/managers/interactive.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/managers/scheduled.py` & `connect_extension_runner-28.4/connect/eaas/runner/managers/scheduled.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/managers/transformation.py` & `connect_extension_runner-28.4/connect/eaas/runner/managers/transformation.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/managers/utils.py` & `connect_extension_runner-28.4/connect/eaas/runner/managers/utils.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/master.py` & `connect_extension_runner-28.4/connect/eaas/runner/master.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/workers/anvil.py` & `connect_extension_runner-28.4/connect/eaas/runner/workers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/workers/base.py` & `connect_extension_runner-28.4/connect/eaas/runner/workers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/workers/events.py` & `connect_extension_runner-28.4/connect/eaas/runner/workers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/workers/transformations.py` & `connect_extension_runner-28.4/connect/eaas/runner/workers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/connect/eaas/runner/workers/web.py` & `connect_extension_runner-28.4/connect/eaas/runner/workers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.3/pyproject.toml` & `connect_extension_runner-28.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-extension-runner"
-version = "28.3"
+version = "28.4"
 description = "CloudBlue Connect EaaS Extension Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
@@ -27,15 +27,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 websockets = "10.*"
 connect-openapi-client = ">=25.16"
 logzio-python-handler = "^3.1.1"
 backoff = "^2.2.1"
-connect-eaas-core = ">=28.7,<29"
+connect-eaas-core = ">=28.9,<29"
 httpx = ">=0.23,<0.25"
 rich = ">=12"
 pyfiglet = "^0.8.post1"
 devtools = "^0.10.0"
 watchfiles = "^0.19.0"
 openpyxl = ">=3.0.0,<4"
 lxml = "^4.9.2"
```

### Comparing `connect_extension_runner-28.3/PKG-INFO` & `connect_extension_runner-28.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-extension-runner
-Version: 28.3
+Version: 28.4
 Summary: CloudBlue Connect EaaS Extension Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: connect-eaas-core (>=28.7,<29)
+Requires-Dist: connect-eaas-core (>=28.9,<29)
 Requires-Dist: connect-openapi-client (>=25.16)
 Requires-Dist: devtools (>=0.10.0,<0.11.0)
 Requires-Dist: httpx (>=0.23,<0.25)
 Requires-Dist: logzio-python-handler (>=3.1.1,<4.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: openpyxl (>=3.0.0,<4)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
```


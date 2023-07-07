# Comparing `tmp/async_mvg_api-0.1.5.tar.gz` & `tmp/async_mvg_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_mvg_api-0.1.5.tar", max compression
+gzip compressed data, was "async_mvg_api-0.2.0.tar", max compression
```

## Comparing `async_mvg_api-0.1.5.tar` & `async_mvg_api-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,33 @@
--rw-r--r--   0        0        0    35184 2022-12-10 11:36:21.271710 async_mvg_api-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2022-12-03 15:42:09.092422 async_mvg_api-0.1.5/mvg_api/__init__.py
--rw-r--r--   0        0        0        0 2022-11-29 14:00:44.819142 async_mvg_api-0.1.5/mvg_api/api/__init__.py
--rw-r--r--   0        0        0     7128 2023-06-25 21:31:14.999622 async_mvg_api-0.1.5/mvg_api/api/api.py
--rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.1.5/mvg_api/models/__init__.py
--rw-r--r--   0        0        0     5774 2023-06-25 21:52:42.316969 async_mvg_api-0.1.5/mvg_api/models/route.py
--rw-r--r--   0        0        0     1572 2022-12-02 23:40:22.454153 async_mvg_api-0.1.5/mvg_api/models/ticker.py
--rw-r--r--   0        0        0     6922 2023-06-25 21:56:29.413298 async_mvg_api-0.1.5/mvg_api/mvg.py
--rw-r--r--   0        0        0        0 2022-12-02 17:39:31.765071 async_mvg_api-0.1.5/mvg_api/tests/__init__.py
--rw-r--r--   0        0        0     2591 2023-06-25 21:30:53.746385 async_mvg_api-0.1.5/mvg_api/tests/api_tests.py
--rw-r--r--   0        0        0    21521 2023-06-25 22:01:03.402019 async_mvg_api-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1404 2022-12-09 23:56:14.842549 async_mvg_api-0.1.5/README.md
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 async_mvg_api-0.1.5/setup.py
--rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 async_mvg_api-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-10 11:36:21.271710 async_mvg_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-03 15:42:09.092422 async_mvg_api-0.2.0/mvg_api/v1/__init__.py
+-rw-r--r--   0        0        0     7136 2023-07-05 22:20:04.280607 async_mvg_api-0.2.0/mvg_api/v1/api.py
+-rw-r--r--   0        0        0     6929 2023-07-05 22:20:04.275525 async_mvg_api-0.2.0/mvg_api/v1/mvg.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.2.0/mvg_api/v1/schemas/__init__.py
+-rw-r--r--   0        0        0     5774 2023-06-25 21:52:42.316969 async_mvg_api-0.2.0/mvg_api/v1/schemas/route.py
+-rw-r--r--   0        0        0     1572 2022-12-02 23:40:22.454153 async_mvg_api-0.2.0/mvg_api/v1/schemas/ticker.py
+-rw-r--r--   0        0        0        0 2022-12-02 17:39:31.765071 async_mvg_api-0.2.0/mvg_api/v1/tests/__init__.py
+-rw-r--r--   0        0        0     2601 2023-07-05 22:18:47.123247 async_mvg_api-0.2.0/mvg_api/v1/tests/api_tests.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:44.819142 async_mvg_api-0.2.0/mvg_api/v2/__init__.py
+-rw-r--r--   0        0        0    35087 2023-07-07 10:40:14.255069 async_mvg_api-0.2.0/mvg_api/v2/api.py
+-rw-r--r--   0        0        0     8002 2023-07-07 10:35:32.794185 async_mvg_api-0.2.0/mvg_api/v2/mvg.py
+-rw-r--r--   0        0        0        0 2022-11-29 14:00:22.839034 async_mvg_api-0.2.0/mvg_api/v2/schemas/__init__.py
+-rw-r--r--   0        0        0      270 2023-07-06 10:58:33.665856 async_mvg_api-0.2.0/mvg_api/v2/schemas/aushang.py
+-rw-r--r--   0        0        0     1590 2023-07-06 18:28:45.552947 async_mvg_api-0.2.0/mvg_api/v2/schemas/connection.py
+-rw-r--r--   0        0        0      591 2023-06-29 23:31:23.767271 async_mvg_api-0.2.0/mvg_api/v2/schemas/departure.py
+-rw-r--r--   0        0        0     1027 2023-07-06 08:58:07.349245 async_mvg_api-0.2.0/mvg_api/v2/schemas/ems.py
+-rw-r--r--   0        0        0      270 2023-06-29 23:40:15.772185 async_mvg_api-0.2.0/mvg_api/v2/schemas/line.py
+-rw-r--r--   0        0        0      304 2023-06-29 23:35:51.159905 async_mvg_api-0.2.0/mvg_api/v2/schemas/lineinfo.py
+-rw-r--r--   0        0        0      814 2023-07-07 08:19:47.823067 async_mvg_api-0.2.0/mvg_api/v2/schemas/location.py
+-rw-r--r--   0        0        0      585 2023-07-05 23:29:30.417705 async_mvg_api-0.2.0/mvg_api/v2/schemas/messages.py
+-rw-r--r--   0        0        0      225 2023-07-06 10:52:03.482021 async_mvg_api-0.2.0/mvg_api/v2/schemas/out_of_order.py
+-rw-r--r--   0        0        0      302 2023-06-29 23:29:29.475391 async_mvg_api-0.2.0/mvg_api/v2/schemas/station.py
+-rw-r--r--   0        0        0      439 2023-06-29 23:39:45.995814 async_mvg_api-0.2.0/mvg_api/v2/schemas/stations.py
+-rw-r--r--   0        0        0      407 2023-07-06 10:56:01.184390 async_mvg_api-0.2.0/mvg_api/v2/schemas/surounding_plans.py
+-rw-r--r--   0        0        0      530 2023-06-29 23:32:55.501012 async_mvg_api-0.2.0/mvg_api/v2/schemas/transportdevice.py
+-rw-r--r--   0        0        0      666 2023-07-06 10:56:01.173385 async_mvg_api-0.2.0/mvg_api/v2/schemas/vehicel.py
+-rw-r--r--   0        0        0      389 2023-07-06 08:58:07.348246 async_mvg_api-0.2.0/mvg_api/v2/schemas/zoom_station.py
+-rw-r--r--   0        0        0     7082 2023-07-07 08:16:19.927087 async_mvg_api-0.2.0/mvg_api/v2/tests/api_tests.py
+-rw-r--r--   0        0        0    21682 2023-07-07 10:48:01.634755 async_mvg_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16171 2023-07-07 10:28:53.645532 async_mvg_api-0.2.0/README.md
+-rw-r--r--   0        0        0    17100 1970-01-01 00:00:00.000000 async_mvg_api-0.2.0/setup.py
+-rw-r--r--   0        0        0    16331 1970-01-01 00:00:00.000000 async_mvg_api-0.2.0/PKG-INFO
```

### Comparing `async_mvg_api-0.1.5/LICENSE` & `async_mvg_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.5/mvg_api/api/api.py` & `async_mvg_api-0.2.0/mvg_api/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, List
 import datetime
 
 import httpx
-from mvg_api.models.ticker import TickerList, SlimList
-from mvg_api.models.route import Connections, LocationList
+from mvg_api.v1.schemas.ticker import TickerList, SlimList
+from mvg_api.v1.schemas.route import Connections, LocationList
 
 
 class RequestFailed(Exception):
     pass
 
 
 class Api:
```

### Comparing `async_mvg_api-0.1.5/mvg_api/models/route.py` & `async_mvg_api-0.2.0/mvg_api/v1/schemas/route.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.5/mvg_api/models/ticker.py` & `async_mvg_api-0.2.0/mvg_api/v1/schemas/ticker.py`

 * *Files identical despite different names*

### Comparing `async_mvg_api-0.1.5/mvg_api/mvg.py` & `async_mvg_api-0.2.0/mvg_api/v1/mvg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 from typing import List
 
 from Levenshtein import ratio
 
-from mvg_api.api.api import Api, AsyncApi
-from mvg_api.models.route import Location, LocationType, Connections, LocationList
-from mvg_api.models.ticker import TickerList, SlimList
+from mvg_api.v1.api import Api, AsyncApi
+from mvg_api.v1.schemas.route import Location, LocationType, Connections, LocationList
+from mvg_api.v1.schemas.ticker import TickerList, SlimList
 
 
 class LocationNotFound(Exception):
     """
     If there is no locations that matches the input String this exception is raised
     """
```

### Comparing `async_mvg_api-0.1.5/mvg_api/tests/api_tests.py` & `async_mvg_api-0.2.0/mvg_api/v1/tests/api_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import datetime
 from typing import List
 
-from mvg_api.api.api import Api, AsyncApi
-from mvg_api.mvg import LocationNotFound
-from mvg_api.models.route import LocationList, LocationType, Connections
-from mvg_api.models.ticker import TickerList, SlimList
+from mvg_api.v1.api import Api, AsyncApi
+from mvg_api.v1.mvg import LocationNotFound
+from mvg_api.v1.schemas.route import LocationList, LocationType, Connections
+from mvg_api.v1.schemas.ticker import TickerList, SlimList
 
 
 def test_get_ticker():
     api = Api()
     response = api.get_ticker()
     assert isinstance(response, TickerList)
```

### Comparing `async_mvg_api-0.1.5/pyproject.toml` & `async_mvg_api-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 [tool.poetry]
 name = "async_mvg_api"
-version = "0.1.5"
+version = "0.2.0"
 description = ""
 authors = ["Lukas Mahr <lukas@yousuckatprogramming.de>"]
 readme = "README.md"
 packages = [{include = "mvg_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.7"
 httpx = "^0.24.0"
 levenshtein = "^0.21.0"
 black = "^23.3.0"
 pylint = "^2.15.7"
 pytest = "^7.2.0"
+dill = "^0.3.6"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "mvg_api",
+]
+
 [tool.pylint.main]
 # Analyse import fallback blocks. This can be used to support both Python 2 and 3
 # compatible code, which means that the block might have code that exists only in
 # one or another interpreter, leading to false positives when analysed.
 # analyse-fallback-blocks =
 
 # Always return a 0 (non-error) status code, even if lint errors are found. This
@@ -71,15 +77,15 @@
 # for modules/projects where namespaces are manipulated during runtime and thus
 # existing member attributes cannot be deduced by static analysis). It supports
 # qualified module names, as well as Unix pattern matching.
 # ignored-modules =
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
-# init-hook =
+init-hook = 'import sys; sys.path.append("."); sys.path.append("mvg_api")'
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
 # avoid hangs.
 jobs = 0
 
 # Control the amount of potential inferred values when inferring a single object.
@@ -363,15 +369,15 @@
 # multiple times (only on the command line, not in the configuration file where
 # it should appear only once). You can also use "--disable=all" to disable
 # everything first and then re-enable specific checks. For example, if you want
 # to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use "--disable=all --enable=classes
 # --disable=W".
-disable = ["missing-function-docstring","missing-class-docstring","missing-module-docstring", "raw-checker-failed", "bad-inline-option", "locally-disabled", "file-ignored", "suppressed-message", "useless-suppression", "deprecated-pragma", "use-symbolic-message-instead"]
+disable = ["similarities", "missing-function-docstring","missing-class-docstring","missing-module-docstring", "raw-checker-failed", "bad-inline-option", "locally-disabled", "file-ignored", "suppressed-message", "useless-suppression", "deprecated-pragma", "use-symbolic-message-instead"]
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where it
 # should appear only once). See also the "--disable" option for examples.
 enable = ["c-extension-no-member"]
```


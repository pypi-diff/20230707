# Comparing `tmp/zavod-0.7.2.tar.gz` & `tmp/zavod-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zavod-0.7.2.tar", last modified: Mon Jul  3 10:09:51 2023, max compression
+gzip compressed data, was "zavod-0.7.3.tar", last modified: Fri Jul  7 12:28:19 2023, max compression
```

## Comparing `zavod-0.7.2.tar` & `zavod-0.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.432818 zavod-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-03 10:07:53.000000 zavod-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 10:07:53.000000 zavod-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 10:09:51.432818 zavod-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-03 10:07:53.000000 zavod-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 10:09:51.432818 zavod-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-03 10:07:53.000000 zavod-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.428818 zavod-0.7.2/zavod/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.428818 zavod-0.7.2/zavod/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/parse/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.432818 zavod-0.7.2/zavod/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/json_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/sinks/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-03 10:07:53.000000 zavod-0.7.2/zavod/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 10:09:51.428818 zavod-0.7.2/zavod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 10:09:35.000000 zavod-0.7.2/zavod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 10:09:51.000000 zavod-0.7.2/zavod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:28:19.854915 zavod-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-07 12:26:24.000000 zavod-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 12:26:24.000000 zavod-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 12:28:19.854915 zavod-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-07 12:26:24.000000 zavod-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:28:19.854915 zavod-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-07 12:26:24.000000 zavod-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:28:19.854915 zavod-0.7.3/zavod/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:28:19.854915 zavod-0.7.3/zavod/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/parse/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/parse/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/parse/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:28:19.854915 zavod-0.7.3/zavod/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/sinks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/sinks/json_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/sinks/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-07 12:26:24.000000 zavod-0.7.3/zavod/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:28:19.854915 zavod-0.7.3/zavod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:28:03.000000 zavod-0.7.3/zavod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 12:28:19.000000 zavod-0.7.3/zavod.egg-info/top_level.txt
```

### Comparing `zavod-0.7.2/LICENSE` & `zavod-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/PKG-INFO` & `zavod-0.7.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.7.2
+Version: 0.7.3
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
-
```

### Comparing `zavod-0.7.2/setup.py` & `zavod-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="zavod",
-    version="0.7.2",
+    version="0.7.3",
     description="Data factory for followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney etl parsing",
     author="Friedrich Lindenberg",
     author_email="friedrich@opensanctions.org",
     url="https://github.com/opensanctions/zavod",
@@ -18,15 +18,15 @@
     packages=find_packages(exclude=["ez_setup", "examples", "tests"]),
     namespace_packages=[],
     include_package_data=True,
     package_data={"": ["zavod/data/*", "zavod/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.2.0, < 4.0.0",
-        "nomenklatura >= 3.1.0, < 4.0.0",
+        "nomenklatura >= 3.2.0, < 4.0.0",
         "addressformatting >= 1.3.0, < 2.0.0",
         "datapatch >= 0.2.1",
         "click >= 8.0.0, < 8.2.0",
         "requests",
         "structlog",
         "lxml",
     ],
```

### Comparing `zavod-0.7.2/zavod/__init__.py` & `zavod-0.7.3/zavod/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from zavod import settings
 from zavod.context import GenericZavod
 from zavod.dataset import ZavodDataset, ZD
 from zavod.logs import configure_logging, get_logger
 from zavod.sinks.common import Sink
 from zavod.sinks.json_entity import JSONEntitySink
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 __all__ = [
     "init",
     "context",
     "Zavod",
     "ZavodDataset",
     "ZD",
     "PathLike",
```

### Comparing `zavod-0.7.2/zavod/audit.py` & `zavod-0.7.3/zavod/audit.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/context.py` & `zavod-0.7.3/zavod/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         )
 
     def make(self, schema: Union[str, Schema]) -> CE:
         """Make a new entity with some dataset context set."""
         return self.entity_type(
             model,
             {"schema": schema},
-            default_dataset=self.dataset.name,
+            default_dataset=self.dataset,
         )
 
     def make_slug(
         self, *parts: Optional[str], strict: bool = True, prefix: Optional[str] = None
     ) -> Optional[str]:
         prefix = self.dataset.prefix if prefix is None else prefix
         return join_slug(*parts, prefix=prefix, strict=strict)
```

### Comparing `zavod-0.7.2/zavod/dataset.py` & `zavod-0.7.3/zavod/dataset.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/http.py` & `zavod-0.7.3/zavod/http.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/logs.py` & `zavod-0.7.3/zavod/logs.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/parse/addresses.py` & `zavod-0.7.3/zavod/parse/addresses.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/parse/names.py` & `zavod-0.7.3/zavod/parse/names.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/parse/xml.py` & `zavod-0.7.3/zavod/parse/xml.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/sinks/common.py` & `zavod-0.7.3/zavod/sinks/common.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/sinks/statement.py` & `zavod-0.7.3/zavod/sinks/statement.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod/util.py` & `zavod-0.7.3/zavod/util.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.2/zavod.egg-info/PKG-INFO` & `zavod-0.7.3/zavod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.7.2
+Version: 0.7.3
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
-
```

### Comparing `zavod-0.7.2/zavod.egg-info/SOURCES.txt` & `zavod-0.7.3/zavod.egg-info/SOURCES.txt`

 * *Files identical despite different names*


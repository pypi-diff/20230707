# Comparing `tmp/tap_readthedocs-0.0.1a3.tar.gz` & `tmp/tap_readthedocs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_readthedocs-0.0.1a3.tar", max compression
+gzip compressed data, was "tap_readthedocs-0.1.0.tar", max compression
```

## Comparing `tap_readthedocs-0.0.1a3.tar` & `tap_readthedocs-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     2734 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/README.md
--rw-r--r--   0        0        0     2296 2023-06-02 04:03:56.301317 tap_readthedocs-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0       46 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/__init__.py
--rw-r--r--   0        0        0     3690 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/client.py
--rw-r--r--   0        0        0     7210 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/streams.py
--rw-r--r--   0        0        0      836 2023-06-02 04:03:36.925190 tap_readthedocs-0.0.1a3/tap_readthedocs/tap.py
--rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 tap_readthedocs-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-07 17:29:20.797075 tap_readthedocs-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3089 2023-07-07 17:29:20.797075 tap_readthedocs-0.1.0/README.md
+-rw-r--r--   0        0        0     2307 2023-07-07 17:29:39.637418 tap_readthedocs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/__init__.py
+-rw-r--r--   0        0        0     3690 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/client.py
+-rw-r--r--   0        0        0     7367 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/streams.py
+-rw-r--r--   0        0        0      836 2023-07-07 17:29:20.801075 tap_readthedocs-0.1.0/tap_readthedocs/tap.py
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 tap_readthedocs-0.1.0/PKG-INFO
```

### Comparing `tap_readthedocs-0.0.1a3/LICENSE` & `tap_readthedocs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a3/README.md` & `tap_readthedocs-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 # tap-readthedocs
 
 <div>
   <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/tap-readthedocs/main">
     <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/tap-readthedocs/main.svg"/>
   </a>
+  <a href="https://github.com/astral-sh/ruff">
+    <img alt="Ruff" style="max-width:100%;" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json">
+  </a>
+  <a href="https://github.com/wntrblm/nox">
+    <img alt="Nox" src="https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg"/>
+  </a>
   <a href="https://github.com/edgarrmondragon/tap-readthedocs/blob/main/LICENSE">
     <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/tap-readthedocs"/>
   </a>
   <a href="https://github.com/edgarrmondragon/tap-readthedocs/">
     <img alt="License" src="https://img.shields.io/pypi/pyversions/tap-readthedocs"/>
   </a>
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                                # tap-readthedocs
-                  [pre-commit.ci_status] [License] [License]
+            [pre-commit.ci_status] [Ruff] [Nox] [License] [License]
 Singer Tap for [**Read the Docs**](https://docs.readthedocs.io). Built with the
                 [Meltano Singer SDK](https://sdk.meltano.com).
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` ##
 Settings | Setting| Required | Default | Description | |:-------|:--------:|:--
 -----:|:------------| | token | True | None | | A full list of supported
 settings and capabilities is available by running: `tap-readthedocs --about` ##
 Installation ```bash pipx install git+https://github.com/edgarrmondragon/tap-
```

### Comparing `tap_readthedocs-0.0.1a3/pyproject.toml` & `tap_readthedocs-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "poetry-core==1.6",
   "poetry-dynamic-versioning",
 ]
 
 [tool.poetry]
 name = "tap-readthedocs"
-version = "0.0.1a3"
+version = "0.1.0"
 description = "`tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
     "ELT",
     "ReadTheDocs",
     "singer.io",
 ]
@@ -19,56 +19,30 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-readthedocs"
 repository = "https://github.com/edgarrmondragon/tap-readthedocs"
 documentation = "https://github.com/edgarrmondragon/tap-readthedocs#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.27.0"
+singer-sdk = "0.29.0"
 toolz = "0.12.0"
 requests-cache = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.1"
-singer-sdk = { version = "0.27.0", extras = ["testing"] }
+singer-sdk = { version = "*", extras = ["testing"] }
 
 [tool.poetry.scripts]
 # CLI declaration
 tap-readthedocs = 'tap_readthedocs.tap:TapReadTheDocs.cli'
 
-[tool.pytest.ini_options]
-addopts = "-vvv"
-
-[tool.mypy]
-python_version = 3.9
-warn_unused_configs = true
-
-[[tool.mypy.overrides]]
-module = ["backoff.*", "toolz.*"]
-ignore_missing_imports = true
-
-[tool.poetry-dynamic-versioning]
-enable = false
-format-jinja = """
-    {%- if distance == 0 -%}
-        {{ serialize_pep440(base, stage, revision) }}
-    {%- elif revision is not none -%}
-        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
-    {%- else -%}
-        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
-    {%- endif -%}
-"""
-metadata = true
-style = "pep440"
-vcs = "git"
-
 [tool.ruff]
 ignore = [
-  "ANN101", # missing-type-self
-  "DJ",     # flake8-django
+  "ANN101",  # missing-type-self
+  "DJ",      # flake8-django
+  "FIX002",  # line-contains-todo
 ]
 line-length = 88
 select = ["ALL"]
 src = ["tap_pulumi_cloud", "tests"]
 target-version = "py37"
 unfixable = [
   "ERA001",  # commented-out-code
@@ -87,7 +61,33 @@
 
 [tool.ruff.isort]
 known-first-party = ["tap_readthedocs"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
+
+[tool.pytest.ini_options]
+addopts = "-vvv"
+
+[tool.mypy]
+python_version = 3.9
+warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+module = ["backoff.*", "toolz.*"]
+ignore_missing_imports = true
+
+[tool.poetry-dynamic-versioning]
+enable = false
+format-jinja = """
+    {%- if distance == 0 -%}
+        {{ serialize_pep440(base, stage, revision) }}
+    {%- elif revision is not none -%}
+        {{ serialize_pep440(base, stage, revision + 1, dev=distance, metadata=[commit]) }}
+    {%- else -%}
+        {{ serialize_pep440(bump_version(base), stage, revision, dev=distance, metadata=[commit]) }}
+    {%- endif -%}
+"""
+metadata = true
+style = "pep440"
+vcs = "git"
```

### Comparing `tap_readthedocs-0.0.1a3/tap_readthedocs/client.py` & `tap_readthedocs-0.1.0/tap_readthedocs/client.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a3/tap_readthedocs/streams.py` & `tap_readthedocs-0.1.0/tap_readthedocs/streams.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Stream type classes for tap-readthedocs."""
 from __future__ import annotations
 
 import logging
+import typing as t
 
 from singer_sdk import typing as th
 from toolz.dicttoolz import update_in
 
 from tap_readthedocs.client import ReadTheDocsStream
 
 logger = logging.getLogger(__name__)
 
 
 class Projects(ReadTheDocsStream):
     """Projects stream."""
 
     name = "projects"
     path = "/api/v3/projects/"
-    primary_keys = ["id"]
+    primary_keys: t.ClassVar[list[str]] = ["id"]
 
     schema = th.PropertiesList(
         th.Property("id", th.IntegerType),
         th.Property("name", th.StringType),
         th.Property("slug", th.StringType),
         th.Property("created", th.DateTimeType),
         th.Property("modified", th.DateTimeType),
@@ -81,15 +82,15 @@
 
 
 class Versions(ReadTheDocsStream):
     """Versions stream."""
 
     name = "versions"
     path = "/api/v3/projects/{project_slug}/versions"
-    primary_keys = ["id"]
+    primary_keys: t.ClassVar[list[str]] = ["id"]
     parent_stream_type = Projects
 
     schema = th.PropertiesList(
         th.Property("id", th.IntegerType),
         th.Property("project_slug", th.StringType),
         th.Property("slug", th.StringType),
         th.Property("verbose_name", th.StringType),
@@ -106,15 +107,15 @@
 
 
 class Builds(ReadTheDocsStream):
     """Builds stream."""
 
     name = "builds"
     path = "/api/v3/projects/{project_slug}/builds"
-    primary_keys = ["id"]
+    primary_keys: t.ClassVar[list[str]] = ["id"]
     parent_stream_type = Projects
 
     schema = th.PropertiesList(
         th.Property("id", th.IntegerType),
         th.Property("project_slug", th.StringType),
         th.Property("version", th.StringType),
         th.Property("project", th.StringType),
@@ -184,45 +185,45 @@
 
 
 class Subprojects(ReadTheDocsStream):
     """Subprojects stream."""
 
     name = "subprojects"
     path = "/api/v3/projects/{project_slug}/subprojects"
-    primary_keys = ["id"]
+    primary_keys: t.ClassVar[list[str]] = ["id"]
     parent_stream_type = Projects
 
     # TODO(edgarrmondragon): get the complete schema
     # https://github.com/edgarrmondragon/tap-readthedocs/issues/2
     schema = th.PropertiesList(
         th.Property("id", th.StringType),
     ).to_dict()
 
 
 class Translations(ReadTheDocsStream):
     """Translations stream."""
 
     name = "translations"
     path = "/api/v3/projects/{project_slug}/translations"
-    primary_keys = ["id"]
+    primary_keys: t.ClassVar[list[str]] = ["id"]
     parent_stream_type = Projects
 
     # TODO(edgarrmondragon): get the complete schema
     # https://github.com/edgarrmondragon/tap-readthedocs/issues/2
     schema = th.PropertiesList(
         th.Property("id", th.StringType),
     ).to_dict()
 
 
 class Redirects(ReadTheDocsStream):
     """Redirects stream."""
 
     name = "redirects"
     path = "/api/v3/projects/{project_slug}/redirects"
-    primary_keys = ["id"]
+    primary_keys: t.ClassVar[list[str]] = ["id"]
     parent_stream_type = Projects
 
     # TODO(edgarrmondragon): get the complete schema
     # https://github.com/edgarrmondragon/tap-readthedocs/issues/2
     schema = th.PropertiesList(
         th.Property("id", th.StringType),
     ).to_dict()
```

### Comparing `tap_readthedocs-0.0.1a3/tap_readthedocs/tap.py` & `tap_readthedocs-0.1.0/tap_readthedocs/tap.py`

 * *Files identical despite different names*

### Comparing `tap_readthedocs-0.0.1a3/PKG-INFO` & `tap_readthedocs-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 Metadata-Version: 2.1
 Name: tap-readthedocs
-Version: 0.0.1a3
+Version: 0.1.0
 Summary: `tap-readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-readthedocs
 License: Apache-2.0
 Keywords: ELT,ReadTheDocs,singer.io
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: singer-sdk (==0.27.0)
+Requires-Dist: singer-sdk (==0.29.0)
 Requires-Dist: toolz (==0.12.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-readthedocs#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-readthedocs
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # tap-readthedocs
 
 <div>
   <a href="https://results.pre-commit.ci/latest/github/edgarrmondragon/tap-readthedocs/main">
     <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/edgarrmondragon/tap-readthedocs/main.svg"/>
   </a>
+  <a href="https://github.com/astral-sh/ruff">
+    <img alt="Ruff" style="max-width:100%;" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json">
+  </a>
+  <a href="https://github.com/wntrblm/nox">
+    <img alt="Nox" src="https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg"/>
+  </a>
   <a href="https://github.com/edgarrmondragon/tap-readthedocs/blob/main/LICENSE">
     <img alt="License" src="https://img.shields.io/github/license/edgarrmondragon/tap-readthedocs"/>
   </a>
   <a href="https://github.com/edgarrmondragon/tap-readthedocs/">
     <img alt="License" src="https://img.shields.io/pypi/pyversions/tap-readthedocs"/>
   </a>
 </div>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: tap-readthedocs Version: 0.0.1a3 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-readthedocs Version: 0.1.0 Summary: `tap-
 readthedocs` is a Singer tap for ReadTheDocs, built with the Meltano SDK for
 Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-readthedocs
 License: Apache-2.0 Keywords: ELT,ReadTheDocs,singer.io Author: Edgar RamÃ­rez-
 MondragÃ³n Author-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: requests-cache (>=1.0.1,<2.0.0) Requires-Dist:
-singer-sdk (==0.27.0) Requires-Dist: toolz (==0.12.0) Project-URL:
+singer-sdk (==0.29.0) Requires-Dist: toolz (==0.12.0) Project-URL:
 Documentation, https://github.com/edgarrmondragon/tap-readthedocs#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-readthedocs
 Description-Content-Type: text/markdown
                                # tap-readthedocs
-                  [pre-commit.ci_status] [License] [License]
+            [pre-commit.ci_status] [Ruff] [Nox] [License] [License]
 Singer Tap for [**Read the Docs**](https://docs.readthedocs.io). Built with the
                 [Meltano Singer SDK](https://sdk.meltano.com).
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` ##
 Settings | Setting| Required | Default | Description | |:-------|:--------:|:--
 -----:|:------------| | token | True | None | | A full list of supported
 settings and capabilities is available by running: `tap-readthedocs --about` ##
 Installation ```bash pipx install git+https://github.com/edgarrmondragon/tap-
```


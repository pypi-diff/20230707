# Comparing `tmp/liege-0.1.3.tar.gz` & `tmp/liege-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liege-0.1.3.tar", max compression
+gzip compressed data, was "liege-0.2.0.tar", max compression
```

## Comparing `liege-0.1.3.tar` & `liege-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1072 2022-09-29 13:38:34.260049 liege-0.1.3/LICENSE
--rw-r--r--   0        0        0     8616 2022-09-29 13:38:34.260049 liege-0.1.3/README.md
--rw-r--r--   0        0        0      332 2022-09-29 13:38:34.260049 liege-0.1.3/liege/__init__.py
--rw-r--r--   0        0        0      269 2022-09-29 13:38:34.260049 liege-0.1.3/liege/exceptions.py
--rw-r--r--   0        0        0     4674 2022-09-29 13:38:34.260049 liege-0.1.3/liege/liege.py
--rw-r--r--   0        0        0     3127 2022-09-29 13:38:34.260049 liege-0.1.3/liege/models.py
--rw-r--r--   0        0        0        0 2022-09-29 13:38:34.260049 liege-0.1.3/liege/py.typed
--rw-r--r--   0        0        0     3841 2022-09-29 13:38:53.715956 liege-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9595 1970-01-01 00:00:00.000000 liege-0.1.3/setup.py
--rw-r--r--   0        0        0     9994 1970-01-01 00:00:00.000000 liege-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 21:56:36.090415 liege-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9036 2023-07-06 21:56:36.090415 liege-0.2.0/README.md
+-rw-r--r--   0        0        0     3744 2023-07-06 21:56:54.588011 liege-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      332 2023-07-06 21:56:36.094415 liege-0.2.0/src/liege/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-06 21:56:36.094415 liege-0.2.0/src/liege/exceptions.py
+-rw-r--r--   0        0        0     4730 2023-07-06 21:56:36.094415 liege-0.2.0/src/liege/liege.py
+-rw-r--r--   0        0        0     3736 2023-07-06 21:56:36.094415 liege-0.2.0/src/liege/models.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:56:36.094415 liege-0.2.0/src/liege/py.typed
+-rw-r--r--   0        0        0    10359 1970-01-01 00:00:00.000000 liege-0.2.0/PKG-INFO
```

### Comparing `liege-0.1.3/LICENSE` & `liege-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2022 Klaas Schoute
+Copyright (c) 2022-2023 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `liege-0.1.3/README.md` & `liege-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-## Python - ODP Liège Client
+<!-- Banner -->
+![alt Banner of the ODP Liege package](https://raw.githubusercontent.com/klaasnicolaas/python-liege/main/assets/header_liege-min.png)
 
 <!-- PROJECT SHIELDS -->
 [![GitHub Release][releases-shield]][releases]
 [![Python Versions][python-versions-shield]][pypi]
 ![Project Stage][project-stage-shield]
 ![Project Maintenance][maintenance-shield]
 [![License][license-shield]](LICENSE)
 
 [![GitHub Activity][commits-shield]][commits-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
 [![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
 
 [![Code Quality][code-quality-shield]][code-quality]
-[![Maintainability][maintainability-shield]][maintainability-url]
-[![Code Coverage][codecov-shield]][codecov-url]
-
 [![Build Status][build-shield]][build-url]
 [![Typing Status][typing-shield]][typing-url]
 
+[![Maintainability][maintainability-shield]][maintainability-url]
+[![Code Coverage][codecov-shield]][codecov-url]
+
 Asynchronous Python client for the open datasets of Liège (Belgium).
 
 ## About
 
 A python package with which you can retrieve data from the Open Data Platform of Liège via [their API][api]. This package was initially created to only retrieve parking data from the API, but the code base is made in such a way that it is easy to extend for other datasets from the same platform.
 
 ## Installation
@@ -120,16 +120,22 @@
 We've set up a separate document for our
 [contribution guidelines](CONTRIBUTING.md).
 
 Thank you for being involved! :heart_eyes:
 
 ## Setting up development environment
 
-This Python project is fully managed using the [Poetry][poetry] dependency
-manager.
+The simplest way to begin is by utilizing the [Dev Container][devcontainer]
+feature of Visual Studio Code or by opening a CodeSpace directly on GitHub.
+By clicking the button below you immediately start a Dev Container in Visual Studio Code.
+
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
+
+This Python project relies on [Poetry][poetry] as its dependency manager,
+providing comprehensive management and control over project dependencies.
 
 You need at least:
 
 - Python 3.9+
 - [Poetry][poetry-install]
 
 Install all packages, including all development requirements:
@@ -168,15 +174,15 @@
 poetry run pytest
 ```
 
 ## License
 
 MIT License
 
-Copyright (c) 2022 Klaas Schoute
+Copyright (c) 2022-2023 Klaas Schoute
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -196,35 +202,33 @@
 [disabled_parking]: https://opendata.liege.be/explore/dataset/stationnement-pmr
 [garages]: https://opendata.liege.be/explore/dataset/parkings-voitures-hors-voirie
 [nipkaart]: https://www.nipkaart.nl
 
 <!-- MARKDOWN LINKS & IMAGES -->
 [build-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/tests.yaml/badge.svg
 [build-url]: https://github.com/klaasnicolaas/python-liege/actions/workflows/tests.yaml
-[code-quality-shield]: https://img.shields.io/lgtm/grade/python/g/klaasnicolaas/python-liege.svg?logo=lgtm&logoWidth=18
-[code-quality]: https://lgtm.com/projects/g/klaasnicolaas/python-liege/context:python
+[code-quality-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/codeql.yaml/badge.svg
+[code-quality]: https://github.com/klaasnicolaas/python-liege/actions/workflows/codeql.yaml
 [commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-liege.svg
 [commits-url]: https://github.com/klaasnicolaas/python-liege/commits/main
 [codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-liege/branch/main/graph/badge.svg?token=jTIsaqV5x0
 [codecov-url]: https://codecov.io/gh/klaasnicolaas/python-liege
-[forks-shield]: https://img.shields.io/github/forks/klaasnicolaas/python-liege.svg
-[forks-url]: https://github.com/klaasnicolaas/python-liege/network/members
-[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-liege.svg
-[issues-url]: https://github.com/klaasnicolaas/python-liege/issues
+[devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-liege
+[downloads-shield]: https://img.shields.io/pypi/dm/liege
+[downloads-url]: https://pypistats.org/packages/liege
 [license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-liege.svg
 [last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-liege.svg
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
 [maintainability-shield]: https://api.codeclimate.com/v1/badges/1b4ebe208e72d8f467f9/maintainability
 [maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-liege/maintainability
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
 [pypi]: https://pypi.org/project/liege/
 [python-versions-shield]: https://img.shields.io/pypi/pyversions/liege
 [typing-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/typing.yaml/badge.svg
 [typing-url]: https://github.com/klaasnicolaas/python-liege/actions/workflows/typing.yaml
 [releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-liege.svg
 [releases]: https://github.com/klaasnicolaas/python-liege/releases
-[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-liege.svg
-[stars-url]: https://github.com/klaasnicolaas/python-liege/stargazers
 
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com
```

### Comparing `liege-0.1.3/liege/liege.py` & `liege-0.2.0/src/liege/liege.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,35 @@
         *,
         method: str = hdrs.METH_GET,
         params: dict[str, Any] | None = None,
     ) -> Any:
         """Handle a request to the Open Data Platform API of Liège.
 
         Args:
+        ----
             uri: Request URI, without '/', for example, 'status'
             method: HTTP method to use, for example, 'GET'
             params: Extra options to improve or limit the response.
 
         Returns:
+        -------
             A Python dictionary (text) with the response from
             the Open Data Platform API of Liège.
 
         Raises:
+        ------
             ODPLiegeConnectionError: Timeout occurred while
                 connecting to the Open Data Platform API.
             ODPLiegeError: If the data is not valid.
         """
         version = metadata.version(__package__)
         url = URL.build(
-            scheme="https", host="opendata.liege.be", path="/api/records/1.0/"
+            scheme="https",
+            host="opendata.liege.be",
+            path="/api/records/1.0/",
         ).join(URL(uri))
 
         headers = {
             "Accept": "application/json",
             "User-Agent": f"PythonODPLiege/{version}",
         }
 
@@ -69,83 +74,84 @@
                     url,
                     params=params,
                     headers=headers,
                     ssl=True,
                 )
                 response.raise_for_status()
         except asyncio.TimeoutError as exception:
+            msg = "Timeout occurred while connecting to the Open Data Platform API."
             raise ODPLiegeConnectionError(
-                "Timeout occurred while connecting to the Open Data Platform API."
+                msg,
             ) from exception
         except (aiohttp.ClientError, socket.gaierror) as exception:
+            msg = "Error occurred while communicating with Open Data Platform API."
             raise ODPLiegeConnectionError(
-                "Error occurred while communicating with Open Data Platform API."
+                msg,
             ) from exception
 
         content_type = response.headers.get("Content-Type", "")
         if "application/json" not in content_type:
             text = await response.text()
+            msg = "Unexpected content type response from the Open Data Platform API"
             raise ODPLiegeError(
-                "Unexpected content type response from the Open Data Platform API",
+                msg,
                 {"Content-Type": content_type, "Response": text},
             )
 
         return await response.json()
 
     async def disabled_parkings(self, limit: int = 10) -> list[DisabledParking]:
         """Get list of disabled parking.
 
         Args:
+        ----
             limit: Maximum number of disabled parkings to return.
 
         Returns:
+        -------
             A list of DisabledParking objects.
         """
-        results: list[DisabledParking] = []
         locations = await self._request(
             "search/",
             params={"dataset": "stationnement-pmr", "rows": limit},
         )
-
-        for item in locations["records"]:
-            results.append(DisabledParking.from_dict(item))
-        return results
+        return [DisabledParking.from_dict(item) for item in locations["records"]]
 
     async def garages(self, limit: int = 10) -> list[Garage]:
         """Get list of parking garages.
 
         Args:
+        ----
             limit: Maximum number of garages to return.
 
         Returns:
+        -------
             A list of Garage objects.
         """
-        results: list[Garage] = []
         locations = await self._request(
             "search/",
             params={"dataset": "parkings-voitures-hors-voirie", "rows": limit},
         )
-
-        for item in locations["records"]:
-            results.append(Garage.from_dict(item))
-        return results
+        return [Garage.from_dict(item) for item in locations["records"]]
 
     async def close(self) -> None:
         """Close open client session."""
         if self.session and self._close_session:
             await self.session.close()
 
     async def __aenter__(self) -> ODPLiege:
         """Async enter.
 
-        Returns:
+        Returns
+        -------
             The Open Data Platform Liège object.
         """
         return self
 
     async def __aexit__(self, *_exc_info: Any) -> None:
         """Async exit.
 
         Args:
+        ----
             _exc_info: Exec type.
         """
         await self.close()
```

### Comparing `liege-0.1.3/pyproject.toml` & `liege-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,76 @@
 [tool.poetry]
 name = "liege"
-version = "0.1.3"
+version = "0.2.0"
 description = "Asynchronous Python client providing Open Data information of Liège (luik)"
 authors = ["Klaas Schoute <hello@student-techlife.com>"]
 maintainers = ["Klaas Schoute <hello@student-techlife.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/klaasnicolaas/python-liege"
 repository = "https://github.com/klaasnicolaas/python-liege"
 documentation = "https://github.com/klaasnicolaas/python-liege"
 keywords = ["open", "data", "platform", "luik", "liege", "parking", "api", "async", "client"]
 classifiers = [
-    "Framework :: AsyncIO",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+  "Framework :: AsyncIO",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3",
+  "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [
-    { include = "liege" }
+  { include = "liege", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 python = "^3.9"
 yarl = ">=1.6.0"
-
-[tool.poetry.dev-dependencies]
-aresponses = "^2.1.6"
-bandit = "^1.7.4"
-black = "^22.8"
-blacken-docs = "^1.12.1"
-codespell = "^2.2.1"
-coverage = {version = "^6.4", extras = ["toml"]}
-darglint = "^1.8.1"
-flake8 = "^4.0.1"
-flake8-bandit = "^3.0.0"
-flake8-bugbear = "^22.9.23"
-flake8-builtins = "^1.5.3"
-flake8-comprehensions = "^3.10.0"
-flake8-docstrings = "^1.5.0"
-flake8-eradicate = "^1.4.0"
-flake8-markdown = "^0.3.0"
-flake8-simplify = "^0.19.3"
-isort = "^5.10.1"
-mypy = "^0.981"
-pre-commit = "^2.20.0"
-pre-commit-hooks = "^4.3.0"
-pylint = "^2.15.3"
-pytest = "^7.1.3"
-pytest-asyncio = "^0.19.0"
-pytest-cov = "^4.0.0"
-pyupgrade = "^2.38.2"
-safety = "^2.2.0"
-vulture = "^2.6"
-yamllint = "^1.28.0"
-types-cachetools = "^5.2.1"
+pytz = ">=2022.7.1,<2024.0.0"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/klaasnicolaas/python-liege/issues"
 Changelog = "https://github.com/klaasnicolaas/python-liege/releases"
 
-[tool.black]
-target-version = ['py39']
+[tool.poetry.group.dev.dependencies]
+ruff = "0.0.277"
+aresponses = "2.1.6"
+black = "23.3.0"
+blacken-docs = "1.14.0"
+codespell = "2.2.5"
+coverage = {version = "7.2.7", extras = ["toml"]}
+mypy = "1.4.1"
+pre-commit = "3.3.3"
+pre-commit-hooks = "4.4.0"
+pylint = "2.17.4"
+pytest = "7.4.0"
+pytest-asyncio = "0.21.0"
+pytest-cov = "4.1.0"
+yamllint = "1.32.0"
+covdefaults = "2.3.0"
+types-pytz = "2023.3.0.0"
 
-[tool.coverage.paths]
+[tool.coverage.run]
+plugins = ["covdefaults"]
 source = ["liege"]
 
 [tool.coverage.report]
+fail_under = 90
 show_missing = true
-exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
-
-[tool.coverage.run]
-branch = true
-source = ["liege"]
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
 
 [tool.mypy]
 # Specify the target platform details in config, so your developers are
 # free to run mypy on Windows, Linux, or macOS and get consistent
 # results.
 platform = "linux"
-python_version = 3.9
+python_version = "3.9"
 
 # flake8-mypy expects the two following for sensible formatting
 show_column_numbers = true
 
 # show error messages from unrelated files
 follow_imports = "normal"
 
@@ -100,65 +79,78 @@
 
 # be strict
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
+disallow_untyped_decorators = true
 disallow_untyped_defs = true
-disallow_untyped_decorators = false # thanks backoff :(
 no_implicit_optional = true
 no_implicit_reexport = true
 strict_optional = true
 warn_incomplete_stub = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
-# No incremental mode
-cache_dir = "/dev/null"
-
 [tool.pylint.BASIC]
 good-names = [
-    "_",
-    "ex",
-    "fp",
-    "i",
-    "id",
-    "j",
-    "k",
-    "on",
-    "Run",
-    "T",
+  "_",
+  "ex",
+  "fp",
+  "i",
+  "id",
+  "j",
+  "k",
+  "on",
+  "Run",
+  "T",
+  "vw"
 ]
 
 [tool.pylint."MESSAGES CONTROL"]
 disable= [
-    "too-few-public-methods",
-    "duplicate-code",
-    "format",
-    "unsubscriptable-object",
+  "duplicate-code",
+  "format",
+  "unsubscriptable-object",
 ]
 
 [tool.pylint.SIMILARITIES]
 ignore-imports = true
 
 [tool.pylint.FORMAT]
-max-line-length=88
+max-line-length = 88
 
 [tool.pylint.DESIGN]
-max-attributes=20
+max-attributes = 20
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
-[tool.vulture]
-min_confidence = 80
-paths = ["liege"]
-verbose = true
+[tool.ruff]
+select = ["ALL"]
+ignore = [
+  "ANN101", # Self... explanatory
+  "ANN401", # Opinioated warning on disallowing dynamically typed expressions
+  "D203", # Conflicts with other rules
+  "D213", # Conflicts with other rules
+  "D417", # False positives in some occasions
+  "PLR2004", # Just annoying, not really useful
+]
+
+[tool.ruff.flake8-pytest-style]
+mark-parentheses = false
+fixture-parentheses = false
+
+[tool.ruff.isort]
+known-first-party = ["liege"]
+
+[tool.ruff.mccabe]
+max-complexity = 25
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0"]
```

### Comparing `liege-0.1.3/setup.py` & `liege-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,265 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: liege
+Version: 0.2.0
+Summary: Asynchronous Python client providing Open Data information of Liège (luik)
+Home-page: https://github.com/klaasnicolaas/python-liege
+License: MIT
+Keywords: open,data,platform,luik,liege,parking,api,async,client
+Author: Klaas Schoute
+Author-email: hello@student-techlife.com
+Maintainer: Klaas Schoute
+Maintainer-email: hello@student-techlife.com
+Requires-Python: >=3.9,<4.0
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiohttp (>=3.0.0)
+Requires-Dist: pytz (>=2022.7.1,<2024.0.0)
+Requires-Dist: yarl (>=1.6.0)
+Project-URL: Bug Tracker, https://github.com/klaasnicolaas/python-liege/issues
+Project-URL: Changelog, https://github.com/klaasnicolaas/python-liege/releases
+Project-URL: Documentation, https://github.com/klaasnicolaas/python-liege
+Project-URL: Repository, https://github.com/klaasnicolaas/python-liege
+Description-Content-Type: text/markdown
 
-packages = \
-['liege']
+<!-- Banner -->
+![alt Banner of the ODP Liege package](https://raw.githubusercontent.com/klaasnicolaas/python-liege/main/assets/header_liege-min.png)
 
-package_data = \
-{'': ['*']}
+<!-- PROJECT SHIELDS -->
+[![GitHub Release][releases-shield]][releases]
+[![Python Versions][python-versions-shield]][pypi]
+![Project Stage][project-stage-shield]
+![Project Maintenance][maintenance-shield]
+[![License][license-shield]](LICENSE)
 
-install_requires = \
-['aiohttp>=3.0.0', 'yarl>=1.6.0']
-
-setup_kwargs = {
-    'name': 'liege',
-    'version': '0.1.3',
-    'description': 'Asynchronous Python client providing Open Data information of Liège (luik)',
-    'long_description': '## Python - ODP Liège Client\n\n<!-- PROJECT SHIELDS -->\n[![GitHub Release][releases-shield]][releases]\n[![Python Versions][python-versions-shield]][pypi]\n![Project Stage][project-stage-shield]\n![Project Maintenance][maintenance-shield]\n[![License][license-shield]](LICENSE)\n\n[![GitHub Activity][commits-shield]][commits-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n[![GitHub Last Commit][last-commit-shield]][commits-url]\n\n[![Code Quality][code-quality-shield]][code-quality]\n[![Maintainability][maintainability-shield]][maintainability-url]\n[![Code Coverage][codecov-shield]][codecov-url]\n\n[![Build Status][build-shield]][build-url]\n[![Typing Status][typing-shield]][typing-url]\n\nAsynchronous Python client for the open datasets of Liège (Belgium).\n\n## About\n\nA python package with which you can retrieve data from the Open Data Platform of Liège via [their API][api]. This package was initially created to only retrieve parking data from the API, but the code base is made in such a way that it is easy to extend for other datasets from the same platform.\n\n## Installation\n\n```bash\npip install liege\n```\n\n## Datasets\n\nYou can read the following datasets with this package:\n\n- [Disabled parking spaces / Stationnement PMR][disabled_parking] (952 locations)\n- [Garages / Les parkings voitures hors voirie][garages] (26 locations)\n\n<details>\n    <summary>Click here to get more details</summary>\n\n### Disabled parkings\n\nParameters:\n\n- **limit** (default: 10) - How many results you want to retrieve.\n\n| Variable | Type | Description |\n| :------- | :--- | :---------- |\n| `spot_id` | int | The ID of the parking spot |\n| `number` | int | How many parking spots there are on this location |\n| `address` | str | The address of the parking spot |\n| `municipality` | str | The municipality of the parking spot |\n| `city` | str | The city of the parking spot |\n| `status` | str | The status of the parking spot |\n| `longitude` | float | The longitude of the parking spot |\n| `latitude` | float | The latitude of the parking spot |\n| `created_at` | datetime | When the parking spot was added to the dataset |\n| `updated_at` | datetime | The last time the data was updated |\n\n### Garages\n\nParameters:\n\n- **limit** (default: 10) - How many results you want to retrieve.\n\n| Variable | Type | Description |\n| :------- | :--- | :---------- |\n| `name` | string | The name of the garage |\n| `capacity` | int | The capacity of the garage |\n| `charging_stations` | int | The number of charging stations |\n| `address` | string | The address of the garage |\n| `municipality` | string | The municipality of the garage |\n| `city` | string | The city of the garage |\n| `provider` | string | The provider of the garage |\n| `schedule` | string | The schedule of the garage |\n| `longitude` | float | The longitude of the garage |\n| `latitude` | float | The latitude of the garage |\n| `created_at` | datetime | When the garage was added to the dataset |\n| `updated_at` | datetime | The last time the data was updated |\n</details>\n\n## Example\n\n```python\nimport asyncio\n\nfrom liege import ODPLiege\n\n\nasync def main() -> None:\n    """Show example on using the Open Data API client."""\n    async with ODPLiege() as client:\n        garages = await client.garages(limit=10)\n        disabled_parkings = await client.disabled_parkings(limit=10)\n        print(garages)\n        print(disabled_parkings)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## Use cases\n\n[NIPKaart.nl][nipkaart]\n\nA website that provides insight into where disabled parking spaces are, based\non data from users and municipalities. Operates mainly in the Netherlands, but\nalso has plans to process data from abroad.\n\n## Contributing\n\nThis is an active open-source project. We are always open to people who want to\nuse the code or contribute to it.\n\nWe\'ve set up a separate document for our\n[contribution guidelines](CONTRIBUTING.md).\n\nThank you for being involved! :heart_eyes:\n\n## Setting up development environment\n\nThis Python project is fully managed using the [Poetry][poetry] dependency\nmanager.\n\nYou need at least:\n\n- Python 3.9+\n- [Poetry][poetry-install]\n\nInstall all packages, including all development requirements:\n\n```bash\npoetry install\n```\n\nPoetry creates by default an virtual environment where it installs all\nnecessary pip packages, to enter or exit the venv run the following commands:\n\n```bash\npoetry shell\nexit\n```\n\nSetup the pre-commit check, you must run this inside the virtual environment:\n\n```bash\npre-commit install\n```\n\n*Now you\'re all set to get started!*\n\nAs this repository uses the [pre-commit][pre-commit] framework, all changes\nare linted and tested with each commit. You can run all checks and tests\nmanually, using the following command:\n\n```bash\npoetry run pre-commit run --all-files\n```\n\nTo run just the Python tests:\n\n```bash\npoetry run pytest\n```\n\n## License\n\nMIT License\n\nCopyright (c) 2022 Klaas Schoute\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the "Software"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n[api]: https://opendata.liege.be/explore\n[disabled_parking]: https://opendata.liege.be/explore/dataset/stationnement-pmr\n[garages]: https://opendata.liege.be/explore/dataset/parkings-voitures-hors-voirie\n[nipkaart]: https://www.nipkaart.nl\n\n<!-- MARKDOWN LINKS & IMAGES -->\n[build-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/tests.yaml/badge.svg\n[build-url]: https://github.com/klaasnicolaas/python-liege/actions/workflows/tests.yaml\n[code-quality-shield]: https://img.shields.io/lgtm/grade/python/g/klaasnicolaas/python-liege.svg?logo=lgtm&logoWidth=18\n[code-quality]: https://lgtm.com/projects/g/klaasnicolaas/python-liege/context:python\n[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-liege.svg\n[commits-url]: https://github.com/klaasnicolaas/python-liege/commits/main\n[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-liege/branch/main/graph/badge.svg?token=jTIsaqV5x0\n[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-liege\n[forks-shield]: https://img.shields.io/github/forks/klaasnicolaas/python-liege.svg\n[forks-url]: https://github.com/klaasnicolaas/python-liege/network/members\n[issues-shield]: https://img.shields.io/github/issues/klaasnicolaas/python-liege.svg\n[issues-url]: https://github.com/klaasnicolaas/python-liege/issues\n[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-liege.svg\n[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-liege.svg\n[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg\n[maintainability-shield]: https://api.codeclimate.com/v1/badges/1b4ebe208e72d8f467f9/maintainability\n[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-liege/maintainability\n[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg\n[pypi]: https://pypi.org/project/liege/\n[python-versions-shield]: https://img.shields.io/pypi/pyversions/liege\n[typing-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/typing.yaml/badge.svg\n[typing-url]: https://github.com/klaasnicolaas/python-liege/actions/workflows/typing.yaml\n[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-liege.svg\n[releases]: https://github.com/klaasnicolaas/python-liege/releases\n[stars-shield]: https://img.shields.io/github/stars/klaasnicolaas/python-liege.svg\n[stars-url]: https://github.com/klaasnicolaas/python-liege/stargazers\n\n[poetry-install]: https://python-poetry.org/docs/#installation\n[poetry]: https://python-poetry.org\n[pre-commit]: https://pre-commit.com\n',
-    'author': 'Klaas Schoute',
-    'author_email': 'hello@student-techlife.com',
-    'maintainer': 'Klaas Schoute',
-    'maintainer_email': 'hello@student-techlife.com',
-    'url': 'https://github.com/klaasnicolaas/python-liege',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+[![GitHub Activity][commits-shield]][commits-url]
+[![PyPi Downloads][downloads-shield]][downloads-url]
+[![GitHub Last Commit][last-commit-shield]][commits-url]
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
 
+[![Code Quality][code-quality-shield]][code-quality]
+[![Build Status][build-shield]][build-url]
+[![Typing Status][typing-shield]][typing-url]
+
+[![Maintainability][maintainability-shield]][maintainability-url]
+[![Code Coverage][codecov-shield]][codecov-url]
+
+Asynchronous Python client for the open datasets of Liège (Belgium).
+
+## About
+
+A python package with which you can retrieve data from the Open Data Platform of Liège via [their API][api]. This package was initially created to only retrieve parking data from the API, but the code base is made in such a way that it is easy to extend for other datasets from the same platform.
+
+## Installation
+
+```bash
+pip install liege
+```
+
+## Datasets
+
+You can read the following datasets with this package:
+
+- [Disabled parking spaces / Stationnement PMR][disabled_parking] (952 locations)
+- [Garages / Les parkings voitures hors voirie][garages] (26 locations)
+
+<details>
+    <summary>Click here to get more details</summary>
+
+### Disabled parkings
+
+Parameters:
+
+- **limit** (default: 10) - How many results you want to retrieve.
+
+| Variable | Type | Description |
+| :------- | :--- | :---------- |
+| `spot_id` | int | The ID of the parking spot |
+| `number` | int | How many parking spots there are on this location |
+| `address` | str | The address of the parking spot |
+| `municipality` | str | The municipality of the parking spot |
+| `city` | str | The city of the parking spot |
+| `status` | str | The status of the parking spot |
+| `longitude` | float | The longitude of the parking spot |
+| `latitude` | float | The latitude of the parking spot |
+| `created_at` | datetime | When the parking spot was added to the dataset |
+| `updated_at` | datetime | The last time the data was updated |
+
+### Garages
+
+Parameters:
+
+- **limit** (default: 10) - How many results you want to retrieve.
+
+| Variable | Type | Description |
+| :------- | :--- | :---------- |
+| `name` | string | The name of the garage |
+| `capacity` | int | The capacity of the garage |
+| `charging_stations` | int | The number of charging stations |
+| `address` | string | The address of the garage |
+| `municipality` | string | The municipality of the garage |
+| `city` | string | The city of the garage |
+| `provider` | string | The provider of the garage |
+| `schedule` | string | The schedule of the garage |
+| `longitude` | float | The longitude of the garage |
+| `latitude` | float | The latitude of the garage |
+| `created_at` | datetime | When the garage was added to the dataset |
+| `updated_at` | datetime | The last time the data was updated |
+</details>
+
+## Example
+
+```python
+import asyncio
+
+from liege import ODPLiege
+
+
+async def main() -> None:
+    """Show example on using the Open Data API client."""
+    async with ODPLiege() as client:
+        garages = await client.garages(limit=10)
+        disabled_parkings = await client.disabled_parkings(limit=10)
+        print(garages)
+        print(disabled_parkings)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+## Use cases
+
+[NIPKaart.nl][nipkaart]
+
+A website that provides insight into where disabled parking spaces are, based
+on data from users and municipalities. Operates mainly in the Netherlands, but
+also has plans to process data from abroad.
+
+## Contributing
+
+This is an active open-source project. We are always open to people who want to
+use the code or contribute to it.
+
+We've set up a separate document for our
+[contribution guidelines](CONTRIBUTING.md).
+
+Thank you for being involved! :heart_eyes:
+
+## Setting up development environment
+
+The simplest way to begin is by utilizing the [Dev Container][devcontainer]
+feature of Visual Studio Code or by opening a CodeSpace directly on GitHub.
+By clicking the button below you immediately start a Dev Container in Visual Studio Code.
+
+[![Open in Dev Containers][devcontainer-shield]][devcontainer]
+
+This Python project relies on [Poetry][poetry] as its dependency manager,
+providing comprehensive management and control over project dependencies.
+
+You need at least:
+
+- Python 3.9+
+- [Poetry][poetry-install]
+
+Install all packages, including all development requirements:
+
+```bash
+poetry install
+```
+
+Poetry creates by default an virtual environment where it installs all
+necessary pip packages, to enter or exit the venv run the following commands:
+
+```bash
+poetry shell
+exit
+```
+
+Setup the pre-commit check, you must run this inside the virtual environment:
+
+```bash
+pre-commit install
+```
+
+*Now you're all set to get started!*
+
+As this repository uses the [pre-commit][pre-commit] framework, all changes
+are linted and tested with each commit. You can run all checks and tests
+manually, using the following command:
+
+```bash
+poetry run pre-commit run --all-files
+```
+
+To run just the Python tests:
+
+```bash
+poetry run pytest
+```
+
+## License
+
+MIT License
+
+Copyright (c) 2022-2023 Klaas Schoute
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+[api]: https://opendata.liege.be/explore
+[disabled_parking]: https://opendata.liege.be/explore/dataset/stationnement-pmr
+[garages]: https://opendata.liege.be/explore/dataset/parkings-voitures-hors-voirie
+[nipkaart]: https://www.nipkaart.nl
+
+<!-- MARKDOWN LINKS & IMAGES -->
+[build-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/tests.yaml/badge.svg
+[build-url]: https://github.com/klaasnicolaas/python-liege/actions/workflows/tests.yaml
+[code-quality-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/codeql.yaml/badge.svg
+[code-quality]: https://github.com/klaasnicolaas/python-liege/actions/workflows/codeql.yaml
+[commits-shield]: https://img.shields.io/github/commit-activity/y/klaasnicolaas/python-liege.svg
+[commits-url]: https://github.com/klaasnicolaas/python-liege/commits/main
+[codecov-shield]: https://codecov.io/gh/klaasnicolaas/python-liege/branch/main/graph/badge.svg?token=jTIsaqV5x0
+[codecov-url]: https://codecov.io/gh/klaasnicolaas/python-liege
+[devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/klaasnicolaas/python-liege
+[downloads-shield]: https://img.shields.io/pypi/dm/liege
+[downloads-url]: https://pypistats.org/packages/liege
+[license-shield]: https://img.shields.io/github/license/klaasnicolaas/python-liege.svg
+[last-commit-shield]: https://img.shields.io/github/last-commit/klaasnicolaas/python-liege.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintainability-shield]: https://api.codeclimate.com/v1/badges/1b4ebe208e72d8f467f9/maintainability
+[maintainability-url]: https://codeclimate.com/github/klaasnicolaas/python-liege/maintainability
+[project-stage-shield]: https://img.shields.io/badge/project%20stage-experimental-yellow.svg
+[pypi]: https://pypi.org/project/liege/
+[python-versions-shield]: https://img.shields.io/pypi/pyversions/liege
+[typing-shield]: https://github.com/klaasnicolaas/python-liege/actions/workflows/typing.yaml/badge.svg
+[typing-url]: https://github.com/klaasnicolaas/python-liege/actions/workflows/typing.yaml
+[releases-shield]: https://img.shields.io/github/release/klaasnicolaas/python-liege.svg
+[releases]: https://github.com/klaasnicolaas/python-liege/releases
+
+[poetry-install]: https://python-poetry.org/docs/#installation
+[poetry]: https://python-poetry.org
+[pre-commit]: https://pre-commit.com
 
-setup(**setup_kwargs)
```


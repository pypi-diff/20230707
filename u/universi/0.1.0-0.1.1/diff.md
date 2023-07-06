# Comparing `tmp/universi-0.1.0.tar.gz` & `tmp/universi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universi-0.1.0.tar", max compression
+gzip compressed data, was "universi-0.1.1.tar", max compression
```

## Comparing `universi-0.1.0.tar` & `universi-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.1.0/LICENSE
--rw-r--r--   0        0        0      921 2023-06-12 19:09:15.566665 universi-0.1.0/README.md
--rw-r--r--   0        0        0     3862 2023-06-12 19:10:06.053331 universi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       80 2023-06-12 19:09:15.559998 universi-0.1.0/universi/__init__.py
--rw-r--r--   0        0        0      132 2023-06-12 19:09:15.559998 universi-0.1.0/universi/__main__.py
--rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 universi-0.1.0/setup.py
--rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 universi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.1.1/LICENSE
+-rw-r--r--   0        0        0      921 2023-07-02 16:05:32.636241 universi-0.1.1/README.md
+-rw-r--r--   0        0        0     4022 2023-07-06 22:53:51.764165 universi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-07-06 22:51:41.661546 universi-0.1.1/universi/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-29 21:29:31.663440 universi-0.1.1/universi/__main__.py
+-rw-r--r--   0        0        0       87 2023-07-02 20:26:35.180294 universi-0.1.1/universi/exceptions.py
+-rw-r--r--   0        0        0     2892 2023-07-06 22:51:57.318127 universi-0.1.1/universi/fields.py
+-rw-r--r--   0        0        0     8421 2023-07-06 22:52:01.291438 universi-0.1.1/universi/generate.py
+-rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.1.1/universi/header.py
+-rw-r--r--   0        0        0     6047 2023-07-06 22:52:01.198105 universi-0.1.1/universi/linting.py
+-rw-r--r--   0        0        0        1 2023-07-03 05:47:19.541761 universi-0.1.1/universi/migration.py
+-rw-r--r--   0        0        0     4587 2023-07-06 22:52:01.184772 universi-0.1.1/universi/routing.py
+-rw-r--r--   0        0        0        0 2023-07-01 12:42:20.762237 universi-0.1.1/universi/structure/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-03 05:47:19.538427 universi-0.1.1/universi/structure/common.py
+-rw-r--r--   0        0        0     4820 2023-07-06 22:52:01.218105 universi-0.1.1/universi/structure/endpoints.py
+-rw-r--r--   0        0        0      847 2023-07-02 14:07:59.549370 universi-0.1.1/universi/structure/responses.py
+-rw-r--r--   0        0        0     4215 2023-07-06 22:51:57.348126 universi-0.1.1/universi/structure/schemas.py
+-rw-r--r--   0        0        0     5566 2023-07-06 22:52:01.214772 universi-0.1.1/universi/structure/versions.py
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 universi-0.1.1/setup.py
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 universi-0.1.1/PKG-INFO
```

### Comparing `universi-0.1.0/LICENSE` & `universi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `universi-0.1.0/README.md` & `universi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `universi-0.1.0/pyproject.toml` & `universi-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 [tool.poetry]
 name = "universi"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/universi"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typing-extensions = "*"
 typer = {version="*", extras=["all"]}
+fastapi = ">=0.96.1"
+type-inspector = "^1.2.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 ruff = "*"
 pytest = ">=7.2.1"
 pytest-cov = ">=4.0.0"
+httpx = ">=0.23.0"
+uvicorn = "*"
+devtools = "*"
+pdbpp = "^0.10.3"
+pytest-pretty = "^1.2.0"
+notebook = "^6.5.4"
 
 [tool.poetry.scripts]
 universi = 'universi.__main__:app'
 
+
 [tool.coverage.report]
 fail_under = 100
 skip_covered = true
 skip_empty = true
 # Taken from https://coverage.readthedocs.io/en/7.1.0/excluding.html#advanced-exclusion
 exclude_lines = [
     "pragma: no cover",
@@ -42,14 +51,15 @@
     "if TYPE_CHECKING:",
     "@(abc\\.)?abstractmethod",
     "@(typing\\.)?overload",
     "__rich_repr__",
     "__repr__",
 ]
 
+
 [tool.ruff]
 line-length = 120
 select = [
     "F",        # pyflakes
     "E",        # pycodestyle errors
     "W",        # pycodestyle warnings
     "C90",      # mccabe
```

### Comparing `universi-0.1.0/setup.py` & `universi-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['universi']
+['universi', 'universi.structure']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['typer[all]', 'typing-extensions']
+['fastapi>=0.96.1',
+ 'type-inspector>=1.2.2,<2.0.0',
+ 'typer[all]',
+ 'typing-extensions']
 
 entry_points = \
 {'console_scripts': ['universi = universi.__main__:app']}
 
 setup_kwargs = {
     'name': 'universi',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# universi\n\nPackage description\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ovsyanka83/universi',
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['universi']
-package_data = \ {'': ['*']} install_requires = \ ['typer[all]', 'typing-
+# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['universi',
+'universi.structure'] package_data = \ {'': ['*']} install_requires = \
+['fastapi>=0.96.1', 'type-inspector>=1.2.2,<2.0.0', 'typer[all]', 'typing-
 extensions'] entry_points = \ {'console_scripts': ['universi =
 universi.__main__:app']} setup_kwargs = { 'name': 'universi', 'version':
-'0.1.0', 'description': '', 'long_description': '# universi\n\nPackage
+'0.1.1', 'description': '', 'long_description': '# universi\n\nPackage
 description\n\n---\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
 \n\n## Installation\n\n```bash\npip install universi\n```\n', 'author':
 'Stanislav Zmiev', 'author_email': 'szmiev2000@gmail.com', 'maintainer':
 'None', 'maintainer_email': 'None', 'url': 'https://github.com/ovsyanka83/
 universi', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'entry_points': entry_points,
```

### Comparing `universi-0.1.0/PKG-INFO` & `universi-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: universi
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/ovsyanka83/universi
 License: MIT
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.96.1)
+Requires-Dist: type-inspector (>=1.2.2,<2.0.0)
 Requires-Dist: typer[all]
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/ovsyanka83/universi
 Description-Content-Type: text/markdown
 
 # universi
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
-Metadata-Version: 2.1 Name: universi Version: 0.1.0 Summary: Home-page: https:/
+Metadata-Version: 2.1 Name: universi Version: 0.1.1 Summary: Home-page: https:/
 /github.com/ovsyanka83/universi License: MIT Author: Stanislav Zmiev Author-
 email: szmiev2000@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: typer[all] Requires-Dist: typing-
-extensions Project-URL: Repository, https://github.com/ovsyanka83/universi
-Description-Content-Type: text/markdown # universi Package description ---
+Language :: Python :: 3.11 Requires-Dist: fastapi (>=0.96.1) Requires-Dist:
+type-inspector (>=1.2.2,<2.0.0) Requires-Dist: typer[all] Requires-Dist:
+typing-extensions Project-URL: Repository, https://github.com/ovsyanka83/
+universi Description-Content-Type: text/markdown # universi Package description
+---
              [Test] [Coverage] [PyPI] [Supported_Python_versions]
 ## Installation ```bash pip install universi ```
```


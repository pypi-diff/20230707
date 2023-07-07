# Comparing `tmp/jaraco.path-3.6.0.tar.gz` & `tmp/jaraco.path-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.path-3.6.0.tar", last modified: Sun Jun 18 21:20:13 2023, max compression
+gzip compressed data, was "jaraco.path-3.7.0.tar", last modified: Fri Jul  7 15:50:43 2023, max compression
```

## Comparing `jaraco.path-3.6.0.tar` & `jaraco.path-3.7.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/jaraco/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/jaraco.path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-18 21:20:13.000000 jaraco.path-3.6.0/jaraco.path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 21:20:13.933183 jaraco.path-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-18 21:19:47.000000 jaraco.path-3.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.014680 jaraco.path-3.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.014680 jaraco.path-3.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/jaraco/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/jaraco.path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-07 15:50:42.000000 jaraco.path-3.7.0/jaraco.path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-07 15:50:43.000000 jaraco.path-3.7.0/jaraco.path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 15:50:42.000000 jaraco.path-3.7.0/jaraco.path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-07 15:50:42.000000 jaraco.path-3.7.0/jaraco.path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 15:50:42.000000 jaraco.path-3.7.0/jaraco.path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 15:50:43.018680 jaraco.path-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 15:50:22.000000 jaraco.path-3.7.0/tox.ini
```

### Comparing `jaraco.path-3.6.0/.github/workflows/main.yml` & `jaraco.path-3.7.0/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,61 +38,55 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -115,16 +109,16 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.path-3.6.0/CHANGES.rst` & `jaraco.path-3.7.0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.7.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v3.6.0
 ======
 
 Added support for ``Symlink``s for the tree maker (``build``).
 
 v3.5.0
 ======
```

### Comparing `jaraco.path-3.6.0/LICENSE` & `jaraco.path-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.6.0/PKG-INFO` & `jaraco.path-3.7.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.path
-Version: 3.6.0
+Version: 3.7.0
 Summary: miscellaneous path functions
 Home-page: https://github.com/jaraco/jaraco.path
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.path.svg
    :target: https://pypi.org/project/jaraco.path
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.path.svg
 
 .. image:: https://github.com/jaraco/jaraco.path/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.path-3.6.0/README.rst` & `jaraco.path-3.7.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.path.svg
 
 .. image:: https://github.com/jaraco/jaraco.path/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.path-3.6.0/docs/conf.py` & `jaraco.path-3.7.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `jaraco.path-3.6.0/jaraco/path.py` & `jaraco.path-3.7.0/jaraco/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,16 @@
 import datetime
 import glob
 import tempfile
 import platform
 import ctypes
 import importlib
 import pathlib
-from typing import Dict, Union
-
-try:
-    from typing import Protocol, runtime_checkable
-except ImportError:  # pragma: no cover
-    # Python 3.7
-    from typing_extensions import Protocol, runtime_checkable  # type: ignore
+from typing import Dict, Protocol, Union
+from typing import runtime_checkable
 
 
 log = logging.getLogger(__name__)
 
 
 def get_unique_pathname(path, root=''):
     """Return a pathname possibly with a number appended to it so that it is
```

### Comparing `jaraco.path-3.6.0/jaraco.path.egg-info/PKG-INFO` & `jaraco.path-3.7.0/jaraco.path.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.path
-Version: 3.6.0
+Version: 3.7.0
 Summary: miscellaneous path functions
 Home-page: https://github.com/jaraco/jaraco.path
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.path.svg
    :target: https://pypi.org/project/jaraco.path
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.path.svg
 
 .. image:: https://github.com/jaraco/jaraco.path/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.path/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.path-3.6.0/pytest.ini` & `jaraco.path-3.7.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.6.0/setup.cfg` & `jaraco.path-3.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	pyobjc; platform_system == "Darwin" and platform_python_implementation != "PyPy"
-	typing-extensions>=3.6.4; python_version < "3.8"
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
@@ -32,21 +31,21 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	jaraco.windows; platform_system == "Windows"
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
```

### Comparing `jaraco.path-3.6.0/tests/test_path.py` & `jaraco.path-3.7.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `jaraco.path-3.6.0/tox.ini` & `jaraco.path-3.7.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -21,14 +17,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```


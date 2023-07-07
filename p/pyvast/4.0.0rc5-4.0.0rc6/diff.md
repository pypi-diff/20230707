# Comparing `tmp/pyvast-4.0.0rc5.tar.gz` & `tmp/pyvast-4.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvast-4.0.0rc5.tar", max compression
+gzip compressed data, was "pyvast-4.0.0rc6.tar", max compression
```

## Comparing `pyvast-4.0.0rc5.tar` & `pyvast-4.0.0rc6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1846 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/README.md
--rw-r--r--   0        0        0     1524 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0       75 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/__init__.py
--rw-r--r--   0        0        0     5814 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/apps/thehive.py
--rw-r--r--   0        0        0     7461 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/utils/arrow.py
--rw-r--r--   0        0        0     2058 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/utils/asyncio.py
--rw-r--r--   0        0        0      736 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/utils/config.py
--rw-r--r--   0        0        0     1925 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/utils/logging.py
--rw-r--r--   0        0        0       70 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/vast/__init__.py
--rw-r--r--   0        0        0     2879 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/vast/cli.py
--rw-r--r--   0        0        0     3637 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/vast/convert.py
--rw-r--r--   0        0        0     6121 2023-07-06 16:13:00.905252 pyvast-4.0.0rc5/pyvast/vast/vast.py
--rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 pyvast-4.0.0rc5/setup.py
--rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 pyvast-4.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1846 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/README.md
+-rw-r--r--   0        0        0     1524 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/__init__.py
+-rw-r--r--   0        0        0     5814 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/apps/thehive.py
+-rw-r--r--   0        0        0     7461 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/utils/arrow.py
+-rw-r--r--   0        0        0     2058 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/utils/asyncio.py
+-rw-r--r--   0        0        0      736 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/utils/config.py
+-rw-r--r--   0        0        0     1925 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/utils/logging.py
+-rw-r--r--   0        0        0       70 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/vast/__init__.py
+-rw-r--r--   0        0        0     2879 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/vast/cli.py
+-rw-r--r--   0        0        0     3637 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/vast/convert.py
+-rw-r--r--   0        0        0     6121 2023-07-07 20:39:13.539969 pyvast-4.0.0rc6/pyvast/vast/vast.py
+-rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 pyvast-4.0.0rc6/setup.py
+-rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 pyvast-4.0.0rc6/PKG-INFO
```

### Comparing `pyvast-4.0.0rc5/README.md` & `pyvast-4.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyproject.toml` & `pyvast-4.0.0rc6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvast"
-version = "4.0.0-rc5"
+version = "4.0.0-rc6"
 description = "A security telemetry engine for detection and response"
 authors = ["Tenzir <engineering@tenzir.com>"]
 maintainers = ["Tenzir <engineering@tenzir.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pyvast-4.0.0rc5/pyvast/apps/thehive.py` & `pyvast-4.0.0rc6/pyvast/apps/thehive.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/utils/arrow.py` & `pyvast-4.0.0rc6/pyvast/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/utils/asyncio.py` & `pyvast-4.0.0rc6/pyvast/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/utils/config.py` & `pyvast-4.0.0rc6/pyvast/utils/config.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/utils/logging.py` & `pyvast-4.0.0rc6/pyvast/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/vast/cli.py` & `pyvast-4.0.0rc6/pyvast/vast/cli.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/vast/convert.py` & `pyvast-4.0.0rc6/pyvast/vast/convert.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/pyvast/vast/vast.py` & `pyvast-4.0.0rc6/pyvast/vast/vast.py`

 * *Files identical despite different names*

### Comparing `pyvast-4.0.0rc5/setup.py` & `pyvast-4.0.0rc6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 entry_points = \
 {'console_scripts': ['app-thehive-count-alerts = '
                      'pyvast.apps.thehive:count_alerts',
                      'app-thehive-run = pyvast.apps.thehive:run']}
 
 setup_kwargs = {
     'name': 'pyvast',
-    'version': '4.0.0rc5',
+    'version': '4.0.0rc6',
     'description': 'A security telemetry engine for detection and response',
     'long_description': '# VAST Python\n\nThe Python package of VAST provides a flexible control plane to integrate VAST\nwith other security tools.\n\n> **Note**\n> The Python effort is still highly experimental and subject to rapid change.\n> Please do not consider it for production use.\n\n## Usage\n\nTo get started, clone the VAST repository and install the Python package via\n[Poetry](https://python-poetry.org/docs/):\n\n```bash\ngit clone https://github.com/tenzir/vast.git\ncd vast/python\npoetry install\n```\n\n## Development\n\nWe recommend that you work with an editable installation, which is the default\nfor `poetry install`.\n\n### Unit Tests\n\nRun the unit tests via pytest:\n\n```bash\npoetry run pytest\n```\n\n### Integration Tests\n\nRun the integrations tests via Docker Compose and pytest:\n\n```bash\n./docker-poetry-run.sh pytest -v\n```\n\n## Packaging\n\nThe following instructions concern maintainers who want to publish the Python\npackage to PyPI.\n\n> **Note**\n> Our releasing scripts and CI run these steps automatically. You do not need to\n> intervene anywhere. The instructions below merely document the steps taken.\n\n### Bump the version\n\nPrior to releasing a new version, bump the version, e.g.:\n\n```bash\npoetry version 2.3.1\n```\n\nThis updates the `pyproject.toml` file.\n\n### Publish to Test PyPI\n\n1. Add a Test PyPi repository:\n\n   ```bash\n   poetry config repositories.test-pypi https://test.pypi.org/legacy/\n   ```\n\n2. Get the token from <https://test.pypi.org/manage/account/token/>.\n\n3. Store the token:\n\n  ```bash\n  poetry config pypi-token.test-pypi pypi-XXXXXXXX\n  ```\n\n4. Publish:\n  \n   ```bash\n   poetry publish --build -r test-pypi\n   ```\n\n### Publish to PyPI\n\n1. Get the token from <https://pypi.org/manage/account/token/>.\n\n2. Store the token:\n\n  ```bash\n  poetry config pypi-token.pypi pypi-XXXXXXXX\n  ```\n\n3. Publish\n\n   ```bash\n   poetry publish --build\n   ```\n',
     'author': 'Tenzir',
     'author_email': 'engineering@tenzir.com',
     'maintainer': 'Tenzir',
     'maintainer_email': 'engineering@tenzir.com',
     'url': 'https://vast.io',
```

### Comparing `pyvast-4.0.0rc5/PKG-INFO` & `pyvast-4.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvast
-Version: 4.0.0rc5
+Version: 4.0.0rc6
 Summary: A security telemetry engine for detection and response
 Home-page: https://vast.io
 License: BSD-3-Clause
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Maintainer: Tenzir
 Maintainer-email: engineering@tenzir.com
```


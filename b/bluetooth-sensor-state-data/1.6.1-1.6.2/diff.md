# Comparing `tmp/bluetooth_sensor_state_data-1.6.1.tar.gz` & `tmp/bluetooth_sensor_state_data-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_sensor_state_data-1.6.1.tar", max compression
+gzip compressed data, was "bluetooth_sensor_state_data-1.6.2.tar", max compression
```

## Comparing `bluetooth_sensor_state_data-1.6.1.tar` & `bluetooth_sensor_state_data-1.6.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11345 2023-02-06 23:32:38.044115 bluetooth_sensor_state_data-1.6.1/LICENSE
--rw-r--r--   0        0        0     3740 2023-02-06 23:32:38.044115 bluetooth_sensor_state_data-1.6.1/README.md
--rw-r--r--   0        0        0     2532 2023-02-06 23:32:39.068133 bluetooth_sensor_state_data-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     2979 2023-02-06 23:32:39.016132 bluetooth_sensor_state_data-1.6.1/src/bluetooth_sensor_state_data/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 23:32:38.044115 bluetooth_sensor_state_data-1.6.1/src/bluetooth_sensor_state_data/py.typed
--rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 bluetooth_sensor_state_data-1.6.1/setup.py
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 bluetooth_sensor_state_data-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-07-07 17:34:25.427437 bluetooth_sensor_state_data-1.6.2/LICENSE
+-rw-r--r--   0        0        0     3740 2023-07-07 17:34:25.427437 bluetooth_sensor_state_data-1.6.2/README.md
+-rw-r--r--   0        0        0     2532 2023-07-07 17:34:26.435433 bluetooth_sensor_state_data-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3128 2023-07-07 17:34:26.399433 bluetooth_sensor_state_data-1.6.2/src/bluetooth_sensor_state_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 17:34:25.427437 bluetooth_sensor_state_data-1.6.2/src/bluetooth_sensor_state_data/py.typed
+-rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 bluetooth_sensor_state_data-1.6.2/PKG-INFO
```

### Comparing `bluetooth_sensor_state_data-1.6.1/LICENSE` & `bluetooth_sensor_state_data-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_sensor_state_data-1.6.1/README.md` & `bluetooth_sensor_state_data-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_sensor_state_data-1.6.1/pyproject.toml` & `bluetooth_sensor_state_data-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-sensor-state-data"
-version = "1.6.1"
+version = "1.6.2"
 description = "Models for storing and converting Bluetooth Sensor State Data"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-sensor-state-data"
 documentation = "https://bluetooth-sensor-state-data.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_sensor_state_data-1.6.1/src/bluetooth_sensor_state_data/__init__.py` & `bluetooth_sensor_state_data-1.6.2/src/bluetooth_sensor_state_data/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 from abc import abstractmethod
 
 from home_assistant_bluetooth import BluetoothServiceInfo
 from sensor_state_data import DeviceClass, SensorData, SensorUpdate, Units
 
 SIGNAL_STRENGTH_KEY = DeviceClass.SIGNAL_STRENGTH.value
@@ -64,14 +64,18 @@
     def supported(self, data: BluetoothServiceInfo) -> bool:
         """Return True if the device is supported."""
         self._start_update(data)
         return bool(self._device_id_to_type)
 
     def update(self, data: BluetoothServiceInfo) -> SensorUpdate:
         """Update a device."""
+        # Ensure events from previous
+        # updates are not carried over
+        # as events are transient.
+        self._events_updates.clear()
         self._start_update(data)
         self.update_signal_strength(data.rssi)
         return self._finish_update()
 
     def update_signal_strength(self, native_value: int | float) -> None:
         """Quick update for an signal strength sensor."""
         for device_id in self._device_id_to_type:
```

### Comparing `bluetooth_sensor_state_data-1.6.1/setup.py` & `bluetooth_sensor_state_data-1.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,91 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bluetooth-sensor-state-data
+Version: 1.6.2
+Summary: Models for storing and converting Bluetooth Sensor State Data
+Home-page: https://github.com/bluetooth-devices/bluetooth-sensor-state-data
+License: Apache Software License 2.0
+Author: J. Nick Koston
+Author-email: nick@koston.org
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: docs
+Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
+Requires-Dist: home-assistant-bluetooth (>=1.3.0)
+Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
+Requires-Dist: sensor-state-data (>=2.0)
+Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
+Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bluetooth-sensor-state-data/issues
+Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-sensor-state-data/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://bluetooth-sensor-state-data.readthedocs.io
+Project-URL: Repository, https://github.com/bluetooth-devices/bluetooth-sensor-state-data
+Description-Content-Type: text/markdown
+
+# bluetooth-sensor-state-data
+
+<p align="center">
+  <a href="https://github.com/bluetooth-devices/bluetooth-sensor-state-data/actions?query=workflow%3ACI">
+    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/bluetooth-sensor-state-data/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >
+  </a>
+  <a href="https://bluetooth-sensor-state-data.readthedocs.io">
+    <img src="https://img.shields.io/readthedocs/bluetooth-sensor-state-data.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">
+  </a>
+  <a href="https://codecov.io/gh/bluetooth-devices/bluetooth-sensor-state-data">
+    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/bluetooth-sensor-state-data.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">
+  </a>
+</p>
+<p align="center">
+  <a href="https://python-poetry.org/">
+    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">
+  </a>
+  <a href="https://github.com/ambv/black">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">
+  </a>
+  <a href="https://github.com/pre-commit/pre-commit">
+    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">
+  </a>
+</p>
+<p align="center">
+  <a href="https://pypi.org/project/bluetooth-sensor-state-data/">
+    <img src="https://img.shields.io/pypi/v/bluetooth-sensor-state-data.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">
+  </a>
+  <img src="https://img.shields.io/pypi/pyversions/bluetooth-sensor-state-data.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">
+  <img src="https://img.shields.io/pypi/l/bluetooth-sensor-state-data.svg?style=flat-square" alt="License">
+</p>
+
+Models for storing and converting Bluetooth Sensor State Data
+
+## Installation
+
+Install this via pip (or your favourite package manager):
+
+`pip install bluetooth-sensor-state-data`
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- prettier-ignore-start -->
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-enable -->
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+<!-- prettier-ignore-end -->
+
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
+## Credits
+
+This package was created with
+[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)
+project template.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['bluetooth_sensor_state_data']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['home-assistant-bluetooth>=1.3.0', 'sensor-state-data>=2.0']
-
-extras_require = \
-{'docs': ['Sphinx>=5.0,<6.0',
-          'sphinx-rtd-theme>=1.0,<2.0',
-          'myst-parser>=0.18,<0.19']}
-
-setup_kwargs = {
-    'name': 'bluetooth-sensor-state-data',
-    'version': '1.6.1',
-    'description': 'Models for storing and converting Bluetooth Sensor State Data',
-    'long_description': '# bluetooth-sensor-state-data\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/bluetooth-sensor-state-data/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/bluetooth-sensor-state-data/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://bluetooth-sensor-state-data.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/bluetooth-sensor-state-data.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/bluetooth-sensor-state-data">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/bluetooth-sensor-state-data.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/bluetooth-sensor-state-data/">\n    <img src="https://img.shields.io/pypi/v/bluetooth-sensor-state-data.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/bluetooth-sensor-state-data.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/bluetooth-sensor-state-data.svg?style=flat-square" alt="License">\n</p>\n\nModels for storing and converting Bluetooth Sensor State Data\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install bluetooth-sensor-state-data`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
-    'author': 'J. Nick Koston',
-    'author_email': 'nick@koston.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/bluetooth-devices/bluetooth-sensor-state-data',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,29 +1,33 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['bluetooth_sensor_state_data'] package_data = \ {'':
-['*']} install_requires = \ ['home-assistant-bluetooth>=1.3.0', 'sensor-state-
-data>=2.0'] extras_require = \ {'docs': ['Sphinx>=5.0,<6.0', 'sphinx-rtd-
-theme>=1.0,<2.0', 'myst-parser>=0.18,<0.19']} setup_kwargs = { 'name':
-'bluetooth-sensor-state-data', 'version': '1.6.1', 'description': 'Models for
-storing and converting Bluetooth Sensor State Data', 'long_description': '#
-bluetooth-sensor-state-data\n\n
-     \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
-                                percentage]\n\n
-\n
-             \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
-\n
-      \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
-\n\nModels for storing and converting Bluetooth Sensor State Data\n\n##
-Installation\n\nInstall this via pip (or your favourite package manager):
-\n\n`pip install bluetooth-sensor-state-data`\n\n## Contributors â¨\n\nThanks
-goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
-en/emoji-key)):\n\n\n\n\n\n\n\n\nThis project follows the [all-contributors]
-(https://github.com/all-contributors/all-contributors) specification.
-Contributions of any kind welcome!\n\n## Credits\n\nThis package was created
-with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n
-[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/
-cookiecutter-pypackage)\nproject template.\n', 'author': 'J. Nick Koston',
-'author_email': 'nick@koston.org', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/bluetooth-devices/bluetooth-sensor-state-
-data', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'extras_require':
-extras_require, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: bluetooth-sensor-state-data Version: 1.6.2 Summary:
+Models for storing and converting Bluetooth Sensor State Data Home-page: https:
+//github.com/bluetooth-devices/bluetooth-sensor-state-data License: Apache
+Software License 2.0 Author: J. Nick Koston Author-email: nick@koston.org
+Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers Classifier: License :: Other/
+Proprietary License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries Provides-Extra: docs
+Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist: home-
+assistant-bluetooth (>=1.3.0) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra
+== "docs" Requires-Dist: sensor-state-data (>=2.0) Requires-Dist: sphinx-rtd-
+theme (>=1.0,<2.0) ; extra == "docs" Project-URL: Bug Tracker, https://
+github.com/bluetooth-devices/bluetooth-sensor-state-data/issues Project-URL:
+Changelog, https://github.com/bluetooth-devices/bluetooth-sensor-state-data/
+blob/main/CHANGELOG.md Project-URL: Documentation, https://bluetooth-sensor-
+state-data.readthedocs.io Project-URL: Repository, https://github.com/
+bluetooth-devices/bluetooth-sensor-state-data Description-Content-Type: text/
+markdown # bluetooth-sensor-state-data
+         [CI_Status] [Documentation_Status] [Test_coverage_percentage]
+                         [Poetry] [black] [pre-commit]
+             [PyPI_Version] [Supported Python versions] [License]
+Models for storing and converting Bluetooth Sensor State Data ## Installation
+Install this via pip (or your favourite package manager): `pip install
+bluetooth-sensor-state-data` ## Contributors â¨ Thanks goes to these wonderful
+people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):       This
+project follows the [all-contributors](https://github.com/all-contributors/all-
+contributors) specification. Contributions of any kind welcome! ## Credits This
+package was created with [Cookiecutter](https://github.com/audreyr/
+cookiecutter) and the [browniebroke/cookiecutter-pypackage](https://github.com/
+browniebroke/cookiecutter-pypackage) project template.
```


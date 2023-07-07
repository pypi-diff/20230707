# Comparing `tmp/mytoyota-0.9.1.tar.gz` & `tmp/mytoyota-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytoyota-0.9.1.tar", max compression
+gzip compressed data, was "mytoyota-0.9.2.tar", max compression
```

## Comparing `mytoyota-0.9.1.tar` & `mytoyota-0.9.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1090 2022-12-07 16:18:08.585079 mytoyota-0.9.1/LICENSE
--rw-r--r--   0        0        0     4074 2022-12-07 16:18:08.585079 mytoyota-0.9.1/README.md
--rw-r--r--   0        0        0      281 2022-12-07 16:18:08.585079 mytoyota-0.9.1/mytoyota/__init__.py
--rw-r--r--   0        0        0     5028 2022-12-07 16:18:08.585079 mytoyota-0.9.1/mytoyota/api.py
--rw-r--r--   0        0        0    22029 2022-12-07 16:18:08.585079 mytoyota-0.9.1/mytoyota/client.py
--rw-r--r--   0        0        0     1757 2022-12-07 16:18:08.585079 mytoyota-0.9.1/mytoyota/const.py
--rw-r--r--   0        0        0     8618 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/controller.py
--rw-r--r--   0        0        0      784 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/exceptions.py
--rw-r--r--   0        0        0     3191 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/dashboard.py
--rw-r--r--   0        0        0      305 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/data.py
--rw-r--r--   0        0        0     3133 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/hvac.py
--rw-r--r--   0        0        0      559 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/location.py
--rw-r--r--   0        0        0     1945 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/lock_unlock.py
--rw-r--r--   0        0        0     4799 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/sensors.py
--rw-r--r--   0        0        0     2740 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/trip.py
--rw-r--r--   0        0        0     4747 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/models/vehicle.py
--rw-r--r--   0        0        0     5157 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/statistics.py
--rw-r--r--   0        0        0        0 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/utils/__init__.py
--rw-r--r--   0        0        0      753 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/utils/conversions.py
--rw-r--r--   0        0        0      374 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/utils/formatters.py
--rw-r--r--   0        0        0      358 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/utils/locale.py
--rw-r--r--   0        0        0     1330 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/utils/logs.py
--rw-r--r--   0        0        0      418 2022-12-07 16:18:08.589079 mytoyota-0.9.1/mytoyota/utils/token.py
--rw-r--r--   0        0        0     1794 2022-12-07 16:18:08.589079 mytoyota-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 mytoyota-0.9.1/setup.py
--rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 mytoyota-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-07 12:12:15.418069 mytoyota-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4445 2023-07-07 12:12:15.418069 mytoyota-0.9.2/README.md
+-rw-r--r--   0        0        0      281 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/__init__.py
+-rw-r--r--   0        0        0     5028 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/api.py
+-rw-r--r--   0        0        0    22098 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/client.py
+-rw-r--r--   0        0        0     1769 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/const.py
+-rw-r--r--   0        0        0     8718 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/controller.py
+-rw-r--r--   0        0        0      784 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/exceptions.py
+-rw-r--r--   0        0        0     3191 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/dashboard.py
+-rw-r--r--   0        0        0      305 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/data.py
+-rw-r--r--   0        0        0     3133 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/hvac.py
+-rw-r--r--   0        0        0      559 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/location.py
+-rw-r--r--   0        0        0     1945 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/lock_unlock.py
+-rw-r--r--   0        0        0     4799 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/sensors.py
+-rw-r--r--   0        0        0     2740 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/trip.py
+-rw-r--r--   0        0        0     4747 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/models/vehicle.py
+-rw-r--r--   0        0        0     5157 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/statistics.py
+-rw-r--r--   0        0        0        0 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/utils/__init__.py
+-rw-r--r--   0        0        0      753 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/utils/conversions.py
+-rw-r--r--   0        0        0      374 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/utils/formatters.py
+-rw-r--r--   0        0        0      358 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/utils/locale.py
+-rw-r--r--   0        0        0     1330 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/utils/logs.py
+-rw-r--r--   0        0        0      418 2023-07-07 12:12:15.418069 mytoyota-0.9.2/mytoyota/utils/token.py
+-rw-r--r--   0        0        0     1847 2023-07-07 12:12:15.418069 mytoyota-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5567 1970-01-01 00:00:00.000000 mytoyota-0.9.2/PKG-INFO
```

### Comparing `mytoyota-0.9.1/LICENSE` & `mytoyota-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/README.md` & `mytoyota-0.9.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [![GitHub Workflow Status][workflow-shield]][workflow]
 [![GitHub Release][releases-shield]][releases]
 [![GitHub Activity][commits-shield]][commits]
 
-# Toyota Connected Services Python module
+# Toyota Connected Services Europe Python module
 
 ### [!] **This is still in beta**
 
+### [!] **Only EU is supported, other regions are not possible so far. See [this](https://github.com/widewing/toyota-na) for North America**
+
 ## Description
 
-Python 3 package to communicate with Toyota Connected Services.
+Python 3 package to communicate with [Toyota Connected Europe](https://www.toyota-europe.com/about-us/toyota-in-europe/toyota-connected-europe) Services.
 This is an unofficial package and Toyota can change their API at any point without warning.
 
 ## Installation
 
 This package can be installed through `pip`.
 
 ```text
@@ -24,20 +26,21 @@
 ```python
 import json
 import asyncio
 from mytoyota.client import MyT
 
 username = "jane@doe.com"
 password = "MyPassword"
+brand = "toyota"  # or lexus
 
 # Get supported regions, can be passed to the optional 'region' argument of MyT
+# At this moment, only the 'europe' region is supported
 print(MyT.get_supported_regions())
 
-client = MyT(username=username, password=password)
-
+client = MyT(username=username, password=password, brand=brand)
 
 async def get_information():
     print("Logging in...")
     await client.login()
 
     print("Retrieving cars...")
     # Returns cars registered to your account + information about each car.
@@ -91,25 +94,25 @@
 
 ## Docs
 
 Coming soon...
 
 ## Contributing
 
-This python module uses poetry and pre-commit.
+This python module uses poetry (>= 1.2.2) and pre-commit.
 
 To start contributing, fork this repository and run `poetry install`. Then create a new branch. Before making a PR, please run pre-commit `poetry run pre-commit run --all-files` and make sure that all tests passes locally first.
 
 ## Note
 
 As I [@DurgNomis-drol](https://github.com/DurgNomis-drol) am not a professional programmer. I will try to maintain it as best as I can. If someone is interested in helping with this, they are more the welcome to message me to be a collaborator on this project.
 
 ## Credits
 
 A huge thanks go to [@calmjm](https://github.com/calmjm) for making [tojota](https://github.com/calmjm/tojota).
 
 [releases-shield]: https://img.shields.io/github/release/DurgNomis-drol/mytoyota.svg?style=for-the-badge
 [releases]: https://github.com/DurgNomis-drol/mytoyota/releases
-[workflow-shield]: https://img.shields.io/github/workflow/status/DurgNomis-drol/mytoyota/Linting?style=for-the-badge
+[workflow-shield]: https://img.shields.io/github/actions/workflow/status/DurgNomis-drol/mytoyota/build.yml?branch=master&style=for-the-badge
 [workflow]: https://github.com/DurgNomis-drol/mytoyota/actions
 [commits-shield]: https://img.shields.io/github/commit-activity/y/DurgNomis-drol/mytoyota.svg?style=for-the-badge
 [commits]: https://github.com/DurgNomis-drol/mytoyota/commits/master
```

### Comparing `mytoyota-0.9.1/mytoyota/api.py` & `mytoyota-0.9.2/mytoyota/api.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/client.py` & `mytoyota-0.9.2/mytoyota/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 
     def __init__(
         self,
         username: str,
         password: str,
         locale: str = "da-dk",
         region: str = "europe",
-        uuid: str = None,
+        brand: str = "toyota",
+        uuid: str | None = None,
         controller_class=Controller,
         disable_locale_check: bool = False,
     ) -> None:
         """Toyota API"""
 
         if username is None or "@" not in username:
             raise ToyotaInvalidUsername
@@ -83,14 +84,15 @@
 
         self.api = Api(
             controller_class(
                 username=username,
                 password=password,
                 locale=locale,
                 region=region,
+                brand=brand,
                 uuid=uuid,
             )
         )
 
     @staticmethod
     def get_supported_regions() -> list:
         """Get supported regions.
```

### Comparing `mytoyota-0.9.1/mytoyota/const.py` & `mytoyota-0.9.2/mytoyota/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,13 +57,16 @@
 
 INTERVAL_SUPPORTED = ["day", "week", "isoweek", "month", "year"]
 
 BASE_HEADERS = {
     "Content-Type": "application/json;charset=UTF-8",
     "Accept": "application/json, text/plain, */*",
     "Sec-Fetch-Dest": "empty",
-    "X-TME-BRAND": "TOYOTA",
-    "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.103 Safari/537.36",
+    "User-Agent": (
+        "Mozilla/5.0 (X11; Linux x86_64) "
+        "AppleWebKit/537.36 (KHTML, like Gecko) "
+        "Chrome/51.0.2704.103 Safari/537.36"
+    ),
 }
 
 # Timestamps
 UNLOCK_TIMESTAMP_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
```

### Comparing `mytoyota-0.9.1/mytoyota/controller.py` & `mytoyota-0.9.2/mytoyota/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,22 @@
 
     def __init__(
         self,
         locale: str,
         region: str,
         username: str,
         password: str,
+        brand: str,
         uuid: str | None = None,
     ) -> None:
         self._locale = locale
         self._region = region
         self._username = username
         self._password = password
+        self._brand = brand
         self._uuid = uuid
 
     @property
     def _auth_endpoint(self) -> str:
         """Returns auth endpoint."""
         return SUPPORTED_REGIONS[self._region].get(ENDPOINT_AUTH)
 
@@ -172,14 +174,15 @@
 
         headers.update(
             {
                 "X-TME-LC": self._locale,
                 "X-TME-LOCALE": self._locale,
                 "X-TME-TOKEN": self._token,
                 "X-TME-APP-VERSION": "4.10.0",
+                "X-TME-BRAND": self._brand.upper(),
             }
         )
 
         if method in ("GET", "POST"):
             headers.update(
                 {
                     "Cookie": f"iPlanetDirectoryPro={self._token}",
```

### Comparing `mytoyota-0.9.1/mytoyota/exceptions.py` & `mytoyota-0.9.2/mytoyota/exceptions.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/dashboard.py` & `mytoyota-0.9.2/mytoyota/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/hvac.py` & `mytoyota-0.9.2/mytoyota/models/hvac.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/location.py` & `mytoyota-0.9.2/mytoyota/models/location.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/lock_unlock.py` & `mytoyota-0.9.2/mytoyota/models/lock_unlock.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/sensors.py` & `mytoyota-0.9.2/mytoyota/models/sensors.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/trip.py` & `mytoyota-0.9.2/mytoyota/models/trip.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/models/vehicle.py` & `mytoyota-0.9.2/mytoyota/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/statistics.py` & `mytoyota-0.9.2/mytoyota/statistics.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/utils/conversions.py` & `mytoyota-0.9.2/mytoyota/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/mytoyota/utils/logs.py` & `mytoyota-0.9.2/mytoyota/utils/logs.py`

 * *Files identical despite different names*

### Comparing `mytoyota-0.9.1/pyproject.toml` & `mytoyota-0.9.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "mytoyota"
 description = "Python client for Toyota Connected Services."
 authors = ["Simon Grud Hansen <simongrud@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-version = "0.9.1"
+version = "0.9.2"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -30,15 +30,15 @@
 langcodes = "^3.1"
 httpx = ">=0.18.1"
 arrow = "^1.1"
 importlib-metadata = {version = "^1.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.20.0"
-black = "^22.10.0"
+black = ">=22.3, !=22.10.0"  # https://github.com/psf/black/issues/3312
 flake8 = "^3.8.4"
 flake8-bugbear = "^22.10.27"
 flake8-comprehensions = "^3.4.0"
 pylint = "^2.7.2"
 isort = "^5.10.1"
 codespell = "^2.0.0"
 pytest = "^7.2.0"
```

### Comparing `mytoyota-0.9.1/setup.py` & `mytoyota-0.9.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,146 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mytoyota
+Version: 0.9.2
+Summary: Python client for Toyota Connected Services.
+Home-page: https://github.com/DurgNomis-drol/mytoyota
+License: MIT
+Keywords: Toyota,Car,MYT
+Author: Simon Grud Hansen
+Author-email: simongrud@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arrow (>=1.1,<2.0)
+Requires-Dist: httpx (>=0.18.1)
+Requires-Dist: importlib-metadata (>=1.0,<2.0) ; python_version < "3.8"
+Requires-Dist: langcodes (>=3.1,<4.0)
+Project-URL: Bug Tracker, https://github.com/DurgNomis-drol/mytoyota/issues
+Project-URL: Repository, https://github.com/DurgNomis-drol/mytoyota
+Project-URL: Release Notes, https://github.com/DurgNomis-drol/mytoyota/releases
+Description-Content-Type: text/markdown
 
-packages = \
-['mytoyota', 'mytoyota.models', 'mytoyota.utils']
+[![GitHub Workflow Status][workflow-shield]][workflow]
+[![GitHub Release][releases-shield]][releases]
+[![GitHub Activity][commits-shield]][commits]
 
-package_data = \
-{'': ['*']}
+# Toyota Connected Services Europe Python module
 
-install_requires = \
-['arrow>=1.1,<2.0', 'httpx>=0.18.1', 'langcodes>=3.1,<4.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0']}
-
-setup_kwargs = {
-    'name': 'mytoyota',
-    'version': '0.9.1',
-    'description': 'Python client for Toyota Connected Services.',
-    'long_description': '[![GitHub Workflow Status][workflow-shield]][workflow]\n[![GitHub Release][releases-shield]][releases]\n[![GitHub Activity][commits-shield]][commits]\n\n# Toyota Connected Services Python module\n\n### [!] **This is still in beta**\n\n## Description\n\nPython 3 package to communicate with Toyota Connected Services.\nThis is an unofficial package and Toyota can change their API at any point without warning.\n\n## Installation\n\nThis package can be installed through `pip`.\n\n```text\npip install mytoyota\n```\n\n## Usage\n\n```python\nimport json\nimport asyncio\nfrom mytoyota.client import MyT\n\nusername = "jane@doe.com"\npassword = "MyPassword"\n\n# Get supported regions, can be passed to the optional \'region\' argument of MyT\nprint(MyT.get_supported_regions())\n\nclient = MyT(username=username, password=password)\n\n\nasync def get_information():\n    print("Logging in...")\n    await client.login()\n\n    print("Retrieving cars...")\n    # Returns cars registered to your account + information about each car.\n    cars = await client.get_vehicles()\n\n    for car in cars:\n\n        # Returns live data from car/last time you used it as an object.\n        vehicle = await client.get_vehicle_status(car)\n\n        # You can either get them all async (Recommended) or sync (Look further down).\n        data = await asyncio.gather(\n            *[\n                client.get_driving_statistics(vehicle.vin, interval="day"),\n                client.get_driving_statistics(vehicle.vin, interval="isoweek"),\n                client.get_driving_statistics(vehicle.vin),\n                client.get_driving_statistics(vehicle.vin, interval="year"),\n            ]\n        )\n\n        # You can access odometer data like this:\n        mileage = vehicle.dashboard.odometer\n        # Or retrieve the energy level (electric or gasoline)\n        fuel = vehicle.dashboard.fuel_level\n        battery = vehicle.dashboard.battery_level\n        # Or Parking information:\n        latitude = vehicle.parkinglocation.latitude\n\n        # Daily stats\n        daily_stats = await client.get_driving_statistics(vehicle.vin, interval="day")\n\n        # ISO 8601 week stats\n        iso_weekly_stats = await client.get_driving_statistics(vehicle.vin, interval="isoweek")\n\n        # Monthly stats is returned by default\n        monthly_stats = await client.get_driving_statistics(vehicle.vin)\n\n        # Get year to date stats.\n        yearly_stats = await client.get_driving_statistics(vehicle.vin, interval="year")\n\n\nloop = asyncio.get_event_loop()\nloop.run_until_complete(get_information())\nloop.close()\n\n```\n\n## Known issues\n\n- Statistical endpoint will return `None` if no trip have been performed in the requested timeframe. This problem will often happen at the start of each week, month or year. Also daily stats will of course also be unavailable if no trip have been performed.\n\n## Docs\n\nComing soon...\n\n## Contributing\n\nThis python module uses poetry and pre-commit.\n\nTo start contributing, fork this repository and run `poetry install`. Then create a new branch. Before making a PR, please run pre-commit `poetry run pre-commit run --all-files` and make sure that all tests passes locally first.\n\n## Note\n\nAs I [@DurgNomis-drol](https://github.com/DurgNomis-drol) am not a professional programmer. I will try to maintain it as best as I can. If someone is interested in helping with this, they are more the welcome to message me to be a collaborator on this project.\n\n## Credits\n\nA huge thanks go to [@calmjm](https://github.com/calmjm) for making [tojota](https://github.com/calmjm/tojota).\n\n[releases-shield]: https://img.shields.io/github/release/DurgNomis-drol/mytoyota.svg?style=for-the-badge\n[releases]: https://github.com/DurgNomis-drol/mytoyota/releases\n[workflow-shield]: https://img.shields.io/github/workflow/status/DurgNomis-drol/mytoyota/Linting?style=for-the-badge\n[workflow]: https://github.com/DurgNomis-drol/mytoyota/actions\n[commits-shield]: https://img.shields.io/github/commit-activity/y/DurgNomis-drol/mytoyota.svg?style=for-the-badge\n[commits]: https://github.com/DurgNomis-drol/mytoyota/commits/master\n',
-    'author': 'Simon Grud Hansen',
-    'author_email': 'simongrud@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DurgNomis-drol/mytoyota',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+### [!] **This is still in beta**
 
+### [!] **Only EU is supported, other regions are not possible so far. See [this](https://github.com/widewing/toyota-na) for North America**
+
+## Description
+
+Python 3 package to communicate with [Toyota Connected Europe](https://www.toyota-europe.com/about-us/toyota-in-europe/toyota-connected-europe) Services.
+This is an unofficial package and Toyota can change their API at any point without warning.
+
+## Installation
+
+This package can be installed through `pip`.
+
+```text
+pip install mytoyota
+```
+
+## Usage
+
+```python
+import json
+import asyncio
+from mytoyota.client import MyT
+
+username = "jane@doe.com"
+password = "MyPassword"
+brand = "toyota"  # or lexus
+
+# Get supported regions, can be passed to the optional 'region' argument of MyT
+# At this moment, only the 'europe' region is supported
+print(MyT.get_supported_regions())
+
+client = MyT(username=username, password=password, brand=brand)
+
+async def get_information():
+    print("Logging in...")
+    await client.login()
+
+    print("Retrieving cars...")
+    # Returns cars registered to your account + information about each car.
+    cars = await client.get_vehicles()
+
+    for car in cars:
+
+        # Returns live data from car/last time you used it as an object.
+        vehicle = await client.get_vehicle_status(car)
+
+        # You can either get them all async (Recommended) or sync (Look further down).
+        data = await asyncio.gather(
+            *[
+                client.get_driving_statistics(vehicle.vin, interval="day"),
+                client.get_driving_statistics(vehicle.vin, interval="isoweek"),
+                client.get_driving_statistics(vehicle.vin),
+                client.get_driving_statistics(vehicle.vin, interval="year"),
+            ]
+        )
+
+        # You can access odometer data like this:
+        mileage = vehicle.dashboard.odometer
+        # Or retrieve the energy level (electric or gasoline)
+        fuel = vehicle.dashboard.fuel_level
+        battery = vehicle.dashboard.battery_level
+        # Or Parking information:
+        latitude = vehicle.parkinglocation.latitude
+
+        # Daily stats
+        daily_stats = await client.get_driving_statistics(vehicle.vin, interval="day")
+
+        # ISO 8601 week stats
+        iso_weekly_stats = await client.get_driving_statistics(vehicle.vin, interval="isoweek")
+
+        # Monthly stats is returned by default
+        monthly_stats = await client.get_driving_statistics(vehicle.vin)
+
+        # Get year to date stats.
+        yearly_stats = await client.get_driving_statistics(vehicle.vin, interval="year")
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(get_information())
+loop.close()
+
+```
+
+## Known issues
+
+- Statistical endpoint will return `None` if no trip have been performed in the requested timeframe. This problem will often happen at the start of each week, month or year. Also daily stats will of course also be unavailable if no trip have been performed.
+
+## Docs
+
+Coming soon...
+
+## Contributing
+
+This python module uses poetry (>= 1.2.2) and pre-commit.
+
+To start contributing, fork this repository and run `poetry install`. Then create a new branch. Before making a PR, please run pre-commit `poetry run pre-commit run --all-files` and make sure that all tests passes locally first.
+
+## Note
+
+As I [@DurgNomis-drol](https://github.com/DurgNomis-drol) am not a professional programmer. I will try to maintain it as best as I can. If someone is interested in helping with this, they are more the welcome to message me to be a collaborator on this project.
+
+## Credits
+
+A huge thanks go to [@calmjm](https://github.com/calmjm) for making [tojota](https://github.com/calmjm/tojota).
+
+[releases-shield]: https://img.shields.io/github/release/DurgNomis-drol/mytoyota.svg?style=for-the-badge
+[releases]: https://github.com/DurgNomis-drol/mytoyota/releases
+[workflow-shield]: https://img.shields.io/github/actions/workflow/status/DurgNomis-drol/mytoyota/build.yml?branch=master&style=for-the-badge
+[workflow]: https://github.com/DurgNomis-drol/mytoyota/actions
+[commits-shield]: https://img.shields.io/github/commit-activity/y/DurgNomis-drol/mytoyota.svg?style=for-the-badge
+[commits]: https://github.com/DurgNomis-drol/mytoyota/commits/master
 
-setup(**setup_kwargs)
```


# Comparing `tmp/python-cmr-0.7.0.tar.gz` & `tmp/python_cmr-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cmr-0.7.0.tar", max compression
+gzip compressed data, was "python_cmr-0.8.0.tar", max compression
```

## Comparing `python-cmr-0.7.0.tar` & `python_cmr-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1063 2021-11-23 23:35:26.733944 python-cmr-0.7.0/LICENSE
--rw-r--r--   0        0        0     8017 2021-11-23 23:35:26.733944 python-cmr-0.7.0/README.md
--rw-r--r--   0        0        0      184 2021-11-23 23:35:26.733944 python-cmr-0.7.0/cmr/__init__.py
--rw-r--r--   0        0        0    26298 2021-11-23 23:35:26.733944 python-cmr-0.7.0/cmr/queries.py
--rw-r--r--   0        0        0      617 2021-11-23 23:35:26.733944 python-cmr-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     9025 2021-11-23 23:35:52.525796 python-cmr-0.7.0/setup.py
--rw-r--r--   0        0        0     8759 2021-11-23 23:35:52.526492 python-cmr-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-06 22:12:32.770764 python_cmr-0.8.0/LICENSE
+-rw-r--r--   0        0        0     8379 2023-07-06 22:12:32.770764 python_cmr-0.8.0/README.md
+-rw-r--r--   0        0        0      244 2023-07-06 22:12:32.770764 python_cmr-0.8.0/cmr/__init__.py
+-rw-r--r--   0        0        0    27169 2023-07-06 22:12:32.770764 python_cmr-0.8.0/cmr/queries.py
+-rw-r--r--   0        0        0      617 2023-07-06 22:12:32.770764 python_cmr-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     9172 1970-01-01 00:00:00.000000 python_cmr-0.8.0/PKG-INFO
```

### Comparing `python-cmr-0.7.0/LICENSE` & `python_cmr-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cmr-0.7.0/README.md` & `python_cmr-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -95,14 +95,18 @@
     # note: when uses GranuleQuery, passing a collection's concept ID will filter by granules associated
     #       with that particular collection.
     >>> api.concept_id("C1299783579-LPDAAC_ECS")
     >>> api.concept_id(["G1327299284-LPDAAC_ECS", "G1326330014-LPDAAC_ECS"])
 
     # search by provider
     >>> api.provider('POCLOUD')
+    
+    # search non-ops CMR environment
+    >>> from cmr import CMR_UAT
+    >>> api.mode(CMR_UAT)
 
 Granule searches support these methods (in addition to the shared methods above):
 
     # search for a granule by its unique ID
     >>> api.granule_ur("SC:AST_L1T.003:2150315169")
     # search for granules from a specific orbit
     >>> api.orbit_number(5000)
@@ -207,14 +211,22 @@
     >>> granules = api.get_all()  # this is a shortcut for api.get(api.hits())
 
 By default the responses will return as json and be accessible as a list of python dictionaries. Other formats can be
 specified before making the request:
 
     >>> granules = api.format("echo10").get(100)
 
+We can add token to the api calls by setting headers using the following functions:
+
+    # Use token function for EDL echo-token or launchpad token
+    >>> api.token(token)
+
+    # Use bearer token function for EDL bearer tokens
+    >>> api.bearer_token(token)
+
 The following formats are supported for both granule and collection queries:
 
 - json (default)
 - xml
 - echo10
 - iso
 - iso19115
@@ -276,8 +288,8 @@
 poetry run flake8
 ```
 
 ## Run Tests
 
 ```shell
 poetry run pytest
-```
+```
```

### Comparing `python-cmr-0.7.0/cmr/queries.py` & `python_cmr-0.8.0/cmr/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     def __init__(self, route, mode=CMR_OPS):
         self.params = {}
         self.options = {}
         self._route = route
         self.mode(mode)
         self.concept_id_chars = []
+        self.headers = None
 
     def get(self, limit=2000):
         """
         Get all results up to some limit, even if spanning multiple pages.
 
         :limit: The number of results to return
         :returns: query results as a list
@@ -49,15 +50,15 @@
         page_size = min(limit, 2000)
         url = self._build_url()
 
         results = []
         page = 1
         while len(results) < limit:
 
-            response = get(url, params={'page_size': page_size, 'page_num': page})
+            response = get(url, headers=self.headers, params={'page_size': page_size, 'page_num': page})
 
             try:
                 response.raise_for_status()
             except exceptions.HTTPError as ex:
                 raise RuntimeError(ex.response.text)
 
             if self._format == "json":
@@ -79,15 +80,15 @@
         making a lightweight query to CMR and inspecting the returned headers.
 
         :returns: number of results reproted by CMR
         """
 
         url = self._build_url()
 
-        response = get(url, params={'page_size': 0})
+        response = get(url, headers=self.headers, params={'page_size': 0})
 
         try:
             response.raise_for_status()
         except exceptions.HTTPError as ex:
             raise RuntimeError(ex.response.text)
 
         return int(response.headers["CMR-Hits"])
@@ -269,26 +270,43 @@
         if mode is None:
             raise ValueError("Please provide a valid mode (CMR_OPS, CMR_UAT, CMR_SIT)")
 
         self._base_url = str(mode) + self._route
 
     def token(self, token):
         """
-        Add token into url request.
+        Add token into authorization headers.
 
-        :param token: Token from EDL.
+        :param token: Token from EDL Echo-Token or NASA Launchpad token.
         :returns: Query instance
         """
 
         if not token:
             return self
 
-        self.params['token'] = token
+        self.headers = {'Authorization': token}
+
+        return self
+
+    def bearer_token(self, bearer_token):
+        """
+        Add token into authorization headers.
+
+        :param token: Token from EDL token.
+        :returns: Query instance
+        """
+
+        if not bearer_token:
+            return self
+
+        self.headers = {'Authorization': 'Bearer ' + bearer_token}
+
         return self
 
+
 class GranuleCollectionBaseQuery(Query):
     """
     Base class for Granule and Collection CMR queries.
     """
 
     def online_only(self, online_only=True):
         """
@@ -413,14 +431,26 @@
         lon = float(lon)
         lat = float(lat)
 
         self.params['point'] = "{},{}".format(lon, lat)
 
         return self
 
+    def circle(self, lon: float, lat: float, dist: int):
+        """Filter by granules within the circle around lat/lon
+
+        :param lon: longitude of geographic point
+        :param lat: latitude of geographic point
+        :param dist: distance in meters around waypoint (lat,lon)
+        :returns: Query instance
+        """
+        self.params['circle'] = f"{lon},{lat},{dist}"
+
+        return self
+
     def polygon(self, coordinates):
         """
         Filter by granules that overlap a polygonal area. Must be used in combination with a
         collection filtering parameter such as short_name or entry_title.
 
         :param coordinates: list of (lon, lat) tuples
         :returns: Query instance
```

### Comparing `python-cmr-0.7.0/pyproject.toml` & `python_cmr-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-cmr"
-version = "0.7.0"
+version = "0.8.0"
 description = "Python wrapper to the NASA Common Metadata Repository (CMR) API."
 authors = ["python_cmr <nasa/python_cmr@github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/nasa/python_cmr"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `python-cmr-0.7.0/setup.py` & `python_cmr-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,316 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-cmr
+Version: 0.8.0
+Summary: Python wrapper to the NASA Common Metadata Repository (CMR) API.
+Home-page: https://github.com/nasa/python_cmr
+License: MIT
+Author: python_cmr
+Author-email: nasa/python_cmr@github.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Project-URL: Repository, https://github.com/nasa/python_cmr
+Description-Content-Type: text/markdown
 
-packages = \
-['cmr']
+This repository is a copy
+of [jddeal/python_cmr](https://github.com/jddeal/python-cmr/tree/ef0f9e7d67ce99d342a568bd6a098c3462df16d2) which is no
+longer maintained. It has been copied here with the permission of the original author for the purpose of continuing to
+develop a python library that can be used for CMR access.
 
-package_data = \
-{'': ['*']}
+----
 
-install_requires = \
-['requests>=2.26.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'python-cmr',
-    'version': '0.7.0',
-    'description': 'Python wrapper to the NASA Common Metadata Repository (CMR) API.',
-    'long_description': 'This repository is a copy\nof [jddeal/python_cmr](https://github.com/jddeal/python-cmr/tree/ef0f9e7d67ce99d342a568bd6a098c3462df16d2) which is no\nlonger maintained. It has been copied here with the permission of the original author for the purpose of continuing to\ndevelop a python library that can be used for CMR access.\n\n----\n\nPython CMR\n==========\n\n[![CodeQL](https://github.com/nasa/python_cmr/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/nasa/python_cmr/actions/workflows/codeql-analysis.yml)\n\nPython CMR is an easy to use wrapper to the NASA\nEOSDIS [Common Metadata Repository API](https://cmr.earthdata.nasa.gov/search/). This package aims to make querying the\nAPI intuitive and less error-prone by providing methods that will preemptively check for invalid input and handle the\nURL encoding the CMR API expects.\n\nGetting access to NASA\'s earth science metadata is as simple as this:\n\n    >>> from cmr import CollectionQuery, GranuleQuery, ToolQuery, ServiceQuery, VariableQuery\n\n    >>> api = CollectionQuery()\n    >>> collections = api.archive_center("LP DAAC").keyword("AST_L1*").get(5)\n\n    >>> for collection in collections:\n    >>>   print(collection["short_name"])\n    AST_L1A\n    AST_L1AE\n    AST_L1T\n\n    >>> api = GranuleQuery()\n    >>> granules = api.short_name("AST_L1T").point(-112.73, 42.5).get(3)\n\n    >>> for granule in granules:\n    >>>   print(granule["title"])\n    SC:AST_L1T.003:2149105822\n    SC:AST_L1T.003:2149105820\n    SC:AST_L1T.003:2149155037\n\nInstallation\n============\n\nTo install from pypi:\n\n    $ pip install python-cmr\n\nTo install from github, perhaps to try out the dev branch:\n\n    $ git clone https://github.com/nasa/python_cmr\n    $ cd python-cmr\n    $ pip install .\n\nExamples\n========\n\nThis library is broken into two classes, CollectionQuery and GranuleQuery. Each of these classes provide a large set of\nmethods used to build a query for CMR. Not all parameters provided by the CMR API are covered by this version of\npython-cmr.\n\nThe following methods are available to both collecton and granule queries:\n\n    # search for granules matching a specific product/short_name\n    >>> api.short_name("AST_L1T")\n\n    # search for granules matching a specific version\n    >>> api.version("006")\n\n    # search for granules at a specific longitude and latitude\n    >>> api.point(-112.73, 42.5)\n\n    # search for granules in an area bound by a box (lower left lon/lat, upper right lon/lat)\n    >>> api.bounding_box(-112.70, 42.5, -110, 44.5)\n\n    # search for granules in a polygon (these need to be in counter clockwise order and the\n    # last coordinate must match the first in order to close the polygon)\n    >>> api.polygon([(-100, 40), (-110, 40), (-105, 38), (-100, 40)])\n\n    # search for granules in a line\n    >>> api.line([(-100, 40), (-90, 40), (-95, 38)])\n\n    # search for granules in an open or closed date range\n    >>> api.temporal("2016-10-10T01:02:00Z", "2016-10-12T00:00:30Z")\n    >>> api.temporal("2016-10-10T01:02:00Z", None)\n    >>> api.temporal(datetime(2016, 10, 10, 1, 2, 0), datetime.now())\n\n    # only include granules available for download\n    >>> api.downloadable()\n\n    # only include granules that are unavailable for download\n    >>> api.online_only()\n\n    # search for collections/granules associated with or identified by concept IDs\n    # note: often the ECHO collection ID can be used here as well\n    # note: when using CollectionQuery, only collection concept IDs can be passed\n    # note: when uses GranuleQuery, passing a collection\'s concept ID will filter by granules associated\n    #       with that particular collection.\n    >>> api.concept_id("C1299783579-LPDAAC_ECS")\n    >>> api.concept_id(["G1327299284-LPDAAC_ECS", "G1326330014-LPDAAC_ECS"])\n\n    # search by provider\n    >>> api.provider(\'POCLOUD\')\n\nGranule searches support these methods (in addition to the shared methods above):\n\n    # search for a granule by its unique ID\n    >>> api.granule_ur("SC:AST_L1T.003:2150315169")\n    # search for granules from a specific orbit\n    >>> api.orbit_number(5000)\n\n    # filter by the day/night flag\n    >>> api.day_night_flag("day")\n\n    # filter by cloud cover percentage range\n    >>> api.cloud_cover(25, 75)\n\n    # filter by specific instrument or platform\n    >>> api.instrument("MODIS")\n    >>> api.platform("Terra")\n\nCollection searches support these methods (in addition to the shared methods above):\n\n    # search for collections from a specific archive center\n    >>> api.archive_center("LP DAAC")\n\n    # case insensitive, wildcard enabled text search through most collection fields\n    >>> api.keyword("M*D09")\n\n    # search by native_id\n    >>> api.native_id(\'native_id\')\n\n    # filter by tool concept id\n    >>> api.tool_concept_id(\'TL2092786348-POCLOUD\')\n\n    # filter by service concept id\n    >>> api.service_concept_id(\'S1962070864-POCLOUD\')\n\nService searches support the following methods\n\n    # Search via provider\n    >>> api = ServiceQuery()\n    >>> api.provider(\'POCLOUD\')\n    \n    # Search via native_id\n    >>> api.native_id(\'POCLOUD_podaac_l2_cloud_subsetter\')\n\n    # Search via name\n    >>> api.name(\'PODAAC L2 Cloud Subsetter\')\n\n    # Search via concept_id\n    >>> api.concept_id(\'S1962070864-POCLOUD\')\n\nTool searches support the following methods\n\n    # Search via provider\n    >>> api = ToolQuery()\n    >>> api.provider(\'POCLOUD\')\n\n    # Search via native_id\n    >>> api.native_id(\'POCLOUD_hitide\')\n\n    # Search via name\n    >>> api.name(\'hitide\')\n\n    # Search via concept_id\n    >>> api.concept_id(\'TL2092786348-POCLOUD\')\n\nVariable searches support the following methods\n\n    # Search via provider\n    >>> api = VariableQuery()\n    >>> api.provider(\'POCLOUD\')\n\n    # Search via native_id\n    >>> api.native_id(\'JASON_CS_S6A_L2_AMR_RAD_STATIC_CALIBRATION-AMR_Side_1-acc_lat\')\n\n    # Search via name\n    >>> api.name(\'/AMR_Side_1/acc_lat\')\n\n    # Search via concept_id\n    >>> api.concept_id(\'V2112019824-POCLOUD\')\n\nAs an alternative to chaining methods together to set the parameters of your query, a method exists to allow you to pass\nyour parameters as keyword arguments:\n\n    # search for AST_L1T version 003 granules at latitude 42, longitude -100\n    >>> api.parameters(\n        short_name="AST_L1T",\n        version="003",\n        point=(-100, 42)\n    )\n\nNote: the kwarg key should match the name of a method from the above examples, and the value should be a tuple if it\'s a\nparameter that requires multiple values.\n\nTo inspect and retreive results from the API, the following methods are available:\n\n    # inspect the number of results the query will return without downloading the results\n    >>> print(api.hits())\n\n    # retrieve 100 granules\n    >>> granules = api.get(100)\n\n    # retrieve 25,000 granules\n    >>> granules = api.get(25000)\n\n    # retrieve all the granules possible for the query\n    >>> granules = api.get_all()  # this is a shortcut for api.get(api.hits())\n\nBy default the responses will return as json and be accessible as a list of python dictionaries. Other formats can be\nspecified before making the request:\n\n    >>> granules = api.format("echo10").get(100)\n\nThe following formats are supported for both granule and collection queries:\n\n- json (default)\n- xml\n- echo10\n- iso\n- iso19115\n- csv\n- atom\n- kml\n- native\n\nCollection queries also support the following formats:\n\n- dif\n- dif10\n- opendata\n- umm\\_json\n- umm\\_json\\_vX\\_Y (ex: umm\\_json\\_v1\\_9)\n\n# Developing\n\npython-cmr uses the [poetry](https://python-poetry.org/) build system. Download and install poetry before starting\ndevelopment\n\n## Install Dependencies\n\nWith dev dependencies:\n```shell\npoetry install\n```\n\nWithout dev dependencies:\n```shell\npoetry install --no-dev\n```\n\n## Update Dependencies\n\n```shell\npoetry update\n```\n\n## Add new Dependency\n\n```shell\npoetry add requests\n```\nDevelopment-only dependency:\n```shell\npoetry add --dev pytest\n```\n\n## Build project\n\n```shell\npoetry build\n```\n\n## Lint project\n\n```shell\npoetry run flake8\n```\n\n## Run Tests\n\n```shell\npoetry run pytest\n```',
-    'author': 'python_cmr',
-    'author_email': 'nasa/python_cmr@github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/nasa/python_cmr',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Python CMR
+==========
 
+[![CodeQL](https://github.com/nasa/python_cmr/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/nasa/python_cmr/actions/workflows/codeql-analysis.yml)
+
+Python CMR is an easy to use wrapper to the NASA
+EOSDIS [Common Metadata Repository API](https://cmr.earthdata.nasa.gov/search/). This package aims to make querying the
+API intuitive and less error-prone by providing methods that will preemptively check for invalid input and handle the
+URL encoding the CMR API expects.
+
+Getting access to NASA's earth science metadata is as simple as this:
+
+    >>> from cmr import CollectionQuery, GranuleQuery, ToolQuery, ServiceQuery, VariableQuery
+
+    >>> api = CollectionQuery()
+    >>> collections = api.archive_center("LP DAAC").keyword("AST_L1*").get(5)
+
+    >>> for collection in collections:
+    >>>   print(collection["short_name"])
+    AST_L1A
+    AST_L1AE
+    AST_L1T
+
+    >>> api = GranuleQuery()
+    >>> granules = api.short_name("AST_L1T").point(-112.73, 42.5).get(3)
+
+    >>> for granule in granules:
+    >>>   print(granule["title"])
+    SC:AST_L1T.003:2149105822
+    SC:AST_L1T.003:2149105820
+    SC:AST_L1T.003:2149155037
+
+Installation
+============
+
+To install from pypi:
+
+    $ pip install python-cmr
+
+To install from github, perhaps to try out the dev branch:
+
+    $ git clone https://github.com/nasa/python_cmr
+    $ cd python-cmr
+    $ pip install .
+
+Examples
+========
+
+This library is broken into two classes, CollectionQuery and GranuleQuery. Each of these classes provide a large set of
+methods used to build a query for CMR. Not all parameters provided by the CMR API are covered by this version of
+python-cmr.
+
+The following methods are available to both collecton and granule queries:
+
+    # search for granules matching a specific product/short_name
+    >>> api.short_name("AST_L1T")
+
+    # search for granules matching a specific version
+    >>> api.version("006")
+
+    # search for granules at a specific longitude and latitude
+    >>> api.point(-112.73, 42.5)
+
+    # search for granules in an area bound by a box (lower left lon/lat, upper right lon/lat)
+    >>> api.bounding_box(-112.70, 42.5, -110, 44.5)
+
+    # search for granules in a polygon (these need to be in counter clockwise order and the
+    # last coordinate must match the first in order to close the polygon)
+    >>> api.polygon([(-100, 40), (-110, 40), (-105, 38), (-100, 40)])
+
+    # search for granules in a line
+    >>> api.line([(-100, 40), (-90, 40), (-95, 38)])
+
+    # search for granules in an open or closed date range
+    >>> api.temporal("2016-10-10T01:02:00Z", "2016-10-12T00:00:30Z")
+    >>> api.temporal("2016-10-10T01:02:00Z", None)
+    >>> api.temporal(datetime(2016, 10, 10, 1, 2, 0), datetime.now())
+
+    # only include granules available for download
+    >>> api.downloadable()
+
+    # only include granules that are unavailable for download
+    >>> api.online_only()
+
+    # search for collections/granules associated with or identified by concept IDs
+    # note: often the ECHO collection ID can be used here as well
+    # note: when using CollectionQuery, only collection concept IDs can be passed
+    # note: when uses GranuleQuery, passing a collection's concept ID will filter by granules associated
+    #       with that particular collection.
+    >>> api.concept_id("C1299783579-LPDAAC_ECS")
+    >>> api.concept_id(["G1327299284-LPDAAC_ECS", "G1326330014-LPDAAC_ECS"])
+
+    # search by provider
+    >>> api.provider('POCLOUD')
+    
+    # search non-ops CMR environment
+    >>> from cmr import CMR_UAT
+    >>> api.mode(CMR_UAT)
+
+Granule searches support these methods (in addition to the shared methods above):
+
+    # search for a granule by its unique ID
+    >>> api.granule_ur("SC:AST_L1T.003:2150315169")
+    # search for granules from a specific orbit
+    >>> api.orbit_number(5000)
+
+    # filter by the day/night flag
+    >>> api.day_night_flag("day")
+
+    # filter by cloud cover percentage range
+    >>> api.cloud_cover(25, 75)
+
+    # filter by specific instrument or platform
+    >>> api.instrument("MODIS")
+    >>> api.platform("Terra")
+
+Collection searches support these methods (in addition to the shared methods above):
+
+    # search for collections from a specific archive center
+    >>> api.archive_center("LP DAAC")
+
+    # case insensitive, wildcard enabled text search through most collection fields
+    >>> api.keyword("M*D09")
+
+    # search by native_id
+    >>> api.native_id('native_id')
+
+    # filter by tool concept id
+    >>> api.tool_concept_id('TL2092786348-POCLOUD')
+
+    # filter by service concept id
+    >>> api.service_concept_id('S1962070864-POCLOUD')
+
+Service searches support the following methods
+
+    # Search via provider
+    >>> api = ServiceQuery()
+    >>> api.provider('POCLOUD')
+    
+    # Search via native_id
+    >>> api.native_id('POCLOUD_podaac_l2_cloud_subsetter')
+
+    # Search via name
+    >>> api.name('PODAAC L2 Cloud Subsetter')
+
+    # Search via concept_id
+    >>> api.concept_id('S1962070864-POCLOUD')
+
+Tool searches support the following methods
+
+    # Search via provider
+    >>> api = ToolQuery()
+    >>> api.provider('POCLOUD')
+
+    # Search via native_id
+    >>> api.native_id('POCLOUD_hitide')
+
+    # Search via name
+    >>> api.name('hitide')
+
+    # Search via concept_id
+    >>> api.concept_id('TL2092786348-POCLOUD')
+
+Variable searches support the following methods
+
+    # Search via provider
+    >>> api = VariableQuery()
+    >>> api.provider('POCLOUD')
+
+    # Search via native_id
+    >>> api.native_id('JASON_CS_S6A_L2_AMR_RAD_STATIC_CALIBRATION-AMR_Side_1-acc_lat')
+
+    # Search via name
+    >>> api.name('/AMR_Side_1/acc_lat')
+
+    # Search via concept_id
+    >>> api.concept_id('V2112019824-POCLOUD')
+
+As an alternative to chaining methods together to set the parameters of your query, a method exists to allow you to pass
+your parameters as keyword arguments:
+
+    # search for AST_L1T version 003 granules at latitude 42, longitude -100
+    >>> api.parameters(
+        short_name="AST_L1T",
+        version="003",
+        point=(-100, 42)
+    )
+
+Note: the kwarg key should match the name of a method from the above examples, and the value should be a tuple if it's a
+parameter that requires multiple values.
+
+To inspect and retreive results from the API, the following methods are available:
+
+    # inspect the number of results the query will return without downloading the results
+    >>> print(api.hits())
+
+    # retrieve 100 granules
+    >>> granules = api.get(100)
+
+    # retrieve 25,000 granules
+    >>> granules = api.get(25000)
+
+    # retrieve all the granules possible for the query
+    >>> granules = api.get_all()  # this is a shortcut for api.get(api.hits())
+
+By default the responses will return as json and be accessible as a list of python dictionaries. Other formats can be
+specified before making the request:
+
+    >>> granules = api.format("echo10").get(100)
+
+We can add token to the api calls by setting headers using the following functions:
+
+    # Use token function for EDL echo-token or launchpad token
+    >>> api.token(token)
+
+    # Use bearer token function for EDL bearer tokens
+    >>> api.bearer_token(token)
+
+The following formats are supported for both granule and collection queries:
+
+- json (default)
+- xml
+- echo10
+- iso
+- iso19115
+- csv
+- atom
+- kml
+- native
+
+Collection queries also support the following formats:
+
+- dif
+- dif10
+- opendata
+- umm\_json
+- umm\_json\_vX\_Y (ex: umm\_json\_v1\_9)
+
+# Developing
+
+python-cmr uses the [poetry](https://python-poetry.org/) build system. Download and install poetry before starting
+development
+
+## Install Dependencies
+
+With dev dependencies:
+```shell
+poetry install
+```
+
+Without dev dependencies:
+```shell
+poetry install --no-dev
+```
+
+## Update Dependencies
+
+```shell
+poetry update
+```
+
+## Add new Dependency
+
+```shell
+poetry add requests
+```
+Development-only dependency:
+```shell
+poetry add --dev pytest
+```
+
+## Build project
+
+```shell
+poetry build
+```
+
+## Lint project
+
+```shell
+poetry run flake8
+```
+
+## Run Tests
+
+```shell
+poetry run pytest
+```
 
-setup(**setup_kwargs)
```


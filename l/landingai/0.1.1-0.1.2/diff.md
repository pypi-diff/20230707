# Comparing `tmp/landingai-0.1.1.tar.gz` & `tmp/landingai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.1.1.tar", max compression
+gzip compressed data, was "landingai-0.1.2.tar", max compression
```

## Comparing `landingai-0.1.1.tar` & `landingai-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2023-07-06 21:38:20.297719 landingai-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     6741 2023-07-06 21:38:20.297719 landingai-0.1.1/README.md
--rw-r--r--   0        0        0      354 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/__init__.py
--rw-r--r--   0        0        0     6833 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8458 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/client.py
--rw-r--r--   0        0        0    19329 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/media.py
--rw-r--r--   0        0        0     4236 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9418 2023-07-06 21:38:20.329719 landingai-0.1.1/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     6843 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/io.py
--rw-r--r--   0        0        0      221 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0     5287 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     4841 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/postprocess.py
--rw-r--r--   0        0        0    25157 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/predict.py
--rw-r--r--   0        0        0     6068 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4374 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1685 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/utils.py
--rw-r--r--   0        0        0    23703 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/vision_pipeline.py
--rw-r--r--   0        0        0    13403 2023-07-06 21:38:20.341719 landingai-0.1.1/landingai/visualize.py
--rw-r--r--   0        0        0     2487 2023-07-06 21:38:21.005723 landingai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-07 02:46:40.278489 landingai-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     6741 2023-07-07 02:46:40.278489 landingai-0.1.2/README.md
+-rw-r--r--   0        0        0      354 2023-07-07 02:46:40.318490 landingai-0.1.2/landingai/__init__.py
+-rw-r--r--   0        0        0     6833 2023-07-07 02:46:40.318490 landingai-0.1.2/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/client.py
+-rw-r--r--   0        0        0    19807 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4720 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9418 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     6843 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/io.py
+-rw-r--r--   0        0        0      221 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5287 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     4841 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/postprocess.py
+-rw-r--r--   0        0        0    25157 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/predict.py
+-rw-r--r--   0        0        0     6068 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4374 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1685 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/utils.py
+-rw-r--r--   0        0        0    23703 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/vision_pipeline.py
+-rw-r--r--   0        0        0    13403 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/visualize.py
+-rw-r--r--   0        0        0     2487 2023-07-07 02:46:41.370501 landingai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.2/PKG-INFO
```

### Comparing `landingai-0.1.1/LICENSE.md` & `landingai-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/README.md` & `landingai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/common.py` & `landingai-0.1.2/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/data_management/client.py` & `landingai-0.1.2/landingai/data_management/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, Optional, Tuple, cast
 
 import aiohttp
 import requests
 
 from landingai.data_management.utils import to_camel_case
 from landingai.exceptions import HttpError
+from landingai.utils import load_api_credential
 
 METADATA_ITEMS = "metadata_items"
 METADATA_UPDATE = "metadata_update"
 MEDIA_LIST = "media_list"
 MEDIA_REGISTER = "media_register"
 MEDIA_SIGN = "media_sign"
 GET_PROJECT = "get_project"
@@ -68,30 +69,28 @@
 class LandingLens:
     """
     LandingLens client
 
     Example
     -------
     # Create a client by specifying API Key and project id
-    >>> client = LandingLens(api_key, project)
+    >>> client = LandingLens(project, api_key)
 
     Parameters
     ----------
-    api-key : str
-        LandingLens API Key.
-    project-id: str
+    project_id: int
         LandingLens project id.  Can override this default in individual commands.
+    api_key: Optional[str]
+        LandingLens API Key. If it's not provided, it will be read from the environment variable LANDINGAI_API_KEY, or from .env file on your project root directory.
     """
 
-    def __init__(
-        self,
-        api_key: str,
-        project_id: int,
-    ):
+    def __init__(self, project_id: int, api_key: Optional[str] = None):
         self.project_id = project_id
+        if not api_key:
+            api_key = load_api_credential().api_key
         self.api_key = api_key
 
     @property
     def _project_id(self) -> int:
         return self.project_id
 
     @property
```

### Comparing `landingai-0.1.1/landingai/data_management/media.py` & `landingai-0.1.2/landingai/data_management/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,30 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 class Media:
     """Media management API client.
     This class provides a set of APIs to manage the medias (images) uploaded to LandingLens.
     For example, you can use this class to upload medias (images) to LandingLens or list the medias are already uploaded to the LandingLens.
+
+    Example
+    -------
+    # Create a Media client by specifying API Key and project id
+    >>> client = Media(project_id, api_key)
+
+    Parameters
+    ----------
+    project_id: int
+        LandingLens project id.  Can override this default in individual commands.
+    api_key: Optional[str]
+        LandingLens API Key. If it's not provided, it will be read from the environment variable LANDINGAI_API_KEY, or from .env file on your project root directory.
     """
 
-    def __init__(self, api_key: str, project_id: int):
-        self._client = LandingLens(api_key=api_key, project_id=project_id)
+    def __init__(self, project_id: int, api_key: Optional[str] = None):
+        self._client = LandingLens(project_id=project_id, api_key=api_key)
         self._media_max_page_size = 1000
         self._metadata_max_page_size = 500
 
     def upload(
         self,
         source: Union[str, Path, Image],
         split: str = "",
```

### Comparing `landingai-0.1.1/landingai/data_management/metadata.py` & `landingai-0.1.2/landingai/data_management/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,30 @@
 )
 
 
 class Metadata:
     """Metadata management API client.
     This class provides a set of APIs to manage the metadata of the medias (images) uploaded to LandingLens.
     For example, you can use this class to update the metadata of the uploaded medias.
+
+    Example
+    -------
+    # Create a Metadata client by specifying API Key and project id
+    >>> client = Metadata(project_id, api_key)
+
+    Parameters
+    ----------
+    project_id: int
+        LandingLens project id.  Can override this default in individual commands.
+    api_key: Optional[str]
+        LandingLens API Key. If it's not provided, it will be read from the environment variable LANDINGAI_API_KEY, or from .env file on your project root directory.
     """
 
-    def __init__(self, api_key: str, project_id: int):
-        self._client = LandingLens(api_key=api_key, project_id=project_id)
+    def __init__(self, project_id: int, api_key: Optional[str] = None):
+        self._client = LandingLens(project_id=project_id, api_key=api_key)
 
     def update(
         self,
         media_ids: Union[int, List[int]],
         **input_metadata: Optional[Dict[str, Any]],
     ) -> Dict[str, Any]:
         """Update or insert a dictionary of metadata for a set of medias.
```

### Comparing `landingai-0.1.1/landingai/data_management/utils.py` & `landingai-0.1.2/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/exceptions.py` & `landingai-0.1.2/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.1.2/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/io.py` & `landingai-0.1.2/landingai/io.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/pipeline/image_source.py` & `landingai-0.1.2/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/postprocess.py` & `landingai-0.1.2/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/predict.py` & `landingai-0.1.2/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/st_utils.py` & `landingai-0.1.2/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/storage/snowflake.py` & `landingai-0.1.2/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/transform.py` & `landingai-0.1.2/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/utils.py` & `landingai-0.1.2/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/vision_pipeline.py` & `landingai-0.1.2/landingai/vision_pipeline.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/landingai/visualize.py` & `landingai-0.1.2/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.1/pyproject.toml` & `landingai-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.1.1"
+version = "0.1.2"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.1.1/PKG-INFO` & `landingai-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


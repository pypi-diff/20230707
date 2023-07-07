# Comparing `tmp/landingai-0.1.2.tar.gz` & `tmp/landingai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.1.2.tar", max compression
+gzip compressed data, was "landingai-0.1.3.tar", max compression
```

## Comparing `landingai-0.1.2.tar` & `landingai-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2023-07-07 02:46:40.278489 landingai-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     6741 2023-07-07 02:46:40.278489 landingai-0.1.2/README.md
--rw-r--r--   0        0        0      354 2023-07-07 02:46:40.318490 landingai-0.1.2/landingai/__init__.py
--rw-r--r--   0        0        0     6833 2023-07-07 02:46:40.318490 landingai-0.1.2/landingai/common.py
--rw-r--r--   0        0        0       72 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     8714 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/client.py
--rw-r--r--   0        0        0    19807 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/media.py
--rw-r--r--   0        0        0     4720 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2188 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9418 2023-07-07 02:46:40.322490 landingai-0.1.2/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     6843 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/io.py
--rw-r--r--   0        0        0      221 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0     5287 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     4841 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/postprocess.py
--rw-r--r--   0        0        0    25157 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/predict.py
--rw-r--r--   0        0        0     6068 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4374 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1685 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/transform.py
--rw-r--r--   0        0        0     1598 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/utils.py
--rw-r--r--   0        0        0    23703 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/vision_pipeline.py
--rw-r--r--   0        0        0    13403 2023-07-07 02:46:40.334490 landingai-0.1.2/landingai/visualize.py
--rw-r--r--   0        0        0     2487 2023-07-07 02:46:41.370501 landingai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-07 12:16:15.079378 landingai-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     6741 2023-07-07 12:16:15.079378 landingai-0.1.3/README.md
+-rw-r--r--   0        0        0      354 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/__init__.py
+-rw-r--r--   0        0        0     6833 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     8714 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/data_management/client.py
+-rw-r--r--   0        0        0    19873 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4722 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2188 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9418 2023-07-07 12:16:15.107379 landingai-0.1.3/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     6843 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/io.py
+-rw-r--r--   0        0        0      221 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0     5287 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     5771 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/postprocess.py
+-rw-r--r--   0        0        0    25157 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/predict.py
+-rw-r--r--   0        0        0     6068 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-07-07 12:16:15.115379 landingai-0.1.3/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4374 2023-07-07 12:16:15.119379 landingai-0.1.3/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1685 2023-07-07 12:16:15.119379 landingai-0.1.3/landingai/transform.py
+-rw-r--r--   0        0        0     1598 2023-07-07 12:16:15.119379 landingai-0.1.3/landingai/utils.py
+-rw-r--r--   0        0        0    23703 2023-07-07 12:16:15.119379 landingai-0.1.3/landingai/vision_pipeline.py
+-rw-r--r--   0        0        0    13403 2023-07-07 12:16:15.119379 landingai-0.1.3/landingai/visualize.py
+-rw-r--r--   0        0        0     2487 2023-07-07 12:16:15.791390 landingai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7986 1970-01-01 00:00:00.000000 landingai-0.1.3/PKG-INFO
```

### Comparing `landingai-0.1.2/LICENSE.md` & `landingai-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/README.md` & `landingai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/common.py` & `landingai-0.1.3/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/data_management/client.py` & `landingai-0.1.3/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/data_management/media.py` & `landingai-0.1.3/landingai/data_management/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,18 @@
 class Media:
     """Media management API client.
     This class provides a set of APIs to manage the medias (images) uploaded to LandingLens.
     For example, you can use this class to upload medias (images) to LandingLens or list the medias are already uploaded to the LandingLens.
 
     Example
     -------
-    # Create a Media client by specifying API Key and project id
     >>> client = Media(project_id, api_key)
+    >>> client.upload("path/to/image.jpg")
+    >>> client.upload("path/to/image_folder")
+    >>> print(client.ls())
 
     Parameters
     ----------
     project_id: int
         LandingLens project id.  Can override this default in individual commands.
     api_key: Optional[str]
         LandingLens API Key. If it's not provided, it will be read from the environment variable LANDINGAI_API_KEY, or from .env file on your project root directory.
@@ -98,15 +100,15 @@
             Path to the segmentation mask file for segmentation project
         seg_defect_map: str
             Path to the segmentation defect_map.json file for segmentation project
         nothing_to_label: bool
             Set the media's label as OK, valid for object detection and segmetation project
         metadata_dict: dict
             A dictionary of metadata to be updated or inserted.
-            The key of the metadata needs to be created/registered (for the first time) before media uploading.
+            The key of the metadata needs to be created/registered (for the first time) on LandingLens before media uploading.
         validate_extensions: bool
             Defaults to True. Files other than jpg/jpeg/png/bmp will be skipped.
             If set to False, will try to upload all files. Behavior of platform
              for unexpected extensions may not be correct - for example, most likely file
              will be uploaded to s3, but won't show in data browser.
 
         Returns
```

### Comparing `landingai-0.1.2/landingai/data_management/metadata.py` & `landingai-0.1.3/landingai/data_management/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 class Metadata:
     """Metadata management API client.
     This class provides a set of APIs to manage the metadata of the medias (images) uploaded to LandingLens.
     For example, you can use this class to update the metadata of the uploaded medias.
 
     Example
     -------
-    # Create a Metadata client by specifying API Key and project id
     >>> client = Metadata(project_id, api_key)
+    >>> client.update([101, 102, 103], creator="tom")
 
     Parameters
     ----------
     project_id: int
         LandingLens project id.  Can override this default in individual commands.
     api_key: Optional[str]
         LandingLens API Key. If it's not provided, it will be read from the environment variable LANDINGAI_API_KEY, or from .env file on your project root directory.
@@ -38,15 +38,15 @@
 
         Parameters
         ----------
         media_ids
             Media ids to update.
         input_metadata
             A dictionary of metadata to be updated or inserted.
-            The key of the metadata needs to be created/registered (for the first time) before media uploading.
+            The key of the metadata needs to be created/registered (for the first time) on LandingLens before calling update().
 
         Returns
         ----------
         Dict[str, Any]
             The result from the update().
             ```
             # Example output
```

### Comparing `landingai-0.1.2/landingai/data_management/utils.py` & `landingai-0.1.3/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/exceptions.py` & `landingai-0.1.3/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.1.3/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/io.py` & `landingai-0.1.3/landingai/io.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/pipeline/image_source.py` & `landingai-0.1.3/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/postprocess.py` & `landingai-0.1.3/landingai/postprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,52 @@
 import math
 from collections import defaultdict
 from itertools import groupby
 from typing import Dict, List, Sequence, Tuple, Union, cast
 
+import numpy as np
+import PIL.Image
+from PIL.Image import Image
+
 from landingai.common import (
     ClassificationPrediction,
     ObjectDetectionPrediction,
+    Prediction,
     SegmentationPrediction,
 )
 
 
+def crop(
+    predictions: Sequence[Prediction], image: Union[np.ndarray, Image]
+) -> Sequence[Image]:
+    """Crop the image based on the bounding boxes in the predictions.
+
+    Parameters
+    ----------
+    predictions: a list of ObjectDetectionPrediction, each of which will be used to crop the image.
+    image: the input image to be cropped from.
+
+    Returns
+    -------
+    A list of cropped images.
+    """
+    if len(predictions) == 0:
+        return []
+    if isinstance(image, np.ndarray):
+        image = PIL.Image.fromarray(image)
+    output = []
+    for pred in predictions:
+        if not isinstance(pred, ObjectDetectionPrediction):
+            raise ValueError(
+                f"Only ObjectDetectionPrediction is supported but {type(pred)} is found."
+            )
+        output.append(image.crop(pred.bboxes))
+    return output
+
+
 def class_map(predictions: Sequence[ClassificationPrediction]) -> Dict[int, str]:
     """Return a map from the predicted class/label index to the class/label name."""
     return {pred.label_index: pred.label_name for pred in predictions}
 
 
 def class_counts(
     predictions: Sequence[ClassificationPrediction],
```

### Comparing `landingai-0.1.2/landingai/predict.py` & `landingai-0.1.3/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/st_utils.py` & `landingai-0.1.3/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/storage/snowflake.py` & `landingai-0.1.3/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/transform.py` & `landingai-0.1.3/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/utils.py` & `landingai-0.1.3/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/vision_pipeline.py` & `landingai-0.1.3/landingai/vision_pipeline.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/landingai/visualize.py` & `landingai-0.1.3/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.1.2/pyproject.toml` & `landingai-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.1.2"
+version = "0.1.3"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.1.2/PKG-INFO` & `landingai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/unstructured_inference-0.5.4.tar.gz` & `tmp/unstructured_inference-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.4.tar", last modified: Thu Jun 29 22:24:50 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.5.tar", last modified: Fri Jul  7 13:44:51 2023, max compression
```

## Comparing `unstructured_inference-0.5.4.tar` & `unstructured_inference-0.5.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.589525 unstructured_inference-0.5.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.589525 unstructured_inference-0.5.4/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.593525 unstructured_inference-0.5.4/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/largemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.597525 unstructured_inference-0.5.4/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-29 22:22:38.000000 unstructured_inference-0.5.4/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 22:24:50.589525 unstructured_inference-0.5.4/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 22:24:50.000000 unstructured_inference-0.5.4/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.112177 unstructured_inference-0.5.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.116177 unstructured_inference-0.5.5/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.120177 unstructured_inference-0.5.5/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/chipper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24262 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.124177 unstructured_inference-0.5.5/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-07 13:42:49.000000 unstructured_inference-0.5.5/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:44:51.116177 unstructured_inference-0.5.5/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-07 13:44:51.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-07 13:44:50.000000 unstructured_inference-0.5.5/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.4/PKG-INFO` & `unstructured_inference-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.4/README.md` & `unstructured_inference-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/setup.py` & `unstructured_inference-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.5/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.5/unstructured_inference/inference/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,15 @@
     )
     return element
 
 
 def load_pdf(
     filename: str,
     dpi: int = 200,
+    chunk_size: int = 100,
 ) -> Tuple[List[List[TextRegion]], List[Image.Image]]:
     """Loads the image and word objects from a pdf using pdfplumber and the image renderings of the
     pdf pages using pdf2image"""
     layouts = []
     for page in extract_pages(filename):
         layout = []
         height = page.height
@@ -402,9 +403,24 @@
             )
             text_region = element_class(x1 * coef, y1 * coef, x2 * coef, y2 * coef, text=_text)
 
             if text_region.area() > 0:
                 layout.append(text_region)
         layouts.append(layout)
 
-    images = pdf2image.convert_from_path(filename, dpi=dpi)
+    # Convert a PDF in small chunks of pages at a time (e.g. 1-10, 11-20... and so on)
+    info = pdf2image.pdfinfo_from_path(filename)
+    total_pages = info["Pages"]
+    images = []
+
+    for start_page in range(1, total_pages + 1, chunk_size):
+        end_page = min(start_page + chunk_size - 1, total_pages)
+        with tempfile.TemporaryDirectory() as tmpdir:
+            chunk_images = pdf2image.convert_from_path(
+                filename,
+                dpi=dpi,
+                first_page=start_page,
+                last_page=end_page,
+                output_folder=tmpdir,
+            )
+            images += chunk_images
     return layouts, images
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.5/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.5.5/unstructured_inference/inference/ordering.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/base.py` & `unstructured_inference-0.5.5/unstructured_inference/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
+from unstructured_inference.models.chipper import MODEL_TYPES as CHIPPER_MODEL_TYPES
+from unstructured_inference.models.chipper import UnstructuredChipperModel
 from unstructured_inference.models.detectron2 import (
     MODEL_TYPES as DETECTRON2_MODEL_TYPES,
 )
 from unstructured_inference.models.detectron2 import (
     UnstructuredDetectronModel,
 )
 from unstructured_inference.models.detectron2onnx import (
     MODEL_TYPES as DETECTRON2_ONNX_MODEL_TYPES,
 )
 from unstructured_inference.models.detectron2onnx import (
     UnstructuredDetectronONNXModel,
 )
-from unstructured_inference.models.largemodel import MODEL_TYPES as LARGE_MODEL_TYPES
-from unstructured_inference.models.largemodel import UnstructuredLargeModel
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.models.yolox import (
     MODEL_TYPES as YOLOX_MODEL_TYPES,
 )
 from unstructured_inference.models.yolox import (
     UnstructuredYoloXModel,
 )
@@ -37,17 +37,17 @@
         model.initialize(**DETECTRON2_MODEL_TYPES[model_name])
     elif model_name in DETECTRON2_ONNX_MODEL_TYPES:
         model = UnstructuredDetectronONNXModel()
         model.initialize(**DETECTRON2_ONNX_MODEL_TYPES[model_name])
     elif model_name in YOLOX_MODEL_TYPES:
         model = UnstructuredYoloXModel()
         model.initialize(**YOLOX_MODEL_TYPES[model_name])
-    elif model_name in LARGE_MODEL_TYPES:
-        model = UnstructuredLargeModel()
-        model.initialize(**LARGE_MODEL_TYPES[model_name])
+    elif model_name in CHIPPER_MODEL_TYPES:
+        model = UnstructuredChipperModel()
+        model.initialize(**CHIPPER_MODEL_TYPES[model_name])
     else:
         raise UnknownModelException(f"Unknown model type: {model_name}")
     return model
 
 
 class UnknownModelException(Exception):
     """Exception for the case where a model is called for with an unrecognized identifier."""
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.5/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.5/unstructured_inference/models/detectron2onnx.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import cv2
 import numpy as np
 import onnxruntime
 from huggingface_hub import hf_hub_download
 from PIL import Image
 
 from unstructured_inference.inference.layoutelement import LayoutElement
-from unstructured_inference.logger import logger
+from unstructured_inference.logger import logger, logger_onnx
 from unstructured_inference.models.unstructuredmodel import (
     UnstructuredObjectDetectionModel,
 )
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 
+onnxruntime.set_default_logger_severity(logger_onnx.getEffectiveLevel())
+
 DEFAULT_LABEL_MAP: Final[Dict[int, str]] = {
     0: "Text",
     1: "Title",
     2: "List",
     3: "Table",
     4: "Figure",
 }
@@ -49,30 +51,39 @@
         """Makes a prediction using detectron2 model."""
         super().predict(image)
 
         prepared_input = self.preprocess(image)
         try:
             bboxes, labels, confidence_scores, _ = self.model.run(None, prepared_input)
         except onnxruntime.capi.onnxruntime_pybind11_state.RuntimeException:
-            logger.error("Something happened while inferencing page")
+            logger_onnx.debug(
+                "Ignoring runtime error from onnx (likely due to encountering blank page).",
+            )
             return []
         input_w, input_h = image.size
         regions = self.postprocess(bboxes, labels, confidence_scores, input_w, input_h)
 
         return regions
 
     def initialize(
         self,
         model_path: Union[str, Path],
         label_map: Dict[int, str],
         confidence_threshold: Optional[float] = None,
     ):
         """Loads the detectron2 model using the specified parameters"""
         logger.info("Loading the Detectron2 layout model ...")
-        self.model = onnxruntime.InferenceSession(model_path, providers=["CPUExecutionProvider"])
+        self.model = onnxruntime.InferenceSession(
+            model_path,
+            providers=[
+                "TensorrtExecutionProvider",
+                "CUDAExecutionProvider",
+                "CPUExecutionProvider",
+            ],
+        )
         self.label_map = label_map
         if confidence_threshold is None:
             confidence_threshold = 0.5
         self.confidence_threshold = confidence_threshold
 
     def preprocess(self, image: Image.Image) -> Dict[str, np.ndarray]:
         """Process input image into required format for ingestion into the Detectron2 ONNX binary.
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.5/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/largemodel.py` & `unstructured_inference-0.5.5/unstructured_inference/models/chipper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     VisionEncoderDecoderModel,
 )
 
 from unstructured_inference.inference.layoutelement import LocationlessLayoutElement
 from unstructured_inference.models.unstructuredmodel import UnstructuredElementExtractionModel
 
 MODEL_TYPES = {
-    "large_model": {
+    "chipper": {
         "tokenizer_name": "xlm-roberta-large",
         "pre_trained_model_name": "unstructuredio/ved-fine-tuning",
     },
 }
 
 LABEL_MAP = [
     "Title",
@@ -53,15 +53,15 @@
 # with element types. The order of this particular list matters as the tokenizer vocabulary must not
 # change. Otherwise we won't correctly decode the tokens generated by the model.
 SPECIAL_TAGS = ["<sep/>"] + [
     f"<{open_or_close}s_{label_type}>" for label_type in LABEL_MAP for open_or_close in ("", "/")
 ]
 
 
-class UnstructuredLargeModel(UnstructuredElementExtractionModel):
+class UnstructuredChipperModel(UnstructuredElementExtractionModel):
     required_w: int = 1248
     required_h: int = 1664
 
     def initialize(
         self,
         tokenizer_name: str,
         pre_trained_model_name: str,
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.5/unstructured_inference/models/table_postprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,27 +188,34 @@
     for package_num, package in enumerate(package_objects):
         match_scores = []
         package_rect = Rect(package["bbox"])
         package_area = package_rect.get_area()
         for container_num, container in enumerate(container_objects):
             container_rect = Rect(container["bbox"])
             intersect_area = container_rect.intersect(Rect(package["bbox"])).get_area()
-            overlap_fraction = intersect_area / package_area
 
-            match_scores.append(
-                {"container": container, "container_num": container_num, "score": overlap_fraction},
-            )
-
-        sorted_match_scores = sort_objects_by_score(match_scores)
-
-        best_match_score = sorted_match_scores[0]
-        best_match_scores.append(best_match_score["score"])
-        if forced_assignment or best_match_score["score"] >= overlap_threshold:
-            container_assignments[best_match_score["container_num"]].append(package_num)
-            package_assignments[package_num].append(best_match_score["container_num"])
+            if package_area > 0:
+                overlap_fraction = intersect_area / package_area
+
+                match_scores.append(
+                    {
+                        "container": container,
+                        "container_num": container_num,
+                        "score": overlap_fraction,
+                    },
+                )
+
+        if len(match_scores) > 0:
+            sorted_match_scores = sort_objects_by_score(match_scores)
+
+            best_match_score = sorted_match_scores[0]
+            best_match_scores.append(best_match_score["score"])
+            if forced_assignment or best_match_score["score"] >= overlap_threshold:
+                container_assignments[best_match_score["container_num"]].append(package_num)
+                package_assignments[package_num].append(best_match_score["container_num"])
 
     return container_assignments, package_assignments, best_match_scores
 
 
 def sort_objects_by_score(objects, reverse=True):
     """
     Put any set of objects in order from high score to low score.
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.5/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.5/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.5/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.5/unstructured_inference/models/yolox.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,22 @@
     def predict(self, x: Image):
         """Predict using YoloX model."""
         super().predict(x)
         return self.image_processing(x)
 
     def initialize(self, model_path: str, label_map: dict):
         """Start inference session for YoloX model."""
-        self.model = onnxruntime.InferenceSession(model_path, providers=["CPUExecutionProvider"])
+        self.model = onnxruntime.InferenceSession(
+            model_path,
+            providers=[
+                "TensorrtExecutionProvider",
+                "CUDAExecutionProvider",
+                "CPUExecutionProvider",
+            ],
+        )
         self.layout_classes = label_map
 
     def image_processing(
         self,
         image: Image = None,
     ) -> List[LayoutElement]:
         """Method runing YoloX for layout detection, returns a PageLayout
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.5/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/utils.py` & `unstructured_inference-0.5.5/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference/visualize.py` & `unstructured_inference-0.5.5/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.4/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.5/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.5.4
+Version: 0.5.5
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.4/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.5/unstructured_inference.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 unstructured_inference/inference/__init__.py
 unstructured_inference/inference/elements.py
 unstructured_inference/inference/layout.py
 unstructured_inference/inference/layoutelement.py
 unstructured_inference/inference/ordering.py
 unstructured_inference/models/__init__.py
 unstructured_inference/models/base.py
+unstructured_inference/models/chipper.py
 unstructured_inference/models/detectron2.py
 unstructured_inference/models/detectron2onnx.py
 unstructured_inference/models/donut.py
-unstructured_inference/models/largemodel.py
 unstructured_inference/models/paddle_ocr.py
 unstructured_inference/models/table_postprocess.py
 unstructured_inference/models/tables.py
 unstructured_inference/models/tesseract.py
 unstructured_inference/models/unstructuredmodel.py
 unstructured_inference/models/yolox.py
 unstructured_inference/patches/__init__.py
```


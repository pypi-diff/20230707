# Comparing `tmp/visionmetrics-0.0.2.tar.gz` & `tmp/visionmetrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionmetrics-0.0.2.tar", last modified: Sat Jul  1 08:56:49 2023, max compression
+gzip compressed data, was "visionmetrics-0.0.3.tar", last modified: Thu Jul  6 23:12:24 2023, max compression
```

## Comparing `visionmetrics-0.0.2.tar` & `visionmetrics-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.454531 visionmetrics-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/tests/test_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/tests/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/tests/test_matting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/tests/test_prediction_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/tests/test_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.454531 visionmetrics-0.0.2/visionmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/visionmetrics/caption/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/caption_eval_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/cider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/coco_evalcap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/meteor.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/caption/rougel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/visionmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/classification/precision_recall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/visionmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/detection/mean_ap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/visionmetrics/matting/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/boundary_foreground_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/boundary_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/foreground_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/l1_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/matting_eval_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/matting/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/prediction_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/visionmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.458531 visionmetrics-0.0.2/visionmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-01 08:53:43.000000 visionmetrics-0.0.2/visionmetrics/retrieval/precision_recall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:56:49.454531 visionmetrics-0.0.2/visionmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-01 08:56:49.000000 visionmetrics-0.0.2/visionmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-01 08:56:49.000000 visionmetrics-0.0.2/visionmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:56:49.000000 visionmetrics-0.0.2/visionmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-01 08:56:49.000000 visionmetrics-0.0.2/visionmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 08:56:49.000000 visionmetrics-0.0.2/visionmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_matting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_prediction_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/tests/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/caption/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/caption_eval_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/cider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/coco_evalcap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/caption/rougel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/classification/precision_recall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/detection/mean_ap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/visionmetrics/matting/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/boundary_foreground_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/boundary_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/foreground_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/l1_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/matting_eval_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/matting/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/prediction_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/visionmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.808267 visionmetrics-0.0.3/visionmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-06 23:09:18.000000 visionmetrics-0.0.3/visionmetrics/retrieval/precision_recall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:12:24.804268 visionmetrics-0.0.3/visionmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 23:12:24.000000 visionmetrics-0.0.3/visionmetrics.egg-info/top_level.txt
```

### Comparing `visionmetrics-0.0.2/LICENSE` & `visionmetrics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/PKG-INFO` & `visionmetrics-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionmetrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Evaluation metric codes for various vision tasks.
 Home-page: https://github.com/microsoft/visionmetrics
 Author: Microsoft
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: caption
```

### Comparing `visionmetrics-0.0.2/README.md` & `visionmetrics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/setup.cfg` & `visionmetrics-0.0.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = visionmetrics
-version = 0.0.2
+version = 0.0.3
 description = Evaluation metric codes for various vision tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Microsoft
 license = MIT
 url = https://github.com/microsoft/visionmetrics
 
 [options]
 packages = find_namespace:
 python_requires = >= 3.8
 install_requires = 
 	numpy
 	torch
-	torchmetrics[detection]
+	torchmetrics[detection]==0.11.4
 	opencv-python-headless
 	Pillow>=6.2.2
 
 [options.packages.find]
 exclude = 
 	test*
```

### Comparing `visionmetrics-0.0.2/tests/test_caption.py` & `visionmetrics-0.0.3/tests/test_caption.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/tests/test_classification.py` & `visionmetrics-0.0.3/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/tests/test_detection.py` & `visionmetrics-0.0.3/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/tests/test_matting.py` & `visionmetrics-0.0.3/tests/test_matting.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/tests/test_prediction_filters.py` & `visionmetrics-0.0.3/tests/test_prediction_filters.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/tests/test_retrieval.py` & `visionmetrics-0.0.3/tests/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/caption/caption_eval_base.py` & `visionmetrics-0.0.3/visionmetrics/caption/caption_eval_base.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/caption/coco_evalcap_utils.py` & `visionmetrics-0.0.3/visionmetrics/caption/coco_evalcap_utils.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/classification/__init__.py` & `visionmetrics-0.0.3/visionmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/classification/precision_recall.py` & `visionmetrics-0.0.3/visionmetrics/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/detection/mean_ap.py` & `visionmetrics-0.0.3/visionmetrics/detection/mean_ap.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/matting/boundary_foreground_iou.py` & `visionmetrics-0.0.3/visionmetrics/matting/boundary_foreground_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/matting/boundary_mean_iou.py` & `visionmetrics-0.0.3/visionmetrics/matting/boundary_mean_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/matting/foreground_iou.py` & `visionmetrics-0.0.3/visionmetrics/matting/foreground_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/matting/l1_error.py` & `visionmetrics-0.0.3/visionmetrics/matting/l1_error.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/matting/matting_eval_base.py` & `visionmetrics-0.0.3/visionmetrics/matting/matting_eval_base.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/matting/mean_iou.py` & `visionmetrics-0.0.3/visionmetrics/matting/mean_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/prediction_filters.py` & `visionmetrics-0.0.3/visionmetrics/prediction_filters.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics/retrieval/precision_recall.py` & `visionmetrics-0.0.3/visionmetrics/retrieval/precision_recall.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.2/visionmetrics.egg-info/PKG-INFO` & `visionmetrics-0.0.3/visionmetrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionmetrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Evaluation metric codes for various vision tasks.
 Home-page: https://github.com/microsoft/visionmetrics
 Author: Microsoft
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: caption
```

### Comparing `visionmetrics-0.0.2/visionmetrics.egg-info/SOURCES.txt` & `visionmetrics-0.0.3/visionmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


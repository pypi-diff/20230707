# Comparing `tmp/matroid-1.2.5.tar.gz` & `tmp/matroid-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matroid-1.2.5.tar", last modified: Thu Apr  6 23:56:30 2023, max compression
+gzip compressed data, was "matroid-1.2.6.tar", last modified: Fri Jul  7 00:38:57 2023, max compression
```

## Comparing `matroid-1.2.5.tar` & `matroid-1.2.6.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:30.693081 matroid-1.2.5/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-04-06 23:56:30.693081 matroid-1.2.5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8690 2023-04-06 23:56:08.000000 matroid-1.2.5/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:30.689081 matroid-1.2.5/matroid/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       83 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3925 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1217 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/error.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:30.689081 matroid-1.2.5/matroid/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2193 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/accounts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7816 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/collections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10796 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/detectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9121 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/helpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3980 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/images.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5243 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/labels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6724 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6980 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/video_summary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3355 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/src/videos.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       18 2023-04-06 23:56:08.000000 matroid-1.2.5/matroid/version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:30.689081 matroid-1.2.5/matroid.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-04-06 23:56:30.000000 matroid-1.2.5/matroid.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-04-06 23:56:30.000000 matroid-1.2.5/matroid.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-06 23:56:30.000000 matroid-1.2.5/matroid.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-06 23:56:30.000000 matroid-1.2.5/matroid.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2023-04-06 23:56:30.000000 matroid-1.2.5/matroid.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-06 23:56:30.693081 matroid-1.2.5/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2023-04-06 23:56:08.000000 matroid-1.2.5/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:30.693081 matroid-1.2.5/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-06 23:56:08.000000 matroid-1.2.5/test/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      969 2023-04-06 23:56:08.000000 matroid-1.2.5/test/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      803 2023-04-06 23:56:08.000000 matroid-1.2.5/test/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      119 2023-04-06 23:56:08.000000 matroid-1.2.5/test/helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1385 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_accounts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5714 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_collections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11943 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_detectors_labels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2328 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_images.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7385 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7580 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_video_summary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1385 2023-04-06 23:56:08.000000 matroid-1.2.5/test/test_videos.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:57.737475 matroid-1.2.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2023-07-07 00:38:35.000000 matroid-1.2.6/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2023-07-07 00:38:57.737475 matroid-1.2.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8690 2023-07-07 00:38:35.000000 matroid-1.2.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:57.733475 matroid-1.2.6/matroid/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3925 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1217 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/error.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:57.737475 matroid-1.2.6/matroid/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2193 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/accounts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7816 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/collections.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10796 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/detectors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9121 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3980 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/images.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5243 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/labels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6724 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/streams.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6964 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/video_summary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3355 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/src/videos.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-07-07 00:38:35.000000 matroid-1.2.6/matroid/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:57.733475 matroid-1.2.6/matroid.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2023-07-07 00:38:57.000000 matroid-1.2.6/matroid.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-07-07 00:38:57.000000 matroid-1.2.6/matroid.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-07 00:38:57.000000 matroid-1.2.6/matroid.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-07-07 00:38:57.000000 matroid-1.2.6/matroid.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-07 00:38:57.000000 matroid-1.2.6/matroid.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-07 00:38:57.737475 matroid-1.2.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-07 00:38:35.000000 matroid-1.2.6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:57.737475 matroid-1.2.6/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-07 00:38:35.000000 matroid-1.2.6/test/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2023-07-07 00:38:35.000000 matroid-1.2.6/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      803 2023-07-07 00:38:35.000000 matroid-1.2.6/test/data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      119 2023-07-07 00:38:35.000000 matroid-1.2.6/test/helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_accounts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5714 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_collections.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11943 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_detectors_labels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2328 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_images.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7385 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_streams.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9491 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_video_summary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-07 00:38:35.000000 matroid-1.2.6/test/test_videos.py
```

### Comparing `matroid-1.2.5/README.md` & `matroid-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/client.py` & `matroid-1.2.6/matroid/client.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/error.py` & `matroid-1.2.6/matroid/error.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/accounts.py` & `matroid-1.2.6/matroid/src/accounts.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/collections.py` & `matroid-1.2.6/matroid/src/collections.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/detectors.py` & `matroid-1.2.6/matroid/src/detectors.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/helpers.py` & `matroid-1.2.6/matroid/src/helpers.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/images.py` & `matroid-1.2.6/matroid/src/images.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/labels.py` & `matroid-1.2.6/matroid/src/labels.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/streams.py` & `matroid-1.2.6/matroid/src/streams.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid/src/video_summary.py` & `matroid-1.2.6/matroid/src/video_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,21 +39,21 @@
         file_to_upload = None
         headers = {"Authorization": self.token.authorization_header()}
         data = {
             "name": name,
             "detectorId": detectorId,
             "labels": labels,
             "fps": fps,
-            "mc_lambda": mc_lambda,
-            "matching_distance": matching_distance,
-            "n_init": n_init,
-            "nn_budget": nn_budget,
-            "max_iou_dist": max_iou_dist,
-            "max_age": max_age,
-            "detection_threshold": detection_threshold,
+            "mcLambda": mc_lambda,
+            "matchingDistance": matching_distance,
+            "nInit": n_init,
+            "nnBudget": nn_budget,
+            "maxIouDist": max_iou_dist,
+            "maxAge": max_age,
+            "detectionThreshold": detection_threshold,
         }
         if file:
             file_to_upload = self.filereader.get_file(file)
             files = {"file": file_to_upload}
 
             return requests.request(
                 method, endpoint, **{"headers": headers, "files": files, "data": data}
@@ -180,21 +180,21 @@
         data = {
             "name": name,
             "startTime": startTime,
             "endTime": endTime,
             "detectorId": detectorId,
             "labels": labels,
             "fps": fps,
-            "mc_lambda": mc_lambda,
-            "matching_distance": matching_distance,
-            "n_init": n_init,
-            "nn_budget": nn_budget,
-            "max_iou_dist": max_iou_dist,
-            "max_age": max_age,
-            "detection_threshold": detection_threshold,
+            "mcLambda": mc_lambda,
+            "matchingDistance": matching_distance,
+            "nInit": n_init,
+            "nnBudget": nn_budget,
+            "maxIouDist": max_iou_dist,
+            "maxAge": max_age,
+            "detectionThreshold": detection_threshold,
         }
 
         return requests.request(method, endpoint, **{"headers": headers, "data": data})
     except Exception as e:
         raise error.APIConnectionError(message=e)
```

### Comparing `matroid-1.2.5/matroid/src/videos.py` & `matroid-1.2.6/matroid/src/videos.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/matroid.egg-info/SOURCES.txt` & `matroid-1.2.6/matroid.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 matroid/__init__.py
 matroid/client.py
 matroid/error.py
 matroid/version.py
 matroid.egg-info/PKG-INFO
```

### Comparing `matroid-1.2.5/test/conftest.py` & `matroid-1.2.6/test/conftest.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/data.py` & `matroid-1.2.6/test/data.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/test_accounts.py` & `matroid-1.2.6/test/test_accounts.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/test_collections.py` & `matroid-1.2.6/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/test_detectors_labels.py` & `matroid-1.2.6/test/test_detectors_labels.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/test_images.py` & `matroid-1.2.6/test/test_images.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/test_streams.py` & `matroid-1.2.6/test/test_streams.py`

 * *Files identical despite different names*

### Comparing `matroid-1.2.5/test/test_videos.py` & `matroid-1.2.6/test/test_videos.py`

 * *Files identical despite different names*


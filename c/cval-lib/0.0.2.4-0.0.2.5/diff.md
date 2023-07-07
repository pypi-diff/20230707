# Comparing `tmp/cval-lib-0.0.2.4.tar.gz` & `tmp/cval-lib-0.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.4.tar", last modified: Thu Jul  6 15:54:11 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.5.tar", last modified: Fri Jul  7 05:09:55 2023, max compression
```

## Comparing `cval-lib-0.0.2.4.tar` & `cval-lib-0.0.2.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5622 2023-07-06 15:50:50.000000 cval-lib-0.0.2.4/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.390924 cval-lib-0.0.2.4/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.4/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.390924 cval-lib-0.0.2.4/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.4/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.394924 cval-lib-0.0.2.4/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1689 2023-07-06 06:27:41.000000 cval-lib-0.0.2.4/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.2.4/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.2.4/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2012 2023-07-02 18:34:57.000000 cval-lib-0.0.2.4/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1306 2023-07-02 18:45:46.000000 cval-lib-0.0.2.4/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.398924 cval-lib-0.0.2.4/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2521 2023-07-06 15:50:50.000000 cval-lib-0.0.2.4/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.4/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1884 2023-07-04 09:05:59.000000 cval-lib-0.0.2.4/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.4/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      946 2023-07-02 19:17:24.000000 cval-lib-0.0.2.4/cval_lib/handlers/frame.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2487 2023-07-04 09:05:59.000000 cval-lib-0.0.2.4/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.398924 cval-lib-0.0.2.4/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.4/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.4/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.4/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.4/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1022 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-06 15:54:11.000000 cval-lib-0.0.2.4/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-06 15:54:11.402924 cval-lib-0.0.2.4/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-06 15:53:54.000000 cval-lib-0.0.2.4/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5608 2023-07-07 04:38:24.000000 cval-lib-0.0.2.5/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.5/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.5/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1689 2023-07-06 06:27:41.000000 cval-lib-0.0.2.5/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.2.5/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.2.5/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-06 16:33:44.000000 cval-lib-0.0.2.5/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1388 2023-07-07 04:38:24.000000 cval-lib-0.0.2.5/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 05:06:34.000000 cval-lib-0.0.2.5/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.5/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1994 2023-07-07 04:49:52.000000 cval-lib-0.0.2.5/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.5/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 04:58:02.000000 cval-lib-0.0.2.5/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 05:09:20.000000 cval-lib-0.0.2.5/cval_lib/handlers/frames.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2454 2023-07-07 04:38:24.000000 cval-lib-0.0.2.5/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.5/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.5/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.5/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1052 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-07 05:09:53.000000 cval-lib-0.0.2.5/setup.py
```

### Comparing `cval-lib-0.0.2.4/LICENSE` & `cval-lib-0.0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/README.md` & `cval-lib-0.0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -181,17 +181,19 @@
 ```python3
 emb = cval.detection()
 print(emd.on_premise_sampling(response_model))
 ```
 > The following method is most relevant when we are dealing with long-term tasks and, accordingly, with asynchronous interaction.
 ##### Polling
 > refers to actively sampling the status of an external device by a client program as a synchronous activity.
+
 ```python3
 from time import sleep
+
 result = None
 sleep_sec = 1
 while result is None:
-    result = emb.result.get_result()
-    sleep(sleep_sec)
-    sleep_sec *= 2
+ result = emb.result.get()
+ sleep(sleep_sec)
+ sleep_sec *= 2
 print(result)
 ```
```

#### html2text {}

```diff
@@ -62,9 +62,9 @@
 bbox_selection_policy='min', selection_strategy='margin',
 sort_strategy='ascending', frames=frames_predictions, ) ``` ##### Run active
 learning ```python3 emb = cval.detection() print(emd.on_premise_sampling
 (response_model)) ``` > The following method is most relevant when we are
 dealing with long-term tasks and, accordingly, with asynchronous interaction.
 ##### Polling > refers to actively sampling the status of an external device by
 a client program as a synchronous activity. ```python3 from time import sleep
-result = None sleep_sec = 1 while result is None: result =
-emb.result.get_result() sleep(sleep_sec) sleep_sec *= 2 print(result) ```
+result = None sleep_sec = 1 while result is None: result = emb.result.get()
+sleep(sleep_sec) sleep_sec *= 2 print(result) ```
```

### Comparing `cval-lib-0.0.2.4/cval_lib/connection.py` & `cval-lib-0.0.2.5/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.5/cval_lib/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.5/cval_lib/examples/embeddings.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.5/cval_lib/examples/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.5/cval_lib/examples/on_pemise.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
 
 if __name__ == '__main__':
     import uuid
     from random import random
 
-    from connection import CVALConnection
+    from cval_lib.connection import CVALConnection
     from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
 
     frames_predictions = list(
         map(
             lambda x: FramePrediction(
                 frame_id=str(uuid.uuid4().hex),
                 predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
             ),
-            range(10)
+            range(100)
         )
     )
 
     print(frames_predictions)
 
     request = DetectionSamplingOnPremise(
         num_of_samples=200,
```

### Comparing `cval-lib-0.0.2.4/cval_lib/examples/result.py` & `cval-lib-0.0.2.5/cval_lib/examples/result.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
 
 
 if __name__ == '__main__':
     from cval_lib.connection import CVALConnection
-    user_api_key = 'user_api_key'
+    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
     cval = CVALConnection(user_api_key)
-    print(cval.result().get_results())
-    cval.result().get_result(cval.result().get_results()[0].result_id)
+    print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
+    print(cval.result().get(cval.result().get_results()[0].result_id))
```

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.5/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.5/cval_lib/handlers/_abstract_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Repeat this process until you achieve an acceptable quality of the model.
 
 Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
 Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
-
+from functools import wraps
 
 from requests import Request, Session, Response
 
 
 class AbstractHandler(Request):
     def __init__(self, session: Session, sub: str = '', url=''):
         self.session = session
@@ -32,14 +32,23 @@
             params=None,
             auth=None,
             cookies=None,
             hooks=None,
             json=None,
         )
 
+    @staticmethod
+    def pos_val(func):
+        @wraps(func)
+        def _(*args, **kwargs):
+            if args:
+                raise ValueError()
+            return func(**kwargs)
+        return _
+
     def _get(self, url: str, params=None, stream=False):
         self.url = url
         self.method = 'get'
         self.params = params
         self.stream = stream
 
     def _delete(self, url: str, params=None):
```

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.5/cval_lib/handlers/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/detection.py` & `cval-lib-0.0.2.5/cval_lib/handlers/detection.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,13 +31,19 @@
     ):
         self.route = f'{MainConfig().main_url}'
         self.result = Result(session)
         super().__init__(session)
 
     def on_premise_sampling(self, config: DetectionSamplingOnPremise):
         """
+        
         :param config: request model
-        :return: result_id
+        :return: ResultResponse
+
         """
-        self._post(self.route + '/on-premice/sampling/detection', json=config.dict())
-        return ResultResponse.parse_obj(self.send().json())
+        self._post(self.route + '/on-premise/sampling/detection', json=config.dict())
+        result = ResultResponse.parse_obj(
+            self.send().json()
+        )
+        self.result.result_id = result.result_id
+        return result
```

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.5/cval_lib/handlers/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/frame.py` & `cval-lib-0.0.2.5/cval_lib/handlers/frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         frame_id: str,
         dataset_id: str = None,
     ):
         self.route = f'{MainConfig.main_url}/dataset/{dataset_id}/{type_of_dataset}/frame/{frame_id}'
         super().__init__(session)
 
     def read(self):
-        self._get(self.url, stream=True)
+        self._get(self.route, stream=True)
         return self.send()
 
     def create(self, file):
         self._post(self.route, file=file)
         return self.send()
 
     def update(self, file):
@@ -30,9 +30,9 @@
         return self.send()
 
     def delete(self):
         self._delete(self.route)
         return self.send()
 
     def hash(self):
-        self._get(self.url+'/hash')
+        self._get(self.route+'/hash')
         return self.send().data
```

### Comparing `cval-lib-0.0.2.4/cval_lib/handlers/result.py` & `cval-lib-0.0.2.5/cval_lib/handlers/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,24 +37,24 @@
     def _set_result_id(self, result_id: str = None):
         if result_id is None:
             result_id = self.result_id
         if result_id is None:
             raise ValueError('result_id cannot be None')
         self.result_id = result_id
 
-    def get_result(self, result_id: str = None) -> ResultResponse:
+    def get(self, result_id: str = None) -> ResultResponse:
         """
         :param result_id: id of result
         :return: ResultResponse
         """
         self._set_result_id(result_id)
         self._get(self.route + f'/{self.result_id}')
         return ResultResponse.parse_obj(self.send().json())
 
     def get_results(self, dataset_id: str = None, limit=100, ):
         """
         :param dataset_id: id of dataset
         :param limit: limit of returned objects
         :return:
         """
-        self._get(self.route + 's', params={'limit': limit, 'dataset_id': dataset_id if dataset_id else 'null'})
+        self._get(self.route + 's', params={'limit': limit, 'dataset_id': dataset_id})
         return [ResultResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.4/cval_lib/models/dataset.py` & `cval-lib-0.0.2.5/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/models/detection.py` & `cval-lib-0.0.2.5/cval_lib/models/detection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/models/embedding.py` & `cval-lib-0.0.2.5/cval_lib/models/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib/models/result.py` & `cval-lib-0.0.2.5/cval_lib/models/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.4/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.5/cval_lib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ./cval_lib/handlers/__async.py
 ./cval_lib/handlers/__init__.py
 ./cval_lib/handlers/_abstract_handler.py
 ./cval_lib/handlers/dataset.py
 ./cval_lib/handlers/detection.py
 ./cval_lib/handlers/embedding.py
 ./cval_lib/handlers/frame.py
+./cval_lib/handlers/frames.py
 ./cval_lib/handlers/result.py
 ./cval_lib/models/__init__.py
 ./cval_lib/models/dataset.py
 ./cval_lib/models/detection.py
 ./cval_lib/models/embedding.py
 ./cval_lib/models/result.py
 ./cval_lib/patterns/__init__.py
```


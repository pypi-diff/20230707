# Comparing `tmp/cval-lib-0.0.2.5.tar.gz` & `tmp/cval-lib-0.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.5.tar", last modified: Fri Jul  7 05:09:55 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.6.tar", last modified: Fri Jul  7 08:12:13 2023, max compression
```

## Comparing `cval-lib-0.0.2.5.tar` & `cval-lib-0.0.2.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5608 2023-07-07 04:38:24.000000 cval-lib-0.0.2.5/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.5/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.5/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1689 2023-07-06 06:27:41.000000 cval-lib-0.0.2.5/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.2.5/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.2.5/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-06 16:33:44.000000 cval-lib-0.0.2.5/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1388 2023-07-07 04:38:24.000000 cval-lib-0.0.2.5/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 05:06:34.000000 cval-lib-0.0.2.5/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.5/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1994 2023-07-07 04:49:52.000000 cval-lib-0.0.2.5/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.5/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 04:58:02.000000 cval-lib-0.0.2.5/cval_lib/handlers/frame.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 05:09:20.000000 cval-lib-0.0.2.5/cval_lib/handlers/frames.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2454 2023-07-07 04:38:24.000000 cval-lib-0.0.2.5/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.5/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.5/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.5/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.5/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1052 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 05:09:55.000000 cval-lib-0.0.2.5/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 05:09:55.281920 cval-lib-0.0.2.5/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-07 05:09:53.000000 cval-lib-0.0.2.5/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5634 2023-07-07 07:57:29.000000 cval-lib-0.0.2.6/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.6/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.6/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 07:53:24.000000 cval-lib-0.0.2.6/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 08:11:49.000000 cval-lib-0.0.2.6/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 08:11:50.000000 cval-lib-0.0.2.6/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-06 16:33:44.000000 cval-lib-0.0.2.6/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 08:11:50.000000 cval-lib-0.0.2.6/cval_lib/examples/polling.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1385 2023-07-07 08:11:50.000000 cval-lib-0.0.2.6/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 05:06:34.000000 cval-lib-0.0.2.6/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.6/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1986 2023-07-07 05:37:42.000000 cval-lib-0.0.2.6/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.6/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 04:58:02.000000 cval-lib-0.0.2.6/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 05:09:20.000000 cval-lib-0.0.2.6/cval_lib/handlers/frames.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2451 2023-07-07 08:11:49.000000 cval-lib-0.0.2.6/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.6/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.6/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.6/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-07 08:11:49.000000 cval-lib-0.0.2.6/setup.py
```

### Comparing `cval-lib-0.0.2.5/LICENSE` & `cval-lib-0.0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/README.md` & `cval-lib-0.0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,16 @@
             frame_id=str(uuid.uuid4().hex),
             predictions=list(
                 map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), score=random.random()), range(100)))
         ),
         range(10)
     )
 )
-
 print(frames_predictions)
 
-
 ```
 
 ##### Construct config
 
 ```python3
 from cval_lib.models.detection import DetectionSamplingOnPremise
 request = DetectionSamplingOnPremise(
@@ -176,24 +174,25 @@
  frames=frames_predictions,
 )
 ```
 
 ##### Run active learning
 ```python3
 emb = cval.detection()
-print(emd.on_premise_sampling(response_model))
+print(emd.on_premise_sampling(request))
 ```
 > The following method is most relevant when we are dealing with long-term tasks and, accordingly, with asynchronous interaction.
 ##### Polling
 > refers to actively sampling the status of an external device by a client program as a synchronous activity.
 
 ```python3
 from time import sleep
 
 result = None
 sleep_sec = 1
 while result is None:
+ print(f'Pollint...\t{sleep_sec}')
  result = emb.result.get()
  sleep(sleep_sec)
  sleep_sec *= 2
 print(result)
 ```
```

#### html2text {}

```diff
@@ -58,13 +58,13 @@
 x: BBoxScores(category_id=str(uuid.uuid4()), score=random.random()), range
 (100))) ), range(10) ) ) print(frames_predictions) ``` ##### Construct config
 ```python3 from cval_lib.models.detection import DetectionSamplingOnPremise
 request = DetectionSamplingOnPremise( num_of_samples=200,
 bbox_selection_policy='min', selection_strategy='margin',
 sort_strategy='ascending', frames=frames_predictions, ) ``` ##### Run active
 learning ```python3 emb = cval.detection() print(emd.on_premise_sampling
-(response_model)) ``` > The following method is most relevant when we are
-dealing with long-term tasks and, accordingly, with asynchronous interaction.
-##### Polling > refers to actively sampling the status of an external device by
-a client program as a synchronous activity. ```python3 from time import sleep
-result = None sleep_sec = 1 while result is None: result = emb.result.get()
-sleep(sleep_sec) sleep_sec *= 2 print(result) ```
+(request)) ``` > The following method is most relevant when we are dealing with
+long-term tasks and, accordingly, with asynchronous interaction. ##### Polling
+> refers to actively sampling the status of an external device by a client
+program as a synchronous activity. ```python3 from time import sleep result =
+None sleep_sec = 1 while result is None: print(f'Pollint...\t{sleep_sec}')
+result = emb.result.get() sleep(sleep_sec) sleep_sec *= 2 print(result) ```
```

### Comparing `cval-lib-0.0.2.5/cval_lib/connection.py` & `cval-lib-0.0.2.6/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.6/cval_lib/examples/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 
 if __name__ == '__main__':
     from cval_lib.connection import CVALConnection
 
     # set up your user_api_key
-    user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
+    user_api_key = 'USER_API_KEY'
     # set up session
     cval = CVALConnection(user_api_key)
     # choose strategy
     ds = cval.dataset()
     # create your dataset
     ds_id = ds.create()
     print(ds_id)
```

### Comparing `cval-lib-0.0.2.5/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.6/cval_lib/examples/monkey_patch.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
 
 
 if __name__ == '__main__':
     from cval_lib.connection import CVALConnection
-    api_key = '1d770d0b3f5898ec9e24c5422480b2419b9363852fc14a2e8881de2c6e43b82a'
+    api_key = 'USER_API_KEY'
     cval = CVALConnection(api_key)
     ds = cval.dataset()
     ds.create()
-    print(ds.result.get_results())
+    print(ds.result.get_many())
```

### Comparing `cval-lib-0.0.2.5/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.6/cval_lib/examples/on_pemise.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/examples/result.py` & `cval-lib-0.0.2.6/cval_lib/examples/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 
 if __name__ == '__main__':
     from cval_lib.connection import CVALConnection
     user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
     cval = CVALConnection(user_api_key)
     print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
-    print(cval.result().get(cval.result().get_results()[0].result_id))
+    print(cval.result().get(cval.result().get_many()[0].result_id))
```

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.6/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.6/cval_lib/handlers/_abstract_handler.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.6/cval_lib/handlers/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/detection.py` & `cval-lib-0.0.2.6/cval_lib/handlers/detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
     ):
         self.route = f'{MainConfig().main_url}'
         self.result = Result(session)
         super().__init__(session)
 
     def on_premise_sampling(self, config: DetectionSamplingOnPremise):
         """
-        
+
         :param config: request model
         :return: ResultResponse
 
         """
-        self._post(self.route + '/on-premise/sampling/detection', json=config.dict())
+        self._post(self.route + '/on-premice/sampling/detection', json=config.dict())
         result = ResultResponse.parse_obj(
             self.send().json()
         )
         self.result.result_id = result.result_id
         return result
```

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.6/cval_lib/handlers/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/frame.py` & `cval-lib-0.0.2.6/cval_lib/handlers/frame.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/frames.py` & `cval-lib-0.0.2.6/cval_lib/handlers/frames.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/handlers/result.py` & `cval-lib-0.0.2.6/cval_lib/handlers/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         :param result_id: id of result
         :return: ResultResponse
         """
         self._set_result_id(result_id)
         self._get(self.route + f'/{self.result_id}')
         return ResultResponse.parse_obj(self.send().json())
 
-    def get_results(self, dataset_id: str = None, limit=100, ):
+    def get_many(self, dataset_id: str = None, limit=100, ):
         """
         :param dataset_id: id of dataset
         :param limit: limit of returned objects
         :return:
         """
         self._get(self.route + 's', params={'limit': limit, 'dataset_id': dataset_id})
         return [ResultResponse.parse_obj(i) for i in self.send().json()]
```

### Comparing `cval-lib-0.0.2.5/cval_lib/models/dataset.py` & `cval-lib-0.0.2.6/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/models/detection.py` & `cval-lib-0.0.2.6/cval_lib/models/detection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/models/embedding.py` & `cval-lib-0.0.2.6/cval_lib/models/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib/models/result.py` & `cval-lib-0.0.2.6/cval_lib/models/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.5/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.6/cval_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ./cval_lib/configs/__init__.py
 ./cval_lib/configs/main_config.py
 ./cval_lib/examples/__init__.py
 ./cval_lib/examples/dataset.py
 ./cval_lib/examples/embeddings.py
 ./cval_lib/examples/monkey_patch.py
 ./cval_lib/examples/on_pemise.py
+./cval_lib/examples/polling.py
 ./cval_lib/examples/result.py
 ./cval_lib/handlers/__async.py
 ./cval_lib/handlers/__init__.py
 ./cval_lib/handlers/_abstract_handler.py
 ./cval_lib/handlers/dataset.py
 ./cval_lib/handlers/detection.py
 ./cval_lib/handlers/embedding.py
```


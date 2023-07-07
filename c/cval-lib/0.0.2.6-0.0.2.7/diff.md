# Comparing `tmp/cval-lib-0.0.2.6.tar.gz` & `tmp/cval-lib-0.0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.6.tar", last modified: Fri Jul  7 08:12:13 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.7.tar", last modified: Fri Jul  7 10:19:41 2023, max compression
```

## Comparing `cval-lib-0.0.2.6.tar` & `cval-lib-0.0.2.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5634 2023-07-07 07:57:29.000000 cval-lib-0.0.2.6/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.6/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.6/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 07:53:24.000000 cval-lib-0.0.2.6/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 08:11:49.000000 cval-lib-0.0.2.6/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 08:11:50.000000 cval-lib-0.0.2.6/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-06 16:33:44.000000 cval-lib-0.0.2.6/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 08:11:50.000000 cval-lib-0.0.2.6/cval_lib/examples/polling.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1385 2023-07-07 08:11:50.000000 cval-lib-0.0.2.6/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 05:06:34.000000 cval-lib-0.0.2.6/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.6/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1986 2023-07-07 05:37:42.000000 cval-lib-0.0.2.6/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.6/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 04:58:02.000000 cval-lib-0.0.2.6/cval_lib/handlers/frame.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 05:09:20.000000 cval-lib-0.0.2.6/cval_lib/handlers/frames.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2451 2023-07-07 08:11:49.000000 cval-lib-0.0.2.6/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.6/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.6/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.6/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.6/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 08:12:13.000000 cval-lib-0.0.2.6/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 08:12:13.078703 cval-lib-0.0.2.6/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-07 08:11:49.000000 cval-lib-0.0.2.6/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     6568 2023-07-07 09:13:46.000000 cval-lib-0.0.2.7/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.7/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.7/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/polling.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1385 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.7/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1986 2023-07-07 10:18:22.000000 cval-lib-0.0.2.7/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.7/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/frames.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2451 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.7/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.7/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.7/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      448 2023-07-07 10:17:09.000000 cval-lib-0.0.2.7/setup.py
```

### Comparing `cval-lib-0.0.2.6/LICENSE` & `cval-lib-0.0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/README.md` & `cval-lib-0.0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
   <p align="center">
     A library designed to interact with the REST-API cval.ai
     <br/>
     <b>
       <a href="https://cval.ai">REST API docs</a>
       ·
       <a href="https://github.com/fangorntreabeard/cval-lib/issues">Report Bug</a>
+      ·
+      <a href="https://colab.research.google.com/drive/1f93b-aCv4MacngujLVUcQBJ9T1mJZBKH?usp=sharing"> Google Colaboratory Demo </a>
     </b>
   </p>
 </div>
 
 # About
 
 With CVAL, you can iteratively **improve your models** by following our active learning loop.
@@ -69,15 +71,15 @@
 
 ## Examples
 
 ##### Set your user_api_key
 
 ```python3
 from cval_lib.connection import CVALConnection
-USER_API_KEY='awesome_api_key'
+USER_API_KEY = 'awesome_api_key'
 cval = CVALConnection(USER_API_KEY)
 ```
 
 > The same actions are available with the rest of the entities, but there are some nuances, for example, somewhere there is the use of models, and somewhere only parameters. But anyway, these examples well reflect possible scenarios when working with cval. The most typical api scenario is a dataset, so let's start with it.
 
 ### Dataset
  > Within the framework of the created system, datasets are spaces in which data for machine learning is stored.
@@ -133,31 +135,31 @@
 ```python3
 emb = cval.embedding(ds_id, 'training')
 emb.upload_many(embeddings)
 print(emb.get_many())
 ```
 
 > The following example is used to invoke active learning
-
+ 
 ### Active learning
 
 ##### Get predictions data
 
 ```python3
-import random
+from random import random
 import uuid
 from cval_lib.models.detection import BBoxScores, FramePrediction
 
 # :NOTE: example only
 frames_predictions = list(
     map(
         lambda x: FramePrediction(
             frame_id=str(uuid.uuid4().hex),
             predictions=list(
-                map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), score=random.random()), range(100)))
+                map(lambda x: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
         ),
         range(10)
     )
 )
 print(frames_predictions)
 
 ```
@@ -174,25 +176,52 @@
  frames=frames_predictions,
 )
 ```
 
 ##### Run active learning
 ```python3
 emb = cval.detection()
-print(emd.on_premise_sampling(request))
+print(emb.on_premise_sampling(request))
 ```
 > The following method is most relevant when we are dealing with long-term tasks and, accordingly, with asynchronous interaction.
 ##### Polling
 > refers to actively sampling the status of an external device by a client program as a synchronous activity.
 
 ```python3
+import uuid
+from random import random
 from time import sleep
 
+from cval_lib.connection import CVALConnection
+from cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction, BBoxScores
+
+frames_predictions = list(
+        map(
+            lambda x: FramePrediction(
+                frame_id=str(uuid.uuid4().hex),
+                predictions=list(map(lambda _: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100)))
+            ),
+            range(1000)
+        )
+    )
+
+request = DetectionSamplingOnPremise(
+        num_of_samples=200,
+        bbox_selection_policy='min',
+        selection_strategy='margin',
+        sort_strategy='ascending',
+        frames=frames_predictions,
+    )
+emb = cval.detection()
+print(emb.on_premise_sampling(request))
+
 result = None
 sleep_sec = 1
 while result is None:
- print(f'Pollint...\t{sleep_sec}')
- result = emb.result.get()
- sleep(sleep_sec)
- sleep_sec *= 2
+    result = emb.result.get().result
+    print(f'Polling... {sleep_sec} s')
+    sleep(sleep_sec)
+    sleep_sec *= 2
+
 print(result)
+
 ```
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
                                   [Cval logo]
                         **** CVAL REST API LIBRARY ****
            A library designed to interact with the REST-API cval.ai
-                          REST_API_docs Â· Report_Bug
+            REST_API_docs Â· Report_Bug Â· Google_Colaboratory_Demo
 # About With CVAL, you can iteratively **improve your models** by following our
 active learning loop. * **First**, manually or semi-automatically annotate a
 random set of images. * **Next**, train your model and use uncertainty and
 diversity methods to score the remaining images for annotation. * **Then**,
 manually or semi-automatically annotate the images marked as more confident to
 increase the accuracy of the model. Repeat this process until you achieve an
 acceptable quality of the model. # Getting started To start using the CVAL Rest
@@ -21,18 +21,18 @@
 github.com/fangorntreabeard/cval-lib.git cval ``` ## Architecture The library
 architecture consists of **three layers**: 1. _A layer of protocols and
 abstract handlers_. Responsible for the use of a particular library. If an
 error is found, it is enough to simply change one method. 2. _A layer of
 handlers._ These are all the methods that are present in the API. Are based on
 abstract 3. _Model layer._ If the data structure changes, only this layer
 changes. ## Examples ##### Set your user_api_key ```python3 from
-cval_lib.connection import CVALConnection USER_API_KEY='awesome_api_key' cval =
-CVALConnection(USER_API_KEY) ``` > The same actions are available with the rest
-of the entities, but there are some nuances, for example, somewhere there is
-the use of models, and somewhere only parameters. But anyway, these examples
+cval_lib.connection import CVALConnection USER_API_KEY = 'awesome_api_key' cval
+= CVALConnection(USER_API_KEY) ``` > The same actions are available with the
+rest of the entities, but there are some nuances, for example, somewhere there
+is the use of models, and somewhere only parameters. But anyway, these examples
 well reflect possible scenarios when working with cval. The most typical api
 scenario is a dataset, so let's start with it. ### Dataset > Within the
 framework of the created system, datasets are spaces in which data for machine
 learning is stored. Creating a dataset is similar to creating a folder. #####
 Create dataset ```python3 # :NOTE: To avoid incomprehensibility of errors, it
 is recommended to use CVALConnection ds_id = cval.dataset().create(name='on-
 premise-scheme-ds', description='') print(ds_id) ``` ##### Update dataset
@@ -47,24 +47,33 @@
 cval_lib.models.embedding import ImageEmbeddingModel img_id_1 = str(uuid.uuid4
 ().hex) img_id_2 = str(uuid.uuid4().hex) embeddings = [ ImageEmbeddingModel
 (id=img_id_1, image_embedding=list(map(lambda x:random(), range(1000)))),
 ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(),
 range(1000)))), ] print(embeddings) ``` ##### Upload & check embeddings
 ```python3 emb = cval.embedding(ds_id, 'training') emb.upload_many(embeddings)
 print(emb.get_many()) ``` > The following example is used to invoke active
-learning ### Active learning ##### Get predictions data ```python3 import
-random import uuid from cval_lib.models.detection import BBoxScores,
+learning ### Active learning ##### Get predictions data ```python3 from random
+import random import uuid from cval_lib.models.detection import BBoxScores,
 FramePrediction # :NOTE: example only frames_predictions = list( map( lambda x:
 FramePrediction( frame_id=str(uuid.uuid4().hex), predictions=list( map(lambda
-x: BBoxScores(category_id=str(uuid.uuid4()), score=random.random()), range
-(100))) ), range(10) ) ) print(frames_predictions) ``` ##### Construct config
-```python3 from cval_lib.models.detection import DetectionSamplingOnPremise
-request = DetectionSamplingOnPremise( num_of_samples=200,
+x: BBoxScores(category_id=str(uuid.uuid4()), score=random()), range(100))) ),
+range(10) ) ) print(frames_predictions) ``` ##### Construct config ```python3
+from cval_lib.models.detection import DetectionSamplingOnPremise request =
+DetectionSamplingOnPremise( num_of_samples=200, bbox_selection_policy='min',
+selection_strategy='margin', sort_strategy='ascending',
+frames=frames_predictions, ) ``` ##### Run active learning ```python3 emb =
+cval.detection() print(emb.on_premise_sampling(request)) ``` > The following
+method is most relevant when we are dealing with long-term tasks and,
+accordingly, with asynchronous interaction. ##### Polling > refers to actively
+sampling the status of an external device by a client program as a synchronous
+activity. ```python3 import uuid from random import random from time import
+sleep from cval_lib.connection import CVALConnection from
+cval_lib.models.detection import DetectionSamplingOnPremise, FramePrediction,
+BBoxScores frames_predictions = list( map( lambda x: FramePrediction
+( frame_id=str(uuid.uuid4().hex), predictions=list(map(lambda _: BBoxScores
+(category_id=str(uuid.uuid4()), score=random()), range(100))) ), range(1000) )
+) request = DetectionSamplingOnPremise( num_of_samples=200,
 bbox_selection_policy='min', selection_strategy='margin',
-sort_strategy='ascending', frames=frames_predictions, ) ``` ##### Run active
-learning ```python3 emb = cval.detection() print(emd.on_premise_sampling
-(request)) ``` > The following method is most relevant when we are dealing with
-long-term tasks and, accordingly, with asynchronous interaction. ##### Polling
-> refers to actively sampling the status of an external device by a client
-program as a synchronous activity. ```python3 from time import sleep result =
-None sleep_sec = 1 while result is None: print(f'Pollint...\t{sleep_sec}')
-result = emb.result.get() sleep(sleep_sec) sleep_sec *= 2 print(result) ```
+sort_strategy='ascending', frames=frames_predictions, ) emb = cval.detection()
+print(emb.on_premise_sampling(request)) result = None sleep_sec = 1 while
+result is None: result = emb.result.get().result print(f'Polling... {sleep_sec}
+s') sleep(sleep_sec) sleep_sec *= 2 print(result) ```
```

### Comparing `cval-lib-0.0.2.6/cval_lib/connection.py` & `cval-lib-0.0.2.7/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.7/cval_lib/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.7/cval_lib/examples/embeddings.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.7/cval_lib/examples/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.7/cval_lib/examples/on_pemise.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/examples/polling.py` & `cval-lib-0.0.2.7/cval_lib/examples/polling.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/examples/result.py` & `cval-lib-0.0.2.7/cval_lib/examples/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.7/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.7/cval_lib/handlers/_abstract_handler.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.7/cval_lib/handlers/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/detection.py` & `cval-lib-0.0.2.7/cval_lib/handlers/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,14 @@
     def on_premise_sampling(self, config: DetectionSamplingOnPremise):
         """
 
         :param config: request model
         :return: ResultResponse
 
         """
-        self._post(self.route + '/on-premice/sampling/detection', json=config.dict())
+        self._post(self.route + '/on-premise/sampling/detection', json=config.dict())
         result = ResultResponse.parse_obj(
             self.send().json()
         )
         self.result.result_id = result.result_id
         return result
```

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.7/cval_lib/handlers/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/frame.py` & `cval-lib-0.0.2.7/cval_lib/handlers/frame.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/frames.py` & `cval-lib-0.0.2.7/cval_lib/handlers/frames.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/handlers/result.py` & `cval-lib-0.0.2.7/cval_lib/handlers/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/models/dataset.py` & `cval-lib-0.0.2.7/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/models/detection.py` & `cval-lib-0.0.2.7/cval_lib/models/detection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/models/embedding.py` & `cval-lib-0.0.2.7/cval_lib/models/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib/models/result.py` & `cval-lib-0.0.2.7/cval_lib/models/result.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.6/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.7/cval_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


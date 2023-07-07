# Comparing `tmp/cval-lib-0.0.2.7.tar.gz` & `tmp/cval-lib-0.0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.2.7.tar", last modified: Fri Jul  7 10:19:41 2023, max compression
+gzip compressed data, was "cval-lib-0.0.2.8.tar", last modified: Fri Jul  7 10:26:12 2023, max compression
```

## Comparing `cval-lib-0.0.2.7.tar` & `cval-lib-0.0.2.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     6568 2023-07-07 09:13:46.000000 cval-lib-0.0.2.7/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.7/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.7/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/embeddings.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/on_pemise.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/polling.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1385 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.536864 cval-lib-0.0.2.7/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.7/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1986 2023-07-07 10:18:22.000000 cval-lib-0.0.2.7/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.7/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/frame.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/frames.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2451 2023-07-07 09:09:28.000000 cval-lib-0.0.2.7/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.7/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.7/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.2.7/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.7/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 10:19:41.000000 cval-lib-0.0.2.7/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 10:19:41.540864 cval-lib-0.0.2.7/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      448 2023-07-07 10:17:09.000000 cval-lib-0.0.2.7/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     6568 2023-07-07 09:13:46.000000 cval-lib-0.0.2.8/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.2.8/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.2.8/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1637 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1829 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1258 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2022 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2367 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/examples/polling.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1383 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2750 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5076 2023-07-06 06:28:17.000000 cval-lib-0.0.2.8/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1984 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.2.8/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      950 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/frame.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      710 2023-07-07 09:09:28.000000 cval-lib-0.0.2.8/cval_lib/handlers/frames.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2449 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3014 2023-07-06 15:53:23.000000 cval-lib-0.0.2.8/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.2.8/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2210 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.2.8/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      204 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1083 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-07 10:26:12.000000 cval-lib-0.0.2.8/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-07 10:26:12.927762 cval-lib-0.0.2.8/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      448 2023-07-07 10:26:10.000000 cval-lib-0.0.2.8/setup.py
```

### Comparing `cval-lib-0.0.2.7/LICENSE` & `cval-lib-0.0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/README.md` & `cval-lib-0.0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/connection.py` & `cval-lib-0.0.2.8/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/examples/dataset.py` & `cval-lib-0.0.2.8/cval_lib/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/examples/embeddings.py` & `cval-lib-0.0.2.8/cval_lib/examples/embeddings.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/examples/monkey_patch.py` & `cval-lib-0.0.2.8/cval_lib/examples/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/examples/on_pemise.py` & `cval-lib-0.0.2.8/cval_lib/examples/on_pemise.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/examples/polling.py` & `cval-lib-0.0.2.8/cval_lib/examples/polling.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/examples/result.py` & `cval-lib-0.0.2.8/cval_lib/examples/result.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 
 if __name__ == '__main__':
     from cval_lib.connection import CVALConnection
     user_api_key = '11a6006a98793bb5086bbf6f6808dd6bd9a706a38ddb36c58a484991263e8535'
     cval = CVALConnection(user_api_key)
     print(cval.result().get('ecb8a52b-9bc0-4e56-a496-e69ce74cc0ec'))
-    print(cval.result().get(cval.result().get_many()[0].result_id))
+    print(cval.result().get(cval.result().get_many()[0].task_id))
```

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/__async.py` & `cval-lib-0.0.2.8/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.2.8/cval_lib/handlers/_abstract_handler.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/dataset.py` & `cval-lib-0.0.2.8/cval_lib/handlers/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/detection.py` & `cval-lib-0.0.2.8/cval_lib/handlers/detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
         :return: ResultResponse
 
         """
         self._post(self.route + '/on-premise/sampling/detection', json=config.dict())
         result = ResultResponse.parse_obj(
             self.send().json()
         )
-        self.result.result_id = result.result_id
+        self.result.result_id = result.task_id
         return result
```

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/embedding.py` & `cval-lib-0.0.2.8/cval_lib/handlers/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/frame.py` & `cval-lib-0.0.2.8/cval_lib/handlers/frame.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/frames.py` & `cval-lib-0.0.2.8/cval_lib/handlers/frames.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/handlers/result.py` & `cval-lib-0.0.2.8/cval_lib/handlers/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.result_id = None
         super().__init__(session)
 
     def _set_result_id(self, result_id: str = None):
         if result_id is None:
             result_id = self.result_id
         if result_id is None:
-            raise ValueError('result_id cannot be None')
+            raise ValueError('task_id cannot be None')
         self.result_id = result_id
 
     def get(self, result_id: str = None) -> ResultResponse:
         """
         :param result_id: id of result
         :return: ResultResponse
         """
```

### Comparing `cval-lib-0.0.2.7/cval_lib/models/dataset.py` & `cval-lib-0.0.2.8/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/models/detection.py` & `cval-lib-0.0.2.8/cval_lib/models/detection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/models/embedding.py` & `cval-lib-0.0.2.8/cval_lib/models/embedding.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.2.7/cval_lib/models/result.py` & `cval-lib-0.0.2.8/cval_lib/models/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,23 @@
     """
     weights_id: str | None
     version: str | None
 
 
 class ResultResponse(BaseModel):
     """
-    :param result_id: id of result for polling
+    :param task_id: id of result for polling
     :param dataset_id: id of dataset
     :param time_start: starting unix timestamp
     :param time_end: ending unix timestamp
     :param type_of_task: type of task: detection, classification
     :param action: action of result: sampling or test
     :param weights: weights of result
     """
-    result_id: str
+    task_id: str
     dataset_id: str | None
     time_start: float
     time_end: float | None
     type_of_task: str
     action: str
     weights: WeightsConfigResponse | None
     result: Any
```

### Comparing `cval-lib-0.0.2.7/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.2.8/cval_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


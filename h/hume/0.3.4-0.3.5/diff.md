# Comparing `tmp/hume-0.3.4.tar.gz` & `tmp/hume-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.3.4.tar", max compression
+gzip compressed data, was "hume-0.3.5.tar", max compression
```

## Comparing `hume-0.3.4.tar` & `hume-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2023-04-24 18:35:19.356412 hume-0.3.4/LICENSE
--rw-r--r--   0        0        0     2303 2023-05-05 00:20:11.927638 hume-0.3.4/README.md
--rw-r--r--   0        0        0      567 2023-05-03 18:27:10.048390 hume-0.3.4/hume/__init__.py
--rw-r--r--   0        0        0      500 2023-05-03 18:27:10.048676 hume-0.3.4/hume/_batch/__init__.py
--rw-r--r--   0        0        0     3464 2023-05-03 20:14:45.408723 hume-0.3.4/hume/_batch/batch_job.py
--rw-r--r--   0        0        0     5800 2023-05-03 20:20:07.806749 hume-0.3.4/hume/_batch/batch_job_details.py
--rw-r--r--   0        0        0      630 2023-05-03 20:19:40.816995 hume-0.3.4/hume/_batch/batch_job_state.py
--rw-r--r--   0        0        0      993 2023-05-01 17:29:24.001284 hume-0.3.4/hume/_batch/batch_job_status.py
--rw-r--r--   0        0        0     9493 2023-06-28 23:54:21.075584 hume-0.3.4/hume/_batch/hume_batch_client.py
--rw-r--r--   0        0        0      939 2023-05-03 21:06:47.512368 hume-0.3.4/hume/_batch/transcription_config.py
--rw-r--r--   0        0        0       19 2022-10-05 20:58:45.000000 hume-0.3.4/hume/_common/__init__.py
--rw-r--r--   0        0        0      124 2023-04-24 18:35:19.357658 hume-0.3.4/hume/_common/api_type.py
--rw-r--r--   0        0        0     1459 2023-06-18 17:06:20.480372 hume-0.3.4/hume/_common/client_base.py
--rw-r--r--   0        0        0     1795 2023-05-02 20:54:26.057667 hume-0.3.4/hume/_common/config_base.py
--rw-r--r--   0        0        0     2320 2023-05-02 00:14:43.888549 hume-0.3.4/hume/_common/config_utils.py
--rw-r--r--   0        0        0     3227 2023-06-11 17:16:41.157744 hume-0.3.4/hume/_common/retry_utils.py
--rw-r--r--   0        0        0      191 2023-04-24 18:35:19.358014 hume-0.3.4/hume/_stream/__init__.py
--rw-r--r--   0        0        0     4454 2023-06-28 23:54:21.075756 hume-0.3.4/hume/_stream/hume_stream_client.py
--rw-r--r--   0        0        0     8146 2023-06-28 23:54:21.075919 hume-0.3.4/hume/_stream/stream_socket.py
--rw-r--r--   0        0        0       19 2023-04-24 18:35:19.358285 hume-0.3.4/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2023-04-24 18:35:19.358345 hume-0.3.4/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       96 2023-04-24 18:35:19.358433 hume-0.3.4/hume/models/__init__.py
--rw-r--r--   0        0        0      587 2023-04-24 18:35:19.358535 hume-0.3.4/hume/models/config/__init__.py
--rw-r--r--   0        0        0      497 2023-04-24 18:35:19.358607 hume-0.3.4/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2777 2023-05-03 20:19:40.817539 hume-0.3.4/hume/models/config/face_config.py
--rw-r--r--   0        0        0      509 2023-05-05 00:20:11.928431 hume-0.3.4/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2235 2023-05-04 23:18:49.287324 hume-0.3.4/hume/models/config/language_config.py
--rw-r--r--   0        0        0      631 2023-05-02 20:54:26.059076 hume-0.3.4/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1000 2023-05-03 20:19:40.817946 hume-0.3.4/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1785 2023-06-09 21:21:24.616184 hume-0.3.4/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      804 2023-04-24 18:35:19.359005 hume-0.3.4/hume/models/model_type.py
--rw-r--r--   0        0        0     2527 2023-06-28 17:19:22.793676 hume-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 hume-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2303 2023-06-29 18:23:24.716744 hume-0.3.5/README.md
+-rw-r--r--   0        0        0      567 2023-06-29 18:23:24.723354 hume-0.3.5/hume/__init__.py
+-rw-r--r--   0        0        0      500 2023-06-29 18:23:24.723574 hume-0.3.5/hume/_batch/__init__.py
+-rw-r--r--   0        0        0     3464 2023-06-29 18:23:24.723718 hume-0.3.5/hume/_batch/batch_job.py
+-rw-r--r--   0        0        0     5800 2023-06-29 18:23:24.723952 hume-0.3.5/hume/_batch/batch_job_details.py
+-rw-r--r--   0        0        0      630 2023-06-29 18:23:24.724125 hume-0.3.5/hume/_batch/batch_job_state.py
+-rw-r--r--   0        0        0      993 2023-06-29 18:23:24.724185 hume-0.3.5/hume/_batch/batch_job_status.py
+-rw-r--r--   0        0        0    10637 2023-07-07 21:46:58.618551 hume-0.3.5/hume/_batch/hume_batch_client.py
+-rw-r--r--   0        0        0      939 2023-06-29 18:23:24.724610 hume-0.3.5/hume/_batch/transcription_config.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.3.5/hume/_common/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-29 18:23:24.724824 hume-0.3.5/hume/_common/api_type.py
+-rw-r--r--   0        0        0     1459 2023-06-29 18:23:24.725035 hume-0.3.5/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1795 2023-06-29 18:23:24.725216 hume-0.3.5/hume/_common/config_base.py
+-rw-r--r--   0        0        0     2320 2023-06-29 18:23:24.725275 hume-0.3.5/hume/_common/config_utils.py
+-rw-r--r--   0        0        0     3227 2023-06-29 18:23:24.725338 hume-0.3.5/hume/_common/retry_utils.py
+-rw-r--r--   0        0        0      191 2023-06-29 18:23:24.725504 hume-0.3.5/hume/_stream/__init__.py
+-rw-r--r--   0        0        0     4454 2023-06-29 18:23:24.725875 hume-0.3.5/hume/_stream/hume_stream_client.py
+-rw-r--r--   0        0        0     8146 2023-06-29 18:23:24.726112 hume-0.3.5/hume/_stream/stream_socket.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.3.5/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2023-06-29 18:23:24.726231 hume-0.3.5/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       96 2023-06-29 18:23:24.726302 hume-0.3.5/hume/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-06-29 18:23:24.726358 hume-0.3.5/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      497 2023-06-29 18:23:24.726421 hume-0.3.5/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2777 2023-06-29 18:23:24.726599 hume-0.3.5/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      509 2023-06-29 18:23:24.726675 hume-0.3.5/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2235 2023-06-29 18:23:24.726847 hume-0.3.5/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      631 2023-06-29 18:23:24.727027 hume-0.3.5/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1000 2023-06-29 18:23:24.727151 hume-0.3.5/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1785 2023-06-29 18:23:24.727409 hume-0.3.5/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      804 2023-06-29 18:23:24.727570 hume-0.3.5/hume/models/model_type.py
+-rw-r--r--   0        0        0     2527 2023-07-07 21:46:58.618696 hume-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 hume-0.3.5/PKG-INFO
```

### Comparing `hume-0.3.4/LICENSE` & `hume-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/README.md` & `hume-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/__init__.py` & `hume-0.3.5/hume/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_batch/batch_job.py` & `hume-0.3.5/hume/_batch/batch_job.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_batch/batch_job_details.py` & `hume-0.3.5/hume/_batch/batch_job_details.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_batch/batch_job_state.py` & `hume-0.3.5/hume/_batch/batch_job_state.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_batch/batch_job_status.py` & `hume-0.3.5/hume/_batch/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_batch/hume_batch_client.py` & `hume-0.3.5/hume/_batch/hume_batch_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Batch API client."""
 import json
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-import requests
+from requests import Session
 
 from hume._batch.batch_job import BatchJob
 from hume._batch.batch_job_details import BatchJobDetails
 from hume._batch.transcription_config import TranscriptionConfig
 from hume._common.api_type import ApiType
 from hume._common.client_base import ClientBase
 from hume._common.config_utils import serialize_configs
@@ -51,14 +51,15 @@
         """Construct a HumeBatchClient.
 
         Args:
             api_key (str): Hume API key.
             timeout (int): Time in seconds before canceling long-running Hume API requests.
         """
         self._timeout = timeout
+        self._session = Session()
         super().__init__(api_key, *args, **kwargs)
 
     @classmethod
     def get_api_type(cls) -> ApiType:
         """Get the ApiType of the client.
 
         Returns:
@@ -114,15 +115,15 @@
         Raises:
             HumeClientException: If the job details cannot be loaded.
 
         Returns:
             BatchJobDetails: Batch job details.
         """
         endpoint = self._construct_endpoint(f"jobs/{job_id}")
-        response = requests.get(
+        response = self._session.get(
             endpoint,
             timeout=self._timeout,
             headers=self._get_client_headers(),
         )
 
         try:
             body = response.json()
@@ -144,15 +145,15 @@
         Raises:
             HumeClientException: If the job predictions cannot be loaded.
 
         Returns:
             Any: Batch job predictions.
         """
         endpoint = self._construct_endpoint(f"jobs/{job_id}/predictions")
-        response = requests.get(
+        response = self._session.get(
             endpoint,
             timeout=self._timeout,
             headers=self._get_client_headers(),
         )
 
         try:
             body = response.json()
@@ -175,15 +176,15 @@
         Raises:
             HumeClientException: If the job artifacts cannot be loaded.
 
         Returns:
             Any: Batch job artifacts.
         """
         endpoint = self._construct_endpoint(f"jobs/{job_id}/artifacts")
-        response = requests.get(
+        response = self._session.get(
             endpoint,
             timeout=self._timeout,
             headers=self._get_client_headers(),
         )
 
         with Path(filepath).open("wb") as f:
             f.write(response.content)
@@ -208,48 +209,47 @@
         if notify is not None:
             request["notify"] = notify
         return request
 
     def _submit_job(
         self,
         request_body: Any,
-        files: Optional[List[Union[str, Path]]],
+        filepaths: Optional[List[Union[str, Path]]],
     ) -> BatchJob:
         """Start a job for batch processing by passing a JSON request body.
 
         This request body should match the request body used by the batch API,
         including both the list of URLs and the models configuration.
 
         Args:
             request_body (Any): JSON request body to be passed to the batch API.
-            files (Optional[List[Union[str, Path]]]): List of paths to files on the local disk to be processed.
+            filepaths (Optional[List[Union[str, Path]]]): List of paths to files on the local disk to be processed.
 
         Raises:
             HumeClientException: If the batch job fails to start.
 
         Returns:
             BatchJob: A `BatchJob` that wraps the batch computation.
         """
         endpoint = self._construct_endpoint("jobs")
 
-        if files is None:
-            response = requests.post(
+        if filepaths is None:
+            response = self._session.post(
                 endpoint,
                 json=request_body,
                 timeout=self._timeout,
                 headers=self._get_client_headers(),
             )
         else:
-            post_files = [("file", Path(path).read_bytes()) for path in files]
-            post_files.append(("json", json.dumps(request_body).encode("utf-8")))
-            response = requests.post(
+            form_data = self._get_multipart_form_data(request_body, filepaths)
+            response = self._session.post(
                 endpoint,
                 timeout=self._timeout,
                 headers=self._get_client_headers(),
-                files=post_files,
+                files=form_data,
             )
 
         try:
             body = response.json()
         except json.decoder.JSONDecodeError:
             # pylint: disable=raise-missing-from
             raise HumeClientException(f"Failed batch request: {response.text}")
@@ -264,7 +264,34 @@
                     if "InvalidApiKey" in error_code:
                         raise HumeClientException("HumeBatchClient initialized with invalid API key.")
                     raise HumeClientException(f"Could not start batch job: {error_code}: {fault_string}")
                 raise HumeClientException(f"Could not start batch job: {fault_string}")
             raise HumeClientException(f"Unexpected error when starting batch job: {body}")
 
         return BatchJob(self, body["job_id"])
+
+    def _get_multipart_form_data(
+        self,
+        request_body: Any,
+        filepaths: List[Union[str, Path]],
+    ) -> List[Tuple[str, Union[bytes, Tuple[str, bytes]]]]:
+        """Convert a list of filepaths into a list of multipart form data.
+
+        Multipart form data allows the client to attach files to the POST request,
+        including both the raw file bytes and the filename.
+
+        Args:
+            request_body (Any): JSON request body to be passed to the batch API.
+            filepaths (List[Union[str, Path]]): List of paths to files on the local disk to be processed.
+
+        Returns:
+            List[Tuple[str, Union[bytes, Tuple[str, bytes]]]]: A list of tuples representing
+                the multipart form data for the POST request.
+        """
+        form_data: List[Tuple[str, Union[bytes, Tuple[str, bytes]]]] = []
+        for filepath in filepaths:
+            path = Path(filepath)
+            post_file = ("file", (path.name, path.read_bytes()))
+            form_data.append(post_file)
+
+        form_data.append(("json", json.dumps(request_body).encode("utf-8")))
+        return form_data
```

### Comparing `hume-0.3.4/hume/_batch/transcription_config.py` & `hume-0.3.5/hume/_batch/transcription_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_common/client_base.py` & `hume-0.3.5/hume/_common/client_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_common/config_base.py` & `hume-0.3.5/hume/_common/config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_common/config_utils.py` & `hume-0.3.5/hume/_common/config_utils.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_common/retry_utils.py` & `hume-0.3.5/hume/_common/retry_utils.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/_stream/hume_stream_client.py` & `hume-0.3.5/hume/_stream/hume_stream_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         Note: Only one config per model type should be passed.
             If more than one config is passed for a given model type, only the last config will be used.
 
         Args:
             configs (List[ModelConfigBase]): List of job configs.
             stream_window_ms (Optional[int]): Length of the sliding window in milliseconds to use when
-                aggregating media across streaming payloads within one websocket connection.
+                aggregating media across streaming payloads within one WebSocket connection.
         """
         endpoint = self._construct_endpoint("models")
         try:
             # pylint: disable=no-member
             async with websockets.connect(  # type: ignore[attr-defined]
                     endpoint,
                     extra_headers=self._get_client_headers(),
```

### Comparing `hume-0.3.4/hume/_stream/stream_socket.py` & `hume-0.3.5/hume/_stream/stream_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/error/hume_client_exception.py` & `hume-0.3.5/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/config/__init__.py` & `hume-0.3.5/hume/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/config/face_config.py` & `hume-0.3.5/hume/models/config/face_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/config/language_config.py` & `hume-0.3.5/hume/models/config/language_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/config/model_config_base.py` & `hume-0.3.5/hume/models/config/model_config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/config/ner_config.py` & `hume-0.3.5/hume/models/config/ner_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/config/prosody_config.py` & `hume-0.3.5/hume/models/config/prosody_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/hume/models/model_type.py` & `hume-0.3.5/hume/models/model_type.py`

 * *Files identical despite different names*

### Comparing `hume-0.3.4/pyproject.toml` & `hume-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "sentiment",
   "emotion",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.3.4"
+version = "0.3.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 requests = "^2.28.2"
 typing-extensions = "^4.3.0"
 websockets = { version = "^10.3", optional = true }
 jupyter = { version = "^1.0.0", optional = true }
```

### Comparing `hume-0.3.4/PKG-INFO` & `hume-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.3.4
+Version: 0.3.5
 Summary: Hume AI Python Client
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
 Keywords: hume,expressive,communication,audio,recognition,ai,analysis,detection,voice,sentiment,emotion
 Author: Hume AI Dev
 Author-email: dev@hume.ai
 Requires-Python: >=3.8.1,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hume Version: 0.3.4 Summary: Hume AI Python Client
+Metadata-Version: 2.1 Name: hume Version: 0.3.5 Summary: Hume AI Python Client
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
 hume,expressive,communication,audio,recognition,ai,analysis,detection,voice,sentiment,emotion
 Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.8.1,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```


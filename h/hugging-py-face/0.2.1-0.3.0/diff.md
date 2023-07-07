# Comparing `tmp/hugging_py_face-0.2.1.tar.gz` & `tmp/hugging_py_face-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hugging_py_face-0.2.1.tar", last modified: Sat Apr 29 17:41:21 2023, max compression
+gzip compressed data, was "dist\hugging_py_face-0.3.0.tar", last modified: Fri Jul  7 14:24:02 2023, max compression
```

## Comparing `hugging_py_face-0.2.1.tar` & `hugging_py_face-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/
--rw-rw-rw-   0        0        0     6177 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4692 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face/
--rw-rw-rw-   0        0        0      466 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/__about__.py
--rw-rw-rw-   0        0        0      112 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/__init__.py
--rw-rw-rw-   0        0        0     3877 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/audio_processing.py
--rw-rw-rw-   0        0        0     2852 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/computer_vision.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face/config/
--rw-rw-rw-   0        0        0      827 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/config/config.yaml
--rw-rw-rw-   0        0        0      265 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/config/logging.yaml
--rw-rw-rw-   0        0        0      320 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/config_parser.py
--rw-rw-rw-   0        0        0       63 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/exceptions.py
--rw-rw-rw-   0        0        0     2471 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/multimedia_processing.py
--rw-rw-rw-   0        0        0    24527 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/hugging_py_face/nlp.py
-drwxrwxrwx   0        0        0        0 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face.egg-info/
--rw-rw-rw-   0        0        0     6177 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/hugging_py_face.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 17:41:21.000000 hugging_py_face-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-04-29 17:40:56.000000 hugging_py_face-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/
+-rw-rw-rw-   0        0        0     6177 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4692 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face/
+-rw-rw-rw-   0        0        0      466 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/__about__.py
+-rw-rw-rw-   0        0        0      112 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/__init__.py
+-rw-rw-rw-   0        0        0     3927 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/audio_processing.py
+-rw-rw-rw-   0        0        0      884 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/base_api.py
+-rw-rw-rw-   0        0        0     2852 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/computer_vision.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face/config/
+-rw-rw-rw-   0        0        0      837 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/config/config.yaml
+-rw-rw-rw-   0        0        0      265 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/config/logging.yaml
+-rw-rw-rw-   0        0        0      320 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/config_parser.py
+-rw-rw-rw-   0        0        0      171 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/exceptions.py
+-rw-rw-rw-   0        0        0     2447 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/multimedia_processing.py
+-rw-rw-rw-   0        0        0    24515 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/hugging_py_face/nlp.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face.egg-info/
+-rw-rw-rw-   0        0        0     6177 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/hugging_py_face.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:24:02.000000 hugging_py_face-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-07-07 14:23:29.000000 hugging_py_face-0.3.0/setup.py
```

### Comparing `hugging_py_face-0.2.1/PKG-INFO` & `hugging_py_face-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging_py_face
-Version: 0.2.1
+Version: 0.3.0
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.2.1/README.md` & `hugging_py_face-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.2.1/hugging_py_face/audio_processing.py` & `hugging_py_face-0.3.0/hugging_py_face/audio_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 from .multimedia_processing import MultimediaProcessing
 
 
 class AudioProcessing(MultimediaProcessing):
     def __init__(self, api_token):
         super().__init__(api_token)
 
-    def speech_recognition(self, inputs: Union[Text, List], model: Optional[Text] = None) -> Union[Dict, List]:
+    def automatic_speech_recognition(self, inputs: Union[Text, List], model: Optional[Text] = None) -> Union[Dict, List]:
         """
         Perform speech recognition on an audio file from a file path or an url.
 
         :param inputs: a string or a list of strings of the file paths or urls of the audio files to perform speech recognition on.
         :param model: the model to use for the speech recognition task. If not provided, the recommended model from Hugging Face will be used.
         :return: a dictionary or a list of dictionaries containing the text recognized from the audio file(s).
         """
         if type(inputs) == list:
-            return self._query_in_list(inputs, model=model, task="speech-recognition")
+            return self._query_in_list(inputs, model=model, task="automatic-speech-recognition")
         elif type(inputs) == str:
-            return self._query(inputs, model=model, task="speech-recognition")
+            return self._query(inputs, model=model, task="automatic-speech-recognition")
 
-    def speech_recognition_in_df(self, df: DataFrame, column: Text, model: Optional[Text] = None) -> DataFrame:
+    def automatic_speech_recognition_in_df(self, df: DataFrame, column: Text, model: Optional[Text] = None) -> DataFrame:
         """
         Perform speech recognition on audio files from a DataFrame.
 
         :param df: a pandas DataFrame containing the audio files to perform speech recognition on.
         :param column: the name of the column containing the file paths or urls of the audio files to perform speech recognition on.
         :param model: the model to use for the speech recognition task. If not provided, the recommended model from Hugging Face will be used.
         :return: a pandas DataFrame with the text recognized from the audio files. The text will be added as a new column called 'predictions' to the original DataFrame.
         """
-        predictions = self._query_in_df(df, column, model=model, task="speech-recognition")
+        predictions = self._query_in_df(df, column, model=model, task="automatic-speech-recognition")
         df["predictions"] = [prediction['text'] for prediction in predictions]
         return df
 
     def audio_classification(self, inputs: Text, model: Optional[Text] = None) -> List:
         """
         Classify an audio file from a file path or an url.
```

### Comparing `hugging_py_face-0.2.1/hugging_py_face/computer_vision.py` & `hugging_py_face-0.3.0/hugging_py_face/computer_vision.py`

 * *Files identical despite different names*

### Comparing `hugging_py_face-0.2.1/hugging_py_face/config/config.yaml` & `hugging_py_face-0.3.0/hugging_py_face/config/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,11 +8,11 @@
   text-classification: distilbert-base-uncased-finetuned-sst-2-english
   text-generation: gpt2
   zero-shot-classification: facebook/bart-large-mnli
   conversational: microsoft/DialoGPT-large
   feature-extraction: julien-c/distilbert-feature-extraction
   image-classification: google/vit-base-patch16-224
   object-detection: facebook/detr-resnet-50
-  speech-recognition: facebook/wav2vec2-base-960h
+  automatic-speech-recognition: facebook/wav2vec2-base-960h
   audio-classification: superb/hubert-large-superb-er
 MAX_RETRIES: 5
 HTTP_SERVICE_UNAVAILABLE: 503
```

### Comparing `hugging_py_face-0.2.1/hugging_py_face/nlp.py` & `hugging_py_face-0.3.0/hugging_py_face/nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import json
 import time
-import logging
 import requests
 import pandas as pd
-import logging.config
 from pandas import DataFrame
 from typing import Text, List, Dict, Optional, Union
 
-from .config_parser import ConfigParser
-from .exceptions import HTTPServiceUnavailableException
+from .base_api import BaseAPI
+from .exceptions import HTTPServiceUnavailableException, APICallException
 
-logging_config_parser = ConfigParser('config/logging.yaml')
-logging.config.dictConfig(logging_config_parser.get_config_dict())
-logger = logging.getLogger()
 
-
-class NLP:
+class NLP(BaseAPI):
     def __init__(self, api_token):
-        self.api_token = api_token
-
-        config_parser = ConfigParser()
-        self.config = config_parser.get_config_dict()
-
-        self.logger = logger
+        super().__init__(api_token)
 
     def _query(self, inputs: Union[Text, List, Dict], parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
+        if model:
+            self._check_model_task_match(model, task)
+
         api_url = f"{self.config['BASE_URL']}/{model if model is not None else self.config['TASK_MODEL_MAP'][task]}"
 
         headers = {
             "Authorization": f"Bearer {self.api_token}"
         }
 
         data = {
@@ -47,16 +39,19 @@
             retries += 1
 
             response = requests.request("POST", api_url, headers=headers, data=json.dumps(data))
             if response.status_code == int(self.config['HTTP_SERVICE_UNAVAILABLE']):
                 self.logger.info(f"Status code: {response.status_code}.")
                 self.logger.info("Retrying..")
                 time.sleep(1)
-            else:
+            elif response.status_code == 200:
                 return json.loads(response.content.decode("utf-8"))
+            else:
+                self.logger.info(f"Status code: {response.status_code}.")
+                raise APICallException(f"API call failed with status code {response.status_code}.")
 
         self.logger.info(f"Status code: {response.status_code}.")
         self.logger.info("Connection to the server failed after reaching maximum retry attempts.")
         self.logger.debug(f"Response: {json.loads(response.content.decode('utf-8'))}.")
         raise HTTPServiceUnavailableException("The HTTP service is unavailable.")
 
     def _query_in_df(self, df: DataFrame, column: Text, parameters: Optional[Dict] = None, options: Optional[Dict] = None, model: Optional[Text] = None, task: Optional[Text] = None) -> Union[Dict, List]:
```

### Comparing `hugging_py_face-0.2.1/hugging_py_face.egg-info/PKG-INFO` & `hugging_py_face-0.3.0/hugging_py_face.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugging-py-face
-Version: 0.2.1
+Version: 0.3.0
 Summary: Hugging-Py-Face, the Python client for the Hugging Face Inference API.
 Home-page: https://github.com/MinuraPunchihewa/hugging_py_face
 Author: Minura Punchihewa
 Author-email: minurapunchihewa17@gmail.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/hugging-py-face/
 Description: # Hugging-Py-Face
```

### Comparing `hugging_py_face-0.2.1/hugging_py_face.egg-info/SOURCES.txt` & `hugging_py_face-0.3.0/hugging_py_face.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 hugging_py_face/__about__.py
 hugging_py_face/__init__.py
 hugging_py_face/audio_processing.py
+hugging_py_face/base_api.py
 hugging_py_face/computer_vision.py
 hugging_py_face/config_parser.py
 hugging_py_face/exceptions.py
 hugging_py_face/multimedia_processing.py
 hugging_py_face/nlp.py
 hugging_py_face.egg-info/PKG-INFO
 hugging_py_face.egg-info/SOURCES.txt
```

### Comparing `hugging_py_face-0.2.1/setup.py` & `hugging_py_face-0.3.0/setup.py`

 * *Files identical despite different names*


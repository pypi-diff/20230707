# Comparing `tmp/audiostack-0.0.6.tar.gz` & `tmp/audiostack-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-0.0.6.tar", last modified: Tue May  9 08:44:14 2023, max compression
+gzip compressed data, was "audiostack-0.0.7.tar", last modified: Thu Jun  1 13:44:18 2023, max compression
```

## Comparing `audiostack-0.0.6.tar` & `audiostack-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.902231 audiostack-0.0.6/
--rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-05-09 08:44:14.902039 audiostack-0.0.6/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.6/README.md
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.891264 audiostack-0.0.6/audiostack/
--rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-05-09 08:43:52.000000 audiostack-0.0.6/audiostack/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.893330 audiostack-0.0.6/audiostack/content/
--rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.6/audiostack/content/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/content/media.py
--rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.6/audiostack/content/root_functions.py
--rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/content/script.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.894326 audiostack-0.0.6/audiostack/delivery/
--rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.6/audiostack/delivery/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2313 2023-05-04 12:16:31.000000 audiostack-0.0.6/audiostack/delivery/encoder.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.894909 audiostack-0.0.6/audiostack/docs/
--rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/docs/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/docs/docs.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.896962 audiostack-0.0.6/audiostack/helpers/
--rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.6/audiostack/helpers/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/api_item.py
--rw-r--r--   0 hackerman   (501) staff       (20)      811 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/api_list.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4301 2023-04-17 07:54:26.000000 audiostack-0.0.6/audiostack/helpers/request_interface.py
--rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/request_types.py
--rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/response.py
--rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/helpers/util.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.897112 audiostack-0.0.6/audiostack/orchestrator/
--rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.898721 audiostack-0.0.6/audiostack/production/
--rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/production/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     3821 2023-05-04 12:16:01.000000 audiostack-0.0.6/audiostack/production/mix.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4349 2023-04-17 07:55:11.000000 audiostack-0.0.6/audiostack/production/sound.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.900001 audiostack-0.0.6/audiostack/speech/
--rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.6/audiostack/speech/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/speech/diction.py
--rw-r--r--   0 hackerman   (501) staff       (20)     4502 2023-03-16 15:15:23.000000 audiostack-0.0.6/audiostack/speech/tts.py
--rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.6/audiostack/speech/voice.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.892015 audiostack-0.0.6/audiostack.egg-info/
--rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 hackerman   (501) staff       (20)      959 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/requires.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-05-09 08:44:14.000000 audiostack-0.0.6/audiostack.egg-info/top_level.txt
--rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-05-09 08:44:14.902292 audiostack-0.0.6/setup.cfg
--rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.6/setup.py
-drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-05-09 08:44:14.901377 audiostack-0.0.6/tests/
--rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.6/tests/__init__.py
--rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.6/tests/test_audience.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.496035 audiostack-0.0.7/
+-rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-06-01 13:44:18.495875 audiostack-0.0.7/PKG-INFO
+-rw-r--r--   0 hackerman   (501) staff       (20)    26796 2022-12-13 14:01:40.000000 audiostack-0.0.7/README.md
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.486341 audiostack-0.0.7/audiostack/
+-rw-r--r--   0 hackerman   (501) staff       (20)      555 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/__init__.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.488871 audiostack-0.0.7/audiostack/content/
+-rw-r--r--   0 hackerman   (501) staff       (20)      459 2023-03-16 15:15:23.000000 audiostack-0.0.7/audiostack/content/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2270 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/content/media.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      947 2023-03-16 15:15:23.000000 audiostack-0.0.7/audiostack/content/root_functions.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     3528 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/content/script.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.489482 audiostack-0.0.7/audiostack/delivery/
+-rw-r--r--   0 hackerman   (501) staff       (20)       48 2022-12-06 15:30:00.000000 audiostack-0.0.7/audiostack/delivery/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2313 2023-05-04 12:16:31.000000 audiostack-0.0.7/audiostack/delivery/encoder.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.490214 audiostack-0.0.7/audiostack/docs/
+-rw-r--r--   0 hackerman   (501) staff       (20)       47 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/docs/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      631 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/docs/docs.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.492062 audiostack-0.0.7/audiostack/helpers/
+-rw-r--r--   0 hackerman   (501) staff       (20)        0 2022-12-06 15:30:00.000000 audiostack-0.0.7/audiostack/helpers/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      716 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/api_item.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      972 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/helpers/api_list.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4322 2023-05-22 09:42:33.000000 audiostack-0.0.7/audiostack/helpers/request_interface.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      163 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/request_types.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      338 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/response.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      227 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/helpers/util.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.492255 audiostack-0.0.7/audiostack/orchestrator/
+-rw-r--r--   0 hackerman   (501) staff       (20)       58 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.493282 audiostack-0.0.7/audiostack/production/
+-rw-r--r--   0 hackerman   (501) staff       (20)       88 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/production/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4149 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/production/mix.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4349 2023-04-17 07:55:11.000000 audiostack-0.0.7/audiostack/production/sound.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.494550 audiostack-0.0.7/audiostack/speech/
+-rw-r--r--   0 hackerman   (501) staff       (20)      126 2022-12-08 09:57:07.000000 audiostack-0.0.7/audiostack/speech/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     2979 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/speech/diction.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     4621 2023-06-01 13:43:58.000000 audiostack-0.0.7/audiostack/speech/tts.py
+-rw-r--r--   0 hackerman   (501) staff       (20)     1215 2023-02-20 16:32:25.000000 audiostack-0.0.7/audiostack/speech/voice.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.487224 audiostack-0.0.7/audiostack.egg-info/
+-rw-r--r--   0 hackerman   (501) staff       (20)    33108 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 hackerman   (501) staff       (20)      959 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)        1 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       45 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/requires.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       17 2023-06-01 13:44:18.000000 audiostack-0.0.7/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 hackerman   (501) staff       (20)       38 2023-06-01 13:44:18.496093 audiostack-0.0.7/setup.cfg
+-rw-r--r--   0 hackerman   (501) staff       (20)     1039 2023-02-20 16:12:26.000000 audiostack-0.0.7/setup.py
+drwxr-xr-x   0 hackerman   (501) staff       (20)        0 2023-06-01 13:44:18.495171 audiostack-0.0.7/tests/
+-rw-r--r--   0 hackerman   (501) staff       (20)      173 2023-02-20 16:03:10.000000 audiostack-0.0.7/tests/__init__.py
+-rw-r--r--   0 hackerman   (501) staff       (20)      659 2023-02-20 16:41:55.000000 audiostack-0.0.7/tests/test_audience.py
```

### Comparing `audiostack-0.0.6/PKG-INFO` & `audiostack-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 License: UNKNOWN
 Description: <p align="center">
         <a href="https://www.api.audio/" rel="noopener">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 0.0.6 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 0.0.7 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai License: UNKNOWN
 Description:
                                [api.audio_logo]
                       **** apiaudio - audiostack SDK ****
 ---
    audiostack is the official api.audio Python 3 SDK. This SDK provides easy
```

### Comparing `audiostack-0.0.6/README.md` & `audiostack-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/__init__.py` & `audiostack-0.0.7/audiostack/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-sdk_version = "0.0.6"
+sdk_version = "0.0.7"
 api_base = "https://v2.api.audio"
 api_key = None
 
-api_version = "0.0.6"
+api_version = "0.0.7"
 verify_ssl_certs = True
 proxy = None
 default_http_client = None
 app_info = None
 enable_telemetry = True
 max_network_retries = 0
```

### Comparing `audiostack-0.0.6/audiostack/content/media.py` & `audiostack-0.0.7/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/content/root_functions.py` & `audiostack-0.0.7/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/content/script.py` & `audiostack-0.0.7/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/delivery/encoder.py` & `audiostack-0.0.7/audiostack/delivery/encoder.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/docs/docs.py` & `audiostack-0.0.7/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/helpers/api_item.py` & `audiostack-0.0.7/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/helpers/api_list.py` & `audiostack-0.0.7/audiostack/helpers/api_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,19 @@
         self.idx += 1
         try:
             item = self.items[self.idx - 1]
             return self.resolve_item(self.list_type, item)
 
         except IndexError:
             self.idx = 0
-            raise StopIteration  # Done iterating.
+            raise StopIteration  
 
     def __getitem__(self, x):
-        return self.items[x]
+        if isinstance(x, slice):
+            return [self.resolve_item(self.list_type, x) for x in self.items[x.start: x.stop]]
+        else:
+            return self.resolve_item(self.list_type, x)
+        
 
     # child classes should override this method, failing to do so will raise an exception!
     def resolve_item(self, list_type):
         raise Exception()
```

### Comparing `audiostack-0.0.6/audiostack/helpers/request_interface.py` & `audiostack-0.0.7/audiostack/helpers/request_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             "x-api-key": audiostack.api_key,
             "x-python-sdk-version": audiostack.sdk_version
             # "x-assume-org": audiostack.assume_org_id,
         }
 
     def resolve_response(self, r):
         if r.status_code >= 500:
+            print(r)
             raise Exception("Internal server error - aborting")
 
         if self.DEBUG_PRINT:
             print(json.dumps(r.json(), indent=4))
 
         if "meta" in r.json():
             if "creditsUsed" in r.json()["meta"]:
```

### Comparing `audiostack-0.0.6/audiostack/production/mix.py` & `audiostack-0.0.7/audiostack/production/mix.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,20 @@
             super().__init__(response)
             self.productionId = self.data["productionId"]
 
         def download(self, fileName="", path="./") -> None:
             sections = self.data["files"]
             for i, s in enumerate(sections):
                 format = s["format"]
+                original_name = s["filename"]
+
                 if not fileName:
-                    full_name = f"default_mix.{format}"
+                    full_name = f"{original_name}.{format}"
                 else:
-                    full_name = f"{fileName}.{format}"
+                    full_name = f"{fileName}_{i}.{format}"
 
                 RequestInterface.download_url(
                     s["url"], destination=path, name=full_name
                 )
 
         def delete(self):
             return Mix.delete(self.productionId)
@@ -45,14 +47,16 @@
         soundTemplate: str = "",
         mediaFiles: dict = {},
         fxFiles: dict = {},
         sectionProperties: dict = {},
         timelineProperties: dict = {},
         masteringPreset: str = "",
         public: bool = False,
+        exportSettings: dict = {},
+        strictValidation: bool = True
     ) -> Item:
         if speechId and speechItem:
             raise Exception("speechId or scriptItem should be supplied not both")
         if not (speechId or speechItem):
             raise Exception("speechId or scriptItem should be supplied")
         if speechItem:
             speechId = speechItem.speechId
@@ -68,20 +72,24 @@
             "soundTemplate": soundTemplate,
             "mediaFiles": mediaFiles,
             "fxFiles": fxFiles,
             "sectionProperties": sectionProperties,
             "timelineProperties": timelineProperties,
             "masteringPreset": masteringPreset,
             "public": public,
+            "exportSettings" : exportSettings,
+            "strictValidation" : strictValidation
         }
 
         r = Mix.interface.send_request(rtype=RequestTypes.POST, route="mix", json=body)
-        if r["statusCode"] == 202:
+        while r["statusCode"] == 202:
             print("Response in progress please wait...")
-            return Mix.get(Mix.Item(r).productionId)
+            r = Mix.interface.send_request(
+                rtype=RequestTypes.GET, route="mix", path_parameters=r["data"]["productionId"]
+            )
         
         return Mix.Item(r)
 
     @staticmethod
     def get(productionId: str) -> Item:
         r = Mix.interface.send_request(
             rtype=RequestTypes.GET, route="mix", path_parameters=productionId
```

### Comparing `audiostack-0.0.6/audiostack/production/sound.py` & `audiostack-0.0.7/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/speech/diction.py` & `audiostack-0.0.7/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack/speech/tts.py` & `audiostack-0.0.7/audiostack/speech/tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,20 @@
             "useDictionary": useDictionary,
             "useTextNormalizer": useTextNormalizer,
             "public": public,
             "sync": sync,
         }
 
         r = TTS.interface.send_request(rtype=RequestTypes.POST, route="tts", json=body)
-        if r["statusCode"] == 202:
+        while r["statusCode"] == 202:
             print("Response in progress please wait...")
-            return TTS.get(TTS.Item(r).speechId)
+            r = TTS.interface.send_request(
+                rtype=RequestTypes.GET, route="tts", path_parameters=r["data"]["speechId"]   
+            )
+            
         return TTS.Item(r)
 
     @staticmethod
     def get(speechId: str) -> Item:
         r = TTS.interface.send_request(
             rtype=RequestTypes.GET, route="tts", path_parameters=speechId
         )
```

### Comparing `audiostack-0.0.6/audiostack/speech/voice.py` & `audiostack-0.0.7/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/audiostack.egg-info/PKG-INFO` & `audiostack-0.0.7/audiostack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 License: UNKNOWN
 Description: <p align="center">
         <a href="https://www.api.audio/" rel="noopener">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 0.0.6 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 0.0.7 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai License: UNKNOWN
 Description:
                                [api.audio_logo]
                       **** apiaudio - audiostack SDK ****
 ---
    audiostack is the official api.audio Python 3 SDK. This SDK provides easy
```

### Comparing `audiostack-0.0.6/audiostack.egg-info/SOURCES.txt` & `audiostack-0.0.7/audiostack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/setup.py` & `audiostack-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `audiostack-0.0.6/tests/test_audience.py` & `audiostack-0.0.7/tests/test_audience.py`

 * *Files identical despite different names*


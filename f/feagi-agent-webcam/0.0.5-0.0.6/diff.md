# Comparing `tmp/feagi_agent_webcam-0.0.5.tar.gz` & `tmp/feagi_agent_webcam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent_webcam-0.0.5.tar", last modified: Thu Mar 23 21:57:16 2023, max compression
+gzip compressed data, was "feagi_agent_webcam-0.0.6.tar", last modified: Fri Jul  7 14:27:11 2023, max compression
```

## Comparing `feagi_agent_webcam-0.0.5.tar` & `feagi_agent_webcam-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:57:16.803193 feagi_agent_webcam-0.0.5/
--rw-r--r--   0 station1   (501) staff       (20)    11344 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/LICENSE
--rw-r--r--   0 station1   (501) staff       (20)     1305 2023-03-23 21:57:16.803277 feagi_agent_webcam-0.0.5/PKG-INFO
--rw-r--r--   0 station1   (501) staff       (20)      766 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/README.md
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:57:16.801814 feagi_agent_webcam-0.0.5/feagi_agent_webcam/
--rw-r--r--   0 station1   (501) staff       (20)        0 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam/__init__.py
--rw-r--r--   0 station1   (501) staff       (20)     1543 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam/__main__.py
--rw-r--r--   0 station1   (501) staff       (20)     1411 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam/configuration.py
--rw-r--r--   0 station1   (501) staff       (20)     9452 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam/controller.py
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:57:16.803051 feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/
--rw-r--r--   0 station1   (501) staff       (20)     1305 2023-03-23 21:57:16.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/PKG-INFO
--rw-r--r--   0 station1   (501) staff       (20)      390 2023-03-23 21:57:16.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/SOURCES.txt
--rw-r--r--   0 station1   (501) staff       (20)        1 2023-03-23 21:57:16.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/dependency_links.txt
--rw-r--r--   0 station1   (501) staff       (20)       64 2023-03-23 21:57:16.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/requires.txt
--rw-r--r--   0 station1   (501) staff       (20)       19 2023-03-23 21:57:16.000000 feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/top_level.txt
--rw-r--r--   0 station1   (501) staff       (20)       99 2023-03-23 21:48:00.000000 feagi_agent_webcam-0.0.5/pyproject.toml
--rw-r--r--   0 station1   (501) staff       (20)      742 2023-03-23 21:57:16.803729 feagi_agent_webcam-0.0.5/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:27:11.359550 feagi_agent_webcam-0.0.6/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1305 2023-07-07 14:27:11.359550 feagi_agent_webcam-0.0.6/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      766 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/README.md
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:27:11.359550 feagi_agent_webcam-0.0.6/feagi_agent_webcam/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1543 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam/__main__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1538 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam/configuration.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     9774 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam/controller.py
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:27:11.359550 feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1305 2023-07-07 14:27:11.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      390 2023-07-07 14:27:11.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-07 14:27:11.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       64 2023-07-07 14:27:11.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/requires.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       19 2023-07-07 14:27:11.000000 feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/top_level.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-07 13:18:01.000000 feagi_agent_webcam-0.0.6/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      742 2023-07-07 14:27:11.359550 feagi_agent_webcam-0.0.6/setup.cfg
```

### Comparing `feagi_agent_webcam-0.0.5/LICENSE` & `feagi_agent_webcam-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent_webcam-0.0.5/PKG-INFO` & `feagi_agent_webcam-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_agent_webcam
-Version: 0.0.5
+Version: 0.0.6
 Summary: Feagi agent webcam to connect feagi with your webcam
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@neuraville.com
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_webcam-0.0.5/README.md` & `feagi_agent_webcam-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `feagi_agent_webcam-0.0.5/feagi_agent_webcam/__main__.py` & `feagi_agent_webcam-0.0.6/feagi_agent_webcam/__main__.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_webcam-0.0.5/feagi_agent_webcam/configuration.py` & `feagi_agent_webcam-0.0.6/feagi_agent_webcam/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
 
 feagi_settings = {
+    # "feagi_auth_url": "http://127.0.0.1:9000/v1/k8/feagi_settings/auth_token",
+    "feagi_url": None,
+    "feagi_dns": None,
     "feagi_host": "127.0.0.1",
     "feagi_api_port": "8000",
 }
 
 agent_settings = {
-    "agent_data_port": "40010",
+    "agent_data_port": "10005",
     "agent_id": "camera_1",
     "agent_type": "embodiment",
     'TTL': 2,
     'last_message': 0,
 }
 
 capabilities = {
```

### Comparing `feagi_agent_webcam-0.0.5/feagi_agent_webcam/controller.py` & `feagi_agent_webcam-0.0.6/feagi_agent_webcam/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # -*- coding: utf-8 -*-
 
 """
 Demo of dot kinematogram
 """
 
 import sys
+sys.path.append('../../feagi_agent_core/')
 import cv2
 import requests
 from time import sleep
 from datetime import datetime
 from feagi_agent import retina as retina
 from feagi_agent import feagi_interface as feagi
+import traceback
 
 
 def chroma_keyer(frame, size, name_id):
     """
     This function allows you to remove the specific color. In psychopy window, it shows a gray which is 128,128,128.
     So this function will remove the 128 and focus on something else than the gray. Consider this as making the data
     into a transparent.
@@ -53,49 +55,42 @@
 
     if len(vision_dict) > 3500:
         return {'camera': {name_id: {}}}
     else:
         return {'camera': {name_id: vision_dict}}
 
 
-def main(feagi_settings, agent_settings, capabilities, message_to_feagi):
+def main(feagi_auth_url, feagi_settings, agent_settings, capabilities, message_to_feagi):
     print("feagi setting: ", feagi_settings)
     print("agent setting: ", agent_settings)
     print("capa: ", capabilities)
     print("message: ", message_to_feagi)
     # Generate runtime dictionary
     previous_data_frame = dict()
-    runtime_data = {"cortical_data": {}, "current_burst_id": None, "stimulation_period": None, "feagi_state": None,
+    runtime_data = {"cortical_data": {}, "current_burst_id": None, "stimulation_period": None,
+                    "feagi_state": None,
                     "feagi_network": None}
 
     # FEAGI section start
     print("Connecting to FEAGI resources...")
-
-    feagi_host, api_port, app_data_port = feagi.feagi_setting_for_registration(feagi_settings, agent_settings)
-
-    print(feagi_host, api_port, app_data_port)
-
-    # address = 'tcp://' + network_settings['feagi_host'] + ':' + network_settings['feagi_opu_port']
-
-    api_address = 'http://' + feagi_host + ':' + api_port
+    runtime_data["feagi_state"] = feagi.feagi_registration(feagi_auth_url=feagi_auth_url, 
+            feagi_settings=feagi_settings, agent_settings=agent_settings, capabilities=capabilities)
+    api_address = runtime_data['feagi_state']["feagi_url"]
 
     stimulation_period_endpoint = feagi.feagi_api_burst_engine()
     burst_counter_endpoint = feagi.feagi_api_burst_counter()
-    print("^ ^ ^")
-    runtime_data["feagi_state"] = feagi.feagi_registration(feagi_host=feagi_host,
-                                                           api_port=api_port, agent_settings=agent_settings,
-                                                           capabilities=capabilities)
-
+    
+    # agent_data_port = agent_settings["agent_data_port"]
+    agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
 
     # todo: to obtain this info directly from FEAGI as part of registration
     # ipu_channel_address = feagi.feagi_inbound(agent_settings["agent_data_port"])
-    ipu_channel_address = feagi.feagi_outbound(feagi_settings['feagi_host'],
-                                               agent_settings["agent_data_port"])
+    ipu_channel_address = feagi.feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
     print("IPU_channel_address=", ipu_channel_address)
     opu_channel_address = feagi.feagi_outbound(feagi_settings['feagi_host'],
                                                runtime_data["feagi_state"]['feagi_opu_port'])
 
     feagi_ipu_channel = feagi.pub_initializer(ipu_channel_address, bind=False)
     feagi_opu_channel = feagi.sub_initializer(opu_address=opu_channel_address)
     # FEAGI section ends
@@ -183,16 +178,30 @@
                 if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
                     feagi_settings['feagi_burst_speed'] = feagi_burst_speed
             if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
                 feagi_settings['feagi_burst_speed'] = feagi_burst_speed
                 msg_counter = feagi_burst_counter
         sleep(feagi_settings['feagi_burst_speed'])
         try:
-            print(len(message_to_feagi['data']['sensory_data']['camera']['C']))
+            print("Len --", len(message_to_feagi['data']['sensory_data']['camera']['C']))
         except:
             pass
         feagi_ipu_channel.send(message_to_feagi)
         message_to_feagi.clear()
         for i in rgb['camera']:
             rgb['camera'][i].clear()
     win.close()
     core.quit()
+
+
+
+if __name__=='__main__':
+    from configuration import feagi_settings, agent_settings, capabilities, message_to_feagi
+    feagi_auth_url = feagi_settings.pop('feagi_auth_url', None)
+    print("FEAGI AUTH URL ------- ", feagi_auth_url)
+    while True:
+        try:
+            main(feagi_auth_url, feagi_settings, agent_settings, capabilities, message_to_feagi)
+        except Exception as e:
+            print(f"Controller run failed", e)
+            traceback.print_exc()
+            sleep(2)
```

### Comparing `feagi_agent_webcam-0.0.5/feagi_agent_webcam.egg-info/PKG-INFO` & `feagi_agent_webcam-0.0.6/feagi_agent_webcam.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi-agent-webcam
-Version: 0.0.5
+Version: 0.0.6
 Summary: Feagi agent webcam to connect feagi with your webcam
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@neuraville.com
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_webcam-0.0.5/setup.cfg` & `feagi_agent_webcam-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_agent_webcam
-version = 0.0.5
+version = 0.0.6
 author = Neuraville LLC
 author_email = info@neuraville.com
 description = Feagi agent webcam to connect feagi with your webcam
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```


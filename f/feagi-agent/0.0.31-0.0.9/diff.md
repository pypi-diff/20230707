# Comparing `tmp/feagi_agent-0.0.31.tar.gz` & `tmp/feagi_agent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent-0.0.31.tar", last modified: Fri Jul  7 14:21:59 2023, max compression
+gzip compressed data, was "feagi_agent-0.0.9.tar", last modified: Fri Oct  7 18:47:46 2022, max compression
```

## Comparing `feagi_agent-0.0.31.tar` & `feagi_agent-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:21:59.216506 feagi_agent-0.0.31/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/LICENSE
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1892 2023-07-07 14:21:59.216506 feagi_agent-0.0.31/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1361 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/README.md
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:21:59.216506 feagi_agent-0.0.31/feagi_agent/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/feagi_agent/__init__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1381 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/feagi_agent/configuration.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    10289 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/feagi_agent/feagi_interface.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5037 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/feagi_agent/retina.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     8685 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/feagi_agent/router.py
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:21:59.216506 feagi_agent-0.0.31/feagi_agent.egg-info/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1892 2023-07-07 14:21:59.000000 feagi_agent-0.0.31/feagi_agent.egg-info/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      354 2023-07-07 14:21:59.000000 feagi_agent-0.0.31/feagi_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-07 14:21:59.000000 feagi_agent-0.0.31/feagi_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       76 2023-07-07 14:21:59.000000 feagi_agent-0.0.31/feagi_agent.egg-info/requires.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       12 2023-07-07 14:21:59.000000 feagi_agent-0.0.31/feagi_agent.egg-info/top_level.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-07 13:18:01.000000 feagi_agent-0.0.31/pyproject.toml
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      747 2023-07-07 14:21:59.216506 feagi_agent-0.0.31/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2022-10-07 18:47:46.231292 feagi_agent-0.0.9/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2022-10-07 14:02:44.000000 feagi_agent-0.0.9/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      575 2022-10-07 18:47:46.231292 feagi_agent-0.0.9/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        6 2022-10-06 20:52:12.000000 feagi_agent-0.0.9/README.md
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2022-10-07 14:03:44.000000 feagi_agent-0.0.9/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      694 2022-10-07 18:47:46.231292 feagi_agent-0.0.9/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2022-10-07 18:47:46.227292 feagi_agent-0.0.9/src/
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2022-10-07 18:47:46.231292 feagi_agent-0.0.9/src/feagi_agent/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2022-10-07 14:00:37.000000 feagi_agent-0.0.9/src/feagi_agent/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     8830 2022-10-07 18:22:11.000000 feagi_agent-0.0.9/src/feagi_agent/feagi_interface.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     4330 2022-10-06 19:25:21.000000 feagi_agent-0.0.9/src/feagi_agent/retina.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     3685 2022-10-06 17:30:32.000000 feagi_agent-0.0.9/src/feagi_agent/router.py
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2022-10-07 18:47:46.231292 feagi_agent-0.0.9/src/feagi_agent.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      575 2022-10-07 18:47:46.000000 feagi_agent-0.0.9/src/feagi_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      313 2022-10-07 18:47:46.000000 feagi_agent-0.0.9/src/feagi_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2022-10-07 18:47:46.000000 feagi_agent-0.0.9/src/feagi_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       12 2022-10-07 18:47:46.000000 feagi_agent-0.0.9/src/feagi_agent.egg-info/top_level.txt
```

### Comparing `feagi_agent-0.0.31/LICENSE` & `feagi_agent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent-0.0.31/feagi_agent/feagi_interface.py` & `feagi_agent-0.0.9/src/feagi_agent/feagi_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,65 @@
-import traceback
+import configuration
 from feagi_agent import router
 from time import sleep
-import requests
 
 
-def pub_initializer(ipu_address, bind=True):
-    return router.Pub(address=ipu_address, bind=bind)
+def pub_initializer(ipu_address):
+    return router.Pub(address=ipu_address)
 
 
 def sub_initializer(opu_address, flags=router.zmq.NOBLOCK):
     return router.Sub(address=opu_address, flags=flags)
 
 
-# def feagi_registration(feagi_host, api_port, agent_settings, capabilities):
-#     host_info = router.app_host_info()
-#     runtime_data = {
-#         "host_network": {},
-#         "feagi_state": None
-#     }
-#     runtime_data["host_network"]["host_name"] = host_info["host_name"]
-#     runtime_data["host_network"]["ip_address"] = host_info["ip_address"]
-
-#     while runtime_data["feagi_state"] is None:
-#         print("\nAwaiting registration with FEAGI...")
-#         print("feagi_host:", feagi_host,
-#               "\tapi_port:", api_port,
-#               "\nagent_settings:", agent_settings)
-#         try:
-#             runtime_data["feagi_state"] = \
-#                 router.register_with_feagi(feagi_ip=feagi_host,
-#                                            feagi_api_port=api_port,
-#                                            agent_type=agent_settings['agent_type'],
-#                                            agent_id=agent_settings['agent_id'],
-#                                            agent_ip=runtime_data["host_network"]["ip_address"],
-#                                            agent_data_port=agent_settings['agent_data_port'],
-#                                            agent_capabilities=capabilities)
-#         except Exception as e:
-#             print("ERROR__: ", e, traceback.print_exc())
-#             pass
-#         sleep(1)
-#     return runtime_data["feagi_state"]
-
-
-def feagi_registration(feagi_auth_url, feagi_settings, agent_settings, capabilities):
-    host_info = router.app_host_info()
+def feagi_registration(feagi_host, api_port, host_info=router.app_host_info()):
     runtime_data = {
         "host_network": {},
         "feagi_state": None
     }
     runtime_data["host_network"]["host_name"] = host_info["host_name"]
     runtime_data["host_network"]["ip_address"] = host_info["ip_address"]
-    agent_settings['agent_ip'] = host_info["ip_address"]
 
     while runtime_data["feagi_state"] is None:
-        print("\nAwaiting registration with FEAGI...")
+        print("Awaiting registration with FEAGI...")
         try:
-            runtime_data["feagi_state"] = \
-                router.register_with_feagi(feagi_auth_url, feagi_settings, agent_settings, capabilities)
+            runtime_data["feagi_state"] = router.register_with_feagi(app_name=configuration.app_name,
+                                                                     feagi_host=feagi_host,
+                                                                     api_port=api_port,
+                                                                     app_capabilities=configuration.capabilities,
+                                                                     app_host_info=runtime_data["host_network"]
+                                                                     )
         except Exception as e:
-            print("ERROR__: ", e, traceback.print_exc())
+            # print("ERROR: ", e)
             pass
         sleep(1)
     return runtime_data["feagi_state"]
 
 
 def block_to_array(block_ref):
     block_id_str = block_ref.split('-')
     array = [int(x) for x in block_id_str]
     return array
 
 
-def feagi_setting_for_registration(feagi_settings, agent_settings):
+def feagi_setting_for_registration():
     """
     Generate all needed information and return the full data to make it easier to connect with
     FEAGI
     """
-    feagi_ip_host = feagi_settings["feagi_host"]
-    api_port = feagi_settings["feagi_api_port"]
-    app_data_port = agent_settings["agent_data_port"]
-    return feagi_ip_host, api_port, app_data_port
+    feagi_ip_host = configuration.network_settings["feagi_host"]
+    api_data = configuration.network_settings["feagi_api_port"]
+    return feagi_ip_host, api_data
+
+
+def feagi_gui_address(feagi_ip_host, api_data):
+    """
+    return a full path to api
+    """
+    return 'http://' + feagi_ip_host + ':' + api_data
 
 
 def feagi_api_burst_engine():
     return '/v1/feagi/feagi/burst_engine/stimulation_period'
 
 
 def feagi_api_burst_counter():
@@ -92,23 +69,23 @@
 def feagi_inbound(feagi_inbound_port):
     """
     Return the zmq address of inbound
     """
     return 'tcp://0.0.0.0:' + feagi_inbound_port
 
 
-def feagi_outbound(feagi_ip_host, feagi_opu_port):
+def feagi_outbound(feagi_ip_host, feagi_outbound_port):
     """
     Return the zmq address of outbound
     """
     return 'tcp://' + feagi_ip_host + ':' + \
-           feagi_opu_port
+           feagi_outbound_port
 
 
-def msg_processor(self, msg, msg_type, capabilities):
+def msg_processor(self, msg, msg_type):
     # TODO: give each subclass a specific msg processor method?
     # TODO: add an attribute that explicitly defines message type (instead of parsing topic name)?
     if 'ultrasonic' in msg_type and msg.ranges[1]:
         return {
             msg_type: {
                 idx: val for idx, val in enumerate([msg.ranges[1]])
             }
@@ -117,15 +94,15 @@
         rgb_vals = list(msg.data)
         avg_intensity = sum(rgb_vals) // len(rgb_vals)
 
         sensor_topic = msg_type.split('/')[0]
         sensor_id = int(''.join(filter(str.isdigit, sensor_topic)))
 
         # print("\n***\nAverage Intensity = ", avg_intensity)
-        if avg_intensity > capabilities["infrared"]["threshold"]:
+        if avg_intensity > configuration.capabilities["infrared"]["threshold"]:
             return {
                 'ir': {
                     sensor_id: False
                 }
             }
         else:
             return {
@@ -159,15 +136,15 @@
         message_to_feagi["data"]["sensory_data"]["battery"] = {1: runtime_data["battery_charge_level"] / 100}
     return message_to_feagi, runtime_data["battery_charge_level"]
 
 
 def opu_processor(data):
     try:
         processed_opu_data = {'motor': {}, 'servo': {}, 'battery': {}, 'discharged_battery': {}, 'reset': {},
-                              'camera': {}, 'misc': {}, 'navigation': {}, 'speed': {}, 'servo_position': {}}
+                              'camera': {}, 'misc': {}, 'navigation': {}, 'speed': {}}
         opu_data = data["opu_data"]
         if opu_data is not None:
             if 'o__mot' in opu_data:
                 for data_point in opu_data['o__mot']:
                     data_point = block_to_array(data_point)
                     device_id = data_point[0]
                     device_power = data_point[2]
@@ -214,21 +191,14 @@
             if 'o__spd' in opu_data:
                 if opu_data['o__spd']:
                     for data_point in opu_data['o__spd']:
                         data_point = block_to_array(data_point)
                         device_id = data_point[0]
                         device_power = data_point[2]
                         processed_opu_data['speed'][device_id] = device_power
-            if 'o__pos' in opu_data:
-                if opu_data['o__pos']:
-                    for data_point in opu_data['o__pos']:
-                        data_point = block_to_array(data_point)
-                        device_id = data_point[0]
-                        device_power = data_point[2]
-                        processed_opu_data['servo_position'][device_id] = device_power
             return processed_opu_data
     except Exception:
         # print("error: ", e)
         pass
 
 
 def control_data_processor(data):
@@ -242,7 +212,8 @@
                     float(control_data['robot_starting_position'][position_index][0])
                 configuration.capabilities["position"][position_index]["y"] = \
                     float(control_data['robot_starting_position'][position_index][1])
                 configuration.capabilities["position"][position_index]["z"] = \
                     float(control_data['robot_starting_position'][position_index][2])
         return configuration.capabilities["motor"]["power_coefficient"], \
                configuration.capabilities["position"]
+
```

### Comparing `feagi_agent-0.0.31/setup.cfg` & `feagi_agent-0.0.9/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 [metadata]
 name = feagi_agent
-version = 0.0.31
+version = 0.0.9
 author = Neuraville LLC
-author_email = info@feagi.org
+author_email = info@neuraville.com
 description = Feagi agent to work with general and simulation robots
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/feagi/feagi
+url = https://github.com/feagi/feagi/tree/feature-refactor-vision/agent
 project_urls = 
 	Bug Tracker = https://github.com/feagi/feagi/issues
 classifiers = 
 	Programming Language :: Python :: 3 :: Only
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
-	= .
+	= src
 packages = find:
 python_requires = >=3.6
-install_requires = 
-	requests
-	numpy
-	zmq
-	numpy
-	opencv-python==4.6.0.66; python_version<"3.8"
 
 [options.packages.find]
-where = .
+where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


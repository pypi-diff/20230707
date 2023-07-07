# Comparing `tmp/feagi_agent_freenove-0.0.6.tar.gz` & `tmp/feagi_agent_freenove-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent_freenove-0.0.6.tar", last modified: Thu Apr  6 22:14:45 2023, max compression
+gzip compressed data, was "feagi_agent_freenove-0.0.7.tar", last modified: Fri Jul  7 14:25:14 2023, max compression
```

## Comparing `feagi_agent_freenove-0.0.6.tar` & `feagi_agent_freenove-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-04-06 22:14:45.925010 feagi_agent_freenove-0.0.6/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/LICENSE
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1639 2023-04-06 22:14:45.925010 feagi_agent_freenove-0.0.6/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1089 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/README.md
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-04-06 22:14:45.925010 feagi_agent_freenove-0.0.6/feagi_agent_freenove/
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2332 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/ADC.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     6227 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/Led.py
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2619 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/PCA9685.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/__init__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1394 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/__main__.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2301 2023-04-06 22:07:21.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/configuration.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    25953 2023-04-06 21:39:43.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/controller.py
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       51 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/requirements.txt
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1215 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/setup.sh
--rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1172 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove/verify.sh
-drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-04-06 22:14:45.925010 feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     1639 2023-04-06 22:14:45.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/PKG-INFO
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      607 2023-04-06 22:14:45.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/SOURCES.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-04-06 22:14:45.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/dependency_links.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       85 2023-04-06 22:14:45.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/requires.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       21 2023-04-06 22:14:45.000000 feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/top_level.txt
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-04-06 16:41:12.000000 feagi_agent_freenove-0.0.6/pyproject.toml
--rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      864 2023-04-06 22:14:45.929010 feagi_agent_freenove-0.0.6/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     4824 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/README.md
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/feagi_agent_freenove/
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2332 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/ADC.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     6227 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/Led.py
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2619 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/PCA9685.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2096 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/__main__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2432 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/configuration.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    26148 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/controller.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       51 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/requirements.txt
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1215 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/setup.sh
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     1172 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove/verify.sh
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:25:14.830376 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     5374 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      607 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       85 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/requires.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       21 2023-07-07 14:25:14.000000 feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/top_level.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-07 13:18:01.000000 feagi_agent_freenove-0.0.7/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      864 2023-07-07 14:25:14.834376 feagi_agent_freenove-0.0.7/setup.cfg
```

### Comparing `feagi_agent_freenove-0.0.6/LICENSE` & `feagi_agent_freenove-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/ADC.py` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/ADC.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/Led.py` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/Led.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/PCA9685.py` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/PCA9685.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/configuration.py` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
 # !/usr/bin/env python3
 
 feagi_settings = {
-    "feagi_host": "feagi",
+    # "feagi_auth_url": "http://127.0.0.1:9000/v1/k8/feagi_settings/auth_token",
+    "feagi_url": None,
+    "feagi_dns": None,
+    "feagi_host": "127.0.0.1",
     "feagi_api_port": "8000",
 }
 
 agent_settings = {
-    "agent_data_port": "40014",
+    "agent_data_port": "10004",
     "agent_id": "freenove",
     "agent_type": "embodiment",
     'TTL': 2,
     'last_message': 0,
 }
 
 capabilities = {
```

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/controller.py` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from feagi_agent import feagi_interface as FEAGI
 import RPi.GPIO as GPIO
 from feagi_agent import retina as retina
-import traceback
 import requests
 import sys
 from feagi_agent_freenove.Led import *
 from feagi_agent_freenove.PCA9685 import PCA9685
-from feagi_agent_freenove.configuration import *
 from picamera import PiCamera
 from datetime import datetime
 from collections import deque
 from picamera.array import PiRGBArray
+from time import sleep
 
 runtime_data = {
     "current_burst_id": 0,
     "feagi_state": None,
     "cortical_list": (),
     "battery_charge_level": 1,
     "host_network": {},
@@ -130,15 +129,16 @@
             else:
                 power *= -1
             if device_index not in runtime_data['servo_status']:
                 runtime_data['servo_status'][device_index] = device_index
 
             device_current_position = runtime_data['servo_status'][device_index]
             self.device_position = float((power * feagi_settings['feagi_burst_speed'] /
-                                          capabilities["servo"]["power_amount"]) + device_current_position)
+                                          capabilities["servo"][
+                                              "power_amount"]) + device_current_position)
 
             self.device_position = self.keep_boundaries(device_id=device_index,
                                                         current_position=self.device_position)
 
             runtime_data['servo_status'][device_index] = self.device_position
             # print("device index, position, power = ", device_index, self.device_position, power)
             # self.servo_node[device_index].publish(self.device_position)
@@ -182,28 +182,25 @@
             return -1 * power
         else:
             return abs(power)
 
     @staticmethod
     def motor_converter(motor_id):
         """
-        This will convert from godot to motor's id. Let's say, you have 8x10 (width x depth from static_genome).
-        So, you click 4 to go forward. It will be like this:
-        o__mot': {'1-0-9': 1, '5-0-9': 1, '3-0-9': 1, '7-0-9': 1}
-        which is 1,3,5,7. So this code will convert from 1,3,5,7 to 0,1,2,3 on motor id.
-
-        Since 0-1 is motor 1, 2-3 is motor 2 and so on. In this case, 0 is for forward and 1 is for backward.
-        """
-        # motor_total = capabilities['motor']['count'] #be sure to update your motor total in configuration.py
-        # increment = 0
-        # for motor in range(motor_total):
-        #     if motor_id <= motor + 1:
-        #         print("motor_id: ", motor_id)
-        #         increment += 1
-        #         return increment
+        This will convert from godot to motor's id. Let's say, you have 8x10 (width x depth from
+        static_genome). So, you click 4 to go forward. It will be like this: o__mot': {'1-0-9':
+        1, '5-0-9': 1, '3-0-9': 1, '7-0-9': 1} which is 1,3,5,7. So this code will convert from
+        1,3,5,7 to 0,1,2,3 on motor id.
+
+        Since 0-1 is motor 1, 2-3 is motor 2 and so on. In this case, 0 is for forward and 1 is
+        for backward.
+        """
+        # motor_total = capabilities['motor']['count'] #be sure to update your motor total in
+        # configuration.py increment = 0 for motor in range(motor_total): if motor_id <= motor +
+        # 1: print("motor_id: ", motor_id) increment += 1 return increment
         if motor_id <= 1:
             return 0
         elif motor_id <= 3:
             return 3
         elif motor_id <= 5:
             return 1
         elif motor_id <= 7:
@@ -313,21 +310,17 @@
         This will convert from godot to motor's id. Let's say, you have 8x10 (width x depth from static_genome).
         So, you click 4 to go forward. It will be like this:
         o__mot': {'1-0-9': 1, '5-0-9': 1, '3-0-9': 1, '7-0-9': 1}
         which is 1,3,5,7. So this code will convert from 1,3,5,7 to 0,1,2,3 on motor id.
 
         Since 0-1 is motor 1, 2-3 is motor 2 and so on. In this case, 0 is for forward and 1 is for backward.
         """
-        # motor_total = capabilities['motor']['count'] #be sure to update your motor total in configuration.py
-        # increment = 0
-        # for motor in range(motor_total):
-        #     if motor_id <= motor + 1:
-        #         print("motor_id: ", motor_id)
-        #         increment += 1
-        #         return increment
+        # motor_total = capabilities['motor']['count'] #be sure to update your motor total in
+        # configuration.py increment = 0 for motor in range(motor_total): if motor_id <= motor +
+        # 1: print("motor_id: ", motor_id) increment += 1 return increment
         if motor_id <= 1:
             return 0
         elif motor_id <= 3:
             return 3
         elif motor_id <= 5:
             return 1
         elif motor_id <= 7:
@@ -400,72 +393,71 @@
 # class Battery:
 #     def battery_total(self):
 #         adc = Adc()
 #         Power = adc.recvADC(2) * 3
 #         # print(Power)
 #         return Power
 
-
-def main():
+def main(feagi_auth_url, feagi_settings, agent_settings, capabilities, message_to_feagi, args):
     GPIO.cleanup()
-
-    # # # FEAGI registration # # #
-    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
+    # # # FEAGI registration # # # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+    # - - - - - - - - - - - - - - - - - - #
     print("Connecting to FEAGI resources...")
-
-    feagi_host, api_port, app_data_port = FEAGI.feagi_setting_for_registration(feagi_settings, agent_settings)
-
-    print(feagi_host, api_port, app_data_port)
-
-    # address = 'tcp://' + network_settings['feagi_host'] + ':' + network_settings['feagi_opu_port']
-
-    api_address = 'http://' + feagi_host + ':' + api_port
+    runtime_data["feagi_state"] = FEAGI.feagi_registration(feagi_auth_url=feagi_auth_url,
+                                                           feagi_settings=feagi_settings,
+                                                           agent_settings=agent_settings,
+                                                           capabilities=capabilities)
+    api_address = runtime_data['feagi_state']["feagi_url"]
 
     stimulation_period_endpoint = FEAGI.feagi_api_burst_engine()
     burst_counter_endpoint = FEAGI.feagi_api_burst_counter()
-    print("^ ^ ^")
-    runtime_data["feagi_state"] = FEAGI.feagi_registration(feagi_host=feagi_host,
-                                                           api_port=api_port, agent_settings=agent_settings,
-                                                           capabilities=capabilities)
 
+    # agent_data_port = agent_settings["agent_data_port"]
+    agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
     print("** **", runtime_data["feagi_state"])
     feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
 
     # todo: to obtain this info directly from FEAGI as part of registration
     # ipu_channel_address = FEAGI.feagi_inbound(agent_settings["agent_data_port"])
-    ipu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'],
-                                               agent_settings["agent_data_port"])
+    ipu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
+    # if args['http_type']:
+    #     http = args['http_type']
+    # else:
+    #     http = 'http://'
+    # if args['port_disabled'] == 'true':
+    #     api_address = http + feagi_host
+    # else:
+    #     api_address = http + feagi_host + ':' + api_port
     print("IPU_channel_address=", ipu_channel_address)
     opu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'],
                                                runtime_data["feagi_state"]['feagi_opu_port'])
 
     feagi_ipu_channel = FEAGI.pub_initializer(ipu_channel_address, bind=False)
     feagi_opu_channel = FEAGI.sub_initializer(opu_address=opu_channel_address)
-    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
+    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+    # - - - #
 
-    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
-    #                            Initializer section
+    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+    # - - - # Initializer section
     motor = Motor()
     servo = Servo()
     ir = IR()
     ultrasonic = Ultrasonic()
-    # battery = Battery()
-    # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
+    # battery = Battery() - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+    # - - - - - - - - - - - - - #
 
     flag = False
     keyboard_flag = True
     rolling_window_len = capabilities['motor']['rolling_window_len']
     motor_count = capabilities['motor']['count']
     msg_counter = 0
-    # rpm = (50 * 60) / 2
-    # DC motor has 2 poles, 50 is the freq and it's constant (why??) and 60 is the
-    # seconds of a minute
-    # w = (rpm / 60) * (2 * math.pi)  # 60 is second/minute
-    # velocity = w * (configuration.capabilities['motor']['diameter_of_wheel'] / 2)
-    # ^ diameter is from config and it just needs radius so I turned the diameter into a radius by divide it with 2
+    # rpm = (50 * 60) / 2 DC motor has 2 poles, 50 is the freq and it's constant (why??) and 60
+    # is the seconds of a minute w = (rpm / 60) * (2 * math.pi)  # 60 is second/minute velocity =
+    # w * (configuration.capabilities['motor']['diameter_of_wheel'] / 2) ^ diameter is from
+    # config and it just needs radius so I turned the diameter into a radius by divide it with 2
 
     motor_data = dict()
     rolling_window = {}
     for motor_id in range(motor_count):
         rolling_window[motor_id] = deque([0] * rolling_window_len)
     camera = PiCamera()
     camera.resolution = (640, 480)
@@ -477,26 +469,29 @@
         try:
             for frame in camera.capture_continuous(rawCapture, format="bgr", use_video_port=True):
                 if keyboard_flag:
                     image = frame.array
                     rawCapture.truncate(0)
                     if capabilities['camera']['disabled'] is not True:
                         retina_data = retina.frame_split(image,
-                                                         capabilities['camera']['retina_width_percent'],
-                                                         capabilities['camera']['retina_height_percent'])
+                                                         capabilities['camera'][
+                                                             'retina_width_percent'],
+                                                         capabilities['camera'][
+                                                             'retina_height_percent'])
                         for i in retina_data:
                             if 'C' in i:
-                                retina_data[i] = retina.center_data_compression(retina_data[i],
-                                                                                capabilities['camera'][
-                                                                                    "central_vision_compression"]
-                                                                                )
+                                retina_data[i] = retina.center_data_compression(
+                                    retina_data[i],
+                                    capabilities['camera']["central_vision_compression"]
+                                )
                             else:
-                                retina_data[i] = retina.center_data_compression(retina_data[i],
-                                                                                capabilities['camera']
-                                                                                ['peripheral_vision_compression'])
+                                retina_data[i] = retina. \
+                                    center_data_compression(retina_data[i],
+                                                            capabilities['camera']
+                                                            ['peripheral_vision_compression'])
                         rgb = dict()
                         rgb['camera'] = dict()
                         if previous_data_frame == {}:
                             for i in retina_data:
                                 previous_name = str(i) + "_prev"
                                 previous_data_frame[previous_name] = {}
                         for i in retina_data:
@@ -509,21 +504,24 @@
                                         retina.get_rgb(data,
                                                        capabilities[
                                                            'camera'][
                                                            'central_vision_compression'],
                                                        previous_data_frame[
                                                            previous_name],
                                                        name,
-                                                       capabilities['camera']['deviation_threshold'])
+                                                       capabilities['camera'][
+                                                           'deviation_threshold'])
                                 else:
                                     previous_name = str(i) + "_prev"
                                     rgb_data, previous_data_frame[previous_name] = \
-                                        retina.get_rgb(data, capabilities['camera']['peripheral_vision_compression'],
+                                        retina.get_rgb(data, capabilities['camera'][
+                                            'peripheral_vision_compression'],
                                                        previous_data_frame[previous_name], name,
-                                                       capabilities['camera']['deviation_threshold'])
+                                                       capabilities['camera'][
+                                                           'deviation_threshold'])
                                 for a in rgb_data['camera']:
                                     rgb['camera'][a] = rgb_data['camera'][a]
                     else:
                         rgb = {}
                 ir_data = ir.read()
                 if ir_data:
                     formatted_ir_data = {'ir': {sensor: True for sensor in ir_data}}
@@ -583,26 +581,23 @@
                 message_to_feagi['timestamp'] = datetime.now()
                 message_to_feagi['counter'] = msg_counter
                 feagi_ipu_channel.send(message_to_feagi)
                 message_to_feagi.clear()
                 msg_counter += 1
                 flag += 1
                 if flag == 10:
-                    feagi_burst_speed = requests.get(api_address + stimulation_period_endpoint).json()
+                    feagi_burst_speed = requests.get(
+                        api_address + stimulation_period_endpoint).json()
                     feagi_burst_counter = requests.get(api_address + burst_counter_endpoint).json()
                     flag = 0
                     if msg_counter < feagi_burst_counter:
                         feagi_opu_channel = FEAGI.sub_initializer(opu_address=opu_channel_address)
                         if feagi_burst_speed != feagi_settings['feagi_burst_speed']:
                             feagi_settings['feagi_burst_speed'] = feagi_burst_speed
                 for id in range(motor_count):
                     motor_power = window_average(rolling_window[id])
                     motor_power = motor_power * capabilities["motor"]["power_amount"]
                     motor.move(id, motor_power)
         except KeyboardInterrupt as ke:  # Keyboard error
             motor.stop()
             keyboard_flag = False
             print(ke)
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/setup.sh` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/setup.sh`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove/verify.sh` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove/verify.sh`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/feagi_agent_freenove.egg-info/SOURCES.txt` & `feagi_agent_freenove-0.0.7/feagi_agent_freenove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_agent_freenove-0.0.6/setup.cfg` & `feagi_agent_freenove-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_agent_freenove
-version = 0.0.6
+version = 0.0.7
 author = Neuraville LLC
 author_email = info@feagi.org
 description = Feagi agent freenove to connect feagi with your freenove_smartcar.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```


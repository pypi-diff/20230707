# Comparing `tmp/mavcom-1.1.2.tar.gz` & `tmp/mavcom-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavcom-1.1.2.tar", last modified: Sat May 27 18:39:35 2023, max compression
+gzip compressed data, was "mavcom-1.1.3.tar", last modified: Fri Jul  7 10:48:31 2023, max compression
```

## Comparing `mavcom-1.1.2.tar` & `mavcom-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:39:35.762527 mavcom-1.1.2/
--rw-rw-r--   0 main      (1000) main      (1000)     1066 2023-05-26 21:59:37.000000 mavcom-1.1.2/LICENSE
--rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 18:39:35.762527 mavcom-1.1.2/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      717 2023-05-26 23:18:10.000000 mavcom-1.1.2/README.md
--rw-rw-r--   0 main      (1000) main      (1000)      886 2023-05-27 18:38:45.000000 mavcom-1.1.2/pyproject.toml
--rw-rw-r--   0 main      (1000) main      (1000)       38 2023-05-27 18:39:35.766527 mavcom-1.1.2/setup.cfg
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:39:35.762527 mavcom-1.1.2/src/
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:39:35.762527 mavcom-1.1.2/src/mavcom/
--rw-rw-r--   0 main      (1000) main      (1000)        0 2023-05-26 10:29:36.000000 mavcom-1.1.2/src/mavcom/__init__.py
--rw-rw-r--   0 main      (1000) main      (1000)     1646 2023-05-26 10:10:28.000000 mavcom-1.1.2/src/mavcom/mavconstants.py
--rw-rw-r--   0 main      (1000) main      (1000)    12499 2023-05-27 18:09:22.000000 mavcom-1.1.2/src/mavcom/mavcontrol.py
--rw-rw-r--   0 main      (1000) main      (1000)     4357 2023-05-27 18:38:35.000000 mavcom-1.1.2/src/mavcom/video.py
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:39:35.762527 mavcom-1.1.2/src/mavcom.egg-info/
--rw-rw-r--   0 main      (1000) main      (1000)     2547 2023-05-27 18:39:35.000000 mavcom-1.1.2/src/mavcom.egg-info/PKG-INFO
--rw-rw-r--   0 main      (1000) main      (1000)      354 2023-05-27 18:39:35.000000 mavcom-1.1.2/src/mavcom.egg-info/SOURCES.txt
--rw-rw-r--   0 main      (1000) main      (1000)        1 2023-05-27 18:39:35.000000 mavcom-1.1.2/src/mavcom.egg-info/dependency_links.txt
--rw-rw-r--   0 main      (1000) main      (1000)       52 2023-05-27 18:39:35.000000 mavcom-1.1.2/src/mavcom.egg-info/entry_points.txt
--rw-rw-r--   0 main      (1000) main      (1000)       49 2023-05-27 18:39:35.000000 mavcom-1.1.2/src/mavcom.egg-info/requires.txt
--rw-rw-r--   0 main      (1000) main      (1000)        7 2023-05-27 18:39:35.000000 mavcom-1.1.2/src/mavcom.egg-info/top_level.txt
-drwxrwxr-x   0 main      (1000) main      (1000)        0 2023-05-27 18:39:35.762527 mavcom-1.1.2/tests/
--rw-rw-r--   0 main      (1000) main      (1000)     1208 2023-05-27 18:09:22.000000 mavcom-1.1.2/tests/test_mavcom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 10:48:19.000000 mavcom-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 10:48:31.269582 mavcom-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 10:48:19.000000 mavcom-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 10:48:19.000000 mavcom-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:48:31.269582 mavcom-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.265582 mavcom-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/src/mavcom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/loracon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/mavconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/mavcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/src/mavcom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 10:48:19.000000 mavcom-1.1.3/tests/test_mavcom.py
```

### Comparing `mavcom-1.1.2/LICENSE` & `mavcom-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.2/PKG-INFO` & `mavcom-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/Mavscient/Mavcom
+Project-URL: Homepage, https://github.com/Vefot/Mavcom
 Keywords: mavlink,drone,drones,pymavlink,dronekit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -50,15 +50,15 @@
 This is an example of how to use Mavcom with a simulated vehicle.
 
 Run SITL:
 
 ```sim_vehicle.py -v ArduCopter```
 
 ```python
-from mavcom import mavcom
+from mavcom import mavcontrol
 import time
 
 vehicle = mavcom.Mavcom(
     connection_path = "127.0.0.1:14551",
 )
 
 vehicle.start()
```

### Comparing `mavcom-1.1.2/README.md` & `mavcom-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 This is an example of how to use Mavcom with a simulated vehicle.
 
 Run SITL:
 
 ```sim_vehicle.py -v ArduCopter```
 
 ```python
-from mavcom import mavcom
+from mavcom import mavcontrol
 import time
 
 vehicle = mavcom.Mavcom(
     connection_path = "127.0.0.1:14551",
 )
 
 vehicle.start()
```

### Comparing `mavcom-1.1.2/pyproject.toml` & `mavcom-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mavcom"
-version = "1.1.2"
+version = "1.1.3"
 description = "A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers"
 readme = "README.md"
 authors = [{ name = "Mavscient", email = "mavscient@xee4c.33mail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -21,11 +21,11 @@
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "pip-tools", "pytest"]
 
 [project.urls]
-Homepage = "https://github.com/Mavscient/Mavcom"
+Homepage = "https://github.com/Vefot/Mavcom"
 
 [project.scripts]
 realpython = "reader.__main__:main"
```

### Comparing `mavcom-1.1.2/src/mavcom/mavconstants.py` & `mavcom-1.1.3/src/mavcom/mavconstants.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.2/src/mavcom/mavcontrol.py` & `mavcom-1.1.3/src/mavcom/mavcontrol.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     The primary Mavlink communication and control object. This class connects to the flight controller
     and sends/receives Mavlink messages. Information from required/desired messages is stored and kept up
     to date.
     
     Parameters
     ----------
     
-    `controller`: Object. If you are using an upstream class to utilise the Mavcom control functions, pass
+    - `controller`: Object. If you are using an upstream class to utilise the Mavcom control functions, pass
     this object as "self".
     
-    `required_message_types`: List[string]. If there are any additional Mavlink messages your code needs the data from,
+    - `required_message_types`: List[string]. If there are any additional Mavlink messages your code needs the data from,
     enter them as a list to this parameter.
     
-    `connection_path`: String. This is the path to connect to the Mavlink stream from the flight controller. A typical serial
+    - `connection_path`: String. This is the path to connect to the Mavlink stream from the flight controller. A typical serial
     connection will look like "/dev/ttyS0". A SITL connection will look like "127.0.0.1:14551".
     
-    `baud`: Int. This is the baud rate which the flight controller is using. This must match.
+    - `baud`: Int. This is the baud rate which the flight controller is using. This must match.
     """
 
     def __init__(self,
                  controller: object = None,
                  required_message_types: List[str] = [],
                  connection_path: str = "/dev/ttyS0",
                  baud: int = 921600
@@ -42,28 +42,32 @@
             "GPS_RAW_INT",
             "EKF_STATUS_REPORT",
             "VFR_HUD"
         ]
         self.required_message_types = required_message_types + [m for m in mandatory_message_types if m not in required_message_types]
         self.current_values = defaultdict(lambda: None)
         self.controller = controller
+        has_controller = True if controller else False
         
         self._flight_mode = None
         self._motors_armed = False
         self.airframe = None
         
-        self.telemetry_thread = threading.Thread(target=self._monitor_mavlink_messages, daemon=True)
+        self.telemetry_thread = threading.Thread(target=self._monitor_mavlink_messages, daemon=has_controller)
 
         self.connection = mavutil.mavlink_connection(connection_path, baud=baud)
         self._get_heartbeat()
 
     def start(self) -> None:
         """
         Starts listening to the Mavlink messages from the flight controller. Has a small delay
         so that Mavcom can populate required data types. Call this function first.
+        
+        If a controller object was passed to this Mavcom instance, the telemetry thread will run as a daemon
+        so that it exits when the caller object terminates.
         """
         print("MAVCOM: Mavcom active")
         self.telemetry_thread.start()
         time.sleep(3)
 
     def _get_heartbeat(self):
         print("MAVCOM: Waiting for heartbeat...")
@@ -112,48 +116,48 @@
         Sends a Takeoff command to the flight controller.
         This will only succeed if the `ready` property is `True`
         and the vehicle is armed (`motors_armed == True`)
         
         Parameters
         ----------
         
-        `alt`: Integer. Altitude in meters to takeoff to.
+        - `alt`: Integer. Altitude in meters to takeoff to.
         """
         print(f"MAVCOM: Takeoff to {alt}m relative")
         self.connection.mav.command_long_send(0, 0, mavutil.mavlink.MAV_CMD_NAV_TAKEOFF,
                                                0, 0, 0, 0, 0, 0, 0, alt)
 
     def travel(self, location: tuple[float], alt: int, groundspeed: int = None):
         """
         Sends a go-to waypoint command to the flight controller. Vehicle must be airborne and armed.
         The vehicle will take the altitude as relative to it's starting position, i.e. the altitude of
         the home position is 0.
         
         Parameters
         ----------
         
-        `location`: Tuple[float]. The latitude, longitude to travel to.
+        - `location`: Tuple[float]. The latitude, longitude to travel to.
         
-        `alt': Integer. Altitude AGL to achieve at the destination.
+        - `alt': Integer. Altitude AGL to achieve at the destination.
         
-        `groundspeed`: Integer. Groundspeed in meters per second to travel at.
+        - `groundspeed`: Integer. Groundspeed in meters per second to travel at.
         """
         print(f"MAVCOM: Travel to {location}, {alt}m AGL relative")
         self.connection.mav.mission_item_send(0, 0, 0, mavutil.mavlink.MAV_FRAME_GLOBAL_RELATIVE_ALT,
                                            mavutil.mavlink.MAV_CMD_NAV_WAYPOINT, 2, 0, 0,
                                            0, 0, 0, location[0], location[1],
                                            alt)
         if groundspeed:
             self.set_groundspeed(groundspeed)
 
     def set_groundspeed(self, speed: int):
         """
         Sets the groundspeed the vehicle will travel at.
         
-        `speed`: Integer. Meters per second.
+        - `speed`: Integer. Meters per second.
         """
         self.connection.mav.command_long_encode(
             0, 0,
             mavutil.mavlink.MAV_CMD_DO_CHANGE_SPEED,
             0,
             1, 
             speed,  
@@ -263,22 +267,25 @@
                     return value
         return None
     
     @property
     def nav_state(self):
         """
         The current state of the navigation system.
+
+        Attributes
+        ----------
         
-        `eph`: standard deviation of horizontal position error (meters)
+        - `eph`: standard deviation of horizontal position error (meters)
         
-        `epv`: standard deviation of vertical position error (meters)
+        - `epv`: standard deviation of vertical position error (meters)
         
-        `fix_type`: 0-8 numerical representation of GPS fix type/quality
+        - `fix_type`: 0-8 numerical representation of GPS fix type/quality
         
-        `satellites_visible`: number of satellites currently visible
+        - `satellites_visible`: number of satellites currently visible
         """
         if "GPS_RAW_INT" not in self.current_values:
             return "GPS not initialised"
         navdata = {
             "eph": self.current_values['GPS_RAW_INT']['eph'],
             "epv": self.current_values['GPS_RAW_INT']['epv'],
             "fix_type": self.current_values['GPS_RAW_INT']['fix_type'],
@@ -286,26 +293,29 @@
         }
         return NavState(navdata['eph'], navdata['epv'], navdata['fix_type'], navdata['satellites_visible'])
     
     @property
     def vehicle_state(self):
         """
         The current travel state of the vehicle.
+
+        Attributes
+        ----------
         
-        `alt`: altitude AGL relative to home position
+        - `alt`: altitude AGL relative to home position
         
-        `groundspeed`: groundspeed in m/s
+        - `groundspeed`: groundspeed in m/s
 
-        `vertical_speed`: ascend/descend speed in m/s
+        - `vertical_speed`: ascend/descend speed in m/s
 
-        `heading`: heading in degrees
+        - `heading`: heading in degrees
 
-        `lat`: latitude in decimal format
+        - `lat`: latitude in decimal format
 
-        `lon`: longitude in decimal format
+        - `lon`: longitude in decimal format
         """
         alt = self.current_values['GLOBAL_POSITION_INT']['relative_alt'] / 1000
         groundspeed = self.current_values["VFR_HUD"]['groundspeed']
         vertical_speed = self.current_values['VFR_HUD']['climb']
         heading = self.current_values['GLOBAL_POSITION_INT']['hdg']
         lat = self.current_values['GLOBAL_POSITION_INT']['lat'] / 1e7
         lon = self.current_values['GLOBAL_POSITION_INT']['lon'] / 1e7
```

### Comparing `mavcom-1.1.2/src/mavcom/video.py` & `mavcom-1.1.3/src/mavcom/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,50 +7,50 @@
 class Recorder():
     """
     Object that controls recording of onboard video. 
     
     Parameters
     ----------
     
-    `controller`: This should be the upstream class that instantiates the Recorder instance. By passing itself to
-    the Recorder instance, the Recorder can access its attributes.
+    - `controller`: This should be the upstream Mavcom instance of whatever object or script is controlling the vehicle. 
+    By passing itself to the Recorder instance, the Recorder can access its attributes.
     
-    `top_text`: text that will be overlaid on this position of the video capture.
+    - `top_text`: text that will be overlaid on this position of the video capture.
     
-    `centre_text`: text that will be overlaid on this position of the video capture.
+    - `centre_text`: text that will be overlaid on this position of the video capture.
     
-    `bottom_text`: text that will be overlaid on this position of the video capture.
+    - `bottom_text`: text that will be overlaid on this position of the video capture.
     
-    `filename`: OPTIONAL - the desired filename. If none is set, it will create a folder 'recordings'
+    - `filename`: OPTIONAL - the desired filename. If none is set, it will create a folder 'recordings'
     in the directory the program was started in and save recordings as `[hostname]-n` where 'n' is the n number of recordings in
     the folder plus 1.
     
-    `show_video`: boolean True or False, only really for testing; shows the video output on-screen.
+    - `show_video`: boolean True or False, only really for testing; shows the video output on-screen.
     """
     
     def __init__(self, controller: object = None, top_text = None, centre_text = None, bottom_text = None, filename=None, show_video=False) -> None:
         self.top_text = top_text
         self.centre_text = centre_text
         self.bottom_text = bottom_text
         self.video_active = False
         self.show = show_video
         self.controller = controller
         
         
         self.recording = threading.Thread(target=self.record, daemon=True)
-        self.hud_update_thread = threading.Thread(target=self.hud_updater, daemon=True)
+        self.hud_updates = threading.Thread(target=self.hud_updater, daemon=True)
         
         os.makedirs("recordings", exist_ok=True)
         if filename is None:
             self.filename = f"{socket.gethostname()}-{len(os.listdir('recordings'))}"
         print(self.filename)
         
     def record(self) -> None:
         """
-        Start recording video.
+        Start recording video. Start by calling `start()` on recording thread.
         """
         self.video_active = True
         font_scale = 2
         font = cv2.FONT_HERSHEY_PLAIN
 
         camera = cv2.VideoCapture(-1)
         width = camera.get(3)
@@ -87,26 +87,29 @@
     def video_mod(self, text_pos: str, text_content: str) -> None:
         """
         Edit the text overlay of the video.
         
         Parameters
         ----------
         
-        text_pos: the position of the text to modify/overlay. Options:
-        `top_text`
-        `centre_text`
-        `bottom_text`
+        - `text_pos`: the position of the text to modify/overlay. Options:
         
-        text_content: the content to put into this position
+            - `top_text`
+            
+            - `centre_text`
+            - `bottom_text`
+        
+        - `text_content`: the content to put into this position
         """
         setattr(self, text_pos, text_content)
         
     def hud_updater(self) -> None:
         """
         Continually updates the top text overlay of the video with name, alt and speed information.
+        Start by calling `start()` on hud_updates thread.
         """
         while self.video_active:
             try:
                 alt = self.controller.vehicle_state.alt
                 speed = self.controller.vehicle_state.groundspeed
                 self.video_mod("top_text", f"{socket.gethostname()} Alt: {alt} Speed: {speed}")
             except Exception as e:
```

### Comparing `mavcom-1.1.2/src/mavcom.egg-info/PKG-INFO` & `mavcom-1.1.3/src/mavcom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,15 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/Mavscient/Mavcom
+Project-URL: Homepage, https://github.com/Vefot/Mavcom
 Keywords: mavlink,drone,drones,pymavlink,dronekit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -50,15 +50,15 @@
 This is an example of how to use Mavcom with a simulated vehicle.
 
 Run SITL:
 
 ```sim_vehicle.py -v ArduCopter```
 
 ```python
-from mavcom import mavcom
+from mavcom import mavcontrol
 import time
 
 vehicle = mavcom.Mavcom(
     connection_path = "127.0.0.1:14551",
 )
 
 vehicle.start()
```

### Comparing `mavcom-1.1.2/tests/test_mavcom.py` & `mavcom-1.1.3/tests/test_mavcom.py`

 * *Files identical despite different names*


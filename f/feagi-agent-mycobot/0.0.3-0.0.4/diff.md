# Comparing `tmp/feagi_agent_mycobot-0.0.3.tar.gz` & `tmp/feagi_agent_mycobot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_agent_mycobot-0.0.3.tar", last modified: Thu Mar 23 21:56:33 2023, max compression
+gzip compressed data, was "feagi_agent_mycobot-0.0.4.tar", last modified: Fri Jul  7 14:26:20 2023, max compression
```

## Comparing `feagi_agent_mycobot-0.0.3.tar` & `feagi_agent_mycobot-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:56:33.962839 feagi_agent_mycobot-0.0.3/
--rw-r--r--   0 station1   (501) staff       (20)    11344 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/LICENSE
--rw-r--r--   0 station1   (501) staff       (20)     3119 2023-03-23 21:56:33.962903 feagi_agent_mycobot-0.0.3/PKG-INFO
--rw-r--r--   0 station1   (501) staff       (20)     2574 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/README.md
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:56:33.961259 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/
--rw-r--r--   0 station1   (501) staff       (20)      516 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/CMakeLists.txt
--rw-r--r--   0 station1   (501) staff       (20)        0 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/__init__.py
--rw-r--r--   0 station1   (501) staff       (20)     2235 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/__main__.py
--rw-r--r--   0 station1   (501) staff       (20)      876 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/package.xml
--rw-r--r--   0 station1   (501) staff       (20)       83 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/setup.cfg
--rw-r--r--   0 station1   (501) staff       (20)      667 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/setup.py
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:56:33.961794 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/src/
--rw-r--r--   0 station1   (501) staff       (20)        0 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/src/__init__.py
--rwxr-xr-x   0 station1   (501) staff       (20)     1973 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/src/configuration.py
--rwxr-xr-x   0 station1   (501) staff       (20)    19202 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/src/mycobot.py
--rwxr-xr-x   0 station1   (501) staff       (20)      157 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/start_mycobot.sh
-drwxr-xr-x   0 station1   (501) staff       (20)        0 2023-03-23 21:56:33.962746 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/
--rw-r--r--   0 station1   (501) staff       (20)     3119 2023-03-23 21:56:33.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/PKG-INFO
--rw-r--r--   0 station1   (501) staff       (20)      615 2023-03-23 21:56:33.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/SOURCES.txt
--rw-r--r--   0 station1   (501) staff       (20)        1 2023-03-23 21:56:33.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/dependency_links.txt
--rw-r--r--   0 station1   (501) staff       (20)       50 2023-03-23 21:56:33.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/requires.txt
--rw-r--r--   0 station1   (501) staff       (20)       20 2023-03-23 21:56:33.000000 feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/top_level.txt
--rw-r--r--   0 station1   (501) staff       (20)       99 2023-03-23 21:48:00.000000 feagi_agent_mycobot-0.0.3/pyproject.toml
--rw-r--r--   0 station1   (501) staff       (20)      847 2023-03-23 21:56:33.963287 feagi_agent_mycobot-0.0.3/setup.cfg
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:26:20.375032 feagi_agent_mycobot-0.0.4/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)    11344 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/LICENSE
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     3119 2023-07-07 14:26:20.375032 feagi_agent_mycobot-0.0.4/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2574 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/README.md
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:26:20.371032 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      516 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/CMakeLists.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/__init__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     2235 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/__main__.py
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      876 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/package.xml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       83 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/setup.cfg
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      667 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/setup.py
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:26:20.371032 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/src/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/src/__init__.py
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)     2104 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/src/configuration.py
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)    19444 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/src/mycobot.py
+-rwxrwxr-x   0 bwuk      (1000) bwuk      (1000)      157 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/start_mycobot.sh
+drwxrwxr-x   0 bwuk      (1000) bwuk      (1000)        0 2023-07-07 14:26:20.375032 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)     3119 2023-07-07 14:26:20.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/PKG-INFO
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      615 2023-07-07 14:26:20.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/SOURCES.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)        1 2023-07-07 14:26:20.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/dependency_links.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       50 2023-07-07 14:26:20.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/requires.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       20 2023-07-07 14:26:20.000000 feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/top_level.txt
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)       99 2023-07-07 13:18:01.000000 feagi_agent_mycobot-0.0.4/pyproject.toml
+-rw-rw-r--   0 bwuk      (1000) bwuk      (1000)      847 2023-07-07 14:26:20.375032 feagi_agent_mycobot-0.0.4/setup.cfg
```

### Comparing `feagi_agent_mycobot-0.0.3/LICENSE` & `feagi_agent_mycobot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/PKG-INFO` & `feagi_agent_mycobot-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_agent_mycobot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Feagi agent mycobot to connect feagi with your cobot arm
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@neuraville.com
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_mycobot-0.0.3/README.md` & `feagi_agent_mycobot-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/CMakeLists.txt` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/__main__.py` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/__main__.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/package.xml` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/package.xml`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/setup.py` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/setup.py`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/src/configuration.py` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/src/configuration.py`

 * *Files 6% similar despite different names*

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
-    "agent_data_port": "40012",
+    "agent_data_port": "10005",
     "agent_id": "mycobot",
     "agent_type": "embodiment",
     'TTL': 2,
     'last_message': 0,
 }
 
 capabilities = {
```

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot/src/mycobot.py` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot/src/mycobot.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,29 +269,38 @@
 mycobot.initialize(capabilities['servo']['count'])
 for i in range(1, capabilities['servo']['count'], 1):
     runtime_data['actual_encoder_position'][i] = deque([0, 0, 0, 0, 0])
 global_arm['0'].set_speed(100)
 
 # # # FEAGI registration # # #
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
-feagi_host, api_port, app_data_port = FEAGI.feagi_setting_for_registration(feagi_settings, agent_settings)
-runtime_data["feagi_state"] = FEAGI.feagi_registration(feagi_host=feagi_host,
-                                                       api_port=api_port,
+feagi_auth_url = feagi_settings.pop('feagi_auth_url', None)
+print("FEAGI AUTH URL ------- ", feagi_auth_url)
+print("Connecting to FEAGI resources...")
+runtime_data["feagi_state"] = FEAGI.feagi_registration(feagi_auth_url=feagi_auth_url,
+                                                       feagi_settings=feagi_settings,
                                                        agent_settings=agent_settings,
                                                        capabilities=capabilities)
-ipu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'],
-                                           agent_settings["agent_data_port"])
+api_address = runtime_data['feagi_state']["feagi_url"]
+
+stimulation_period_endpoint = FEAGI.feagi_api_burst_engine()
+burst_counter_endpoint = FEAGI.feagi_api_burst_counter()
+
+# agent_data_port = agent_settings["agent_data_port"]
+agent_data_port = str(runtime_data["feagi_state"]['agent_state']['agent_data_port'])
+print("** **", runtime_data["feagi_state"])
+feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
+
+ipu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'], agent_data_port)
+print("IPU_channel_address=", ipu_channel_address)
 opu_channel_address = FEAGI.feagi_outbound(feagi_settings['feagi_host'],
                                            runtime_data["feagi_state"]['feagi_opu_port'])
 feagi_ipu_channel = FEAGI.pub_initializer(ipu_channel_address, bind=False)
 feagi_opu_channel = FEAGI.sub_initializer(opu_address=opu_channel_address)
-api_address = 'http://' + feagi_host + ':' + api_port
-stimulation_period_endpoint = FEAGI.feagi_api_burst_engine()
-burst_counter_endpoint = FEAGI.feagi_api_burst_counter()
-feagi_settings['feagi_burst_speed'] = float(runtime_data["feagi_state"]['burst_duration'])
+
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - #
 
 # Camera section
 # camera = PiCamera()
 # camera = cv2.VideoCapture('/dev/video2')
 # camera.resolution = (640, 480)
```

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/PKG-INFO` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi-agent-mycobot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Feagi agent mycobot to connect feagi with your cobot arm
 Home-page: https://github.com/feagi/feagi
 Author: Neuraville LLC
 Author-email: info@neuraville.com
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_agent_mycobot-0.0.3/feagi_agent_mycobot.egg-info/SOURCES.txt` & `feagi_agent_mycobot-0.0.4/feagi_agent_mycobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_agent_mycobot-0.0.3/setup.cfg` & `feagi_agent_mycobot-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_agent_mycobot
-version = 0.0.3
+version = 0.0.4
 author = Neuraville LLC
 author_email = info@neuraville.com
 description = Feagi agent mycobot to connect feagi with your cobot arm
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi
 project_urls =
```


# Comparing `tmp/vocalhost-1.0.7.tar.gz` & `tmp/vocalhost-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalhost-1.0.7.tar", last modified: Wed Jun 28 11:43:02 2023, max compression
+gzip compressed data, was "vocalhost-1.0.8.tar", last modified: Fri Jul  7 17:33:20 2023, max compression
```

## Comparing `vocalhost-1.0.7.tar` & `vocalhost-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:43:02.586866 vocalhost-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-28 11:43:02.586866 vocalhost-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-28 11:42:48.000000 vocalhost-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 11:43:02.586866 vocalhost-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-28 11:42:48.000000 vocalhost-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:43:02.586866 vocalhost-1.0.7/vocalhost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-28 11:43:02.000000 vocalhost-1.0.7/vocalhost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 11:43:02.000000 vocalhost-1.0.7/vocalhost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:43:02.000000 vocalhost-1.0.7/vocalhost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-28 11:43:02.000000 vocalhost-1.0.7/vocalhost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-28 11:43:02.000000 vocalhost-1.0.7/vocalhost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-28 11:42:48.000000 vocalhost-1.0.7/vocalhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:33:20.272684 vocalhost-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 17:33:20.272684 vocalhost-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-07 17:33:08.000000 vocalhost-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:33:20.272684 vocalhost-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 17:33:08.000000 vocalhost-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:33:20.272684 vocalhost-1.0.8/vocalhost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-07 17:33:08.000000 vocalhost-1.0.8/vocalhost.py
```

### Comparing `vocalhost-1.0.7/PKG-INFO` & `vocalhost-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.0.7
+Version: 1.0.8
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.0.7/README.md` & `vocalhost-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vocalhost-1.0.7/vocalhost.egg-info/PKG-INFO` & `vocalhost-1.0.8/vocalhost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.0.7
+Version: 1.0.8
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.0.7/vocalhost.py` & `vocalhost-1.0.8/vocalhost.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 import asyncio
 import websockets
 import ssl
 import uuid
 import certifi
 import requests
 
+API_KEY = None
+process_message = None
+
 class Receiver:
     def _generate_unique_id():
         return str(uuid.uuid4())
 
-    def __init__(self, process_message, client_id, API_KEY):
+    def __init__(self):
         self.websocket = None
-        self.client_id = client_id if client_id else Receiver._generate_unique_id()
         self.received_message = None
-        self.process_message = process_message
-        self.API_KEY = API_KEY
 
-    async def receive_message(self):
+    async def receive_message():
         while True:
-            received_message = await self.websocket.recv()
-            response = self.process_message(received_message)
-            await self.websocket.send(response)
+            received_message = await Receiver.websocket.recv()
+            response = process_message(received_message)
+            await Receiver.websocket.send(response)
 
-    async def _connect_to_server(self):
+    async def _connect_to_server(client_id=None):
         ssl_context = ssl.create_default_context(cafile=certifi.where())
         ssl_context.verify_mode = ssl.CERT_REQUIRED
         remote_url = 'wss://vocalhost.reiserx.com/'
 
         try:
-            async with websockets.connect(remote_url+'ws/?client_id=' + self.client_id + '&api_key='+self.API_KEY, ssl=ssl_context) as websocket:
-                print("Connected: " + self.client_id)
-                self.websocket = websocket
-                await self.receive_message()
+            async with websockets.connect(remote_url+'ws/?client_id=' + client_id + '&api_key='+API_KEY, ssl=ssl_context) as websocket:
+                print("Connected: " + client_id)
+                Receiver.websocket = websocket
+                await Receiver.receive_message()
 
         except websockets.ConnectionClosedError as e:
             print(f"Connection closed: {e}")
             # Handle connection closure, if needed
-
-        except Exception as e:
-            print(f"Error occurred: {e}")
             
-    def connect(self):
-        asyncio.run(self._connect_to_server())
+    def connect(client_id=None):
+        asyncio.run(Receiver._connect_to_server(client_id=client_id))
 
 
 class Request:
-    def __init__(self, api_key):
-        self.api_key = api_key
-
-    def send(self, message, receiver_id, timeout=60):
+    def send(message, receiver_id, timeout=60):
         receiver_id = str(receiver_id)
-        self.url = 'https://vocalhost.reiserx.com/connect/'+ receiver_id +'/'
+        url = 'https://vocalhost.reiserx.com/connect/'+ receiver_id +'/'
         data = {
             'message': message
         }
         
-        self.headers = {
+        headers = {
             'Timeout': str(timeout),
-            'Authorization': self.api_key
+            'Authorization': API_KEY
         }
         
-        response = requests.post(self.url, headers=self.headers, json=data)
+        response = requests.post(url, headers=headers, json=data)
         return response
```


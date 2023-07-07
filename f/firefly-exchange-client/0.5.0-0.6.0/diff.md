# Comparing `tmp/firefly_exchange_client-0.5.0.tar.gz` & `tmp/firefly_exchange_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.5.0.tar", last modified: Mon Jun 26 19:22:21 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.6.0.tar", last modified: Fri Jul  7 10:05:53 2023, max compression
```

## Comparing `firefly_exchange_client-0.5.0.tar` & `firefly_exchange_client-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.585265 firefly_exchange_client-0.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    37470 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-26 19:22:12.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:21.589265 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 19:22:21.000000 firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:05:53.238887 firefly_exchange_client-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-07 10:05:53.238887 firefly_exchange_client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:05:53.238887 firefly_exchange_client-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:05:53.234887 firefly_exchange_client-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:05:53.234887 firefly_exchange_client-0.6.0/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37470 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-07 10:05:43.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:05:53.238887 firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-07 10:05:53.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 10:05:53.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:05:53.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-07 10:05:53.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-07 10:05:53.000000 firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.5.0/LICENSE` & `firefly_exchange_client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/PKG-INFO` & `firefly_exchange_client-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly_exchange_client
-Version: 0.5.0
+Version: 0.6.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.5.0/README.md` & `firefly_exchange_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/pyproject.toml` & `firefly_exchange_client-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.5.0"
+version = "0.6.0"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/api_service.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/constants.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/enumerations.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/interfaces.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/sockets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import socketio
+import time
 from .enumerations import MARKET_SYMBOLS, SOCKET_EVENTS
-
+import asyncio
 sio = socketio.Client()
 
 
 class Sockets:
     callbacks = {}
 
     def __init__(self, url, timeout=10, token=None) -> None:
@@ -69,14 +70,32 @@
             elif "default" in Sockets.callbacks.keys():
                 Sockets.callbacks["default"]({"event": event, "data": data})
             else:
                 pass
         except:
             pass
         return
+        
+    @sio.event
+    def connect():
+        print("Connected To Socket Server")
+        # add 10 seconds sleep to allow connection to be established before callbacks for connections are executed
+        if 'connect' in Sockets.callbacks:
+            # Execute the callback using asyncio.run() if available
+            time.sleep(10)
+            asyncio.run(Sockets.callbacks['connect']())
+        
+
+    @sio.event
+    def disconnect():
+        print('Disconnected From Socket Server')
+        if 'disconnect' in Sockets.callbacks:
+            # Execute the callback using asyncio.run() if available
+            asyncio.run(Sockets.callbacks['disconnect']())
+
 
     async def listen(self, event, callback):
         """
             Assigns callbacks to desired events
         """
         Sockets.callbacks[event] = callback
         return
```

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client/websocket_client.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firefly-exchange-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `firefly_exchange_client-0.5.0/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.6.0/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


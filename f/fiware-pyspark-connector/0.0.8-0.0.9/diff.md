# Comparing `tmp/fiware_pyspark_connector-0.0.8.tar.gz` & `tmp/fiware_pyspark_connector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiware_pyspark_connector-0.0.8.tar", last modified: Wed Jun 21 10:37:36 2023, max compression
+gzip compressed data, was "fiware_pyspark_connector-0.0.9.tar", last modified: Tue Jul  4 12:17:05 2023, max compression
```

## Comparing `fiware_pyspark_connector-0.0.8.tar` & `fiware_pyspark_connector-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 10:37:36.494695 fiware_pyspark_connector-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-21 10:37:36.490695 fiware_pyspark_connector-0.0.8/FPC/
--rw-rw-rw-   0        0        0        0 2023-06-21 07:44:47.000000 fiware_pyspark_connector-0.0.8/FPC/__init__.py
--rw-rw-rw-   0        0        0    15652 2023-06-21 09:17:50.000000 fiware_pyspark_connector-0.0.8/FPC/connector.py
--rw-rw-rw-   0        0        0     2858 2023-06-21 07:33:02.000000 fiware_pyspark_connector-0.0.8/FPC/connectorconf.py
--rw-rw-rw-   0        0        0     7653 2023-06-21 10:32:29.000000 fiware_pyspark_connector-0.0.8/FPC/subscribing_tool.py
--rw-rw-rw-   0        0        0    34500 2023-06-21 07:33:56.000000 fiware_pyspark_connector-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     6777 2023-06-21 10:37:36.494695 fiware_pyspark_connector-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6207 2023-06-21 07:33:53.000000 fiware_pyspark_connector-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 10:37:36.493694 fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/
--rw-rw-rw-   0        0        0     6777 2023-06-21 10:37:36.000000 fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2023-06-21 10:37:36.000000 fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 10:37:36.000000 fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-21 10:37:36.000000 fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-21 10:37:36.000000 fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-06-21 07:54:36.000000 fiware_pyspark_connector-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      709 2023-06-21 10:37:36.494695 fiware_pyspark_connector-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-04 12:17:05.787202 fiware_pyspark_connector-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-07-04 12:17:05.781904 fiware_pyspark_connector-0.0.9/FPC/
+-rw-rw-rw-   0        0        0        0 2023-06-21 07:44:47.000000 fiware_pyspark_connector-0.0.9/FPC/__init__.py
+-rw-rw-rw-   0        0        0    15485 2023-07-04 12:14:28.000000 fiware_pyspark_connector-0.0.9/FPC/connector.py
+-rw-rw-rw-   0        0        0     2649 2023-07-04 10:58:09.000000 fiware_pyspark_connector-0.0.9/FPC/connectorconf.py
+-rw-rw-rw-   0        0        0     7581 2023-07-04 12:15:17.000000 fiware_pyspark_connector-0.0.9/FPC/subscribing_tool.py
+-rw-rw-rw-   0        0        0    34500 2023-06-21 07:33:56.000000 fiware_pyspark_connector-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     6777 2023-07-04 12:17:05.787202 fiware_pyspark_connector-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6207 2023-06-21 07:33:53.000000 fiware_pyspark_connector-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 12:17:05.786228 fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/
+-rw-rw-rw-   0        0        0     6777 2023-07-04 12:17:05.000000 fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-07-04 12:17:05.000000 fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 12:17:05.000000 fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-04 12:17:05.000000 fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-04 12:17:05.000000 fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-06-21 07:54:36.000000 fiware_pyspark_connector-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      709 2023-07-04 12:17:05.788175 fiware_pyspark_connector-0.0.9/setup.cfg
```

### Comparing `fiware_pyspark_connector-0.0.8/FPC/connector.py` & `fiware_pyspark_connector-0.0.9/FPC/connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pyspark import SparkContext, SparkConf
 from pyspark.streaming import StreamingContext
 from pyspark.storagelevel import StorageLevel
 from typing import Union, Tuple, List, Type, Any
 from threading import Thread
 from datetime import datetime
 
-from FPC.connectorconf import *
+from fpc.connectorconf import *
 
 
 
 ### RECEIVER-SIDE FUNCTIONS ###
 
 def parse_context(api_json: dict) -> Tuple[str, bool]:
     '''
@@ -311,26 +311,28 @@
             s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             s.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
             s.bind(socket_address)
             break
         except OSError as e:
             configuration.socket_port += 1
         except Exception as e:
-            exit()
+            print(e)
+            exit(1)
     print(f"Started Multi-Thread socket servet at: {socket_address}")
 
     while True:
         try:
             server_address = (configuration.http_address, configuration.http_port)
             httpd = HTTPServer(server_address, OrionPysparkRequestHandler)
             break
         except OSError as e:
             configuration.http_port += 1
         except Exception as e:
-            exit()
+            print(e)
+            exit(1)
     print(f"Bound HTTP endpoint at: {server_address}")
 
     threadserver = ServerThread(httpd)
     threadserver.start()
 
     threadsocket = SocketThread(s, socket_address, threadserver)
     threadsocket.start()
@@ -402,50 +404,48 @@
         else:
             raise ValueError("Method not allowed")
         return reply.text
     except Exception as e:
         return e
                 
         
-def ReplyToBroker(values: Any, api_url: str = REPL_SINGLETON.api_url, api_method: str = REPL_SINGLETON.api_method) -> str:
+def ReplyToBroker(values: Any, api_url: str, api_method: str) -> str:
     '''
     Function for structured and complex requests, using the 'BLUEPRINTFILE' specified in the
     configuration file and replacing values using the 'PLACEHOLDER' string.
     Values MUST be in the same order of the replacing strings.
     Builds the request on-the-fly and send it to the context broker
     '''
     message = replaceJSON(values)
     return sendRequest(message, api_url, api_method)
     
     
-def SemistructuredReplyToBroker(values: Any, body: str, api_url: str = REPL_SINGLETON.api_url, api_method: str = REPL_SINGLETON.api_method) -> str:
+def SemistructuredReplyToBroker(values: Any, body: str, api_url: str, api_method: str) -> str:
     '''
     Function for averagely complex requests, passing an encoded request body and some values
     that have to be replaced in body when the 'PLACEHOLDER' string is encountered.
     Values MUST be in the same order of the replacing strings.
     Builds the request on-the-fly and send it to the context broker.
     '''
     values = listify(values)
     for v in values:
         body = body.replace(REPL_SINGLETON.placeholder_string, str(v), 1)
         
     return sendRequest(body, api_url, api_method)
    
     
-def UnstructuredReplyToBroker(body: str, api_url: str = REPL_SINGLETON.api_url, api_method: str = REPL_SINGLETON.api_method) -> str:
+def UnstructuredReplyToBroker(body: str, api_url: str, api_method: str) -> str:
     '''
     Function for simple and short requests, passing directly the request body.
     No correctness is ensured by the connector, so every character has to be checked by the user.
     Sends the passed message to the context broker.
     '''
     return sendRequest(body, api_url, api_method)
 
 
-def Test():
-    print(RECV_SINGLETON.http_address)
 
     
 
 
 
 
     
@@ -463,8 +463,7 @@
     
     
     
     
     
 	
 
-
```

### Comparing `fiware_pyspark_connector-0.0.8/FPC/connectorconf.py` & `fiware_pyspark_connector-0.0.9/FPC/connectorconf.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,17 +36,14 @@
     def __new__(cls) :
         
         if not cls._instance:
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self):
-        # Context Broker API to send back data
-        self.api_url = "http://localhost:1026/v2/entities/urn:ngsi-ld:Product:010/attrs/price/"
-        self.api_method = "PUT" #Choose among POST, PUT or PATCH
         # Context broker service and subservice
         self.fiware_service = "opcua_car"
         self.fiware_servicepath = "/demo"
         # Content Type of the request
         self.content_type = "application/json; charset=utf-8"
         # Advanced configuration for more complex requests 
         self.blueprint_file = "Test.txt"
@@ -95,8 +92,8 @@
 
 class NGSIEventv2():
     
     def __init__(self, timestamp, svc, svcpath, entities):
         self.creationtime = timestamp
         self.service = svc
         self.servicePath = svcpath
-        self.entities = entities
+        self.entities = entities
```

### Comparing `fiware_pyspark_connector-0.0.8/FPC/subscribing_tool.py` & `fiware_pyspark_connector-0.0.9/FPC/subscribing_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 import requests
 import json
 
-from FPC.connectorconf import NGSIAttribute, NGSIEntityv2, NGSIEntityLD, RECV_SINGLETON, REPL_SINGLETON
+from fpc.connectorconf import *
 import sys
 
 
 
 def ReturnEntityIfExists(ent):
 
     isLD = False
```

### Comparing `fiware_pyspark_connector-0.0.8/LICENSE.txt` & `fiware_pyspark_connector-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.8/PKG-INFO` & `fiware_pyspark_connector-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiware_pyspark_connector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Connects FIWARE Context Brokers with fiware_pyspark_connector
 Home-page: https://github.com/Engineering-Research-and-Development/fiware-orion-pyspark-connector
 Author: Emilio Cimino
 Author-email: emilio.cimino@outlook.it
 License: "AGPL-3.0-only"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fiware_pyspark_connector-0.0.8/README.md` & `fiware_pyspark_connector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fiware_pyspark_connector-0.0.8/fiware_pyspark_connector.egg-info/PKG-INFO` & `fiware_pyspark_connector-0.0.9/fiware_pyspark_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiware-pyspark-connector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Connects FIWARE Context Brokers with fiware_pyspark_connector
 Home-page: https://github.com/Engineering-Research-and-Development/fiware-orion-pyspark-connector
 Author: Emilio Cimino
 Author-email: emilio.cimino@outlook.it
 License: "AGPL-3.0-only"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `fiware_pyspark_connector-0.0.8/setup.cfg` & `fiware_pyspark_connector-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 6977 6172 655f 7079 7370 6172   = fiware_pyspar
 00000020: 6b5f 636f 6e6e 6563 746f 720d 0a76 6572  k_connector..ver
-00000030: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000030: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000040: 7468 6f72 203d 2045 6d69 6c69 6f20 4369  thor = Emilio Ci
 00000050: 6d69 6e6f 0d0a 6175 7468 6f72 5f65 6d61  mino..author_ema
 00000060: 696c 203d 2065 6d69 6c69 6f2e 6369 6d69  il = emilio.cimi
 00000070: 6e6f 406f 7574 6c6f 6f6b 2e69 740d 0a64  no@outlook.it..d
 00000080: 6573 6372 6970 7469 6f6e 203d 2043 6f6e  escription = Con
 00000090: 6e65 6374 7320 4649 5741 5245 2043 6f6e  nects FIWARE Con
 000000a0: 7465 7874 2042 726f 6b65 7273 2077 6974  text Brokers wit
```


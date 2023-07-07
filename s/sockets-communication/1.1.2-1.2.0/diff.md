# Comparing `tmp/sockets-communication-1.1.2.tar.gz` & `tmp/sockets-communication-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-1.1.2.tar", last modified: Mon Jul  3 14:36:19 2023, max compression
+gzip compressed data, was "sockets-communication-1.2.0.tar", last modified: Fri Jul  7 15:17:58 2023, max compression
```

## Comparing `sockets-communication-1.1.2.tar` & `sockets-communication-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 14:36:19.015408 sockets-communication-1.1.2/
--rw-rw-rw-   0        0        0       98 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-07-03 14:36:19.015408 sockets-communication-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.1.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.1.2/build.py
--rw-rw-rw-   0        0        0      708 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.1.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 14:36:19.015408 sockets-communication-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-07-03 14:36:07.000000 sockets-communication-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:36:18.999371 sockets-communication-1.1.2/sockets_communication/
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.1.2/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.1.2/sockets_communication/process.py
--rw-rw-rw-   0        0        0     3614 2023-07-03 14:35:41.000000 sockets-communication-1.1.2/sockets_communication/service.py
--rw-rw-rw-   0        0        0    20172 2023-07-03 14:36:00.000000 sockets-communication-1.1.2/sockets_communication/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-03 14:36:19.014370 sockets-communication-1.1.2/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-03 14:36:18.000000 sockets-communication-1.1.2/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 15:17:58.502296 sockets-communication-1.2.0/
+-rw-rw-rw-   0        0        0       98 2023-07-07 15:17:58.000000 sockets-communication-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-07-07 15:17:58.502296 sockets-communication-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-1.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 sockets-communication-1.2.0/build.py
+-rw-rw-rw-   0        0        0      708 2023-07-07 15:09:04.000000 sockets-communication-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       53 2023-06-28 17:44:26.000000 sockets-communication-1.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 15:17:58.502296 sockets-communication-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-07-07 15:09:00.000000 sockets-communication-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:17:58.496296 sockets-communication-1.2.0/sockets_communication/
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-1.2.0/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-1.2.0/sockets_communication/process.py
+-rw-rw-rw-   0        0        0     7797 2023-07-07 15:10:32.000000 sockets-communication-1.2.0/sockets_communication/service.py
+-rw-rw-rw-   0        0        0    20255 2023-07-07 15:17:20.000000 sockets-communication-1.2.0/sockets_communication/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-07 15:17:58.501297 sockets-communication-1.2.0/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-07-07 15:17:58.000000 sockets-communication-1.2.0/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-07-07 15:17:58.000000 sockets-communication-1.2.0/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 15:17:58.000000 sockets-communication-1.2.0/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-07 15:17:58.000000 sockets-communication-1.2.0/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-07 15:17:58.000000 sockets-communication-1.2.0/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-1.1.2/PKG-INFO` & `sockets-communication-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.1.2
+Version: 1.2.0
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-1.1.2/README.md` & `sockets-communication-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.2/build.py` & `sockets-communication-1.2.0/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.2/pyproject.toml` & `sockets-communication-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '1.1.2'
+version = '1.2.0'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-1.1.2/setup.py` & `sockets-communication-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='1.1.2',
+        version='1.2.0',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-1.1.2/sockets_communication/exceptions.py` & `sockets-communication-1.2.0/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.2/sockets_communication/process.py` & `sockets-communication-1.2.0/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-1.1.2/sockets_communication/sockets.py` & `sockets-communication-1.2.0/sockets_communication/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 __all__ = [
     "Components",
     "Communication",
     "SocketClient",
     "SocketServer",
     "ClientsCollection",
     "bluetooth_socket_request",
-    "bluetooth_socket_client"
+    "bluetooth_socket"
 ]
 
 Socket = socket.socket
 Host = str
 Port = Union[str, int]
 Address = Tuple[Host, Port]
 Number = Union[int, float]
@@ -171,25 +171,21 @@
     # end receive
 # end Communication
 
 @represent
 class SocketClient(Communication):
     """Creates the client to communicate with the server."""
 
-    def __init__(self, connection: Socket) -> None:
-        """
-        Defines the server address and creates the client object.
+    def __init__(self) -> None:
+        """Defines the server address and creates the client object."""
 
-        :param connection: The connection socket.
-        """
+        self.connection: Optional[socket.socket] = None
 
-        self.connection = connection
-
-        self.host = None
-        self.port = None
+        self.host: Optional[str] = None
+        self.port: Optional[int] = None
     # end __init__
 
     def send(self, message: bytes, connection: Optional[Socket] = None) -> None:
         """
         Sends a message to the client or server by its connection.
 
         :param message: The message to send to the client.
@@ -215,22 +211,25 @@
         if connection is None:
             connection = self.connection
         # end if
 
         return super().receive(connection=connection)
     # end receive
 
-    def connect(self, host: Host, port: Port) -> None:
+    def connect(self, connection: Socket, host: Host, port: Port) -> None:
         """
         Creates the sockets' connection for the client object with the server.
 
+        :param connection: The connection socket.
         :param host: The ip address of the server.
         :param port: The port for the server connection.
         """
 
+        self.connection = connection
+
         self.host = host
         self.port = port
 
         self.connection.connect((self.host, self.port))
     # end connect
 
     def send_message_to_server(self, message: bytes) -> None:
@@ -561,15 +560,17 @@
 
         self.run(**self._run_parameters)
     # end run
 
     def stop_serving(self) -> None:
         """Stops the serving process."""
 
-        self._serving = False
+        if self.serving:
+            self._serving = False
+        # end if
 
         if self.created and self._listening_process.is_alive():
             self._listening_process = None
         # end if
     # end stop_serving
 
     def terminate(self) -> None:
@@ -657,28 +658,26 @@
         :param address: The tuple of the ip address and the port of the connection
         """
 
         self.clients.remove_client(address)
     # end remove_client
 # end SocketServer
 
-def bluetooth_socket_client() -> SocketClient:
+def bluetooth_socket() -> socket:
     """
     Sends a request through the bluetooth sockets.
 
     :return: The client object..
     """
 
-    connection = socket.socket(
+    return socket.socket(
         socket.AF_BLUETOOTH, socket.SOCK_STREAM,
         socket.BTPROTO_RFCOMM
     )
-
-    return SocketClient(connection=connection)
-# end bluetooth_socket_client
+# end bluetooth_socket
 
 def bluetooth_socket_request(
         host: Host,
         port: Port,
         endpoint: Optional[str] = None,
         parameters: Optional[Dict[str, Any]] = None
 ) -> Any:
@@ -689,17 +688,19 @@
     :param endpoint: The path to the endpoint.
     :param port: The sending port.
     :param parameters: The request parameters.
 
     :return: The returned value.
     """
 
-    client = bluetooth_socket_client()
+    client = SocketClient()
+
+    connection = bluetooth_socket()
 
-    client.connect(host=host, port=port)
+    client.connect(connection=connection, host=host, port=port)
 
     req = PreparedRequest()
     # noinspection HttpUrlsUsage
     req.prepare_url(
         f"http://{host}:{port}/{endpoint or ''}",
         parameters or {}
     )
```

### Comparing `sockets-communication-1.1.2/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-1.2.0/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 1.1.2
+Version: 1.2.0
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```


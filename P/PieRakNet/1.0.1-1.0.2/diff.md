# Comparing `tmp/PieRakNet-1.0.1.tar.gz` & `tmp/PieRakNet-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PieRakNet-1.0.1.tar", last modified: Thu Jul  6 10:53:37 2023, max compression
+gzip compressed data, was "PieRakNet-1.0.2.tar", last modified: Thu Jul  6 11:38:35 2023, max compression
```

## Comparing `PieRakNet-1.0.1.tar` & `PieRakNet-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 10:53:37.049191 PieRakNet-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      985 2023-07-06 10:53:37.047192 PieRakNet-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 10:53:36.836336 PieRakNet-1.0.1/PieRakNet.egg-info/
--rw-rw-rw-   0        0        0      985 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 10:53:35.000000 PieRakNet-1.0.1/PieRakNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 10:53:37.034465 PieRakNet-1.0.1/pieraknet/
--rw-rw-rw-   0        0        0       89 2023-07-06 08:27:19.000000 PieRakNet-1.0.1/pieraknet/__init__.py
--rw-rw-rw-   0        0        0     4988 2023-07-06 07:52:28.000000 PieRakNet-1.0.1/pieraknet/buffer.py
--rw-rw-rw-   0        0        0     9947 2023-07-06 10:40:18.000000 PieRakNet-1.0.1/pieraknet/connection.py
--rw-rw-rw-   0        0        0      608 2023-07-06 10:03:10.000000 PieRakNet-1.0.1/pieraknet/protocol_info.py
--rw-rw-rw-   0        0        0     3869 2023-07-06 10:48:10.000000 PieRakNet-1.0.1/pieraknet/server.py
--rw-rw-rw-   0        0        0       42 2023-07-06 10:53:37.050189 PieRakNet-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-07-06 10:48:10.000000 PieRakNet-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:38:35.527612 PieRakNet-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      985 2023-07-06 11:38:35.524620 PieRakNet-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 11:38:35.171715 PieRakNet-1.0.2/PieRakNet.egg-info/
+-rw-rw-rw-   0        0        0      985 2023-07-06 11:38:33.000000 PieRakNet-1.0.2/PieRakNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-06 11:38:33.000000 PieRakNet-1.0.2/PieRakNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 11:38:33.000000 PieRakNet-1.0.2/PieRakNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 11:38:33.000000 PieRakNet-1.0.2/PieRakNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 11:38:35.519636 PieRakNet-1.0.2/pieraknet/
+-rw-rw-rw-   0        0        0       89 2023-07-06 08:27:19.000000 PieRakNet-1.0.2/pieraknet/__init__.py
+-rw-rw-rw-   0        0        0     4988 2023-07-06 07:52:28.000000 PieRakNet-1.0.2/pieraknet/buffer.py
+-rw-rw-rw-   0        0        0    10384 2023-07-06 11:36:48.000000 PieRakNet-1.0.2/pieraknet/connection.py
+-rw-rw-rw-   0        0        0      608 2023-07-06 10:03:10.000000 PieRakNet-1.0.2/pieraknet/protocol_info.py
+-rw-rw-rw-   0        0        0     3869 2023-07-06 10:48:10.000000 PieRakNet-1.0.2/pieraknet/server.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 11:38:35.527612 PieRakNet-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-07-06 11:36:47.000000 PieRakNet-1.0.2/setup.py
```

### Comparing `PieRakNet-1.0.1/LICENSE` & `PieRakNet-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.1/PKG-INFO` & `PieRakNet-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.1
+Version: 1.0.2
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: nikitagavrilin005@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.1/PieRakNet.egg-info/PKG-INFO` & `PieRakNet-1.0.2/PieRakNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PieRakNet
-Version: 1.0.1
+Version: 1.0.2
 Summary: RakNet implementation, written in Python. Created for PieMC.
 Home-page: https://github.com/PieMC-Dev/PieRakNet
 Author: lapismyt
 Author-email: nikitagavrilin005@gmail.com
 Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
 Project-URL: Developer, https://github.com/PieMC-Dev
 Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
```

### Comparing `PieRakNet-1.0.1/pieraknet/buffer.py` & `PieRakNet-1.0.2/pieraknet/buffer.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.1/pieraknet/connection.py` & `PieRakNet-1.0.2/pieraknet/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pieraknet.packets.frame_set import FrameSet, Frame
 from pieraknet.protocol_info import ProtocolInfo
 from pieraknet.packets.acknowledgement import Ack, Nack
 from pieraknet.handlers.connection_request import ConnectionRequestHandler
 from pieraknet.handlers.online_ping import OnlinePingHandler
 from pieraknet.packets.online_ping import OnlinePing
 from pieraknet.packets.new_incoming_connection import NewIncomingConnection
+from pieraknet.packets.disconnect import Disconnect
 
 
 class Connection:
     def __init__(self, address, server, mtu_size, guid):
         self.address = address
         self.mtu_size = mtu_size
         self.server = server
@@ -125,18 +126,22 @@
             elif packet.body[0] == ProtocolInfo.ONLINE_PING:
                 new_frame = Frame()
                 new_frame.reliability = 0
                 new_frame.body = OnlinePingHandler.handle(OnlinePing(packet.body), self, self.server)
                 self.add_to_queue(new_frame, False)
             elif packet.body[0] == ProtocolInfo.DISCONNECT:
                 self.disconnect()
+            elif packet.body[0] == ProtocolInfo.GAME_PACKET:
+                if hasattr(self.server, "interface"):
+                    if hasattr(self.server.interface, "on_game_packet"):
+                        self.server.interface.on_game_packet(packet, self)
             else:
                 if hasattr(self.server, "interface"):
-                    if hasattr(self.server.interface, "on_frame"):
-                        self.server.interface.on_frame(packet, self)
+                    if hasattr(self.server.interface, "on_unknown_packet"):
+                        self.server.interface.on_unknown_packet(packet, self)
 
     def send_queue(self):
         if len(self.queue.frames) > 0:
             self.queue.sequence_number = self.server_sequence_number
             self.server_sequence_number += 1
             self.recovery_queue[self.queue.sequence_number] = self.queue
             self.queue.encode()
@@ -204,13 +209,15 @@
             self.nack_queue = []
             packet.encode()
             self.send_data(packet.getvalue())
 
     def disconnect(self):
         new_frame = Frame()
         new_frame.reliability = 0
-        new_frame.body = b"\x15"
+        disconnect_packet = Disconnect()
+        disconnect_packet.encode()
+        new_frame.body = disconnect_packet.getvalue()
         self.add_to_queue(new_frame)
         self.server.remove_connection(self.address)
         if hasattr(self.server, "interface"):
             if hasattr(self.server.interface, "on_disconnect"):
                 self.server.interface.on_disconnect(self)
```

### Comparing `PieRakNet-1.0.1/pieraknet/protocol_info.py` & `PieRakNet-1.0.2/pieraknet/protocol_info.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.1/pieraknet/server.py` & `PieRakNet-1.0.2/pieraknet/server.py`

 * *Files identical despite different names*

### Comparing `PieRakNet-1.0.1/setup.py` & `PieRakNet-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='PieRakNet',
-    version='1.0.1',
+    version='1.0.2',
     author='lapismyt',
     author_email='nikitagavrilin005@gmail.com',
     description='RakNet implementation, written in Python. Created for PieMC.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/PieMC-Dev/PieRakNet',
     packages=find_packages(),
```


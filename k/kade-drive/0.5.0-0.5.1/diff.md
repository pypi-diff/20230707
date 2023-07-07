# Comparing `tmp/kade_drive-0.5.0.tar.gz` & `tmp/kade_drive-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kade_drive-0.5.0.tar", max compression
+gzip compressed data, was "kade_drive-0.5.1.tar", max compression
```

## Comparing `kade_drive-0.5.0.tar` & `kade_drive-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.5.0/LICENSE
--rw-r--r--   0        0        0      391 2023-07-05 21:17:07.160141 kade_drive-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.5.0/kade_drive/__init__.py
--rw-r--r--   0        0        0     1424 2023-07-06 00:47:02.809455 kade_drive-0.5.0/kade_drive/cli.py
--rw-r--r--   0        0        0     7392 2023-07-06 00:47:02.809455 kade_drive-0.5.0/kade_drive/client.py
--rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.5.0/kade_drive/core/__init__.py
--rw-r--r--   0        0        0      130 2023-07-06 00:47:02.809455 kade_drive-0.5.0/kade_drive/core/config.py
--rw-r--r--   0        0        0     9533 2023-07-06 00:47:02.809455 kade_drive-0.5.0/kade_drive/core/crawling.py
--rw-r--r--   0        0        0    18641 2023-07-06 00:47:02.809455 kade_drive-0.5.0/kade_drive/core/network.py
--rw-r--r--   0        0        0     3916 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/core/node.py
--rw-r--r--   0        0        0     7846 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/core/protocol.py
--rw-r--r--   0        0        0     8680 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/core/routing.py
--rw-r--r--   0        0        0     8928 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/core/storage.py
--rw-r--r--   0        0        0     1486 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 21:17:07.162141 kade_drive-0.5.0/kade_drive/message_system/__init__.py
--rw-r--r--   0        0        0     6617 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/message_system/message_system.py
--rw-r--r--   0        0        0     2619 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/server.py
--rw-r--r--   0        0        0      702 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/test_store_file.py
--rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.5.0/kade_drive/tests/__init__.py
--rw-r--r--   0        0        0     1698 2023-07-06 00:27:01.589732 kade_drive-0.5.0/kade_drive/tests/conftest.py
--rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.5.0/kade_drive/tests/data_to_split.txt
--rw-r--r--   0        0        0     1785 2023-07-06 00:26:57.630729 kade_drive-0.5.0/kade_drive/tests/test_node.py
--rw-r--r--   0        0        0     4631 2023-07-06 00:47:02.810454 kade_drive-0.5.0/kade_drive/tests/test_routing.py
--rw-r--r--   0        0        0        1 2023-07-06 00:26:51.787726 kade_drive-0.5.0/kade_drive/tests/test_server.py
--rw-r--r--   0        0        0      757 2023-07-06 00:47:02.811454 kade_drive-0.5.0/kade_drive/tests/test_splitdata.py
--rw-r--r--   0        0        0     1459 2023-07-06 00:47:02.811454 kade_drive-0.5.0/kade_drive/tests/test_storage.py
--rw-r--r--   0        0        0      716 2023-07-06 00:47:02.811454 kade_drive-0.5.0/kade_drive/tests/test_utils.py
--rw-r--r--   0        0        0      508 2023-07-06 00:47:24.220656 kade_drive-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 kade_drive-0.5.0/setup.py
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 kade_drive-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.5.1/LICENSE
+-rw-r--r--   0        0        0      778 2023-07-06 05:54:09.008851 kade_drive-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.5.1/kade_drive/__init__.py
+-rw-r--r--   0        0        0     1426 2023-07-06 05:42:11.364669 kade_drive-0.5.1/kade_drive/cli.py
+-rw-r--r--   0        0        0     7392 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/client.py
+-rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.5.1/kade_drive/core/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/core/config.py
+-rw-r--r--   0        0        0     9533 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/core/crawling.py
+-rw-r--r--   0        0        0    18641 2023-07-06 00:47:02.809455 kade_drive-0.5.1/kade_drive/core/network.py
+-rw-r--r--   0        0        0     3916 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/node.py
+-rw-r--r--   0        0        0     7846 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/protocol.py
+-rw-r--r--   0        0        0     8680 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/routing.py
+-rw-r--r--   0        0        0     8928 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/storage.py
+-rw-r--r--   0        0        0     1486 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:07.162141 kade_drive-0.5.1/kade_drive/message_system/__init__.py
+-rw-r--r--   0        0        0     6617 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/message_system/message_system.py
+-rw-r--r--   0        0        0     2619 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/server.py
+-rw-r--r--   0        0        0      702 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/test_store_file.py
+-rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.5.1/kade_drive/tests/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-06 00:27:01.589732 kade_drive-0.5.1/kade_drive/tests/conftest.py
+-rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.5.1/kade_drive/tests/data_to_split.txt
+-rw-r--r--   0        0        0     1785 2023-07-06 00:26:57.630729 kade_drive-0.5.1/kade_drive/tests/test_node.py
+-rw-r--r--   0        0        0     4631 2023-07-06 00:47:02.810454 kade_drive-0.5.1/kade_drive/tests/test_routing.py
+-rw-r--r--   0        0        0        1 2023-07-06 00:26:51.787726 kade_drive-0.5.1/kade_drive/tests/test_server.py
+-rw-r--r--   0        0        0      757 2023-07-06 00:47:02.811454 kade_drive-0.5.1/kade_drive/tests/test_splitdata.py
+-rw-r--r--   0        0        0     1459 2023-07-06 00:47:02.811454 kade_drive-0.5.1/kade_drive/tests/test_storage.py
+-rw-r--r--   0        0        0      716 2023-07-06 00:47:02.811454 kade_drive-0.5.1/kade_drive/tests/test_utils.py
+-rw-r--r--   0        0        0      515 2023-07-07 06:01:44.822501 kade_drive-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 kade_drive-0.5.1/setup.py
+-rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 kade_drive-0.5.1/PKG-INFO
```

### Comparing `kade_drive-0.5.0/LICENSE` & `kade_drive-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/cli.py` & `kade_drive-0.5.1/kade_drive/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 import sys
 from client import ClientSession
 
 client_session: ClientSession | None = None
 
+
+
 if __name__ == "__main__":
     ip = None
     port = 8086
 
     if len(sys.argv) == 2:
         ip = sys.argv[1]
```

### Comparing `kade_drive-0.5.0/kade_drive/client.py` & `kade_drive-0.5.1/kade_drive/client.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/crawling.py` & `kade_drive-0.5.1/kade_drive/core/crawling.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/network.py` & `kade_drive-0.5.1/kade_drive/core/network.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/node.py` & `kade_drive-0.5.1/kade_drive/core/node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/protocol.py` & `kade_drive-0.5.1/kade_drive/core/protocol.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/routing.py` & `kade_drive-0.5.1/kade_drive/core/routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/storage.py` & `kade_drive-0.5.1/kade_drive/core/storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/core/utils.py` & `kade_drive-0.5.1/kade_drive/core/utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/message_system/message_system.py` & `kade_drive-0.5.1/kade_drive/message_system/message_system.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/server.py` & `kade_drive-0.5.1/kade_drive/server.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/test_store_file.py` & `kade_drive-0.5.1/kade_drive/test_store_file.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/conftest.py` & `kade_drive-0.5.1/kade_drive/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/data_to_split.txt` & `kade_drive-0.5.1/kade_drive/tests/data_to_split.txt`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/test_node.py` & `kade_drive-0.5.1/kade_drive/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/test_routing.py` & `kade_drive-0.5.1/kade_drive/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/test_splitdata.py` & `kade_drive-0.5.1/kade_drive/tests/test_splitdata.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/test_storage.py` & `kade_drive-0.5.1/kade_drive/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/kade_drive/tests/test_utils.py` & `kade_drive-0.5.1/kade_drive/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.5.0/setup.py` & `kade_drive-0.5.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces==0.11.0', 'rpyc==5.3.1', 'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'kade-drive',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'distributed file system based on kademlia dht',
-    'long_description': 'Distributed file system based on <https://github.com/bmuller/kademlia>\n\n\n## Basic Usage\n\n- Clone the repo and run poetry install\n- Run server.py in one pc or several pc in a local network\n- Run cli.py in any pc of the network and start playing with the system\n\n## Installation\n\n- pip install kade-drive\n  \n### Tests\n\nTo run tests make shure that there is at least one server in the network.\n',
+    'long_description': 'Distributed file system based on <https://github.com/bmuller/kademlia> for the final project of distributed systems\n\n## Basic Usage\n\n- Clone the repo and run poetry install\n- Run server.py in one pc or several pc in a local network\n- Run cli.py in any pc of the network and start playing with the system\n\n## Installation\n\n```console\n- pip install kade-drive\n```\n\n## Server\n\n```Python\nfrom kade_drive.server import start_server\n\nstart_server()\n```\n\n## Client\n\n### Note: Make shure that there exist at least a server in the local network\n\n```Python\nfrom kade_drive.cli import ClientSession\n\nclient = ClientSession()\nclient.connect()\nclient.put(4, 5)\nvalue = client.get(4)\nassert value == 5\n```\n\n### Tests\n\nTo run tests make shure that there is at least one server in the network.\n',
     'author': 'DanielUH2019',
     'author_email': 'danielcardenascabrera2016@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.10,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `kade_drive-0.5.0/PKG-INFO` & `kade_drive-0.5.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,57 @@
 Metadata-Version: 2.1
 Name: kade-drive
-Version: 0.5.0
+Version: 0.5.1
 Summary: distributed file system based on kademlia dht
 License: MIT
 Author: DanielUH2019
 Author-email: danielcardenascabrera2016@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: netifaces (==0.11.0)
 Requires-Dist: rpyc (==5.3.1)
 Requires-Dist: typer (==0.9.0)
 Description-Content-Type: text/markdown
 
-Distributed file system based on <https://github.com/bmuller/kademlia>
-
+Distributed file system based on <https://github.com/bmuller/kademlia> for the final project of distributed systems
 
 ## Basic Usage
 
 - Clone the repo and run poetry install
 - Run server.py in one pc or several pc in a local network
 - Run cli.py in any pc of the network and start playing with the system
 
 ## Installation
 
+```console
 - pip install kade-drive
-  
+```
+
+## Server
+
+```Python
+from kade_drive.server import start_server
+
+start_server()
+```
+
+## Client
+
+### Note: Make shure that there exist at least a server in the local network
+
+```Python
+from kade_drive.cli import ClientSession
+
+client = ClientSession()
+client.connect()
+client.put(4, 5)
+value = client.get(4)
+assert value == 5
+```
+
 ### Tests
 
 To run tests make shure that there is at least one server in the network.
```


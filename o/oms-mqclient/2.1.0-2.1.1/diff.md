# Comparing `tmp/oms-mqclient-2.1.0.tar.gz` & `tmp/oms-mqclient-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.1.0.tar", last modified: Tue Apr 25 16:27:16 2023, max compression
+gzip compressed data, was "oms-mqclient-2.1.1.tar", last modified: Thu Jul  6 22:28:21 2023, max compression
```

## Comparing `oms-mqclient-2.1.0.tar` & `oms-mqclient-2.1.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2674 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/mqclient/
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5808 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12421 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    12342 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15483 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    22378 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1118 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-25 16:27:16.000000 oms-mqclient-2.1.0/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2725 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.368254 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7026 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    33482 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    18702 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:27:16.372254 oms-mqclient-2.1.0/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-04-25 16:27:13.000000 oms-mqclient-2.1.0/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.795826 oms-mqclient-2.1.1/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-06 22:28:19.000000 oms-mqclient-2.1.1/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5808 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.795826 oms-mqclient-2.1.1/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12421 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    12368 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    15483 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    22595 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-06 22:28:21.000000 oms-mqclient-2.1.1/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.795826 oms-mqclient-2.1.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    33482 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    18702 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.799826 oms-mqclient-2.1.1/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:28:21.803827 oms-mqclient-2.1.1/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-07-06 22:28:18.000000 oms-mqclient-2.1.1/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.1.0/LICENSE` & `oms-mqclient-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/PKG-INFO` & `oms-mqclient-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.1.0/README.md` & `oms-mqclient-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/mqclient/__init__.py` & `oms-mqclient-2.1.1/mqclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Public init."""
 
+
 from .queue import Queue
 
 __all__ = ["Queue"]
 
+
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.1.0/mqclient/broker_client_interface.py` & `oms-mqclient-2.1.1/mqclient/broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/mqclient/broker_client_manager.py` & `oms-mqclient-2.1.1/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.1.1/mqclient/broker_clients/apachepulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/mqclient/broker_clients/nats.py` & `oms-mqclient-2.1.1/mqclient/broker_clients/nats.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         self.js: Optional[nats.js.JetStreamContext] = None
 
         LOGGER.debug(f"Stream & Subject: {stream_id}/{self.subject}")
 
     async def connect(self) -> None:
         """Set up connection and channel."""
         await super().connect()
-        self._nats_client = await nats.connect(self.endpoint)
+        self._nats_client = await nats.connect(self.endpoint)  # type: ignore[arg-type]
         # Create JetStream context
         self.js = self._nats_client.jetstream(timeout=TIMEOUT_MILLIS_DEFAULT // 1000)
         await self.js.add_stream(name=self.stream_id, subjects=[self.subject])
 
     async def close(self) -> None:
         """Close connection."""
         await super().close()
```

### Comparing `oms-mqclient-2.1.0/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.1.1/mqclient/broker_clients/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/mqclient/log_msgs.py` & `oms-mqclient-2.1.1/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/mqclient/queue.py` & `oms-mqclient-2.1.1/mqclient/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Queue class encapsulating a pub-sub messaging system."""
 
 import contextlib
 import logging
+import os
 import sys
 import types
 import uuid
 from typing import (
     Any,
     AsyncGenerator,
     AsyncIterator,
@@ -19,14 +20,20 @@
 from . import broker_client_manager
 from . import telemetry as wtt
 from .broker_client_interface import AckException, Message, NackException, Pub, Sub
 
 LOGGER = logging.getLogger("mqclient")
 
 
+# deprecation check
+for envvar in ["RABBITMQ_HEARTBEAT", "PULSAR_UNACKED_MESSAGES_TIMEOUT_SEC"]:
+    if os.getenv(envvar):
+        raise RuntimeError(f"Environment variable {envvar} has been deprecated.")
+
+
 def _message_size_message(msg: Message) -> str:
     return (
         f"{sys.getsizeof(msg.payload)} bytes "
         f"(data={sys.getsizeof(msg.data)}, headers={sys.getsizeof(msg.headers)}) "
         f"[msg_id={msg.msg_id!r}]"
     )
```

### Comparing `oms-mqclient-2.1.0/mqclient/telemetry.py` & `oms-mqclient-2.1.1/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.1.1/oms_mqclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.1.0
+Version: 2.1.1
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.1.0/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.1.1/oms_mqclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 mqclient/__init__.py
 mqclient/broker_client_interface.py
 mqclient/broker_client_manager.py
-mqclient/config.py
 mqclient/log_msgs.py
 mqclient/py.typed
 mqclient/queue.py
 mqclient/telemetry.py
 mqclient/broker_clients/__init__.py
 mqclient/broker_clients/apachepulsar.py
 mqclient/broker_clients/nats.py
```

### Comparing `oms-mqclient-2.1.0/setup.cfg` & `oms-mqclient-2.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 [options.extras_require]
 all = 
 	%(pulsar)s
 	%(rabbitmq)s
 	%(nats)s
 pulsar = 
-	pulsar-client
+	pulsar-client<3.2.0
 rabbitmq = 
 	pika
 nats = 
 	nats-py[nkeys]
 telemetry = 
 	wipac-telemetry
 dev =
```

### Comparing `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.1.1/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/integrate/conftest.py` & `oms-mqclient-2.1.1/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/integrate/test_nats.py` & `oms-mqclient-2.1.1/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/integrate/test_pulsar.py` & `oms-mqclient-2.1.1/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.1.1/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.1.1/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.1.0/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.1.1/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*


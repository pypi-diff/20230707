# Comparing `tmp/cmem_plugin_kafka-1.3.1rc1.tar.gz` & `tmp/cmem_plugin_kafka-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kafka-1.3.1rc1.tar", max compression
+gzip compressed data, was "cmem_plugin_kafka-1.4.0rc1.tar", max compression
```

## Comparing `cmem_plugin_kafka-1.3.1rc1.tar` & `cmem_plugin_kafka-1.4.0rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11334 2023-06-26 06:54:32.897262 cmem_plugin_kafka-1.3.1rc1/LICENSE
--rw-r--r--   0        0        0     3733 2023-06-26 06:54:32.897262 cmem_plugin_kafka-1.3.1rc1/README-public.md
--rw-r--r--   0        0        0        0 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/__init__.py
--rw-r--r--   0        0        0     4331 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/constants.py
--rw-r--r--   0        0        0    14787 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/kafka_handlers.py
--rw-r--r--   0        0        0    12053 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/utils.py
--rw-r--r--   0        0        0        0 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/__init__.py
--rw-r--r--   0        0        0    11646 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/consumer.py
--rw-r--r--   0        0        0     9739 2023-06-26 06:54:32.901262 cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/producer.py
--rw-r--r--   0        0        0     2242 2023-06-26 06:54:59.489295 cmem_plugin_kafka-1.3.1rc1/pyproject.toml
--rw-r--r--   0        0        0     4843 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.3.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     3733 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/README-public.md
+-rw-r--r--   0        0        0        0 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/__init__.py
+-rw-r--r--   0        0        0     4331 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/constants.py
+-rw-r--r--   0        0        0    14406 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/kafka_handlers.py
+-rw-r--r--   0        0        0    12410 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/utils.py
+-rw-r--r--   0        0        0        0 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/workflow/__init__.py
+-rw-r--r--   0        0        0    11673 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/workflow/consumer.py
+-rw-r--r--   0        0        0     9739 2023-07-07 09:26:34.009262 cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/workflow/producer.py
+-rw-r--r--   0        0        0     2242 2023-07-07 09:27:06.141319 cmem_plugin_kafka-1.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4843 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.4.0rc1/PKG-INFO
```

### Comparing `cmem_plugin_kafka-1.3.1rc1/LICENSE` & `cmem_plugin_kafka-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.1rc1/README-public.md` & `cmem_plugin_kafka-1.4.0rc1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/constants.py` & `cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/constants.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/kafka_handlers.py` & `cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/kafka_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 The `kafka_handlers` module provides a base class `KafkaDataHandler` for producing
 messages from data to/from a Kafka topic.
 """
+import hashlib
 import json
 import re
 from abc import ABC
+from datetime import datetime
 from typing import Any, Sequence, Optional
 from xml.sax.saxutils import escape  # nosec B406
 
 import defusedxml.ElementTree as ET
 import json_stream
 import json_stream.requests
 from cmem_plugin_base.dataintegration.context import ExecutionContext, ExecutionReport
@@ -358,58 +360,53 @@
             for i, path in enumerate(paths):
                 values[path.path] = list(entity.values[i])
             result["entity"] = {"uri": entity.uri, "values": values}
             kafka_payload = json.dumps(result, indent=4)
             yield KafkaMessage(key=None, value=kafka_payload)
 
     def _aggregate_data(self):
-        try:
-            schema = self.get_schema()
-            if not schema:
-                return None
-            entities = self.get_entities()
-            return Entities(entities=entities, schema=schema)
-        except (KeyError, json.decoder.JSONDecodeError) as ex:
-            raise ValueError("Kafka Message is not in expected format") from ex
+        schema = self.get_schema()
+        entities = self.get_entities()
+        return Entities(entities=entities, schema=schema)
 
     def get_schema(self):
         """Return kafka message schema paths"""
-        message = self._kafka_consumer.get_first_message()
-        if not message:
-            return None
-        json_payload = json.loads(message.value)
-        schema_paths = []
-        self._log.info(f'values : {json_payload["entity"]["values"]}')
-        for path in self._get_paths(json_payload["entity"]["values"]):
-            path_uri = f"{path}"
-            schema_paths.append(EntityPath(path=path_uri))
+        schema_paths = [
+            EntityPath(path='key'),
+            EntityPath(path='content'),
+            EntityPath(path='offset'),
+            EntityPath(path='ts-production'),
+            EntityPath(path='ts-consumption'),
+        ]
         self._schema = EntitySchema(
-            type_uri=json_payload["schema"]["type_uri"],
+            type_uri="https://github.com/eccenca/cmem-plugin-kafka#PlainMessage",
             paths=schema_paths,
         )
         return self._schema
 
     def _get_paths(self, values: dict):
         self._log.info(f"_get_paths: Values dict {values}")
         return list(values.keys())
 
     def get_entities(self):
         """Generate the entities from kafka messages"""
-        if self._kafka_consumer.get_first_message():
-            yield self._get_entity(self._kafka_consumer.get_first_message())
 
         for message in self._kafka_consumer.poll():
             yield self._get_entity(message)
 
         self._kafka_consumer.commit()
+        self._kafka_consumer.close()
 
-    def _get_entity(self, message: KafkaMessage):
-        try:
-            json_payload = json.loads(message.value)
-        except json.decoder.JSONDecodeError as exc:
-            raise ValueError("Kafka message in not in valid JSON format") from exc
-
-        entity_uri = json_payload["entity"]["uri"]
+    @staticmethod
+    def _get_entity(message: KafkaMessage):
+        sha256 = hashlib.sha256(
+            message.key.encode() if message.key else "".encode()
+        ).hexdigest()
+        entity_uri = f"urn:hash::sha256:{sha256}"
         values = [
-            json_payload["entity"]["values"].get(_.path) for _ in self._schema.paths
+            [message.key],
+            [message.value],
+            [f"{message.offset}"],
+            [f"{message.timestamp}"],
+            [f"{int(round(datetime.now().timestamp() * 1000))}"]
         ]
         return Entity(uri=entity_uri, values=values)
```

### Comparing `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/utils.py` & `cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,19 +39,26 @@
     key : str
         Kafka message key
     value : str
         Kafka message payload
     """
 
     def __init__(
-        self, key: Optional[str] = None, headers: Optional[dict] = None, value: str = ""
+            self,
+            key: Optional[str] = None,
+            headers: Optional[dict] = None,
+            value: str = "",
+            offset: Optional[int] = None,
+            timestamp: Optional[int] = None
     ):
         self.value: str = value
         self.key: Optional[str] = key
         self.headers: Optional[dict] = headers
+        self.offset = offset
+        self.timestamp = timestamp
 
 
 class KafkaProducer:
     """Kafka producer wrapper over confluent producer"""
 
     def __init__(self, config: dict, topic: str):
         """Create Producer instance"""
@@ -151,14 +158,16 @@
             self._log.error(f"Consumer poll Error:{msg.error()}")
             raise KafkaException(msg.error())
         else:
             self._first_message = KafkaMessage(
                 key=msg.key().decode("utf-8") if msg.key() else "",
                 headers=msg.headers(),
                 value=msg.value().decode("utf-8"),
+                offset=msg.offset(),
+                timestamp=msg.timestamp()[1],
             )
         return self._first_message
 
     def poll(self) -> Iterator[KafkaMessage]:
         """Polls the consumer for events and calls the corresponding callbacks"""
         while True:
             if 0 <= self.fetch_limit == self._no_of_success_messages:
@@ -175,14 +184,16 @@
 
             self._no_of_success_messages += 1
 
             kafka_message = KafkaMessage(
                 key=msg.key().decode("utf-8") if msg.key() else "",
                 headers=msg.headers(),
                 value=msg.value().decode("utf-8"),
+                offset=msg.offset(),
+                timestamp=msg.timestamp()[1],
             )
 
             if not self._first_message:
                 self._first_message = kafka_message
             if not self._no_of_success_messages % 10:
                 self._context.report.update(
                     ExecutionReport(
```

### Comparing `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/consumer.py` & `cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/workflow/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
             label="Messages Dataset",
             description="Where do you want to save the messages?"
             " The dropdown lists usable datasets from the current"
             " project only. In case you miss your dataset, check for"
             " the correct type (XML/JSON) and build project.",
             param_type=DatasetParameterType(dataset_type="xml,json"),
             default_value="",
+            advanced=True,
         ),
         PluginParameter(
             name="sasl_mechanisms",
             label="SASL Mechanisms",
             param_type=ChoiceParameterType(SASL_MECHANISMS),
             advanced=True,
             default_value="PLAIN",
```

### Comparing `cmem_plugin_kafka-1.3.1rc1/cmem_plugin_kafka/workflow/producer.py` & `cmem_plugin_kafka-1.4.0rc1/cmem_plugin_kafka/workflow/producer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.1rc1/pyproject.toml` & `cmem_plugin_kafka-1.4.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kafka"
-version = "1.3.1rc1"
+version = "1.4.0rc1"
 license = "Apache-2.0"
 description = "Send and receive messages from Apache Kafka."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `cmem_plugin_kafka-1.3.1rc1/PKG-INFO` & `cmem_plugin_kafka-1.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kafka
-Version: 1.3.1rc1
+Version: 1.4.0rc1
 Summary: Send and receive messages from Apache Kafka.
 Home-page: https://github.com/eccenca/cmem-plugin-kafka
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kafka,kafka-producer,kafka-consumer
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
```


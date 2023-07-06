# Comparing `tmp/grai_source_metabase-0.1.1a1.tar.gz` & `tmp/grai_source_metabase-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_metabase-0.1.1a1.tar", max compression
+gzip compressed data, was "grai_source_metabase-0.1.1a2.tar", max compression
```

## Comparing `grai_source_metabase-0.1.1a1.tar` & `grai_source_metabase-0.1.1a2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       29 2023-07-06 18:33:54.210141 grai_source_metabase-0.1.1a1/README.md
--rw-r--r--   0        0        0      607 2023-07-06 20:41:26.464528 grai_source_metabase-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0      126 2023-07-06 20:41:11.975437 grai_source_metabase-0.1.1a1/src/grai_source_metabase/__init__.py
--rw-r--r--   0        0        0    10393 2023-07-06 18:33:54.212223 grai_source_metabase-0.1.1a1/src/grai_source_metabase/adapters.py
--rw-r--r--   0        0        0     1624 2023-07-06 20:46:24.184345 grai_source_metabase-0.1.1a1/src/grai_source_metabase/base.py
--rw-r--r--   0        0        0     9969 2023-07-06 18:33:54.212723 grai_source_metabase-0.1.1a1/src/grai_source_metabase/loader.py
--rw-r--r--   0        0        0     3299 2023-07-06 18:33:54.212794 grai_source_metabase-0.1.1a1/src/grai_source_metabase/mock_tools.py
--rw-r--r--   0        0        0      783 2023-07-06 18:33:54.212995 grai_source_metabase-0.1.1a1/src/grai_source_metabase/models.py
--rw-r--r--   0        0        0      186 2023-07-06 18:33:54.213324 grai_source_metabase-0.1.1a1/src/grai_source_metabase/package_definitions.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 grai_source_metabase-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-07-06 18:33:54.210141 grai_source_metabase-0.1.1a2/README.md
+-rw-r--r--   0        0        0      784 2023-07-06 21:31:42.320460 grai_source_metabase-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-07-06 21:31:58.229774 grai_source_metabase-0.1.1a2/src/grai_source_metabase/__init__.py
+-rw-r--r--   0        0        0    10225 2023-07-06 21:31:58.236058 grai_source_metabase-0.1.1a2/src/grai_source_metabase/adapters.py
+-rw-r--r--   0        0        0     1618 2023-07-06 21:31:58.233939 grai_source_metabase-0.1.1a2/src/grai_source_metabase/base.py
+-rw-r--r--   0        0        0     9818 2023-07-06 21:31:58.231680 grai_source_metabase-0.1.1a2/src/grai_source_metabase/loader.py
+-rw-r--r--   0        0        0     3223 2023-07-06 21:31:58.228203 grai_source_metabase-0.1.1a2/src/grai_source_metabase/mock_tools.py
+-rw-r--r--   0        0        0      783 2023-07-06 18:33:54.212995 grai_source_metabase-0.1.1a2/src/grai_source_metabase/models.py
+-rw-r--r--   0        0        0      186 2023-07-06 18:33:54.213324 grai_source_metabase-0.1.1a2/src/grai_source_metabase/package_definitions.py
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 grai_source_metabase-0.1.1a2/PKG-INFO
```

### Comparing `grai_source_metabase-0.1.1a1/src/grai_source_metabase/adapters.py` & `grai_source_metabase-0.1.1a2/src/grai_source_metabase/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from grai_schemas import config as base_config
 from grai_schemas.schema import Schema
 from grai_schemas.v1 import EdgeV1, NodeV1
 from grai_schemas.v1.metadata.edges import EdgeMetadataTypeLabels, GenericEdgeMetadataV1
 from grai_schemas.v1.metadata.nodes import (
     GenericNodeMetadataV1,
     NodeMetadataTypeLabels,
+    QueryMetadata,
     TableMetadata,
 )
-from grai_source_metabase.models import Edge, NodeTypes, Question, Table
-from grai_source_metabase.package_definitions import config
 from multimethod import multimethod
 from pydantic import BaseModel
 
+from grai_source_metabase.models import Edge, NodeTypes, Question, Table
+from grai_source_metabase.package_definitions import config
+
 
 @multimethod
 def build_grai_metadata(current: Any, desired: Any) -> None:
     """
     Build grai metadata for a given object.
 
     Args:
@@ -28,23 +30,19 @@
         None: grai metadata object.
 
     Raises:
         NotImplementedError: If no adapter is available between the `current` and `desired` types.
 
     """
 
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_table(
-    current: Table, version: Literal["v1"] = "v1"
-) -> TableMetadata:
+def build_grai_metadata_from_table(current: Table, version: Literal["v1"] = "v1") -> TableMetadata:
     """
     Build grai metadata for a Table object.
 
     Args:
         current (Table): The Table object to build grai metadata from.
         version (Literal["v1"], optional): The version of grai metadata to build. Defaults to "v1".
 
@@ -63,17 +61,15 @@
         "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_question(
-    current: Question, version: Literal["v1"] = "v1"
-) -> GenericNodeMetadataV1:
+def build_grai_metadata_from_question(current: Question, version: Literal["v1"] = "v1") -> GenericNodeMetadataV1:
     """
     Build grai metadata for a Question object.
 
     Args:
         current (Question): The Question object to build grai metadata from.
         version (Literal["v1"], optional): The version of grai metadata to build. Defaults to "v1".
 
@@ -83,26 +79,24 @@
     Raises:
         None.
 
     """
 
     data = {
         "version": version,
-        "node_type": NodeMetadataTypeLabels.generic.value,
+        "node_type": NodeMetadataTypeLabels.query.value,
         "node_attributes": {},
         "tags": [config.metadata_id],
     }
 
-    return GenericNodeMetadataV1(**data)
+    return QueryMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_edge(
-    current: Edge, version: Literal["v1"] = "v1"
-) -> GenericEdgeMetadataV1:
+def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
     """
     Build grai metadata for an Edge object.
 
     Args:
         current (Edge): The Edge object to build grai metadata from.
         version (Literal["v1"], optional): The version of grai metadata to build. Defaults to "v1".
 
@@ -136,23 +130,19 @@
         None: Application-specific metadata object.
 
     Raises:
         NotImplementedError: If no adapter is available between the `current` and `desired` types.
 
     """
 
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_app_metadata.register
-def build_metadata_from_table(
-    current: BaseModel, version: Literal["v1"] = "v1"
-) -> Dict:
+def build_metadata_from_table(current: BaseModel, version: Literal["v1"] = "v1") -> Dict:
     """
     Build application-specific metadata for a Table object.
 
     Args:
         current (Table): The Table object to build application-specific metadata from.
         version (Literal["v1"], optional): The version of the metadata to build. Defaults to "v1".
 
@@ -255,21 +245,19 @@
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
         "metadata": build_metadata(current, version),
     }
 
-    return Schema.to_model(spec_dict, version=version, typing_type="Node")
+    return NodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_question_to_client(
-    current: Question, version: Literal["v1"] = "v1"
-) -> NodeV1:
+def adapt_question_to_client(current: Question, version: Literal["v1"] = "v1") -> NodeV1:
     """
     Adapt a Question object to the desired client format.
 
     Args:
         current (Question): The Question object to adapt.
         version (Literal["v1"], optional): The version of the client format to adapt to. Defaults to "v1".
 
@@ -285,15 +273,15 @@
         "name": current.full_name,
         "namespace": current.namespace,
         "display_name": current.name,
         "data_source": config.integration_name,
         "metadata": build_metadata(current, version),
     }
 
-    return Schema.to_model(spec_dict, version=version, typing_type="Node")
+    return NodeV1.from_spec(spec_dict)
 
 
 def make_name(node1: NodeTypes, node2: NodeTypes) -> str:
     """
     Creates a name for an edge based on the given nodes.
 
     Args:
@@ -341,21 +329,19 @@
         "destination": {
             "name": current.destination.full_name,
             "namespace": current.destination.namespace,
         },
         "metadata": build_metadata(current, version),
     }
 
-    return Schema.to_model(spec_dict, version=version, typing_type="Edge")
+    return EdgeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_seq_to_client(
-    objs: Sequence, version: Literal["v1"]
-) -> List[Union[NodeV1, EdgeV1]]:
+def adapt_seq_to_client(objs: Sequence, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
     """
     Adapt a sequence of objects to the desired client format.
 
     Args:
         objs (Sequence): The sequence of objects to adapt.
         version (Literal["v1"]): The version of the client format to adapt to.
 
@@ -368,17 +354,15 @@
     """
     entities = [adapt_to_client(item, version) for item in objs]
     entities = {entity for entity in entities}
     return list(entities)
 
 
 @adapt_to_client.register
-def adapt_list_to_client(
-    objs: List, version: Literal["v1"]
-) -> List[Union[NodeV1, EdgeV1]]:
+def adapt_list_to_client(objs: List, version: Literal["v1"]) -> List[Union[NodeV1, EdgeV1]]:
     """
     Adapt a list of objects to the desired client format.
 
     Args:
         objs (List): The list of objects to adapt.
         version (Literal["v1"]): The version of the client format to adapt to.
```

### Comparing `grai_source_metabase-0.1.1a1/src/grai_source_metabase/base.py` & `grai_source_metabase-0.1.1a2/src/grai_source_metabase/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import List, Literal, Optional, Tuple
 
 from grai_client.endpoints.client import BaseClient
 from grai_client.update import update
-from grai_schemas.base import Node, Edge
+from grai_schemas.base import Edge, Node
 
 from grai_source_metabase.adapters import adapt_to_client
 from grai_source_metabase.loader import MetabaseConnector
 
 
-def get_nodes_and_edges(
-    connector: MetabaseConnector, version: Literal["v1"]
-) -> Tuple[List[Node], List[Edge]]:
+def get_nodes_and_edges(connector: MetabaseConnector, version: Literal["v1"]) -> Tuple[List[Node], List[Edge]]:
     """
 
     Args:
         connector (MetabaseConnector):
         version (Literal["v1"]):
 
     Returns:
```

### Comparing `grai_source_metabase-0.1.1a1/src/grai_source_metabase/loader.py` & `grai_source_metabase-0.1.1a2/src/grai_source_metabase/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 from itertools import chain
 from typing import Callable, Dict, List, Optional, Union
 
 import requests
-from grai_source_metabase.models import Edge, NodeTypes, Question, Table
 from pydantic import BaseSettings, SecretStr, validator
 from requests.exceptions import ConnectionError
 from retrying import retry
 
+from grai_source_metabase.models import Edge, NodeTypes, Question, Table
+
 
 class MetabaseConfig(BaseSettings):
     endpoint: str
     username: SecretStr
     password: SecretStr
 
     @validator("endpoint")
@@ -43,17 +44,15 @@
     ):
         passthrough_kwargs = {
             "username": username,
             "password": password,
             "endpoint": endpoint,
         }
 
-        self.config = MetabaseConfig(
-            **{k: v for k, v in passthrough_kwargs.items() if v is not None}
-        )
+        self.config = MetabaseConfig(**{k: v for k, v in passthrough_kwargs.items() if v is not None})
         self.api_endpoint = f"{self.config.endpoint}/api"
 
         self.session = requests.Session()
         self.session.headers.update({"Content-Type": "application/json"})
         self.session.headers.update(self.authenticate())
 
     @retry(stop_max_attempt_number=3, wait_fixed=5000)
@@ -145,17 +144,15 @@
             dict: The JSON response containing the list of collections.
 
         """
 
         pass
 
 
-def build_namespace_map(
-    dbs: Dict, namespace_map: Union[str, Dict, None], metabase_namespace: str
-) -> Dict:
+def build_namespace_map(dbs: Dict, namespace_map: Union[str, Dict, None], metabase_namespace: str) -> Dict:
     if isinstance(namespace_map, str):
         namespace_map = json.loads(namespace_map)
     elif namespace_map is None:
         namespace_map = {}
 
     for k, v in dbs.items():
         db_id_ns = f"{metabase_namespace}.{k}.{v['name']}"
@@ -197,30 +194,22 @@
         super().__init__(*args, **kwargs)
         self._lineage_ready = False
         self.metabase_namespace = metabase_namespace
 
         # This line creates a list of tables by modifying each table dictionary obtained from the get_tables() method.
         # It replaces the "schema" key with a new key "schema_name" while preserving the other key-value pairs.
         # this is because the "schema" key is a reserved keyword in the pydantic.
-        self.tables = [
-            {**table, "schema_name": table.pop("schema")} for table in self.get_tables()
-        ]
-        self.tables_map = {
-            table["id"]: table for table in self.tables if table["active"]
-        }
+        self.tables = [{**table, "schema_name": table.pop("schema")} for table in self.get_tables()]
+        self.tables_map = {table["id"]: table for table in self.tables if table["active"]}
         self.dbs_map = {db["id"]: db for db in self.get_dbs()["data"]}
 
         self.questions_map = {
-            question["id"]: question
-            for question in self.get_questions()
-            if question["archived"] is False
+            question["id"]: question for question in self.get_questions() if question["archived"] is False
         }
-        self.namespace_map = build_namespace_map(
-            self.dbs_map, namespaces, self.metabase_namespace
-        )
+        self.namespace_map = build_namespace_map(self.dbs_map, namespaces, self.metabase_namespace)
 
         self.question_table_map = {}
         self.table_db_map = {}
         # self.question_db_map = {}
 
     def build_lineage(self):
         """
@@ -230,16 +219,15 @@
         and `question_db_map` attributes.
 
         """
 
         self.question_table_map = {
             question["id"]: question["table_id"]
             for question in self.questions_map.values()
-            if question["table_id"]
-            and self.tables_map.get(question["table_id"]) is not None
+            if question["table_id"] and self.tables_map.get(question["table_id"]) is not None
         }
 
         self.table_db_map = {
             table["id"]: table["db_id"]
             for table in self.tables
             if table["id"] is not None and table["db_id"] is not None
         }
@@ -263,17 +251,15 @@
 
         for question in self.questions_map.values():
             question["namespace"] = self.metabase_namespace
 
         for table in self.tables_map.values():
             table["namespace"] = self.namespace_map[self.table_db_map[table["id"]]]
 
-        verified_questions = [
-            Question(**question) for question in self.questions_map.values()
-        ]
+        verified_questions = [Question(**question) for question in self.questions_map.values()]
         verified_tables = [Table(**table) for table in self.tables_map.values()]
         nodes = chain(verified_questions, verified_tables)
 
         return list(nodes)
 
     def get_edges(self) -> List[Edge]:
         """
```

### Comparing `grai_source_metabase-0.1.1a1/src/grai_source_metabase/mock_tools.py` & `grai_source_metabase-0.1.1a2/src/grai_source_metabase/mock_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 from functools import wraps
 from typing import Callable, TypeVar
 
-from grai_source_metabase.models import Question, Edge, Table
+from grai_source_metabase.models import Edge, Question, Table
 
 T = TypeVar("T")
 
 has_faker = importlib.util.find_spec("faker") is not None
 if has_faker:
     from faker import Faker
 
@@ -35,17 +35,15 @@
 
         Returns:
 
         Raises:
 
         """
         if not has_faker:
-            raise ModuleNotFoundError(
-                "Mock testing tools require `faker`. Try running `pip install faker`"
-            )
+            raise ModuleNotFoundError("Mock testing tools require `faker`. Try running `pip install faker`")
         return fn(*args, **kwargs)
 
     return inner
 
 
 class MockMetabaseObjects:
     """ """
@@ -64,17 +62,15 @@
             id=fake.pyint(1, 10000),
             result_metadata=[
                 {
                     "display_name": "display_name",
                     "name": "display_name",
                     "base_type": "type/Text",
                     "effective_type": "type/Text",
-                    "fingerprint": {
-                        "global": {"distinct-count": 1, "nil%": 0, "sample": "sample"}
-                    },
+                    "fingerprint": {"global": {"distinct-count": 1, "nil%": 0, "sample": "sample"}},
                 }
             ],
             creator={
                 "id": fake.pyint(1, 2000),
                 "first_name": fake.first_name(),
                 "last_name": fake.last_name(),
                 "email": fake.email(),
```

### Comparing `grai_source_metabase-0.1.1a1/src/grai_source_metabase/models.py` & `grai_source_metabase-0.1.1a2/src/grai_source_metabase/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.1a1/PKG-INFO` & `grai_source_metabase-0.1.1a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: grai-source-metabase
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: 
 Author: Elseagle
 Author-email: dowolebolu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grai-client (>=0.2.19,<0.3.0)
-Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
+Requires-Dist: grai-schemas (>=0.1.16,<0.2.0)
 Requires-Dist: multimethod (>=1.9.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: retrying (>=1.3.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 "# Grai Metabase Integration"
```


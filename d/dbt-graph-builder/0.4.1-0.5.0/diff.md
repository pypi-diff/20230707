# Comparing `tmp/dbt-graph-builder-0.4.1.tar.gz` & `tmp/dbt-graph-builder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.4.1.tar", last modified: Wed Jul  5 12:41:20 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.5.0.tar", last modified: Fri Jul  7 10:22:12 2023, max compression
```

## Comparing `dbt-graph-builder-0.4.1.tar` & `dbt-graph-builder-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 12:41:20.061091 dbt-graph-builder-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-05 12:41:04.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 12:41:20.057091 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 12:41:20.000000 dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.485221 dbt-graph-builder-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-07 10:21:55.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:22:12.489220 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 10:22:12.000000 dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/top_level.txt
```

### Comparing `dbt-graph-builder-0.4.1/LICENSE` & `dbt-graph-builder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.1/PKG-INFO` & `dbt-graph-builder-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.4.1
+Version: 0.5.0
 Summary: DBT Graph Builder
-Author-email: Piotr Tutak <piotr.tutak@getindata.com>
+Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
             in the Software without restriction, including without limitation the rights
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt-graph-builder-0.4.1/README.md` & `dbt-graph-builder-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.1/pyproject.toml` & `dbt-graph-builder-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbt-graph-builder"
 description = "DBT Graph Builder"
 authors = [
+    {name = "Piotr Pękala", email = "piotr.pekala@getindata.com"},
+    {name = "Andrzej Swatowski", email = "andrzej.swatowski@getindata.com"},
     {name = "Piotr Tutak", email = "piotr.tutak@getindata.com"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt-graph-builder-0.4.1/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.5.0/src/dbt_graph_builder/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,37 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
-from typing import Any, NamedTuple
+from typing import Any
 
-from dbt_graph_builder.gateway import GatewayConfiguration, TaskGraphConfiguration
-from dbt_graph_builder.graph import DbtManifestGraph
+from dbt_graph_builder.gateway import GatewayConfiguration
+from dbt_graph_builder.graph import DbtManifestGraph, GraphConfiguration
 
 LOGGER = logging.getLogger(__name__)
 
 
-class GraphConfiguration(NamedTuple):
-    """Graph configuration."""
-
-    gateway_config: GatewayConfiguration = GatewayConfiguration(gateway_task_name="gateway", separation_schemas=[])
-    enable_dags_dependencies: bool = False
-    show_ephemeral_models: bool = False
-
-
 def create_tasks_graph(
     manifest: dict[str, Any],
-    graph_config: GraphConfiguration = GraphConfiguration(),
+    graph_config: GraphConfiguration | None = None,
 ) -> DbtManifestGraph:
     """Create tasks graph.
 
     Args:
         manifest (dict[str, Any]): Manifest.
-        graph_config (GraphConfiguration, optional): Graph configuration. Defaults to GraphConfiguration().
+        graph_config (GraphConfiguration, optional): Graph configuration. Defaults to None.
 
     Returns:
         DbtManifestGraph: Tasks graph.
     """
+    if graph_config is None:
+        graph_config = GraphConfiguration()
     LOGGER.info("Creating tasks graph")
-    dbt_airflow_graph = DbtManifestGraph(TaskGraphConfiguration(graph_config.gateway_config))
+    dbt_airflow_graph = DbtManifestGraph(graph_config)
     dbt_airflow_graph.add_execution_tasks(manifest)
     if graph_config.enable_dags_dependencies:
         LOGGER.debug("Adding external dependencies")
         dbt_airflow_graph.add_external_dependencies(manifest)
     dbt_airflow_graph.create_edges_from_dependencies(graph_config.enable_dags_dependencies)
     if not graph_config.show_ephemeral_models:
         LOGGER.debug("Removing ephemeral nodes from graph")
@@ -68,11 +62,15 @@
     Args:
         airflow_config (dict[str, Any]): Airflow config.
 
     Returns:
         GatewayConfiguration: Gateway configuration.
     """
     LOGGER.info("Creating gateway config")
+    if "save_points" in airflow_config:
+        separation_schemas = airflow_config["save_points"]
+    else:
+        separation_schemas = []
     return GatewayConfiguration(
-        separation_schemas=airflow_config.get("save_points", []),
+        separation_schemas=separation_schemas,
         gateway_task_name="gateway",
     )
```

### Comparing `dbt-graph-builder-0.4.1/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.5.0/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.1/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.5.0/src/dbt_graph_builder/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import itertools
 import logging
+from dataclasses import dataclass, field
 from typing import Any
 
 import networkx as nx
 from networkx.classes.reportviews import NodeDataView, OutEdgeDataView
 
 from dbt_graph_builder.gateway import (
+    GatewayConfiguration,
     NodeProperties,
     SeparationLayer,
-    TaskGraphConfiguration,
     add_gateway_to_dependencies,
     create_gateway_name,
     get_gateway_dependencies,
     is_gateway_valid_dependency,
     should_gateway_be_added,
 )
 from dbt_graph_builder.node_type import NodeType
@@ -22,22 +23,36 @@
     is_ephemeral_task,
     is_model_run_task,
     is_source_sensor_task,
     is_test_task,
 )
 
 
+def _default_gateway_config() -> GatewayConfiguration:
+    return GatewayConfiguration([], "gateway")
+
+
+@dataclass(frozen=True)
+class GraphConfiguration:
+    """Graph configuration."""
+
+    gateway_config: GatewayConfiguration = field(default_factory=_default_gateway_config)
+    dbt_manifest_props: dict[str, str] = field(default_factory=dict)
+    enable_dags_dependencies: bool = False
+    show_ephemeral_models: bool = False
+
+
 class DbtManifestGraph:
     """DbtManifestGraph class is used to create a DAG from DBT manifest.json file."""
 
-    def __init__(self, configuration: TaskGraphConfiguration) -> None:
+    def __init__(self, configuration: GraphConfiguration) -> None:
         """Create DbtManifestGraph.
 
         Args:
-            configuration (TaskGraphConfiguration): _description_
+            configuration (GraphConfiguration): Graph configuration.
         """
         self._graph = nx.DiGraph()
         self._configuration = configuration
 
     @property
     def graph(self) -> nx.DiGraph:
         """Get graph.
@@ -63,16 +78,16 @@
                 is_test_task(node_name)
                 and len(self._get_model_dependencies_from_manifest_node(manifest_node, manifest)) > 1
             ):
                 logging.info("Creating tasks for: " + node_name)
                 self._add_graph_node_for_multiple_deps_test(node_name, manifest_node, manifest)
 
     def _add_gateway_execution_tasks(self, manifest: dict[str, Any]) -> None:
-        if len(self._configuration.gateway.separation_schemas) >= 2:
-            separation_layers = self._configuration.gateway.separation_schemas
+        if len(self._configuration.gateway_config.separation_schemas) >= 2:
+            separation_layers = self._configuration.gateway_config.separation_schemas
 
             for index, _ in enumerate(separation_layers[:-1]):
                 separation_layer_left = separation_layers[index]
                 separation_layer_right = separation_layers[index + 1]
                 self._add_gateway_node(
                     manifest=manifest,
                     separation_layer=SeparationLayer(left=separation_layer_left, right=separation_layer_right),
@@ -152,27 +167,27 @@
 
     def contract_test_nodes(self) -> None:
         """Contract test nodes."""
         tests_with_more_deps = self._get_test_with_multiple_deps_names_by_deps()
         for depends_on_tuple, test_node_names in tests_with_more_deps.items():
             self._contract_test_nodes_same_deps(depends_on_tuple, test_node_names)
 
-    @staticmethod
-    def get_default_node_values(manifest_node: dict[str, Any]) -> dict[str, Any]:
+    def get_default_node_values(self, manifest_node: dict[str, Any]) -> dict[str, Any]:
         """Get default node values.
 
         Args:
             manifest_node (dict): Manifest node.
 
         Returns:
             dict: Default node values.
         """
         result: dict[str, Any] = {}
-        if "alias" in manifest_node:
-            result["alias"] = manifest_node["alias"]
+        for key, value in self._configuration.dbt_manifest_props.items():
+            if key in manifest_node:
+                result[value] = manifest_node[key]
         return result
 
     def _add_execution_graph_node(
         self, node_name: str, manifest_node: dict[str, Any], node_type: NodeType, manifest: dict[str, Any]
     ) -> None:
         self._graph.add_node(
             node_name,
@@ -190,15 +205,15 @@
             node_type=NodeType.SOURCE_SENSOR,
             **self.get_default_node_values(manifest_node),
         )
 
     def _add_gateway_node(self, manifest: dict[str, Any], separation_layer: SeparationLayer) -> None:
         node_name = create_gateway_name(
             separation_layer=separation_layer,
-            gateway_task_name=self._configuration.gateway.gateway_task_name,
+            gateway_task_name=self._configuration.gateway_config.gateway_task_name,
         )
         self._graph.add_node(
             node_name,
             select=node_name,
             depends_on=get_gateway_dependencies(separation_layer=separation_layer, manifest=manifest),
             node_type=NodeType.MOCK_GATEWAY,
             **self.get_default_node_values({"alias": node_name}),
@@ -256,17 +271,17 @@
 
     def _get_model_dependencies_from_manifest_node(self, node: dict[str, Any], manifest: dict[str, Any]) -> list[str]:
         filtered_records = list(filter(DbtManifestGraph._is_valid_dependency, node["depends_on"]["nodes"]))
         node_schema = node.get("schema", None)
 
         if should_gateway_be_added(
             node_schema=node_schema,
-            separation_schemas=self._configuration.gateway.separation_schemas,
+            separation_schemas=self._configuration.gateway_config.separation_schemas,
         ):
-            node_schema_index = self._configuration.gateway.separation_schemas.index(node_schema)
+            node_schema_index = self._configuration.gateway_config.separation_schemas.index(node_schema)
             if node_schema_index >= 1:
                 filtered_records = self._filter_to_gateway_conditions(
                     node_schema_index=node_schema_index,
                     manifest=manifest,
                     node=node,
                     filtered_records=filtered_records,
                 )
@@ -276,15 +291,15 @@
     def _filter_to_gateway_conditions(
         self,
         node_schema_index: int,
         manifest: dict[str, Any],
         node: dict[str, Any],
         filtered_records: list[str],
     ) -> list[str]:
-        separation_layers = self._configuration.gateway.separation_schemas
+        separation_layers = self._configuration.gateway_config.separation_schemas
         separation_layer_left = separation_layers[node_schema_index - 1]
         separation_layer_right = separation_layers[node_schema_index]
 
         filtered_dependencies = list(
             filter(
                 lambda dep_node: is_gateway_valid_dependency(
                     separation_layer=SeparationLayer(left=separation_layer_left, right=separation_layer_right),
@@ -296,15 +311,15 @@
         )
 
         add_gateway_to_dependencies(
             filtered_dependencies=filtered_dependencies,
             filtered_records=filtered_records,
             gateway_name=create_gateway_name(
                 separation_layer=SeparationLayer(left=separation_layer_left, right=separation_layer_right),
-                gateway_task_name=self._configuration.gateway.gateway_task_name,
+                gateway_task_name=self._configuration.gateway_config.gateway_task_name,
             ),
         )
         return filtered_dependencies
 
     @staticmethod
     def _is_valid_dependency(node_name: str) -> bool:
         return is_model_run_task(node_name) or is_source_sensor_task(node_name)  # type: ignore
```

### Comparing `dbt-graph-builder-0.4.1/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.5.0/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.4.1/src/dbt_graph_builder/workflow.py` & `dbt-graph-builder-0.5.0/src/dbt_graph_builder/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         in_degree = int(self._graph.graph.in_degree(node))
         for predecessor in self._graph.graph.predecessors(node):
             if predecessor in self._processed_nodes:
                 in_degree -= 1
         return in_degree
 
     def _get_step(self, node: str) -> Step:
-        step = self._factory.create_single_step(node, self._graph.graph.nodes[node])
+        step = self._factory.create_node_step(node, self._graph.graph.nodes[node])
         self._processed_nodes_this_iteration[node] = step
         if self._graph.graph.out_degree(node) == 0:
             return step
         step = self._factory.create_chain_step(step)
         self._processed_nodes_this_iteration[node] = step
         if self._graph.graph.out_degree(node) == 1:
             next_step = self._process_node(next(self._graph.graph.successors(node)))
@@ -115,15 +115,15 @@
         return step
 
 
 class StepFactory(ABC):
     """StepFactory is an abstract class that defines the step creation strategy of the graph."""
 
     @abstractmethod
-    def create_single_step(self, node: str, node_data: dict[str, Any]) -> Step:
+    def create_node_step(self, node: str, node_data: dict[str, Any]) -> Step:
         """Return a single step materialization.
 
         Args:
             node (str): The node to process.
             node_data (dict[str, Any]): The data of the node.
         """
```

### Comparing `dbt-graph-builder-0.4.1/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.5.0/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.4.1
+Version: 0.5.0
 Summary: DBT Graph Builder
-Author-email: Piotr Tutak <piotr.tutak@getindata.com>
+Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
             of this software and associated documentation files (the "Software"), to deal
             in the Software without restriction, including without limitation the rights
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


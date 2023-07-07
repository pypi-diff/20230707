# Comparing `tmp/opcua-tools-0.0.81.tar.gz` & `tmp/opcua-tools-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opcua-tools-0.0.81.tar", last modified: Mon Dec 12 11:01:24 2022, max compression
+gzip compressed data, was "opcua-tools-0.0.82.tar", last modified: Fri Jul  7 12:27:09 2023, max compression
```

## Comparing `opcua-tools-0.0.81.tar` & `opcua-tools-0.0.82.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 11:01:24.865238 opcua-tools-0.0.81/
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2022-12-12 11:01:24.865238 opcua-tools-0.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 11:01:24.861238 opcua-tools-0.0.81/opcua_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21945 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/nodes_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15649 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/nodeset_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/nodeset_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 11:01:24.865238 opcua-tools-0.0.81/opcua_tools/static/
--rw-r--r--   0 runner    (1001) docker     (123)  2767306 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/static/Opc.Ua.NodeSet2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    19128 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/static/UANodeSet.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    14355 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/ua_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24504 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/ua_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/opcua_tools/value_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 11:01:24.861238 opcua-tools-0.0.81/opcua_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2022-12-12 11:01:24.000000 opcua-tools-0.0.81/opcua_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-12 11:01:24.000000 opcua-tools-0.0.81/opcua_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 11:01:24.000000 opcua-tools-0.0.81/opcua_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-12 11:01:24.000000 opcua-tools-0.0.81/opcua_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-12 11:01:24.000000 opcua-tools-0.0.81/opcua_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 11:01:24.865238 opcua-tools-0.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2022-12-12 11:01:11.000000 opcua-tools-0.0.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:27:09.044856 opcua-tools-0.0.82/
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-07 12:27:09.044856 opcua-tools-0.0.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:27:09.036856 opcua-tools-0.0.82/opcua_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21945 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/nodes_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/nodeset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/nodeset_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:27:09.040856 opcua-tools-0.0.82/opcua_tools/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  2767306 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/static/Opc.Ua.NodeSet2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/static/UANodeSet.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    40175 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/ua_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25519 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/ua_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/opcua_tools/value_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:27:09.040856 opcua-tools-0.0.82/opcua_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-07 12:27:09.000000 opcua-tools-0.0.82/opcua_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 12:27:09.000000 opcua-tools-0.0.82/opcua_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:27:09.000000 opcua-tools-0.0.82/opcua_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-07 12:27:09.000000 opcua-tools-0.0.82/opcua_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 12:27:09.000000 opcua-tools-0.0.82/opcua_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:27:09.044856 opcua-tools-0.0.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:27:09.040856 opcua-tools-0.0.82/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_paper_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49664 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_ua_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_ua_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_uagraph_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-07 12:26:59.000000 opcua-tools-0.0.82/tests/test_value_parser.py
```

### Comparing `opcua-tools-0.0.81/LICENSE` & `opcua-tools-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/PKG-INFO` & `opcua-tools-0.0.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opcua-tools
-Version: 0.0.81
+Version: 0.0.82
 Summary: OPCUA Tools for Python using Pandas DataFrames
 Home-page: https://github.com/PrediktorAS/opcua-tools
 Author: Magnus Bakken
 Author-email: olav.pedersen@prediktor.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opcua-tools-0.0.81/README.md` & `opcua-tools-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/__init__.py` & `opcua-tools-0.0.82/opcua_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/navigation.py` & `opcua-tools-0.0.82/opcua_tools/navigation.py`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/nodes_manipulation.py` & `opcua-tools-0.0.82/opcua_tools/nodes_manipulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from opcua_tools.ua_graph import UAGraph
 from typing import Dict
 from opcua_tools.ua_data_types import (
     UAEnumeration,
     UAInt32,
     UAListOf,
-    UnparsedUAExtensionObject,
+    UAExtensionObject,
     UALocalizedText,
 )
 
 import xmltodict
 import pandas as pd
 import logging
 
@@ -45,17 +45,17 @@
     """
 
     # The enum definition can be stored in different ways. The two versions observed
     # is as an unparsed UAExtentionObject in xml or as UALocalizedText.
     enum_tuple = row["Value"]
     enum_dict = dict()
     for index, content in enumerate(enum_tuple):
-        if isinstance(content, UnparsedUAExtensionObject):
+        if isinstance(content, UAExtensionObject):
             ua_structure = content.body
-            xml_string = ua_structure.xmlstring
+            xml_string = ua_structure.value
             xml_dict = xmltodict.parse(xml_string)
 
             # This notation and searching is to ignore xmlns handling
             enum_value_dict = [
                 val for key, val in xml_dict.items() if "EnumValueType" in key
             ]
             value = [val for key, val in enum_value_dict[0].items() if "Value" in key][
```

### Comparing `opcua-tools-0.0.81/opcua_tools/nodeset_generator.py` & `opcua-tools-0.0.82/opcua_tools/nodeset_generator.py`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/nodeset_parser.py` & `opcua-tools-0.0.82/opcua_tools/nodeset_parser.py`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/static/Opc.Ua.NodeSet2.xml` & `opcua-tools-0.0.82/opcua_tools/static/Opc.Ua.NodeSet2.xml`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/static/UANodeSet.xsd` & `opcua-tools-0.0.82/opcua_tools/static/UANodeSet.xsd`

 * *Files identical despite different names*

### Comparing `opcua-tools-0.0.81/opcua_tools/ua_graph.py` & `opcua-tools-0.0.82/opcua_tools/ua_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,126 +77,148 @@
 
     def all_references_of_type(self, browsename: str):
         return self.references[
             self.references["ReferenceType"]
             == self.reference_type_by_browsename(browsename)
         ].copy()
 
-    def reference_type_by_browsename(self, browsename: str) -> int:
+    def __ua_nodeclass_by_browsename(
+        self, browsename: str, nodeclass: Optional[str] = None
+    ) -> int:
+        """Retrieves the internal id from the OPC UA graph which has a NodeClass `nodeclass`
+        (UAVariableType in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+            nodeclass (Optional[str], optional): NodeClass of the node to find. Defaults to None.
+
+        Raises:
+            ValueError: If browsename is None or empty string.
+            ValueError: If no node is found.
+            ValueError: If multiple nodes are found.
+
+        Returns:
+            int: The internal id of the node.
+        """
         if browsename is None or browsename == "":
             raise ValueError(
-                '"browsename" must not be None or empty string, should be BrowseName of ReferenceType'
+                f'"browsename" must not be None or empty string, should be BrowseName of {nodeclass}'
             )
 
-        reference_type_nodes = self.nodes[self.nodes["NodeClass"] == "UAReferenceType"]
-        reference_type_ids = resolve_ids_from_browsenames(
-            nodes=reference_type_nodes, browsenames=[browsename]
-        )
-        if len(reference_type_ids) == 0:
-            raise ValueError("Could not find ReferenceType " + browsename)
-        elif len(reference_type_ids) > 1:
-            raise ValueError(
-                "Multiple hits for ReferenceType "
-                + browsename
-                + " please specify namespace"
-            )
+        if nodeclass:
+            nodeclass_nodes = self.nodes[self.nodes["NodeClass"] == f"UA{nodeclass}"]
         else:
-            reference_type_id = reference_type_ids.iloc[0]
-
-        return int(reference_type_id)
-
-    def object_type_by_browsename(self, browsename: str) -> int:
-        if browsename is None or browsename == "":
-            raise ValueError(
-                '"browsename" must not be None or empty string, should be BrowseName of ObjectType'
-            )
+            nodeclass_nodes = self.nodes
 
-        object_type_nodes = self.nodes[self.nodes["NodeClass"] == "UAObjectType"]
-        object_type_ids = resolve_ids_from_browsenames(
-            nodes=object_type_nodes, browsenames=[browsename]
+        nodeclass_ids = resolve_ids_from_browsenames(
+            nodes=nodeclass_nodes, browsenames=[browsename]
         )
-        if len(object_type_ids) == 0:
-            raise ValueError("Could not find object type " + browsename)
-        elif len(object_type_ids) > 1:
-            raise ValueError(
-                "Multiple hits for object type "
-                + browsename
-                + " please specify namespace"
-            )
+        if len(nodeclass_ids) == 0:
+            raise ValueError(f"Could not find {nodeclass} " + browsename)
+        elif len(nodeclass_ids) > 1:
+            raise ValueError(f"Multiple hits for {nodeclass} " + browsename + " found.")
         else:
-            object_type_id = object_type_ids.iloc[0]
-
-        return int(object_type_id)
+            nodeclass_id = nodeclass_ids.iloc[0]
+        return int(nodeclass_id)
 
-    def variable_type_by_browsename(self, browsename: str) -> int:
-        if browsename is None or browsename == "":
-            raise ValueError(
-                '"browsename" must not be None or empty string, should be BrowseName of VariableType'
-            )
+    def reference_type_by_browsename(self, browsename: str) -> int:
+        """Retrieves the internal id from the OPC UA graph which has a NodeClass "ReferenceType"
+        (UAReferenceType in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+
+        Returns:
+            int: The internal id of the node.
+        """
+        return self.__ua_nodeclass_by_browsename(browsename, "ReferenceType")
 
-        variable_type_nodes = self.nodes[self.nodes["NodeClass"] == "UAVariableType"]
-        variable_type_ids = resolve_ids_from_browsenames(
-            nodes=variable_type_nodes, browsenames=[browsename]
-        )
-        if len(variable_type_ids) == 0:
-            raise ValueError("Could not find variable type " + browsename)
-        elif len(variable_type_ids) > 1:
-            raise ValueError(
-                "Multiple hits for variable type "
-                + browsename
-                + " please specify namespace"
-            )
-        else:
-            variable_type_id = variable_type_ids.iloc[0]
+    def object_type_by_browsename(self, browsename: str) -> int:
+        """Retrieves the internal id from the OPC UA graph which has a NodeClass "ObjectType"
+        (UAObjectType in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+
+        Returns:
+            int: The internal id of the node.
+        """
+        return self.__ua_nodeclass_by_browsename(browsename, "ObjectType")
 
-        return int(variable_type_id)
+    def variable_type_by_browsename(self, browsename: str) -> int:
+        """Retrieves the internal id from the OPC UA graph which has a NodeClass "VariableType"
+        (UAVariableType in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+
+        Returns:
+            int: The internal id of the node.
+        """
+        return self.__ua_nodeclass_by_browsename(browsename, "VariableType")
 
     def data_type_by_browsename(self, browsename: str) -> int:
-        if browsename is None or browsename == "":
-            raise ValueError(
-                '"browsename" must not be None or empty string, should be BrowseName of DataType'
-            )
-
-        data_type_nodes = self.nodes[self.nodes["NodeClass"] == "UADataType"]
-        data_type_ids = resolve_ids_from_browsenames(
-            nodes=data_type_nodes, browsenames=[browsename]
-        )
-        if len(data_type_ids) == 0:
-            raise ValueError("Could not find data type " + browsename)
-        elif len(data_type_ids) > 1:
-            raise ValueError(
-                "Multiple hits for data type "
-                + browsename
-                + " please specify namespace"
-            )
-        else:
-            data_type_id = data_type_ids.iloc[0]
-
-        return int(data_type_id)
+        """Retrieves the internal id from the OPC UA graph which has a NodeClass "DataType"
+        (UADataType in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+
+        Returns:
+            int: The internal id of the node.
+        """
+        return self.__ua_nodeclass_by_browsename(browsename, "DataType")
 
     def object_by_browsename(self, browsename: str) -> int:
-        if browsename is None or browsename == "":
-            raise ValueError(
-                '"browsename" must not be None or empty string, should be BrowseName of Object'
-            )
-
-        object_nodes = self.nodes[self.nodes["NodeClass"] == "UAObject"]
-        object_ids = resolve_ids_from_browsenames(
-            nodes=object_nodes, browsenames=[browsename]
-        )
-        if len(object_ids) == 0:
-            raise ValueError("Could not find object " + browsename)
-        elif len(object_ids) > 1:
-            raise ValueError(
-                "Multiple hits for object " + browsename + " please specify namespace"
-            )
+        """Retrieves the internal id from the OPC UA graph which has a NodeClass "Object"
+        (UAObject in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+
+        Returns:
+            int: The internal id of the node.
+        """
+        return self.__ua_nodeclass_by_browsename(browsename, "Object")
+
+    def nodeid_by_browsename(
+        self, browsename: str, nodeclass: Optional[str] = None
+    ) -> int:
+        """Retrieves the NodeId from the OPC UA graph which has a NodeClass `nodeclass`
+        (UAVariableType in the UAGraph), for the given `browsename` input. If multiple nodes
+        are found, an error is raised. Please note that the 'nodeclass' variable has to be
+        a string, e.g. "VariableType", "DataType", etc. in the form of CamelCase.
+
+        Args:
+            browsename (str): BrowseName of the node to find.
+            nodeclass (Optional[str], optional): NodeClass of the node to find. Defaults to None.
+
+        Raises:
+            ValueError: If browsename is None or empty string.
+            ValueError: If no node is found.
+            ValueError: If multiple nodes are found.
+
+        Returns:
+            int: The NodeId of the node.
+        """
+        if nodeclass:
+            id = self.__ua_nodeclass_by_browsename(browsename, nodeclass)
         else:
-            reference_type_id = object_ids.iloc[0]
+            id = self.__ua_nodeclass_by_browsename(browsename)
 
-        return int(reference_type_id)
+        if id is None:
+            raise ValueError(f"Could not find node with browsename {browsename}")
+        node_id = self.nodes.loc[self.nodes["id"] == id, "NodeId"].values[0]
+        return node_id
 
     def write_nodeset(
         self,
         filename_or_stringio: Union[str, StringIO],
         namespace_uri: str,
         include_outgoing_instance_level_references: Optional[bool] = True,
         last_modified: Optional[datetime] = None,
```

### Comparing `opcua-tools-0.0.81/opcua_tools/value_parser.py` & `opcua-tools-0.0.82/opcua_tools/value_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,44 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import base64
 import re
-
-import lxml.etree as ET
-from lxml import objectify
-from dateutil import parser
 import copy
+import lxml.etree as ET
 
-from typing import Dict
-from opcua_tools.ua_data_types import *
+from dateutil import parser
+from typing import Dict, Optional
+from opcua_tools.ua_data_types import (
+    UASByte,
+    UAByte,
+    UAInt16,
+    UAUInt16,
+    UAInt32,
+    UAUInt32,
+    UAInt64,
+    UAUInt64,
+    UAFloat,
+    UADouble,
+    UAGuid,
+    UAByteString,
+    UAXMLElement,
+    UADateTime,
+    UAEngineeringUnits,
+    UAExtensionObject,
+    UANodeId,
+    UABoolean,
+    UAString,
+    UAEURange,
+    UALocalizedText,
+    UAListOf,
+    NodeIdType,
+)
 
 simple = {
     "Boolean",
     "SByte",
     "Byte",
     "Int16",
     "UInt16",
@@ -180,46 +202,49 @@
         if typeid is None:
             parsed_typeid = None
         else:
             parsed_typeid = parse_value_element(typeid)
 
         body = val.find(uaxsd + "Body")
 
-        if parsed_typeid is not None and type(parsed_typeid) == UANodeId:
+        if parsed_typeid is not None:
             if (
                 parsed_typeid.namespace == 0
                 and parsed_typeid.nodeid_type == NodeIdType.NUMERIC
                 and parsed_typeid.value == "888"
             ):
                 return parse_engineering_units(body)
             if (
                 parsed_typeid.namespace == 0
                 and parsed_typeid.nodeid_type == NodeIdType.NUMERIC
                 and parsed_typeid.value == "885"
             ):
                 return parse_eu_range(body)
 
-        if body is not None:
+        if body is not None and len(body) > 0:
             nextbody = next(n for n in body)
             if nextbody is None:
                 parsednextbody = None
             else:
                 parsednextbody = parse_value_element(nextbody)
         else:
             parsednextbody = None
 
-        return UnparsedUAExtensionObject(type_nodeid=parsed_typeid, body=parsednextbody)
+        if parsednextbody is not None and parsed_typeid is not None:
+            return UAExtensionObject(type_nodeid=parsed_typeid, body=parsednextbody)
+        else:
+            return None
 
     else:
         # Need to copy element, cleanup_namespaces only works if a copy is made
         val_copy = copy.copy(val)
         # Remove unused xml namespaces
         ET.cleanup_namespaces(val_copy)
 
-        return UAStructure(xmlstring=ET.tostring(val_copy).decode("utf-8"))
+        return UAXMLElement(value=ET.tostring(val_copy).decode("utf-8"))
 
     raise NotImplementedError(tagtype)
 
 
 def parse_nodeid(
     nodeidstr: str,
     namespace_map: Optional[Dict[int, int]] = None,
@@ -252,16 +277,25 @@
         text = None
     else:
         text = txt.text
 
     loc = el.find(uaxsd + "Locale")
     if loc is None:
         locale = None
+    elif loc.text is None:
+        locale = None
+    elif type(loc.text) == str:
+        loc_text_str = loc.text.strip()
+        if loc_text_str == "":
+            locale = None
+        else:
+            locale = loc.text
     else:
-        locale = loc.text
+        raise ValueError("Unexpected type for localized text locale")
+
     return UALocalizedText(text=text, locale=locale)
 
 
 def parse_engineering_units(el):
     if el is not None:
         euinfo = el.find(uaxsd + "EUInformation")
         if euinfo is not None:
```

### Comparing `opcua-tools-0.0.81/opcua_tools.egg-info/PKG-INFO` & `opcua-tools-0.0.82/opcua_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opcua-tools
-Version: 0.0.81
+Version: 0.0.82
 Summary: OPCUA Tools for Python using Pandas DataFrames
 Home-page: https://github.com/PrediktorAS/opcua-tools
 Author: Magnus Bakken
 Author-email: olav.pedersen@prediktor.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opcua-tools-0.0.81/setup.py` & `opcua-tools-0.0.82/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="opcua-tools",
-    version="0.0.81",
+    version="0.0.82",
     description="OPCUA Tools for Python using Pandas DataFrames",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/PrediktorAS/opcua-tools",
     author="Magnus Bakken",
     author_email="olav.pedersen@prediktor.com",
     license="Apache License 2.0",
```


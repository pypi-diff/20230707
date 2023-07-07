# Comparing `tmp/iam_actions-1.2.20230706.tar.gz` & `tmp/iam_actions-1.2.20230707.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230706.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230707.tar", max compression
```

## Comparing `iam_actions-1.2.20230706.tar` & `iam_actions-1.2.20230707.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/README.md
--rw-r--r--   0        0        0      228 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/__init__.py
--rw-r--r--   0        0        0  4362696 2023-07-06 02:56:53.344974 iam_actions-1.2.20230706/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-06 02:55:22.011863 iam_actions-1.2.20230706/iam_actions/generate/services.py
--rw-r--r--   0        0        0   560956 2023-07-06 02:56:53.344974 iam_actions-1.2.20230706/iam_actions/policies.json
--rw-r--r--   0        0        0   197380 2023-07-06 02:56:53.344974 iam_actions-1.2.20230706/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   544073 2023-07-06 02:56:53.344974 iam_actions-1.2.20230706/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-06 02:56:54.152984 iam_actions-1.2.20230706/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230706/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230706/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/README.md
+-rw-r--r--   0        0        0      228 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4363235 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-07 02:51:55.749546 iam_actions-1.2.20230707/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   560956 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/policies.json
+-rw-r--r--   0        0        0   197380 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   544073 2023-07-07 02:53:42.310673 iam_actions-1.2.20230707/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-07 02:53:43.110682 iam_actions-1.2.20230707/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230707/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230707/PKG-INFO
```

### Comparing `iam_actions-1.2.20230706/LICENSE` & `iam_actions-1.2.20230707/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/README.md` & `iam_actions-1.2.20230707/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/actions.json` & `iam_actions-1.2.20230707/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999674778083869%*

 * *Differences: {"'kafka'": "{'BatchAssociateScramSecret': {'resources': ['cluster']}, "*

 * *            "'BatchDisassociateScramSecret': {'resources': ['cluster']}, 'CreateCluster': "*

 * *            "{'resources': ['cluster']}, 'CreateClusterV2': {'resources': ['cluster']}, "*

 * *            "'CreateConfiguration': {'resources': ['configuration']}, 'CreateVpcConnection': "*

 * *            "{'resources': ['cluster', 'vpc-connection']}, 'DeleteCluster': {'resources': "*

 * *            "['cluster']}, 'DeleteConfiguration': {'resources': ['conf […]*

```diff
@@ -83774,72 +83774,87 @@
     "kafka": {
         "BatchAssociateScramSecret": {
             "access_level": "Write",
             "action": "BatchAssociateScramSecret",
             "condition_keys": [],
             "description": "Grants permission to associate one or more Scram Secrets with an Amazon MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "BatchDisassociateScramSecret": {
             "access_level": "Write",
             "action": "BatchDisassociateScramSecret",
             "condition_keys": [],
             "description": "Grants permission to disassociate one or more Scram Secrets from an Amazon MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "CreateCluster": {
             "access_level": "Write",
             "action": "CreateCluster",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "CreateClusterV2": {
             "access_level": "Write",
             "action": "CreateClusterV2",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "CreateConfiguration": {
             "access_level": "Write",
             "action": "CreateConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create an MSK configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "configuration"
+            ]
         },
         "CreateVpcConnection": {
             "access_level": "Write",
             "action": "CreateVpcConnection",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a MSK VPC connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster",
+                "vpc-connection"
+            ]
         },
         "DeleteCluster": {
             "access_level": "Write",
             "action": "DeleteCluster",
             "condition_keys": [],
             "description": "Grants permission to delete an MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "DeleteClusterPolicy": {
             "access_level": "Write",
             "action": "DeleteClusterPolicy",
             "condition_keys": [],
             "description": "Grants permission to delete a cluster resource-based policy",
             "orphan": false,
@@ -83849,15 +83864,17 @@
         },
         "DeleteConfiguration": {
             "access_level": "Write",
             "action": "DeleteConfiguration",
             "condition_keys": [],
             "description": "Grants permission to delete the specified MSK configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "configuration"
+            ]
         },
         "DeleteVpcConnection": {
             "access_level": "Write",
             "action": "DeleteVpcConnection",
             "condition_keys": [],
             "description": "Grants permission to delete a MSK VPC connection",
             "orphan": false,
@@ -83867,15 +83884,17 @@
         },
         "DescribeCluster": {
             "access_level": "Read",
             "action": "DescribeCluster",
             "condition_keys": [],
             "description": "Grants permission to describe an MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "DescribeClusterOperation": {
             "access_level": "Read",
             "action": "DescribeClusterOperation",
             "condition_keys": [],
             "description": "Grants permission to describe the cluster operation that is specified by the given ARN",
             "orphan": false,
@@ -83883,15 +83902,17 @@
         },
         "DescribeClusterV2": {
             "access_level": "Read",
             "action": "DescribeClusterV2",
             "condition_keys": [],
             "description": "Grants permission to describe an MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "DescribeConfiguration": {
             "access_level": "Read",
             "action": "DescribeConfiguration",
             "condition_keys": [],
             "description": "Grants permission to describe an MSK configuration",
             "orphan": false,
@@ -83957,15 +83978,17 @@
         },
         "ListClusterOperations": {
             "access_level": "List",
             "action": "ListClusterOperations",
             "condition_keys": [],
             "description": "Grants permission to return a list of all the operations that have been performed on the specified MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "ListClusters": {
             "access_level": "List",
             "action": "ListClusters",
             "condition_keys": [],
             "description": "Grants permission to list all MSK clusters in this account",
             "orphan": false,
@@ -83981,15 +84004,17 @@
         },
         "ListConfigurationRevisions": {
             "access_level": "List",
             "action": "ListConfigurationRevisions",
             "condition_keys": [],
             "description": "Grants permission to list all revisions for an MSK configuration in this account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "configuration"
+            ]
         },
         "ListConfigurations": {
             "access_level": "List",
             "action": "ListConfigurations",
             "condition_keys": [],
             "description": "Grants permission to list all MSK configurations in this account",
             "orphan": false,
@@ -84005,23 +84030,27 @@
         },
         "ListNodes": {
             "access_level": "List",
             "action": "ListNodes",
             "condition_keys": [],
             "description": "Grants permission to list brokers in an MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "ListScramSecrets": {
             "access_level": "List",
             "action": "ListScramSecrets",
             "condition_keys": [],
             "description": "Grants permission to list the Scram Secrets associated with an Amazon MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags of an MSK resource",
             "orphan": false,
@@ -84049,24 +84078,27 @@
         },
         "RebootBroker": {
             "access_level": "Write",
             "action": "RebootBroker",
             "condition_keys": [],
             "description": "Grants permission to reboot broker",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "RejectClientVpcConnection": {
             "access_level": "Write",
             "action": "RejectClientVpcConnection",
             "condition_keys": [],
             "description": "Grants permission to reject a MSK VPC connection",
             "orphan": false,
             "resources": [
-                "cluster"
+                "cluster",
+                "vpc-connection"
             ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -84094,89 +84126,110 @@
         },
         "UpdateBrokerCount": {
             "access_level": "Write",
             "action": "UpdateBrokerCount",
             "condition_keys": [],
             "description": "Grants permission to update the number of brokers of the MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateBrokerStorage": {
             "access_level": "Write",
             "action": "UpdateBrokerStorage",
             "condition_keys": [],
             "description": "Grants permission to update the storage size of the brokers of the MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateBrokerType": {
             "access_level": "Write",
             "action": "UpdateBrokerType",
             "condition_keys": [],
             "description": "Grants permission to update the broker type of an Amazon MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateClusterConfiguration": {
             "access_level": "Write",
             "action": "UpdateClusterConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update the configuration of the MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster",
+                "configuration"
+            ]
         },
         "UpdateClusterKafkaVersion": {
             "access_level": "Write",
             "action": "UpdateClusterKafkaVersion",
             "condition_keys": [],
             "description": "Grants permission to update the MSK cluster to the specified Apache Kafka version",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateConfiguration": {
             "access_level": "Write",
             "action": "UpdateConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create a new revision of the MSK configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "configuration"
+            ]
         },
         "UpdateConnectivity": {
             "access_level": "Write",
             "action": "UpdateConnectivity",
             "condition_keys": [
                 "kafka:publicAccessEnabled"
             ],
             "description": "Grants permission to update the connectivity settings for the MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateMonitoring": {
             "access_level": "Write",
             "action": "UpdateMonitoring",
             "condition_keys": [],
             "description": "Grants permission to update the monitoring settings for the MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateSecurity": {
             "access_level": "Write",
             "action": "UpdateSecurity",
             "condition_keys": [],
             "description": "Grants permission to update the security settings for the MSK cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "UpdateStorage": {
             "access_level": "Write",
             "action": "UpdateStorage",
             "condition_keys": [],
             "description": "Grants permission to update the EBS storage (size or provisioned throughput) associated with MSK brokers or set cluster storage mode to TIERED",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         }
     },
     "kafka-cluster": {
         "AlterCluster": {
             "access_level": "Write",
             "action": "AlterCluster",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230706/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230707/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230707/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/generate/generate.py` & `iam_actions-1.2.20230707/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230707/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230707/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/generate/services.py` & `iam_actions-1.2.20230707/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/policies.json` & `iam_actions-1.2.20230707/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230707/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/iam_actions/services.json` & `iam_actions-1.2.20230707/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230706/pyproject.toml` & `iam_actions-1.2.20230707/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230706"
+version = "1.2.20230707"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230706/setup.py` & `iam_actions-1.2.20230707/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230706',
+    'version': '1.2.20230707',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230706/PKG-INFO` & `iam_actions-1.2.20230707/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230706
+Version: 1.2.20230707
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


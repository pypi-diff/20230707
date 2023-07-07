# Comparing `tmp/censys_cloud_connectors-3.1.3.tar.gz` & `tmp/censys_cloud_connectors-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys_cloud_connectors-3.1.3.tar", max compression
+gzip compressed data, was "censys_cloud_connectors-3.1.4.tar", max compression
```

## Comparing `censys_cloud_connectors-3.1.3.tar` & `censys_cloud_connectors-3.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11342 2023-06-21 16:29:59.071797 censys_cloud_connectors-3.1.3/LICENSE
--rw-r--r--   0        0        0     2143 2023-06-21 16:29:59.071797 censys_cloud_connectors-3.1.3/README.md
--rw-r--r--   0        0        0     4491 2023-06-21 16:29:59.083792 censys_cloud_connectors-3.1.3/pyproject.toml
--rw-r--r--   0        0        0      920 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/__init__.py
--rw-r--r--   0        0        0      439 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/__init__.py
--rw-r--r--   0        0        0    27101 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/connector.py
--rw-r--r--   0        0        0     2766 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/enums.py
--rw-r--r--   0        0        0    18732 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/provider_setup.py
--rwxr-xr-x   0        0        0     1240 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/serverless.py
--rw-r--r--   0        0        0     8355 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/service.py
--rw-r--r--   0        0        0     4192 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/settings.py
--rw-r--r--   0        0        0      343 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/__init__.py
--rw-r--r--   0        0        0    10933 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/connector.py
--rw-r--r--   0        0        0      895 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/enums.py
--rw-r--r--   0        0        0     9199 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/provider_setup.py
--rw-r--r--   0        0        0     1665 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/settings.py
--rw-r--r--   0        0        0      713 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/__init__.py
--rw-r--r--   0        0        0      849 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/__init__.py
--rw-r--r--   0        0        0      888 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/args.py
--rw-r--r--   0        0        0     6405 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/base.py
--rw-r--r--   0        0        0       87 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/__init__.py
--rw-r--r--   0        0        0     2948 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/config.py
--rw-r--r--   0        0        0     3277 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/scan.py
--rw-r--r--   0        0        0     9860 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/provider_setup.py
--rw-r--r--   0        0        0     2609 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cloud_asset.py
--rw-r--r--   0        0        0     8524 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/connector.py
--rw-r--r--   0        0        0      659 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/context.py
--rw-r--r--   0        0        0     1598 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/enums.py
--rw-r--r--   0        0        0     6533 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/healthcheck.py
--rw-r--r--   0        0        0      957 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/ignore_list.py
--rw-r--r--   0        0        0      857 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/logger.py
--rw-r--r--   0        0        0      506 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/models.py
--rw-r--r--   0        0        0      296 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/__init__.py
--rw-r--r--   0        0        0      489 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/events.py
--rw-r--r--   0        0        0     1455 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/plugin.py
--rw-r--r--   0        0        0     5633 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/registry.py
--rw-r--r--   0        0        0     2858 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/seed.py
--rw-r--r--   0        0        0     8864 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/settings.py
--rw-r--r--   0        0        0      329 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/__init__.py
--rw-r--r--   0        0        0    12081 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/connector.py
--rw-r--r--   0        0        0     5883 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/enums.py
--rw-r--r--   0        0        0    27935 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/provider_setup.py
--rw-r--r--   0        0        0     1688 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/settings.py
--rw-r--r--   0        0        0       36 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/__init__.py
--rw-r--r--   0        0        0    14168 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/aws_tags.py
--rw-r--r--   0        0        0     1882 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/example.py
--rw-r--r--   0        0        0        0 2023-06-21 16:29:59.087791 censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/py.typed
--rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 censys_cloud_connectors-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-07-07 18:16:27.220244 censys_cloud_connectors-3.1.4/LICENSE
+-rw-r--r--   0        0        0     2143 2023-07-07 18:16:27.220244 censys_cloud_connectors-3.1.4/README.md
+-rw-r--r--   0        0        0     4491 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0      920 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/__init__.py
+-rw-r--r--   0        0        0    27441 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/connector.py
+-rw-r--r--   0        0        0     2766 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/enums.py
+-rw-r--r--   0        0        0    18732 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/provider_setup.py
+-rwxr-xr-x   0        0        0     1240 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/serverless.py
+-rw-r--r--   0        0        0     8355 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/service.py
+-rw-r--r--   0        0        0     4192 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/settings.py
+-rw-r--r--   0        0        0      343 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/__init__.py
+-rw-r--r--   0        0        0    10933 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/connector.py
+-rw-r--r--   0        0        0      895 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/enums.py
+-rw-r--r--   0        0        0     9274 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/provider_setup.py
+-rw-r--r--   0        0        0     1665 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/settings.py
+-rw-r--r--   0        0        0      713 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/__init__.py
+-rw-r--r--   0        0        0      888 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/args.py
+-rw-r--r--   0        0        0     6405 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/base.py
+-rw-r--r--   0        0        0       87 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2948 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/commands/config.py
+-rw-r--r--   0        0        0     3277 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/commands/scan.py
+-rw-r--r--   0        0        0     9860 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/provider_setup.py
+-rw-r--r--   0        0        0     2609 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cloud_asset.py
+-rw-r--r--   0        0        0     7785 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/connector.py
+-rw-r--r--   0        0        0      659 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/context.py
+-rw-r--r--   0        0        0     1598 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/enums.py
+-rw-r--r--   0        0        0     6533 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/healthcheck.py
+-rw-r--r--   0        0        0      957 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/ignore_list.py
+-rw-r--r--   0        0        0      857 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/logger.py
+-rw-r--r--   0        0        0      506 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/models.py
+-rw-r--r--   0        0        0      296 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/plugins/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/plugins/events.py
+-rw-r--r--   0        0        0     1455 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/plugins/plugin.py
+-rw-r--r--   0        0        0     5633 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/plugins/registry.py
+-rw-r--r--   0        0        0     2858 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/seed.py
+-rw-r--r--   0        0        0     8974 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/settings.py
+-rw-r--r--   0        0        0      329 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/__init__.py
+-rw-r--r--   0        0        0    12081 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/connector.py
+-rw-r--r--   0        0        0     5883 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/enums.py
+-rw-r--r--   0        0        0    27935 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/provider_setup.py
+-rw-r--r--   0        0        0     1669 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/settings.py
+-rw-r--r--   0        0        0       36 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/plugins/__init__.py
+-rw-r--r--   0        0        0    14928 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/plugins/aws_tags.py
+-rw-r--r--   0        0        0     1882 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/plugins/example.py
+-rw-r--r--   0        0        0        0 2023-07-07 18:16:27.236243 censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/py.typed
+-rw-r--r--   0        0        0     4131 1970-01-01 00:00:00.000000 censys_cloud_connectors-3.1.4/PKG-INFO
```

### Comparing `censys_cloud_connectors-3.1.3/LICENSE` & `censys_cloud_connectors-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/README.md` & `censys_cloud_connectors-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/pyproject.toml` & `censys_cloud_connectors-3.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censys-cloud-connectors"
-version = "3.1.3"
+version = "3.1.4"
 description = "The Censys Unified Cloud Connector is a standalone connector that gathers assets from various cloud providers and stores them in Censys ASM."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "censys/cloud_connectors", from = "src" }]
 keywords = ["censys", "cloud", "connector", "attack surface management"]
 classifiers = [
@@ -39,15 +39,15 @@
 
 [tool.poetry.scripts]
 censys-cc = "censys.cloud_connectors.common.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 backoff = "^2.2.1"
-censys = "^2.2.2"
+censys = "^2.2.4"
 inquirerpy = "^0.3.3"
 pydantic = {extras = ["dotenv", "email"], version = "^1.9.0"}
 PyYAML = "^6.0"
 requests = "^2.30.0"
 rich = "^13.3.5"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/__init__.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/connector.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """AWS Cloud Connector."""
 import contextlib
 from collections.abc import Generator, Sequence
-from typing import Any, Optional, TypeVar
+from typing import Any, Optional, TypeVar, Union
 
 import boto3
 import botocore
 from botocore.exceptions import ClientError
 from mypy_boto3_apigateway import APIGatewayClient
 from mypy_boto3_apigatewayv2 import ApiGatewayV2Client
 from mypy_boto3_ec2 import EC2Client
@@ -389,37 +389,37 @@
         self.get_load_balancers_v2()
 
     def get_network_interfaces(self):
         """Retrieve EC2 Elastic Network Interfaces (ENI) data and emit seeds."""
         label = self.format_label(SeedLabel.NETWORK_INTERFACE)
 
         interfaces = self.describe_network_interfaces()
-        instance_tags = self.get_resource_tags()
+        instance_tags, instance_tag_sets = self.get_resource_tags()
 
         for ip_address, record in interfaces.items():
             instance_id = record["InstanceId"]
             tags = instance_tags.get(instance_id)
             if tags and self.has_ignored_tag(tags):
                 self.logger.debug(
                     f"Skipping ignored tag for network instance {ip_address}"
                 )
                 continue
 
             with SuppressValidationError():
                 ip_seed = IpSeed(value=ip_address, label=label)
-                self.add_seed(ip_seed, tags=tags)
+                self.add_seed(ip_seed, tags=instance_tag_sets.get(instance_id))
 
     def describe_network_interfaces(self) -> dict:
         """Retrieve EC2 Elastic Network Interfaces (ENI) data.
 
         Returns:
             dict: Network Interfaces.
         """
         ec2: EC2Client = self.get_aws_client(AwsServices.EC2)
-        interfaces = {}
+        interfaces: dict[str, dict[str, Union[None, str, list]]] = {}
 
         # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_network_interfaces
         filters: Sequence[FilterTypeDef] = [
             {"Name": "association.public-ip", "Values": ["*"]}
         ]
 
         try:
@@ -442,15 +442,15 @@
                         }
         except ClientError as e:
             self.logger.error(f"Could not connect to ENI Service. Error: {e}")
 
         return interfaces
 
     def get_resource_tags_paginated(
-        self, resource_types: list[str] = None
+        self, resource_types: Optional[list[str]] = None
     ) -> Generator[TagDescriptionTypeDef, None, None]:
         """Retrieve EC2 resource tags paginated.
 
         Args:
             resource_types (Optional[list[str]]): Resource types. Defaults to None.
 
         Yields:
@@ -465,41 +465,46 @@
             Filters=[
                 {"Name": "resource-type", "Values": resource_types or ["instance"]}
             ]
         ):
             tags = page.get("Tags", [])
             yield from tags
 
-    def get_resource_tags(self, resource_types: list[str] = None) -> dict:
+    def get_resource_tags(
+        self, resource_types: Optional[list[str]] = None
+    ) -> tuple[dict, dict]:
         """Get EC2 resource tags based on resource types.
 
         Args:
-            resource_types (list[str]): Resource type filter.
+            resource_types (Optional[list[str]]): Resource type filter.
 
         Returns:
-            dict: Tags grouped by resource keys.
+            tuple[dict, dict]: Instance tags and tag sets.
         """
         resource_tags: dict = {}
+        resource_tag_sets: dict = {}
 
         for tag in self.get_resource_tags_paginated(resource_types):
             # Tags come in two formats:
-            # 1. Tag = { Key = "Name", Value= "actual-tag-name" }
+            # 1. Tag = { Key = "Name", Value = "actual-tag-name" }
             # 2. Tag = { Key = "actual-key-name", Value = "tag-value-that-is-unused-here"}
             tag_name = tag.get("Key")
             if tag_name == "Name":
                 tag_name = tag.get("Value")
 
             # Note: resource id is instance id
             resource_id = tag.get("ResourceId")
             if _resource_tags := resource_tags.get(resource_id):
                 _resource_tags.append(tag_name)
+                resource_tag_sets[resource_id].append(tag)
             else:
                 resource_tags[resource_id] = [tag_name]
+                resource_tag_sets[resource_id] = [tag]
 
-        return resource_tags
+        return resource_tags, resource_tag_sets
 
     def network_interfaces_ignored_tags(self, data: NetworkInterfaceTypeDef) -> bool:
         """Check if network interface has ignored tags.
 
         Args:
             data (NetworkInterfaceTypeDef): Raw AWS tag data in key value pairs.
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/enums.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/provider_setup.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/serverless.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/serverless.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/service.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/service.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/aws_connector/settings.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/aws_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/connector.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/enums.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/provider_setup.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/provider_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Azure specific setup CLI."""
+import contextlib
 from typing import Optional
 
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError
 from azure.identity import ClientSecretCredential
 from azure.mgmt.network import NetworkManagementClient
 from pydantic import validate_arguments
 
@@ -189,15 +190,16 @@
             tenant_id=provider_setting.tenant_id,
             client_id=provider_setting.client_id,
             client_secret=provider_setting.client_secret,
         )
         for subscription_id in provider_setting.subscription_id:
             network_client = NetworkManagementClient(credential, subscription_id)
             res = network_client.public_ip_addresses.list_all()
-            next(res)
+            with contextlib.suppress(StopIteration):
+                next(res)
         return True
 
     def setup_with_cli(self) -> None:
         """Setup with the Azure CLI."""
         subscriptions = self.get_subscriptions_from_cli()
         if len(subscriptions) == 0:
             self.print_error(AzureMessages.ERROR_NO_SUBSCRIPTIONS_FOUND)
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/azure_connector/settings.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/azure_connector/settings.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/__init__.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/__init__.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/args.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/base.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/base.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/config.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/commands/scan.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/commands/scan.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cli/provider_setup.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cli/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/cloud_asset.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/cloud_asset.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/connector.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Base class for all cloud connectors."""
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from enum import Enum
 from logging import Logger
 from typing import Callable, Optional, Union
 
-from requests.exceptions import JSONDecodeError
-
-from censys.asm import Seeds
+from censys.asm import Beta, Seeds
 from censys.common.exceptions import CensysAsmException
 
 from .cloud_asset import CloudAsset
 from .enums import EventTypeEnum, ProviderEnum
 from .logger import get_logger
 from .plugins import CloudConnectorPluginRegistry, EventContext
 from .seed import Seed
@@ -23,14 +21,15 @@
 
     provider: ProviderEnum
     provider_settings: ProviderSpecificSettings
     label_prefix: str
     settings: Settings
     logger: Logger
     seeds_api: Seeds
+    beta_api: Beta
     seeds: dict[str, set[Seed]]
     cloud_assets: dict[str, set[CloudAsset]]
     seed_scanners: dict[str, Callable[[], None]]
     cloud_asset_scanners: dict[str, Callable[[], None]]
     current_service: Optional[Union[str, Enum]]
 
     def __init__(self, settings: Settings):
@@ -53,16 +52,19 @@
 
         self.seeds_api = Seeds(
             settings.censys_api_key,
             url=settings.censys_asm_api_base_url,
             user_agent=settings.censys_user_agent,
             cookies=settings.censys_cookies,
         )
-        self._add_cloud_asset_path = (
-            f"{settings.censys_asm_api_base_url}/beta/cloudConnector/addCloudAssets"
+        self.beta_api = Beta(
+            settings.censys_api_key,
+            url=settings.censys_asm_api_base_url,
+            user_agent=settings.censys_user_agent,
+            cookies=settings.censys_cookies,
         )
 
         self.seeds = defaultdict(set)
         self.cloud_assets = defaultdict(set)
         self.current_service = None
 
     def get_seeds(self) -> None:
@@ -173,50 +175,25 @@
         self.dispatch_event(EventTypeEnum.SEEDS_SUBMITTED, count=submitted_seeds)
 
     def submit_cloud_assets(self):
         """Submit the cloud assets to the Censys ASM."""
         submitted_assets = 0
         for uid, cloud_assets in self.cloud_assets.items():
             try:
-                data = {
-                    "cloudConnectorUid": uid,
-                    "cloudAssets": [asset.to_dict() for asset in cloud_assets],
-                }
-                self._add_cloud_assets(data)
+                self.beta_api.add_cloud_assets(
+                    uid, [asset.to_dict() for asset in cloud_assets]
+                )
                 submitted_assets += len(cloud_assets)
-            except (CensysAsmException, JSONDecodeError) as e:
+            except CensysAsmException as e:
                 self.logger.error(f"Error submitting cloud assets for {uid}: {e}")
         self.logger.info(f"Submitted {submitted_assets} cloud assets.")
         self.dispatch_event(
             EventTypeEnum.CLOUD_ASSETS_SUBMITTED, count=submitted_assets
         )
 
-    def _add_cloud_assets(self, data: dict) -> dict:
-        """Add cloud assets to the Censys ASM.
-
-        Args:
-            data (dict): The data to add.
-
-        Returns:
-            dict: The response from the Censys ASM.
-
-        Raises:
-            CensysAsmException: If the response is not valid.
-        """
-        res = self.seeds_api._session.post(self._add_cloud_asset_path, json=data)
-        json_data = res.json()
-        if error_message := json_data.get("error"):
-            raise CensysAsmException(
-                res.status_code,
-                error_message,
-                res.text,
-                error_code=json_data.get("errorCode"),
-            )
-        return json_data
-
     def clear(self):
         """Clear the seeds and cloud assets."""
         self.seeds.clear()
         self.cloud_assets.clear()
 
     def submit(self):  # pragma: no cover
         """Submit the seeds and cloud assets to the Censys ASM."""
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/context.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/context.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/enums.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/healthcheck.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/healthcheck.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/ignore_list.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/ignore_list.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/logger.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/logger.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/plugin.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/plugins/registry.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/seed.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/seed.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/common/settings.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/common/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from abc import abstractmethod
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Any, DefaultDict, Optional, Union
 
 import yaml
 from pydantic import BaseSettings, Field, validate_arguments, validator
 
+from censys.common.version import __version__ as censys_common_version
+
 from .. import __version__ as censys_cloud_connectors_version
 from .enums import ProviderEnum
 
 if TYPE_CHECKING:
     from censys.cloud_connectors.common.connector import CloudConnector
 
 
@@ -144,15 +146,15 @@
     )
     censys_asm_api_base_url: str = Field(
         default="https://app.censys.io/api",
         env="CENSYS_ASM_API_BASE_URL",
         description="Censys ASM API Base URL",
     )
     censys_user_agent: str = Field(
-        default=f"censys-cloud-connector/{censys_cloud_connectors_version}",
+        default=f"censys-python/{censys_common_version} censys-cloud-connector/{censys_cloud_connectors_version}",
         env="CENSYS_USER_AGENT",
         description="Censys User Agent",
     )
     censys_cookies: dict = Field(
         default={}, env="CENSYS_COOKIES", description="Censys Cookies"
     )
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/connector.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/connector.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/enums.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/enums.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/provider_setup.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/provider_setup.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/gcp_connector/settings.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/gcp_connector/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     provider = ProviderEnum.GCP
 
     ignore: Optional[list[GcpSecurityCenterResourceTypes]] = None
 
     organization_id: int = Field(
         gt=1,
-        lt=10**12,
         description="GCP organization ID.",
     )
     service_account_json_file: Path = Field(
         description="Path to service account json file."
     )
     service_account_email: EmailStr = Field(description="Service account email.")
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/aws_tags.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/plugins/aws_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Callable, Optional
 
 from botocore.exceptions import ClientError
 from mypy_boto3_elb import ElasticLoadBalancingClient
 from mypy_boto3_elbv2 import ElasticLoadBalancingv2Client
 from mypy_boto3_route53 import Route53Client
 from mypy_boto3_s3 import S3Client
-from requests import HTTPError
 
 from censys.asm import AsmClient
 from censys.common.exceptions import (
     CensysAsmException,
     CensysDomainNotFoundException,
     CensysException,
 )
@@ -164,15 +163,17 @@
             tag_set: Tag set.
 
         Returns:
             Formatted tag set.
         """
         return f"{tag_set['Key']}: {tag_set['Value']}"
 
-    def add_ip_tags(self, context: EventContext, seed: IpSeed, tag_set: dict) -> None:
+    def add_ip_tags(
+        self, context: EventContext, seed: IpSeed, tag_set: list[dict]
+    ) -> None:
         """Add IP tags.
 
         Args:
             context: Event context.
             seed: Seed.
             tag_set: Tag set.
         """
@@ -233,14 +234,16 @@
             context: Event context.
             seed: Seed.
             tag_set: Tags.
         """
         client = self.get_client(context)
         for tag in tag_set:
             tag_string = self.format_tag_set_as_string(tag)
+            # We first try to add the tag to the domain itself
+            # If that fails, we try to add the tag to the subdomain at the base domain
             try:
                 client.domains.add_tag(str(seed.value), tag_string)
             except CensysDomainNotFoundException:
                 self.add_subdomain_tag(str(seed.value), tag_string)
 
     def add_cloud_asset_tags(
         self, context: EventContext, cloud_asset: CloudAsset, tag_set: list[dict]
@@ -248,26 +251,25 @@
         """Add cloud asset tags.
 
         Args:
             context: Event context.
             cloud_asset: Cloud asset.
             tag_set: Tags.
         """
-        settings = context["connector"].settings
         client = self.get_client(context)
         url_encoded_object_storage_key = urllib.parse.quote_plus(
             cloud_asset.value + "/"
         )
         for tag in tag_set:
-            res = client.domains._session.post(
-                f"{settings.censys_asm_api_base_url}/beta/assets/object-storages/{url_encoded_object_storage_key}/tags",
-                json={"name": self.format_tag_set_as_string(tag)},
-            )
-            with contextlib.suppress(HTTPError):
-                res.raise_for_status()
+            # We need to suppress the exception here incase the tag is already added
+            # or if the tag is invalid
+            with contextlib.suppress(CensysAsmException):
+                client.object_storages.add_tag(
+                    url_encoded_object_storage_key, self.format_tag_set_as_string(tag)
+                )
 
     def _get_api_gateway_tags(
         self, context: EventContext, seed: DomainSeed, **kwargs
     ) -> None:
         """Get API Gateway tags.
 
         Args:
@@ -334,15 +336,20 @@
             seed: Seed.
             kwargs: Additional event data.
         """
         tags = kwargs.get("tags", [])
         if not tags:
             return
 
-        self.add_ip_tags(context, seed, tags)
+        # Filter out AWS internal tags
+        filtered_tags = [tag for tag in tags if not tag["Key"].startswith("aws:")]
+        if not filtered_tags:
+            return
+
+        self.add_ip_tags(context, seed, filtered_tags)
 
     def _get_rds_tags(
         self,
         context: EventContext,
         seed: DomainSeed,
         **kwargs,
     ) -> None:
@@ -386,17 +393,15 @@
         pre_processed_tags = client.list_tags_for_resource(
             ResourceType="hostedzone", ResourceId=resource_id
         )["ResourceTagSet"]["Tags"]
 
         if not pre_processed_tags:
             return
 
-        tags = {tag["Key"]: tag["Value"] for tag in pre_processed_tags}
-
-        self.add_domain_tags(context, seed, tags)  # type: ignore
+        self.add_domain_tags(context, seed, pre_processed_tags)  # type: ignore
 
     def _get_ecs_tags(self, context: EventContext, seed: DomainSeed, **kwargs) -> None:
         """Get ECS tags.
 
         Args:
             context: Event context.
             seed: Seed.
@@ -418,21 +423,37 @@
     ) -> None:
         """Get S3 tags.
 
         Args:
             context: Event context.
             cloud_asset: Cloud asset.
             kwargs: Additional event data.
+
+        Raises:
+            ClientError: If the bucket does not exist.
         """
         bucket_name = kwargs.get("bucket_name")
         client: S3Client = kwargs.get("aws_client")  # type: ignore
         if not bucket_name or not client:
             return
 
         try:
             tag_set = client.get_bucket_tagging(Bucket=bucket_name).get("TagSet", [])
-            self.add_cloud_asset_tags(context, cloud_asset, tag_set)  # type: ignore
-        except ClientError:
-            pass
+            if not tag_set:
+                return
+
+            # Filter out AWS internal tags
+            filtered_tags = [
+                tag for tag in tag_set if not tag["Key"].startswith("aws:")
+            ]
+            if not filtered_tags:
+                return
+
+            self.add_cloud_asset_tags(context, cloud_asset, filtered_tags)  # type: ignore
+        except ClientError as e:
+            # If there are no tag sets, it will raise a ClientError with the code "NoSuchTagSet"
+            if e.response.get("Error", {}).get("Code") == "NoSuchTagSet":
+                return
+            raise
 
 
 __plugin__ = AwsTagsPlugin
```

### Comparing `censys_cloud_connectors-3.1.3/src/censys/cloud_connectors/plugins/example.py` & `censys_cloud_connectors-3.1.4/src/censys/cloud_connectors/plugins/example.py`

 * *Files identical despite different names*

### Comparing `censys_cloud_connectors-3.1.3/PKG-INFO` & `censys_cloud_connectors-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censys-cloud-connectors
-Version: 3.1.3
+Version: 3.1.4
 Summary: The Censys Unified Cloud Connector is a standalone connector that gathers assets from various cloud providers and stores them in Censys ASM.
 License: Apache-2.0
 Keywords: censys,cloud,connector,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: censys (>=2.2.2,<3.0.0)
+Requires-Dist: censys (>=2.2.4,<3.0.0)
 Requires-Dist: inquirerpy (>=0.3.3,<0.4.0)
 Requires-Dist: pydantic[dotenv,email] (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Project-URL: Censys Homepage, https://censys.io/
 Project-URL: Changelog, https://github.com/censys/censys-cloud-connector/releases
 Project-URL: Discussions, https://github.com/censys/censys-cloud-connector/discussions
```


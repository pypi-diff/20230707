# Comparing `tmp/threemystic_cloud_data_client-0.1.7.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.8.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.7.tar` & `threemystic_cloud_data_client-0.1.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/LICENSE
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/hatch.toml
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5772 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7106 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/hatch.toml
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.8/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.base_class.base import cloud_data_client_azure_client_action_base as base
 import asyncio
-from azure.mgmt.keyvault import KeyVaultManagementClient
-from azure.keyvault.secrets import SecretClient
-from azure.keyvault.keys import KeyClient
-from azure.keyvault.administration import KeyVaultAccessControlClient
+from azure.mgmt.compute import ComputeManagementClient
+from azure.mgmt.resource import ResourceManagementClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
-      data_action="database", 
-      logger_name= "cloud_data_client_azure_client_action_database", 
-      uniqueid_lambda = lambda: True,
+      data_action="vmss", 
+      logger_name= "cloud_data_client_azure_client_action_vmss", 
+      uniqueid_lambda = lambda: True, 
       *args, **kwargs)
   
- 
-  async def _process_account_data(self, account, loop, *args, **kwargs):
+  
     
-    # WIP
-    # This will be DBs
-    # ms sql, postgress, dynamodb, auora, azure sql ...
+  async def __process_get_resources_vmss(self, account, *args, **kwargs):
+    resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+    try:
+      return { self.get_cloud_client().get_resource_id_from_resource(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
+          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Compute/virtualMachineScaleSets'", expand="createdTime,changedTime,provisioningState")
+        )
+      }
+    except:
+      return []
+        
+  async def _process_account_data(self, account, loop, *args, **kwargs):
+    client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+    tasks = {
+      "resource": loop.create_task(self.__process_get_resources_vmss(account= account))
+    }
+
+    await asyncio.wait(tasks.values())
 
     return {
-        "account": account,
-        "data": [
-          #  self.get_common().helper_type().dictionary().merge_dictionary([
-          #   {},
-          #   self.get_base_return_data(
-          #     account= self.get_cloud_client().serialize_azresource(resource= account),
-          #     resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
-          #     resource= item,
-          #     region= self.get_cloud_client().get_azresource_location(resource= item),
-          #     resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
-          #   ),
-          #   {
-          #     "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #     "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #       load_balancers_by_nics = tasks["load_balancers"].result()
-          #     ),
-          #   },
-          # ]) for item in self.get_cloud_client().sdk_request(
-          #  tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          #  lambda_sdk_command=lambda: client.virtual_machines.list_all()
-          # )
-        ]
+      "account": account,
+      "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
+          {},
+          self.get_base_return_data(
+            account= self.get_cloud_client().serialize_azresource(resource= account),
+            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+            resource= item,
+            region= self.get_cloud_client().get_azresource_location(resource= item),
+            resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
+          ),
+          {
+            "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
+            "extra_vmss_vms": [ self.get_cloud_client().serialize_azresource(vm) for vm in client.virtual_machine_scale_set_vms.list(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(item), virtual_machine_scale_set_name= item.name) ]
+          },
+          ]) for item in self.get_cloud_client().sdk_request(
+          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+          lambda_sdk_command=lambda: client.virtual_machine_scale_sets.list_all()
+        )
+      ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.base_class.base import cloud_data_client_azure_client_action_base as base
 import asyncio
-from azure.mgmt.keyvault import KeyVaultManagementClient
-from azure.keyvault.secrets import SecretClient
-from azure.keyvault.keys import KeyClient
-from azure.keyvault.administration import KeyVaultAccessControlClient
+from azure.mgmt.redis import RedisManagementClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
-      data_action="datawarehouse", 
-      logger_name= "cloud_data_client_azure_client_action_datawarehouse", 
+      data_action="memorydb", 
+      logger_name= "cloud_data_client_azure_client_action_memorydb", 
       uniqueid_lambda = lambda: True,
       *args, **kwargs)
   
  
   async def _process_account_data(self, account, loop, *args, **kwargs):
     
-    # WIP
-    #  redshift/synapse
+    client = RedisManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
     
     return {
         "account": account,
         "data": [
-          #  self.get_common().helper_type().dictionary().merge_dictionary([
-          #   {},
-          #   self.get_base_return_data(
-          #     account= self.get_cloud_client().serialize_azresource(resource= account),
-          #     resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
-          #     resource= item,
-          #     region= self.get_cloud_client().get_azresource_location(resource= item),
-          #     resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
-          #   ),
-          #   {
-          #     "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-          #     "extra_availability_set": tasks["availability_sets"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #     "extra_nics": tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #     "extra_load_balancers": await self._process_account_data_get_vm_load_balancers(
-          #       vm_nics= tasks["nics"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item)),
-          #       load_balancers_by_nics = tasks["load_balancers"].result()
-          #     ),
-          #   },
-          # ]) for item in self.get_cloud_client().sdk_request(
-          #  tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          #  lambda_sdk_command=lambda: client.virtual_machines.list_all()
-          # )
+           self.get_common().helper_type().dictionary().merge_dictionary([
+            {},
+            self.get_base_return_data(
+              account= self.get_cloud_client().serialize_azresource(resource= account),
+              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+              resource= item,
+              region= self.get_cloud_client().get_azresource_location(resource= item),
+              resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
+            ),
+            {
+              
+            },
+          ]) for item in self.get_cloud_client().sdk_request(
+           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+           lambda_sdk_command=lambda: client.redis.list_by_subscription()
+          )
         ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 from threemystic_cloud_data_client.cloud_providers.azure.client.actions.base_class.base import cloud_data_client_azure_client_action_base as base
 import asyncio
-from azure.mgmt.compute import ComputeManagementClient
-from azure.mgmt.resource import ResourceManagementClient
+from azure.mgmt.synapse import SynapseManagementClient
 
 
 class cloud_data_client_azure_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
-      data_action="vmss", 
-      logger_name= "cloud_data_client_azure_client_action_vmss", 
-      uniqueid_lambda = lambda: True, 
+      data_action="datawarehouse", 
+      logger_name= "cloud_data_client_azure_client_action_datawarehouse", 
+      uniqueid_lambda = lambda: True,
       *args, **kwargs)
   
-  
-    
-  async def __process_get_resources_vmss(self, account, *args, **kwargs):
-    resource_client = ResourceManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
-    try:
-      return { self.get_cloud_client().get_resource_id_from_resource(resource= resource): resource for resource in self.get_cloud_client().sdk_request(
-          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          lambda_sdk_command=lambda: resource_client.resources.list(filter="resourceType eq 'Microsoft.Compute/virtualMachineScaleSets'", expand="createdTime,changedTime,provisioningState")
-        )
-      }
-    except:
-      return []
-        
+ 
   async def _process_account_data(self, account, loop, *args, **kwargs):
-    client = ComputeManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
-    tasks = {
-      "resource": loop.create_task(self.__process_get_resources_vmss(account= account))
-    }
-
-    await asyncio.wait(tasks.values())
-
+    
+    client = SynapseManagementClient(credential= self.get_cloud_client().get_tenant_credential(tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True)), subscription_id= self.get_cloud_client().get_account_id(account= account))
+    
     return {
-      "account": account,
-      "data": [ self.get_common().helper_type().dictionary().merge_dictionary([
-          {},
-          self.get_base_return_data(
-            account= self.get_cloud_client().serialize_azresource(resource= account),
-            resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
-            resource= item,
-            region= self.get_cloud_client().get_azresource_location(resource= item),
-            resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
-          ),
-          {
-            "extra_resource": self.get_cloud_client().serialize_azresource(tasks["resource"].result().get(self.get_cloud_client().get_resource_id_from_resource(resource= item))),
-            "extra_vmss_vms": [ self.get_cloud_client().serialize_azresource(vm) for vm in client.virtual_machine_scale_set_vms.list(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(item), virtual_machine_scale_set_name= item.name) ]
-          },
+        "account": account,
+        "data": [
+           self.get_common().helper_type().dictionary().merge_dictionary([
+            {},
+            self.get_base_return_data(
+              account= self.get_cloud_client().serialize_azresource(resource= account),
+              resource_id= self.get_cloud_client().get_resource_id_from_resource(resource= item),
+              resource= item,
+              region= self.get_cloud_client().get_azresource_location(resource= item),
+              resource_groups= [self.get_cloud_client().get_resource_group_from_resource(resource= item)],
+            ),
+            {
+              "extra_sql_pools": [
+                self.get_cloud_client().serialize_azresource(resource= pool)
+                for pool in client.sql_pools.list_by_workspace(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(resource= item), workspace_name= item.name)
+              ],
+              "extra_big_data_pools": [
+                self.get_cloud_client().serialize_azresource(resource= pool)
+                for pool in client.big_data_pools.list_by_workspace(resource_group_name= self.get_cloud_client().get_resource_group_from_resource(resource= item), workspace_name= item.name)
+              ] 
+            },
           ]) for item in self.get_cloud_client().sdk_request(
-          tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
-          lambda_sdk_command=lambda: client.virtual_machine_scale_sets.list_all()
-        )
-      ]
+           tenant= self.get_cloud_client().get_tenant_id(tenant= account, is_account= True), 
+           lambda_sdk_command=lambda: client.workspaces.list()
+          )
+        ]
     }
```

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,39 @@
         "const": "vmss",
         "dest": "data_action",
         "help": "Data Action: This pulls either ASG or VMSS depending on the provider",
         "action": 'store_const'
       }
     }
   
+  def get_data_only_parser_args_actions(self, *args, **kwargs):
+    return {
+      "--dns": {
+        "default": None, 
+        "const": "dns",
+        "dest": "data_action",
+        "help": "Data Action: This pulls DNS Data (private DNS/Public/Route53)",
+        "action": 'store_const'
+      },
+      "--datawarehouse": {
+        "default": None, 
+        "const": "datawarehouse",
+        "dest": "data_action",
+        "help": "Data Action: This pulls Data Warehouse (Synapse/RedShift)",
+        "action": 'store_const'
+      },
+      "--db": {
+        "default": None, 
+        "const": "database",
+        "dest": "data_action",
+        "help": "Data Action: This pulls the various non-inmemory databses",
+        "action": 'store_const'
+      },
+    }
+  
   def get_parser_args(self, *args, **kwargs):
     if hasattr(self, "_data_parser_args"):
       return self._data_parser_args
     
     
     self._data_parser_args = self.get_common().helper_type().dictionary().merge_dictionary([
       {},
@@ -99,14 +124,15 @@
           "type": str,
           "dest": "data_accounts",
           "help": "Filter: A comma seperated list of accounts to filter, put a minus to exclude accounts. 123454,12345,-234534",
           "action": 'store'
         }
       },
       self.get_default_parser_args_actions(),
+      self.get_data_only_parser_args_actions()
     ])
     return self.get_parser_args()
   
   def get_suppres_parser_help(self, *args, **kwargs):
     if hasattr(self, "_suppres_parser_help"):
       return self._suppres_parser_help
     return False
```

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.8/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/.gitignore` & `threemystic_cloud_data_client-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/LICENSE` & `threemystic_cloud_data_client-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/README.md` & `threemystic_cloud_data_client-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/hatch.toml` & `threemystic_cloud_data_client-0.1.8/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.7/pyproject.toml` & `threemystic_cloud_data_client-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -23,30 +23,38 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.4",
-  "threemystic-cloud-client >= 0.1.6",
+  "threemystic-common >= 0.1.5",
+  "threemystic-cloud-client >= 0.1.14",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
-  "azure-mgmt-subscription == 3.*",
-  "azure-mgmt-managementgroups == 1.*",
-  "azure-mgmt-resourcegraph == 8.*",
-  "azure-mgmt-costmanagement == 4.*",
-  "azure-mgmt-network == 23.*",
-  "azure-mgmt-monitor == 5.*",
-  "azure-mgmt-keyvault == 10.*",
-  "azure-keyvault-administration == 4.*",
-  "azure-keyvault-certificates == 4.*",
-  "azure-keyvault-keys == 4.*",
-  "azure-keyvault-secrets == 4.*",
+  "azure-mgmt-cosmosdb >= 9",
+  "azure-mgmt-costmanagement >= 4",
+  "azure-mgmt-dns >= 8",
+  "azure-mgmt-keyvault >= 10",
+  "azure-mgmt-managementgroups >= 1",
+  "azure-mgmt-monitor >= 5",
+  "azure-mgmt-network >= 23",
+  "azure-mgmt-privatedns >= 1",
+  "azure-mgmt-rdbms >= 10",
+  "azure-mgmt-redis >= 14",
+  "azure-mgmt-resourcegraph >= 8",
+  "azure-mgmt-sql >= 3",
+  "azure-mgmt-sqlvirtualmachine >= 0.6",
+  "azure-mgmt-subscription >= 3",
+  "azure-mgmt-synapse >= 2",
+  "azure-keyvault-administration >= 4",
+  "azure-keyvault-certificates >= 4",
+  "azure-keyvault-keys >= 4",
+  "azure-keyvault-secrets >= 4",
 
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/3MysticApes/3mystic_cloud_data_client"
 "Bug Tracker" = "https://github.com/3MysticApes/3mystic_cloud_data_client/issues"
```

### Comparing `threemystic_cloud_data_client-0.1.7/PKG-INFO` & `threemystic_cloud_data_client-0.1.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -14,28 +14,36 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
-Requires-Dist: azure-keyvault-administration==4.*
-Requires-Dist: azure-keyvault-certificates==4.*
-Requires-Dist: azure-keyvault-keys==4.*
-Requires-Dist: azure-keyvault-secrets==4.*
-Requires-Dist: azure-mgmt-costmanagement==4.*
-Requires-Dist: azure-mgmt-keyvault==10.*
-Requires-Dist: azure-mgmt-managementgroups==1.*
-Requires-Dist: azure-mgmt-monitor==5.*
-Requires-Dist: azure-mgmt-network==23.*
-Requires-Dist: azure-mgmt-resourcegraph==8.*
-Requires-Dist: azure-mgmt-subscription==3.*
+Requires-Dist: azure-keyvault-administration>=4
+Requires-Dist: azure-keyvault-certificates>=4
+Requires-Dist: azure-keyvault-keys>=4
+Requires-Dist: azure-keyvault-secrets>=4
+Requires-Dist: azure-mgmt-cosmosdb>=9
+Requires-Dist: azure-mgmt-costmanagement>=4
+Requires-Dist: azure-mgmt-dns>=8
+Requires-Dist: azure-mgmt-keyvault>=10
+Requires-Dist: azure-mgmt-managementgroups>=1
+Requires-Dist: azure-mgmt-monitor>=5
+Requires-Dist: azure-mgmt-network>=23
+Requires-Dist: azure-mgmt-privatedns>=1
+Requires-Dist: azure-mgmt-rdbms>=10
+Requires-Dist: azure-mgmt-redis>=14
+Requires-Dist: azure-mgmt-resourcegraph>=8
+Requires-Dist: azure-mgmt-sql>=3
+Requires-Dist: azure-mgmt-sqlvirtualmachine>=0.6
+Requires-Dist: azure-mgmt-subscription>=3
+Requires-Dist: azure-mgmt-synapse>=2
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.6
-Requires-Dist: threemystic-common>=0.1.4
+Requires-Dist: threemystic-cloud-client>=0.1.14
+Requires-Dist: threemystic-common>=0.1.5
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
 Currently supports AWS/Azure
```


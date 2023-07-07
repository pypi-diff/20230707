# Comparing `tmp/ignos-api-client-2023.6.14.5376.tar.gz` & `tmp/ignos-api-client-2023.7.7.5556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignos-api-client-2023.6.14.5376.tar", last modified: Wed Jun 14 13:11:17 2023, max compression
+gzip compressed data, was "ignos-api-client-2023.7.7.5556.tar", last modified: Fri Jul  7 07:21:56 2023, max compression
```

## Comparing `ignos-api-client-2023.6.14.5376.tar` & `ignos-api-client-2023.7.7.5556.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/
--rw-r--r--   0 vsts      (1001) docker     (123)      171 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.022585 ignos-api-client-2023.6.14.5376/ignos/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.022585 ignos-api-client-2023.6.14.5376/ignos/api/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.026585 ignos-api-client-2023.6.14.5376/ignos/api/client/
--rw-r--r--   0 vsts      (1001) docker     (123)      866 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14050 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_vendor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.030585 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/
--rw-r--r--   0 vsts      (1001) docker     (123)      813 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14349 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2985 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.030585 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3657 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   863930 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.034585 ignos-api-client-2023.6.14.5376/ignos/api/client/models/
--rw-r--r--   0 vsts      (1001) docker     (123)    26096 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4978 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)   669585 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/models/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3657 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)  1055635 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      171 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      986 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-14 13:11:17.000000 ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-14 13:11:17.038585 ignos-api-client-2023.6.14.5376/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-06-14 13:11:07.000000 ignos-api-client-2023.6.14.5376/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.110681 ignos-api-client-2023.7.7.5556/
+-rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-07-07 07:21:56.110681 ignos-api-client-2023.7.7.5556/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.102681 ignos-api-client-2023.7.7.5556/ignos/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.102681 ignos-api-client-2023.7.7.5556/ignos/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.102681 ignos-api-client-2023.7.7.5556/ignos/api/client/
+-rw-r--r--   0 vsts      (1001) docker     (123)      866 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15043 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/_vendor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      494 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.106681 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/
+-rw-r--r--   0 vsts      (1001) docker     (123)      813 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15358 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2985 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.106681 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3933 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   917642 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.106681 ignos-api-client-2023.7.7.5556/ignos/api/client/models/
+-rw-r--r--   0 vsts      (1001) docker     (123)    28376 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7278 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/models/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   738404 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/models/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/models/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.110681 ignos-api-client-2023.7.7.5556/ignos/api/client/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3933 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  1119094 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/ignos/api/client/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-07 07:21:56.110681 ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      170 2023-07-07 07:21:56.000000 ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      986 2023-07-07 07:21:56.000000 ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-07 07:21:56.000000 ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-07-07 07:21:56.000000 ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-07 07:21:56.000000 ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-07 07:21:56.110681 ignos-api-client-2023.7.7.5556/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      957 2023-07-07 07:21:45.000000 ignos-api-client-2023.7.7.5556/setup.py
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/__init__.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/_client.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     AzureRegionsOperations,
     CdfOperations,
     CncFileTransferOperations,
     CncSetupOperations,
     CountriesOperations,
     CustomerOrdersOperations,
     CustomersOperations,
+    DocumentTypesOperations,
+    DocumentsOperations,
     ElectricalOperations,
     ExternalAccessOperations,
     ExternalOperations,
     ExternalServicesOperations,
     LinksOperations,
     MachineAlarmsOperations,
     MachineUtilizationOperations,
@@ -37,20 +39,22 @@
     MeasurementFormSchemasOperations,
     MeasurementFormsInstancesOperations,
     MeasuringToolsOperations,
     MesOperations,
     MesProductionOrderOperations,
     MesProductionScheduleOperations,
     MesResourceOperations,
+    MrbOperations,
     OperatorCalculatorsOperations,
     PowerOperations,
     PresentationOperations,
     SuppliersOperations,
     SustainabilityOperations,
     SystemHealthDashboardOperations,
+    TraceOperations,
     UploadOperations,
     UsersOperations,
     WeldingOperations,
     WorkordersOperations,
     WorkspaceTemplatesAdminOperations,
     WorkspaceTemplatesOperations,
     WorkspacesOperations,
@@ -76,14 +80,18 @@
     :vartype cnc_file_transfer: ignos.api.client.operations.CncFileTransferOperations
     :ivar cnc_setup: CncSetupOperations operations
     :vartype cnc_setup: ignos.api.client.operations.CncSetupOperations
     :ivar countries: CountriesOperations operations
     :vartype countries: ignos.api.client.operations.CountriesOperations
     :ivar customers: CustomersOperations operations
     :vartype customers: ignos.api.client.operations.CustomersOperations
+    :ivar documents: DocumentsOperations operations
+    :vartype documents: ignos.api.client.operations.DocumentsOperations
+    :ivar document_types: DocumentTypesOperations operations
+    :vartype document_types: ignos.api.client.operations.DocumentTypesOperations
     :ivar customer_orders: CustomerOrdersOperations operations
     :vartype customer_orders: ignos.api.client.operations.CustomerOrdersOperations
     :ivar workorders: WorkordersOperations operations
     :vartype workorders: ignos.api.client.operations.WorkordersOperations
     :ivar external: ExternalOperations operations
     :vartype external: ignos.api.client.operations.ExternalOperations
     :ivar external_access: ExternalAccessOperations operations
@@ -115,26 +123,30 @@
     :vartype mes: ignos.api.client.operations.MesOperations
     :ivar mes_production_order: MesProductionOrderOperations operations
     :vartype mes_production_order: ignos.api.client.operations.MesProductionOrderOperations
     :ivar mes_production_schedule: MesProductionScheduleOperations operations
     :vartype mes_production_schedule: ignos.api.client.operations.MesProductionScheduleOperations
     :ivar mes_resource: MesResourceOperations operations
     :vartype mes_resource: ignos.api.client.operations.MesResourceOperations
+    :ivar mrb: MrbOperations operations
+    :vartype mrb: ignos.api.client.operations.MrbOperations
     :ivar operator_calculators: OperatorCalculatorsOperations operations
     :vartype operator_calculators: ignos.api.client.operations.OperatorCalculatorsOperations
     :ivar power: PowerOperations operations
     :vartype power: ignos.api.client.operations.PowerOperations
     :ivar presentation: PresentationOperations operations
     :vartype presentation: ignos.api.client.operations.PresentationOperations
     :ivar suppliers: SuppliersOperations operations
     :vartype suppliers: ignos.api.client.operations.SuppliersOperations
     :ivar sustainability: SustainabilityOperations operations
     :vartype sustainability: ignos.api.client.operations.SustainabilityOperations
     :ivar system_health_dashboard: SystemHealthDashboardOperations operations
     :vartype system_health_dashboard: ignos.api.client.operations.SystemHealthDashboardOperations
+    :ivar trace: TraceOperations operations
+    :vartype trace: ignos.api.client.operations.TraceOperations
     :ivar upload: UploadOperations operations
     :vartype upload: ignos.api.client.operations.UploadOperations
     :ivar users: UsersOperations operations
     :vartype users: ignos.api.client.operations.UsersOperations
     :ivar workspaces: WorkspacesOperations operations
     :vartype workspaces: ignos.api.client.operations.WorkspacesOperations
     :ivar workspace_templates_admin: WorkspaceTemplatesAdminOperations operations
@@ -162,14 +174,16 @@
         self.cdf = CdfOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cnc_file_transfer = CncFileTransferOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.cnc_setup = CncSetupOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customers = CustomersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.documents = DocumentsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.document_types = DocumentTypesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customer_orders = CustomerOrdersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workorders = WorkordersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external = ExternalOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_access = ExternalAccessOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_services = ExternalServicesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -193,24 +207,26 @@
         self.mes_production_order = MesProductionOrderOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.mes_production_schedule = MesProductionScheduleOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.mes_resource = MesResourceOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.mrb = MrbOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operator_calculators = OperatorCalculatorsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.power = PowerOperations(self._client, self._config, self._serialize, self._deserialize)
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.suppliers = SuppliersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sustainability = SustainabilityOperations(self._client, self._config, self._serialize, self._deserialize)
         self.system_health_dashboard = SystemHealthDashboardOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.trace = TraceOperations(self._client, self._config, self._serialize, self._deserialize)
         self.upload = UploadOperations(self._client, self._config, self._serialize, self._deserialize)
         self.users = UsersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspaces = WorkspacesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspace_templates_admin = WorkspaceTemplatesAdminOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.workspace_templates = WorkspaceTemplatesOperations(
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/_configuration.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/_patch.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/_serialization.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/_serialization.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/_vendor.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/_vendor.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/__init__.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_client.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     AzureRegionsOperations,
     CdfOperations,
     CncFileTransferOperations,
     CncSetupOperations,
     CountriesOperations,
     CustomerOrdersOperations,
     CustomersOperations,
+    DocumentTypesOperations,
+    DocumentsOperations,
     ElectricalOperations,
     ExternalAccessOperations,
     ExternalOperations,
     ExternalServicesOperations,
     LinksOperations,
     MachineAlarmsOperations,
     MachineUtilizationOperations,
@@ -37,20 +39,22 @@
     MeasurementFormSchemasOperations,
     MeasurementFormsInstancesOperations,
     MeasuringToolsOperations,
     MesOperations,
     MesProductionOrderOperations,
     MesProductionScheduleOperations,
     MesResourceOperations,
+    MrbOperations,
     OperatorCalculatorsOperations,
     PowerOperations,
     PresentationOperations,
     SuppliersOperations,
     SustainabilityOperations,
     SystemHealthDashboardOperations,
+    TraceOperations,
     UploadOperations,
     UsersOperations,
     WeldingOperations,
     WorkordersOperations,
     WorkspaceTemplatesAdminOperations,
     WorkspaceTemplatesOperations,
     WorkspacesOperations,
@@ -76,14 +80,18 @@
     :vartype cnc_file_transfer: ignos.api.client.aio.operations.CncFileTransferOperations
     :ivar cnc_setup: CncSetupOperations operations
     :vartype cnc_setup: ignos.api.client.aio.operations.CncSetupOperations
     :ivar countries: CountriesOperations operations
     :vartype countries: ignos.api.client.aio.operations.CountriesOperations
     :ivar customers: CustomersOperations operations
     :vartype customers: ignos.api.client.aio.operations.CustomersOperations
+    :ivar documents: DocumentsOperations operations
+    :vartype documents: ignos.api.client.aio.operations.DocumentsOperations
+    :ivar document_types: DocumentTypesOperations operations
+    :vartype document_types: ignos.api.client.aio.operations.DocumentTypesOperations
     :ivar customer_orders: CustomerOrdersOperations operations
     :vartype customer_orders: ignos.api.client.aio.operations.CustomerOrdersOperations
     :ivar workorders: WorkordersOperations operations
     :vartype workorders: ignos.api.client.aio.operations.WorkordersOperations
     :ivar external: ExternalOperations operations
     :vartype external: ignos.api.client.aio.operations.ExternalOperations
     :ivar external_access: ExternalAccessOperations operations
@@ -117,27 +125,31 @@
     :ivar mes_production_order: MesProductionOrderOperations operations
     :vartype mes_production_order: ignos.api.client.aio.operations.MesProductionOrderOperations
     :ivar mes_production_schedule: MesProductionScheduleOperations operations
     :vartype mes_production_schedule:
      ignos.api.client.aio.operations.MesProductionScheduleOperations
     :ivar mes_resource: MesResourceOperations operations
     :vartype mes_resource: ignos.api.client.aio.operations.MesResourceOperations
+    :ivar mrb: MrbOperations operations
+    :vartype mrb: ignos.api.client.aio.operations.MrbOperations
     :ivar operator_calculators: OperatorCalculatorsOperations operations
     :vartype operator_calculators: ignos.api.client.aio.operations.OperatorCalculatorsOperations
     :ivar power: PowerOperations operations
     :vartype power: ignos.api.client.aio.operations.PowerOperations
     :ivar presentation: PresentationOperations operations
     :vartype presentation: ignos.api.client.aio.operations.PresentationOperations
     :ivar suppliers: SuppliersOperations operations
     :vartype suppliers: ignos.api.client.aio.operations.SuppliersOperations
     :ivar sustainability: SustainabilityOperations operations
     :vartype sustainability: ignos.api.client.aio.operations.SustainabilityOperations
     :ivar system_health_dashboard: SystemHealthDashboardOperations operations
     :vartype system_health_dashboard:
      ignos.api.client.aio.operations.SystemHealthDashboardOperations
+    :ivar trace: TraceOperations operations
+    :vartype trace: ignos.api.client.aio.operations.TraceOperations
     :ivar upload: UploadOperations operations
     :vartype upload: ignos.api.client.aio.operations.UploadOperations
     :ivar users: UsersOperations operations
     :vartype users: ignos.api.client.aio.operations.UsersOperations
     :ivar workspaces: WorkspacesOperations operations
     :vartype workspaces: ignos.api.client.aio.operations.WorkspacesOperations
     :ivar workspace_templates_admin: WorkspaceTemplatesAdminOperations operations
@@ -165,14 +177,16 @@
         self.cdf = CdfOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cnc_file_transfer = CncFileTransferOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.cnc_setup = CncSetupOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customers = CustomersOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.documents = DocumentsOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.document_types = DocumentTypesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customer_orders = CustomerOrdersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workorders = WorkordersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external = ExternalOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_access = ExternalAccessOperations(self._client, self._config, self._serialize, self._deserialize)
         self.external_services = ExternalServicesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -196,24 +210,26 @@
         self.mes_production_order = MesProductionOrderOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.mes_production_schedule = MesProductionScheduleOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.mes_resource = MesResourceOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.mrb = MrbOperations(self._client, self._config, self._serialize, self._deserialize)
         self.operator_calculators = OperatorCalculatorsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.power = PowerOperations(self._client, self._config, self._serialize, self._deserialize)
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.suppliers = SuppliersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sustainability = SustainabilityOperations(self._client, self._config, self._serialize, self._deserialize)
         self.system_health_dashboard = SystemHealthDashboardOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.trace = TraceOperations(self._client, self._config, self._serialize, self._deserialize)
         self.upload = UploadOperations(self._client, self._config, self._serialize, self._deserialize)
         self.users = UsersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspaces = WorkspacesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.workspace_templates_admin = WorkspaceTemplatesAdminOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.workspace_templates = WorkspaceTemplatesOperations(
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_configuration.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/_patch.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/__init__.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ._operations import AssetsOperations
 from ._operations import AzureRegionsOperations
 from ._operations import CdfOperations
 from ._operations import CncFileTransferOperations
 from ._operations import CncSetupOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
+from ._operations import DocumentsOperations
+from ._operations import DocumentTypesOperations
 from ._operations import CustomerOrdersOperations
 from ._operations import WorkordersOperations
 from ._operations import ExternalOperations
 from ._operations import ExternalAccessOperations
 from ._operations import ExternalServicesOperations
 from ._operations import ElectricalOperations
 from ._operations import WeldingOperations
@@ -29,20 +31,22 @@
 from ._operations import MeasurementFormSchemasOperations
 from ._operations import MeasurementFormsInstancesOperations
 from ._operations import MeasuringToolsOperations
 from ._operations import MesOperations
 from ._operations import MesProductionOrderOperations
 from ._operations import MesProductionScheduleOperations
 from ._operations import MesResourceOperations
+from ._operations import MrbOperations
 from ._operations import OperatorCalculatorsOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
 from ._operations import SuppliersOperations
 from ._operations import SustainabilityOperations
 from ._operations import SystemHealthDashboardOperations
+from ._operations import TraceOperations
 from ._operations import UploadOperations
 from ._operations import UsersOperations
 from ._operations import WorkspacesOperations
 from ._operations import WorkspaceTemplatesAdminOperations
 from ._operations import WorkspaceTemplatesOperations
 
 from ._patch import __all__ as _patch_all
@@ -54,14 +58,16 @@
     "AssetsOperations",
     "AzureRegionsOperations",
     "CdfOperations",
     "CncFileTransferOperations",
     "CncSetupOperations",
     "CountriesOperations",
     "CustomersOperations",
+    "DocumentsOperations",
+    "DocumentTypesOperations",
     "CustomerOrdersOperations",
     "WorkordersOperations",
     "ExternalOperations",
     "ExternalAccessOperations",
     "ExternalServicesOperations",
     "ElectricalOperations",
     "WeldingOperations",
@@ -73,20 +79,22 @@
     "MeasurementFormSchemasOperations",
     "MeasurementFormsInstancesOperations",
     "MeasuringToolsOperations",
     "MesOperations",
     "MesProductionOrderOperations",
     "MesProductionScheduleOperations",
     "MesResourceOperations",
+    "MrbOperations",
     "OperatorCalculatorsOperations",
     "PowerOperations",
     "PresentationOperations",
     "SuppliersOperations",
     "SustainabilityOperations",
     "SystemHealthDashboardOperations",
+    "TraceOperations",
     "UploadOperations",
     "UsersOperations",
     "WorkspacesOperations",
     "WorkspaceTemplatesAdminOperations",
     "WorkspaceTemplatesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_operations.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,23 @@
     build_countries_list_countries_request,
     build_customer_orders_upsert_customer_order_line_request,
     build_customer_orders_upsert_customer_order_request,
     build_customers_delete_customer_request,
     build_customers_get_current_customer_request,
     build_customers_list_customers_request,
     build_customers_upsert_customer_request,
+    build_document_types_active_document_type_request,
+    build_document_types_create_document_type_request,
+    build_document_types_deactive_document_type_request,
+    build_document_types_delete_document_type_request,
+    build_document_types_list_available_tags_for_document_type_request,
+    build_document_types_list_document_types_request,
+    build_document_types_update_document_type_request,
+    build_documents_import_document_contents_request,
+    build_documents_import_document_request,
     build_electrical_create_electrical_iot_config_request,
     build_electrical_delete_electrical_iot_config_request,
     build_electrical_list_electrical_data_configs_request,
     build_electrical_list_electrical_source_types_request,
     build_external_accept_supplier_invite_request,
     build_external_access_create_company_user_request,
     build_external_access_delete_company_customer_request,
@@ -250,14 +259,20 @@
     build_mes_list_employees_request,
     build_mes_list_production_companies_request,
     build_mes_production_order_get_production_order_request,
     build_mes_production_schedule_list_production_schedule_operations_request,
     build_mes_resource_list_resource_group_resources_request,
     build_mes_resource_list_resource_groups_request,
     build_mes_set_current_production_company_request,
+    build_mrb_attach_pdf_request,
+    build_mrb_create_mrb_template_request,
+    build_mrb_delete_mrb_template_request,
+    build_mrb_get_mrb_template_request,
+    build_mrb_list_mrb_templates_request,
+    build_mrb_update_mrb_template_request,
     build_operator_calculators_calculate_bar_weight_request,
     build_operator_calculators_calculate_right_angled_triangle_request,
     build_operator_calculators_calculate_spindle_and_cutting_speed_request,
     build_operator_calculators_list_materials_with_density_request,
     build_power_list_power_regions_request,
     build_presentation_get_component_settings_request,
     build_suppliers_create_supplier_invite_request,
@@ -270,14 +285,15 @@
     build_sustainability_get_consumption_request,
     build_sustainability_get_customer_order_consumption_request,
     build_sustainability_get_power_request,
     build_sustainability_get_product_consumption_request,
     build_sustainability_get_work_order_consumption_request,
     build_sustainability_test_request,
     build_system_health_dashboard_get_machine_data_health_request,
+    build_trace_get_work_order_trace_request,
     build_upload_create_upload_info_request,
     build_users_list_users_request,
     build_welding_create_welding_iot_config_request,
     build_welding_delete_welding_iot_config_request,
     build_welding_list_electrical_data_configs_request,
     build_welding_list_welding_source_types_request,
     build_workorders_check_resource_status_request,
@@ -291,16 +307,18 @@
     build_workorders_register_workorder_operation_event_request,
     build_workorders_set_workorder_customer_order_reference_request,
     build_workorders_start_workorder_operation_request,
     build_workorders_start_workorder_operation_v2_request,
     build_workorders_stop_workorder_operation_request,
     build_workorders_stop_workorder_operation_v2_request,
     build_workorders_update_workorder_operation_event_timestamps_request,
+    build_workorders_upsert_workorder_consumption_request,
     build_workorders_upsert_workorder_request,
     build_workorders_upsert_workorder_traces_request,
+    build_workorders_upsert_workorder_v2_request,
     build_workspace_templates_admin_create_workspace_template_request,
     build_workspace_templates_admin_delete_workspace_template_request,
     build_workspace_templates_admin_delete_workspace_template_widget_request,
     build_workspace_templates_admin_get_workspace_template_request,
     build_workspace_templates_admin_update_workspace_template_request,
     build_workspace_templates_admin_update_workspace_template_widget_settings_request,
     build_workspace_templates_admin_update_workspace_template_widgets_request,
@@ -5609,14 +5627,615 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class DocumentsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`documents` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    async def import_document(
+        self, body: Optional[_models.ImportDocument] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        """Import document with revisions from other systems.
+
+        Import document with revisions from other systems.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.ImportDocument
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def import_document(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        """Import document with revisions from other systems.
+
+        Import document with revisions from other systems.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: JSON
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def import_document(self, body: Optional[Union[_models.ImportDocument, IO]] = None, **kwargs: Any) -> JSON:
+        """Import document with revisions from other systems.
+
+        Import document with revisions from other systems.
+
+        :param body: Is either a ImportDocument type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.ImportDocument or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: JSON
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "ImportDocument")
+            else:
+                _json = None
+
+        request = build_documents_import_document_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("object", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def import_document_contents(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[JSON] = None, **kwargs: Any
+    ) -> None:
+        """Register imported content for document revisions.
+
+        Register imported content for document revisions.
+
+        :param body: Default value is None.
+        :type body: JSON
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: str = kwargs.pop("content_type", _headers.pop("Content-Type", "application/json"))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        if body is not None:
+            _json = self._serialize.body(body, "object")
+        else:
+            _json = None
+
+        request = build_documents_import_document_contents_request(
+            content_type=content_type,
+            json=_json,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
+class DocumentTypesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`document_types` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace_async
+    async def list_document_types(
+        self, *, include_inactive: bool = False, **kwargs: Any
+    ) -> List[_models.DocumentTypeDto]:
+        """list_document_types.
+
+        :keyword include_inactive: Default value is False.
+        :paramtype include_inactive: bool
+        :return: list of DocumentTypeDto
+        :rtype: list[~ignos.api.client.models.DocumentTypeDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.DocumentTypeDto]] = kwargs.pop("cls", None)
+
+        request = build_document_types_list_document_types_request(
+            include_inactive=include_inactive,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[DocumentTypeDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    async def create_document_type(
+        self,
+        body: Optional[_models.CreateDocumentType] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """create_document_type.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateDocumentType
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_document_type(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """create_document_type.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_document_type(
+        self, body: Optional[Union[_models.CreateDocumentType, IO]] = None, **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """create_document_type.
+
+        :param body: Is either a CreateDocumentType type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.CreateDocumentType or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.DocumentTypeDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateDocumentType")
+            else:
+                _json = None
+
+        request = build_document_types_create_document_type_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("DocumentTypeDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def update_document_type(
+        self, id: str, body: Optional[JSON] = None, **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """update_document_type.
+
+        :param id: Required.
+        :type id: str
+        :param body: Default value is None.
+        :type body: JSON
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: str = kwargs.pop("content_type", _headers.pop("Content-Type", "application/json"))
+        cls: ClsType[_models.DocumentTypeDto] = kwargs.pop("cls", None)
+
+        if body is not None:
+            _json = self._serialize.body(body, "object")
+        else:
+            _json = None
+
+        request = build_document_types_update_document_type_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("DocumentTypeDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def delete_document_type(  # pylint: disable=inconsistent-return-statements
+        self, id: str, **kwargs: Any
+    ) -> None:
+        """Delete document type. Only allowed if not used.
+
+        Delete document type. Only allowed if not used.
+
+        :param id: Required.
+        :type id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_document_types_delete_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace_async
+    async def active_document_type(  # pylint: disable=inconsistent-return-statements
+        self, id: str, **kwargs: Any
+    ) -> None:
+        """active_document_type.
+
+        :param id: Required.
+        :type id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_document_types_active_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace_async
+    async def deactive_document_type(  # pylint: disable=inconsistent-return-statements
+        self, id: str, **kwargs: Any
+    ) -> None:
+        """deactive_document_type.
+
+        :param id: Required.
+        :type id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_document_types_deactive_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace_async
+    async def list_available_tags_for_document_type(self, id: str, **kwargs: Any) -> List[str]:
+        """list_available_tags_for_document_type.
+
+        :param id: Required.
+        :type id: str
+        :return: list of str
+        :rtype: list[str]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[str]] = kwargs.pop("cls", None)
+
+        request = build_document_types_list_available_tags_for_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[str]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+
 class CustomerOrdersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.aio.IgnosPortal`'s
@@ -5988,14 +6607,116 @@
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})
 
+    @overload
+    async def upsert_workorder_v2(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.UpsertWorkorderV2] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Create or update a workorder.
+
+        Create or update a workorder.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkorderV2
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def upsert_workorder_v2(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Create or update a workorder.
+
+        Create or update a workorder.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def upsert_workorder_v2(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.UpsertWorkorderV2, IO]] = None, **kwargs: Any
+    ) -> None:
+        """Create or update a workorder.
+
+        Create or update a workorder.
+
+        :param body: Is either a UpsertWorkorderV2 type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkorderV2 or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpsertWorkorderV2")
+            else:
+                _json = None
+
+        request = build_workorders_upsert_workorder_v2_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
     @distributed_trace_async
     async def list_workorders(
         self,
         *,
         page_size: int = 50,
         search: Optional[str] = None,
         active_orders: Optional[bool] = None,
@@ -6059,14 +6780,129 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @overload
+    async def upsert_workorder_consumption(  # pylint: disable=inconsistent-return-statements
+        self,
+        id: str,
+        body: Optional[_models.UpsertWorkOrderConsumptionsRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Update consumed materials on work order.
+
+        Update consumed materials on work order.
+
+        :param id: Work order id. Required.
+        :type id: str
+        :param body: Consumption details. Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkOrderConsumptionsRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def upsert_workorder_consumption(  # pylint: disable=inconsistent-return-statements
+        self, id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Update consumed materials on work order.
+
+        Update consumed materials on work order.
+
+        :param id: Work order id. Required.
+        :type id: str
+        :param body: Consumption details. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def upsert_workorder_consumption(  # pylint: disable=inconsistent-return-statements
+        self, id: str, body: Optional[Union[_models.UpsertWorkOrderConsumptionsRequest, IO]] = None, **kwargs: Any
+    ) -> None:
+        """Update consumed materials on work order.
+
+        Update consumed materials on work order.
+
+        :param id: Work order id. Required.
+        :type id: str
+        :param body: Consumption details. Is either a UpsertWorkOrderConsumptionsRequest type or a IO
+         type. Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkOrderConsumptionsRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpsertWorkOrderConsumptionsRequest")
+            else:
+                _json = None
+
+        request = build_workorders_upsert_workorder_consumption_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
     async def upsert_workorder_traces(  # pylint: disable=inconsistent-return-statements
         self,
         id: str,
         body: Optional[_models.UpsertWorkorderTracesRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -19656,14 +20492,573 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class MrbOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`mrb` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    async def attach_pdf(  # pylint: disable=inconsistent-return-statements
+        self,
+        template_id: str,
+        body: Optional[_models.AttachPdfRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """attach_pdf.
+
+        :param template_id: Required.
+        :type template_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.AttachPdfRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def attach_pdf(  # pylint: disable=inconsistent-return-statements
+        self, template_id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """attach_pdf.
+
+        :param template_id: Required.
+        :type template_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def attach_pdf(  # pylint: disable=inconsistent-return-statements
+        self, template_id: str, body: Optional[Union[_models.AttachPdfRequest, IO]] = None, **kwargs: Any
+    ) -> None:
+        """attach_pdf.
+
+        :param template_id: Required.
+        :type template_id: str
+        :param body: Is either a AttachPdfRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.AttachPdfRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "AttachPdfRequest")
+            else:
+                _json = None
+
+        request = build_mrb_attach_pdf_request(
+            template_id=template_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace_async
+    async def get_mrb_template(self, template_id: str, **kwargs: Any) -> _models.MrbTemplateDto:
+        """Get a single MRB template by id.
+
+        Get a single MRB template by id.
+
+        :param template_id: Required.
+        :type template_id: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.MrbTemplateDto] = kwargs.pop("cls", None)
+
+        request = build_mrb_get_mrb_template_request(
+            template_id=template_id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("MrbTemplateDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def list_mrb_templates(
+        self, *, customer_id: Optional[str] = None, customer_group_id: Optional[str] = None, **kwargs: Any
+    ) -> List[_models.MrbTemplateDto]:
+        """Get a list of MRB templates.
+
+        Get a list of MRB templates.
+
+        :keyword customer_id: Default value is None.
+        :paramtype customer_id: str
+        :keyword customer_group_id: Default value is None.
+        :paramtype customer_group_id: str
+        :return: list of MrbTemplateDto
+        :rtype: list[~ignos.api.client.models.MrbTemplateDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.MrbTemplateDto]] = kwargs.pop("cls", None)
+
+        request = build_mrb_list_mrb_templates_request(
+            customer_id=customer_id,
+            customer_group_id=customer_group_id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[MrbTemplateDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    async def create_mrb_template(
+        self,
+        body: Optional[_models.CreateMrbTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Create a new MRB template.
+
+        Create a new MRB template.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateMrbTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def create_mrb_template(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Create a new MRB template.
+
+        Create a new MRB template.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def create_mrb_template(
+        self, body: Optional[Union[_models.CreateMrbTemplateRequest, IO]] = None, **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Create a new MRB template.
+
+        Create a new MRB template.
+
+        :param body: Is either a CreateMrbTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.CreateMrbTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MrbTemplateDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateMrbTemplateRequest")
+            else:
+                _json = None
+
+        request = build_mrb_create_mrb_template_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("MrbTemplateDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    async def update_mrb_template(
+        self,
+        body: Optional[_models.UpdateMrbTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Update an MRB template.
+
+        Update an MRB template.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UpdateMrbTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def update_mrb_template(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Update an MRB template.
+
+        Update an MRB template.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def update_mrb_template(
+        self, body: Optional[Union[_models.UpdateMrbTemplateRequest, IO]] = None, **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Update an MRB template.
+
+        Update an MRB template.
+
+        :param body: Is either a UpdateMrbTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.UpdateMrbTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MrbTemplateDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpdateMrbTemplateRequest")
+            else:
+                _json = None
+
+        request = build_mrb_update_mrb_template_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("MrbTemplateDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    async def delete_mrb_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.DeleteMrbTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Delete an MRB template.
+
+        Delete an MRB template.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.DeleteMrbTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def delete_mrb_template(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Delete an MRB template.
+
+        Delete an MRB template.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def delete_mrb_template(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.DeleteMrbTemplateRequest, IO]] = None, **kwargs: Any
+    ) -> None:
+        """Delete an MRB template.
+
+        Delete an MRB template.
+
+        :param body: Is either a DeleteMrbTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.DeleteMrbTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "DeleteMrbTemplateRequest")
+            else:
+                _json = None
+
+        request = build_mrb_delete_mrb_template_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
 class OperatorCalculatorsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.aio.IgnosPortal`'s
@@ -21249,14 +22644,82 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class TraceOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.aio.IgnosPortal`'s
+        :attr:`trace` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace_async
+    async def get_work_order_trace(self, id: str, **kwargs: Any) -> _models.TraceDto:
+        """get_work_order_trace.
+
+        :param id: Required.
+        :type id: str
+        :return: TraceDto
+        :rtype: ~ignos.api.client.models.TraceDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.TraceDto] = kwargs.pop("cls", None)
+
+        request = build_trace_get_work_order_trace_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("TraceDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+
 class UploadOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.aio.IgnosPortal`'s
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/aio/operations/_patch.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/models/__init__.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ._models import AssetComsumptionDto
 from ._models import AssetDto
 from ._models import AssetDtoPagedResult
 from ._models import AssetPowerDto
 from ._models import AssetSimpleStructureDto
 from ._models import AssetStructureDto
 from ._models import AttachCalibrationCertificateRequest
+from ._models import AttachPdfRequest
 from ._models import AzureRegionDto
 from ._models import BatchInsertValueRequest
 from ._models import BatchInsertValuesResponseDto
 from ._models import CalculateBarWeight
 from ._models import CalculateRightAngledTriangle
 from ._models import CalculateSpindleAndCuttingSpeed
 from ._models import CalibrationListToolDto
@@ -51,55 +52,64 @@
 from ._models import CreateAsset
 from ._models import CreateCncMachine
 from ._models import CreateCncMachineOperation
 from ._models import CreateCncMachineOperationToolRequest
 from ._models import CreateCncPart
 from ._models import CreateCompanyUserRequest
 from ._models import CreateCustomerOrderLineGhgReport
+from ._models import CreateDocumentType
 from ._models import CreateElectricalIotConfig
 from ._models import CreateLinkRequest
 from ._models import CreateMachineGroup
 from ._models import CreateMachineGroupResponse
 from ._models import CreateMeasurementFormInstanceRequest
 from ._models import CreateMeasurementFormMapping
 from ._models import CreateMeasurementFormSchema
 from ._models import CreateMeasurementFormSchemaFeedbackRequest
 from ._models import CreateMeasurementFormSchemaLinkRequest
 from ._models import CreateMeasuringToolManufacturer
 from ._models import CreateMeasuringToolRequest
 from ._models import CreateMeasuringToolSubTypeRequest
 from ._models import CreateMeasuringToolType
 from ._models import CreateMeasuringUnit
+from ._models import CreateMrbTemplateRequest
 from ._models import CreateSchemaElement
 from ._models import CreateSupplierInvite
 from ._models import CreateWorkspace
 from ._models import CreateWorkspaceFromTemplate
 from ._models import CreateWorkspaceTemplate
 from ._models import CurrentCustomerDto
 from ._models import CustomerDto
 from ._models import CustomerDtoPagedResult
 from ._models import CustomerOrderConsumptionRequest
 from ._models import CustomerOrderInfoDto
 from ._models import CustomerOrderLineDto
 from ._models import DataHealthDto
+from ._models import DeleteMrbTemplateRequest
 from ._models import DeletePartDrawingRequest
 from ._models import DeprecateToolRequest
+from ._models import DocumentRevisionApprovalDto
+from ._models import DocumentSubTypeDto
+from ._models import DocumentTagDto
+from ._models import DocumentTypeDto
 from ._models import DownloadDto
 from ._models import ElectricalIotConfigDto
 from ._models import EmployeeDto
 from ._models import ExportDimensionReportRequest
 from ._models import ExternalRoleDto
 from ._models import ExternalServiceCredentialDto
 from ._models import ExternalSupplierDto
 from ._models import FactoryUtilizationDto
 from ._models import FileDto
 from ._models import FilterWorkorderOperationEvents
 from ._models import GetConsumption
 from ._models import GetPower
 from ._models import ImageFileDto
+from ._models import ImportDocument
+from ._models import ImportDocumentRevisionDto
 from ._models import ImportMeasurementFormInstanceRequest
 from ._models import ImportMeasurementFormInstanceSchemaToolDto
 from ._models import ImportMeasurementFormInstanceSchemaValueDto
 from ._models import ImportMeasurementFormInstanceSchemaValuesDto
 from ._models import ImportMeasurementFormInstanceValueRequest
 from ._models import ImportMeasurementFormPartDto
 from ._models import ImportMeasurementFormSchema
@@ -132,14 +142,15 @@
 from ._models import MachineStateDatapoint
 from ._models import MachineStateDto
 from ._models import MachineStateListDto
 from ._models import MachineStatesSummaryDto
 from ._models import MachineUtilizationDto
 from ._models import MachineUtilizationV2Dto
 from ._models import ManufacturerDto
+from ._models import MaterialConsumptionDto
 from ._models import MaterialMassDensityDto
 from ._models import MaterialWeightDto
 from ._models import MeasurementFormBalloonMappingDto
 from ._models import MeasurementFormBalloonMappingRequestDto
 from ._models import MeasurementFormCustomerSettingsDto
 from ._models import MeasurementFormDto
 from ._models import MeasurementFormElementDto
@@ -187,14 +198,16 @@
 from ._models import MeasuringToolDtoPagedData
 from ._models import MeasuringToolSettingsDto
 from ._models import MeasuringToolSubTypeDto
 from ._models import MeasuringToolTypeDto
 from ._models import MeasuringToolWhitelistDto
 from ._models import MeasuringToolWhitelistDtoPagedData
 from ._models import MeasuringUnitDto
+from ._models import MrbTemplateDto
+from ._models import MrbTemplateElementDto
 from ._models import NumericDataPointDto
 from ._models import NumericNullableValueWithTimestamp
 from ._models import OperationPrerequisitesDto
 from ._models import OperatorAndMachineDto
 from ._models import PartDto
 from ._models import PowerDto
 from ._models import PowerOnUtilizationDto
@@ -240,14 +253,19 @@
 from ._models import SubscriberDto
 from ._models import SupplierInviteDto
 from ._models import SurroundingOperationDto
 from ._models import SustainabilityCustomerOrderDto
 from ._models import SustainabilityNodeDto
 from ._models import SustainabilityNodeProcurementInfoDto
 from ._models import SustainabilityPartInfoDto
+from ._models import TraceDto
+from ._models import TraceItemConsumptionDto
+from ._models import TraceItemDto
+from ._models import TraceListItemDto
+from ._models import TraceMaterialDetailDto
 from ._models import UnregisteredToolValueDto
 from ._models import UpdateCdfConfig
 from ._models import UpdateCncMachineCommunicationSettingsRequest
 from ._models import UpdateCncMachineOperationRequest
 from ._models import UpdateCncMachineOperationToolRequest
 from ._models import UpdateCncMachineRequest
 from ._models import UpdateCncMachineToolRequest
@@ -259,14 +277,15 @@
 from ._models import UpdateMeasurementFormInstanceRequest
 from ._models import UpdateMeasurementFormSchemaRequest
 from ._models import UpdateMeasurementFormSettings
 from ._models import UpdateMeasuringToolRequest
 from ._models import UpdateMeasuringToolSettings
 from ._models import UpdateMeasuringToolSubTypeRequest
 from ._models import UpdateMeasuringToolTypeRequest
+from ._models import UpdateMrbTemplateRequest
 from ._models import UpdateSchemaGroupedElementDto
 from ._models import UpdateSchemaGroupedElementsRequest
 from ._models import UpdateSchemaInstanceElementsRequest
 from ._models import UpdateWhitelistedMeasuringTool
 from ._models import UpdateWorkorderOperationEventTimestamps
 from ._models import UpdateWorkspaceRequest
 from ._models import UpdateWorkspaceWidgetSettingsRequest
@@ -279,29 +298,32 @@
 from ._models import UploadFileRequest
 from ._models import UploadInfoDto
 from ._models import UploadPartDrawingRequest
 from ._models import UploadRequest
 from ._models import UpsertCustomerOrderRequest
 from ._models import UpsertCustomerRequest
 from ._models import UpsertSupplierToMeasurementFormInstanceRequest
+from ._models import UpsertWorkOrderConsumptionsRequest
 from ._models import UpsertWorkorder
 from ._models import UpsertWorkorderTracesRequest
+from ._models import UpsertWorkorderV2
 from ._models import UptimeDowntimeDto
 from ._models import UptimeDowntimesDto
 from ._models import UserAppDto
 from ._models import UserDetailsDto
 from ._models import UserDto
 from ._models import UserDtoPagedResult
 from ._models import UtilizationDetailsDto
 from ._models import UtilizationDto
 from ._models import UtilizationListDto
 from ._models import UtilizationSummaryDto
 from ._models import UtilizationWorkorderDto
 from ._models import ValidationRuleDto
 from ._models import WhitelistMeasuringTool
+from ._models import WorkOrderProject
 from ._models import WorkOrderProjectDto
 from ._models import WorkorderCustomerOrderReferenceDto
 from ._models import WorkorderDto
 from ._models import WorkorderHierarchyDto
 from ._models import WorkorderImportTraceItemDto
 from ._models import WorkorderListDto
 from ._models import WorkorderListDtoPagedResult
@@ -316,28 +338,40 @@
 
 from ._enums import BonusType
 from ._enums import CalibrationListStatus
 from ._enums import CalibrationStatusDto
 from ._enums import CncOperationStatus
 from ._enums import CustomerOrderLineStatus
 from ._enums import CustomerOrderStatus
+from ._enums import DocumentNumberKey
+from ._enums import DocumentRequirementStrategy
+from ._enums import DocumentSource
+from ._enums import DocumentStatus
+from ._enums import DocumentTypeCategory
+from ._enums import DocumentTypeSearchOption
+from ._enums import DocumentWorkflowType
+from ._enums import EmptyChapterStrategy
 from ._enums import ExternalServiceName
 from ._enums import FileTransferDirection
 from ._enums import FileTransferStatus
 from ._enums import MachineAlarmType
 from ._enums import MachineState
 from ._enums import MaterialStatus
 from ._enums import MeasurementFormInstanceStatus
 from ._enums import MeasurementFormSource
 from ._enums import MeasurementFormStatus
 from ._enums import MeasurementFormValueType
 from ._enums import MeasurementFrequency
+from ._enums import MrbElementType
 from ._enums import NotificationChannelDto
 from ._enums import OperationStatus
 from ._enums import SchemaFeedbackStatus
+from ._enums import TraceIncludeStatus
+from ._enums import TraceItemStatus
+from ._enums import TraceType
 from ._enums import WorkorderStatus
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AcceptSupplierInviteRequest",
@@ -346,14 +380,15 @@
     "AssetComsumptionDto",
     "AssetDto",
     "AssetDtoPagedResult",
     "AssetPowerDto",
     "AssetSimpleStructureDto",
     "AssetStructureDto",
     "AttachCalibrationCertificateRequest",
+    "AttachPdfRequest",
     "AzureRegionDto",
     "BatchInsertValueRequest",
     "BatchInsertValuesResponseDto",
     "CalculateBarWeight",
     "CalculateRightAngledTriangle",
     "CalculateSpindleAndCuttingSpeed",
     "CalibrationListToolDto",
@@ -385,55 +420,64 @@
     "CreateAsset",
     "CreateCncMachine",
     "CreateCncMachineOperation",
     "CreateCncMachineOperationToolRequest",
     "CreateCncPart",
     "CreateCompanyUserRequest",
     "CreateCustomerOrderLineGhgReport",
+    "CreateDocumentType",
     "CreateElectricalIotConfig",
     "CreateLinkRequest",
     "CreateMachineGroup",
     "CreateMachineGroupResponse",
     "CreateMeasurementFormInstanceRequest",
     "CreateMeasurementFormMapping",
     "CreateMeasurementFormSchema",
     "CreateMeasurementFormSchemaFeedbackRequest",
     "CreateMeasurementFormSchemaLinkRequest",
     "CreateMeasuringToolManufacturer",
     "CreateMeasuringToolRequest",
     "CreateMeasuringToolSubTypeRequest",
     "CreateMeasuringToolType",
     "CreateMeasuringUnit",
+    "CreateMrbTemplateRequest",
     "CreateSchemaElement",
     "CreateSupplierInvite",
     "CreateWorkspace",
     "CreateWorkspaceFromTemplate",
     "CreateWorkspaceTemplate",
     "CurrentCustomerDto",
     "CustomerDto",
     "CustomerDtoPagedResult",
     "CustomerOrderConsumptionRequest",
     "CustomerOrderInfoDto",
     "CustomerOrderLineDto",
     "DataHealthDto",
+    "DeleteMrbTemplateRequest",
     "DeletePartDrawingRequest",
     "DeprecateToolRequest",
+    "DocumentRevisionApprovalDto",
+    "DocumentSubTypeDto",
+    "DocumentTagDto",
+    "DocumentTypeDto",
     "DownloadDto",
     "ElectricalIotConfigDto",
     "EmployeeDto",
     "ExportDimensionReportRequest",
     "ExternalRoleDto",
     "ExternalServiceCredentialDto",
     "ExternalSupplierDto",
     "FactoryUtilizationDto",
     "FileDto",
     "FilterWorkorderOperationEvents",
     "GetConsumption",
     "GetPower",
     "ImageFileDto",
+    "ImportDocument",
+    "ImportDocumentRevisionDto",
     "ImportMeasurementFormInstanceRequest",
     "ImportMeasurementFormInstanceSchemaToolDto",
     "ImportMeasurementFormInstanceSchemaValueDto",
     "ImportMeasurementFormInstanceSchemaValuesDto",
     "ImportMeasurementFormInstanceValueRequest",
     "ImportMeasurementFormPartDto",
     "ImportMeasurementFormSchema",
@@ -466,14 +510,15 @@
     "MachineStateDatapoint",
     "MachineStateDto",
     "MachineStateListDto",
     "MachineStatesSummaryDto",
     "MachineUtilizationDto",
     "MachineUtilizationV2Dto",
     "ManufacturerDto",
+    "MaterialConsumptionDto",
     "MaterialMassDensityDto",
     "MaterialWeightDto",
     "MeasurementFormBalloonMappingDto",
     "MeasurementFormBalloonMappingRequestDto",
     "MeasurementFormCustomerSettingsDto",
     "MeasurementFormDto",
     "MeasurementFormElementDto",
@@ -521,14 +566,16 @@
     "MeasuringToolDtoPagedData",
     "MeasuringToolSettingsDto",
     "MeasuringToolSubTypeDto",
     "MeasuringToolTypeDto",
     "MeasuringToolWhitelistDto",
     "MeasuringToolWhitelistDtoPagedData",
     "MeasuringUnitDto",
+    "MrbTemplateDto",
+    "MrbTemplateElementDto",
     "NumericDataPointDto",
     "NumericNullableValueWithTimestamp",
     "OperationPrerequisitesDto",
     "OperatorAndMachineDto",
     "PartDto",
     "PowerDto",
     "PowerOnUtilizationDto",
@@ -574,14 +621,19 @@
     "SubscriberDto",
     "SupplierInviteDto",
     "SurroundingOperationDto",
     "SustainabilityCustomerOrderDto",
     "SustainabilityNodeDto",
     "SustainabilityNodeProcurementInfoDto",
     "SustainabilityPartInfoDto",
+    "TraceDto",
+    "TraceItemConsumptionDto",
+    "TraceItemDto",
+    "TraceListItemDto",
+    "TraceMaterialDetailDto",
     "UnregisteredToolValueDto",
     "UpdateCdfConfig",
     "UpdateCncMachineCommunicationSettingsRequest",
     "UpdateCncMachineOperationRequest",
     "UpdateCncMachineOperationToolRequest",
     "UpdateCncMachineRequest",
     "UpdateCncMachineToolRequest",
@@ -593,14 +645,15 @@
     "UpdateMeasurementFormInstanceRequest",
     "UpdateMeasurementFormSchemaRequest",
     "UpdateMeasurementFormSettings",
     "UpdateMeasuringToolRequest",
     "UpdateMeasuringToolSettings",
     "UpdateMeasuringToolSubTypeRequest",
     "UpdateMeasuringToolTypeRequest",
+    "UpdateMrbTemplateRequest",
     "UpdateSchemaGroupedElementDto",
     "UpdateSchemaGroupedElementsRequest",
     "UpdateSchemaInstanceElementsRequest",
     "UpdateWhitelistedMeasuringTool",
     "UpdateWorkorderOperationEventTimestamps",
     "UpdateWorkspaceRequest",
     "UpdateWorkspaceWidgetSettingsRequest",
@@ -613,29 +666,32 @@
     "UploadFileRequest",
     "UploadInfoDto",
     "UploadPartDrawingRequest",
     "UploadRequest",
     "UpsertCustomerOrderRequest",
     "UpsertCustomerRequest",
     "UpsertSupplierToMeasurementFormInstanceRequest",
+    "UpsertWorkOrderConsumptionsRequest",
     "UpsertWorkorder",
     "UpsertWorkorderTracesRequest",
+    "UpsertWorkorderV2",
     "UptimeDowntimeDto",
     "UptimeDowntimesDto",
     "UserAppDto",
     "UserDetailsDto",
     "UserDto",
     "UserDtoPagedResult",
     "UtilizationDetailsDto",
     "UtilizationDto",
     "UtilizationListDto",
     "UtilizationSummaryDto",
     "UtilizationWorkorderDto",
     "ValidationRuleDto",
     "WhitelistMeasuringTool",
+    "WorkOrderProject",
     "WorkOrderProjectDto",
     "WorkorderCustomerOrderReferenceDto",
     "WorkorderDto",
     "WorkorderHierarchyDto",
     "WorkorderImportTraceItemDto",
     "WorkorderListDto",
     "WorkorderListDtoPagedResult",
@@ -649,25 +705,37 @@
     "WorkspaceWidgetDto",
     "BonusType",
     "CalibrationListStatus",
     "CalibrationStatusDto",
     "CncOperationStatus",
     "CustomerOrderLineStatus",
     "CustomerOrderStatus",
+    "DocumentNumberKey",
+    "DocumentRequirementStrategy",
+    "DocumentSource",
+    "DocumentStatus",
+    "DocumentTypeCategory",
+    "DocumentTypeSearchOption",
+    "DocumentWorkflowType",
+    "EmptyChapterStrategy",
     "ExternalServiceName",
     "FileTransferDirection",
     "FileTransferStatus",
     "MachineAlarmType",
     "MachineState",
     "MaterialStatus",
     "MeasurementFormInstanceStatus",
     "MeasurementFormSource",
     "MeasurementFormStatus",
     "MeasurementFormValueType",
     "MeasurementFrequency",
+    "MrbElementType",
     "NotificationChannelDto",
     "OperationStatus",
     "SchemaFeedbackStatus",
+    "TraceIncludeStatus",
+    "TraceItemStatus",
+    "TraceType",
     "WorkorderStatus",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/models/_enums.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/models/_enums.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,14 +60,86 @@
     DRAFT = "Draft"
     READY = "Ready"
     ONGOING = "Ongoing"
     COMPLETED = "Completed"
     DELETED = "Deleted"
 
 
+class DocumentNumberKey(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentNumberKey."""
+
+    MULTIPLE = "Multiple"
+    SINGLE_DOCUMENT = "SingleDocument"
+
+
+class DocumentRequirementStrategy(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentRequirementStrategy."""
+
+    NONE = "None"
+    WORK_ORDER = "WorkOrder"
+    LOT = "Lot"
+    DRAWING = "Drawing"
+    CUSTOMER_ORDER_LINE = "CustomerOrderLine"
+
+
+class DocumentSource(int, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentSource."""
+
+    ZERO = 0
+    ONE = 1
+    TWO = 2
+    THREE = 3
+
+
+class DocumentStatus(int, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentStatus."""
+
+    ZERO = 0
+    ONE = 1
+    TWO = 2
+    THREE = 3
+    TEN = 10
+    NINETY = 90
+
+
+class DocumentTypeCategory(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentTypeCategory."""
+
+    GENERAL = "General"
+    PROCEDURE = "Procedure"
+    DRAWING = "Drawing"
+    REPORT = "Report"
+    CERTIFICATE = "Certificate"
+
+
+class DocumentTypeSearchOption(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentTypeSearchOption."""
+
+    INCLUDE_APPROVED = "IncludeApproved"
+    INCLUDE_DRAFT = "IncludeDraft"
+    EXCLUDE = "Exclude"
+
+
+class DocumentWorkflowType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """DocumentWorkflowType."""
+
+    NONE = "None"
+    CUSTOMER_PROVIDED = "CustomerProvided"
+    CUSTOMER_APPROVAL = "CustomerApproval"
+    INTERNAL_WITH_FIX = "InternalWithFix"
+
+
+class EmptyChapterStrategy(int, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """EmptyChapterStrategy."""
+
+    ZERO = 0
+    ONE = 1
+    TWO = 2
+
+
 class ExternalServiceName(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """ExternalServiceName."""
 
     DB_EXTRACTOR = "DbExtractor"
     MT_CONNECT_EXTRACTOR = "MtConnectExtractor"
     MQTT_CONNECTOR = "MqttConnector"
 
@@ -166,36 +238,72 @@
     N_FIRST = "NFirst"
     N_PERCENT = "NPercent"
     ISO2859 = "ISO2859"
     NTH = "Nth"
     NONE = "None"
 
 
+class MrbElementType(int, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """MrbElementType."""
+
+    ZERO = 0
+    ONE = 1
+    TWO = 2
+    THREE = 3
+    FOUR = 4
+
+
 class NotificationChannelDto(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """NotificationChannelDto."""
 
     TEAMS = "Teams"
 
 
 class OperationStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """OperationStatus."""
 
     NOT_READY = "NotReady"
     READY = "Ready"
     ONGOING = "Ongoing"
     COMPLETED = "Completed"
+    STOPPED = "Stopped"
 
 
 class SchemaFeedbackStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """SchemaFeedbackStatus."""
 
     NEW = "New"
     IN_PROGRESS = "InProgress"
 
 
+class TraceIncludeStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """TraceIncludeStatus."""
+
+    NONE = "None"
+    FORCE_INCLUDE = "ForceInclude"
+    EXCLUDE = "Exclude"
+
+
+class TraceItemStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """TraceItemStatus."""
+
+    NONE = "None"
+    OK = "OK"
+    SCRAP = "Scrap"
+
+
+class TraceType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """TraceType."""
+
+    NONE = "None"
+    LOT = "Lot"
+    BATCH = "Batch"
+    SERIAL_NUMBER = "SerialNumber"
+
+
 class WorkorderStatus(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """WorkorderStatus."""
 
     DRAFT = "Draft"
     READY = "Ready"
     ONGOING = "Ongoing"
     COMPLETED = "Completed"
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/models/_models.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/models/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,14 +547,40 @@
         :paramtype filename: str
         """
         super().__init__(**kwargs)
         self.upload_key = upload_key
         self.filename = filename
 
 
+class AttachPdfRequest(_serialization.Model):
+    """AttachPdfRequest.
+
+    :ivar upload_key:
+    :vartype upload_key: str
+    :ivar filename:
+    :vartype filename: str
+    """
+
+    _attribute_map = {
+        "upload_key": {"key": "uploadKey", "type": "str"},
+        "filename": {"key": "filename", "type": "str"},
+    }
+
+    def __init__(self, *, upload_key: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword upload_key:
+        :paramtype upload_key: str
+        :keyword filename:
+        :paramtype filename: str
+        """
+        super().__init__(**kwargs)
+        self.upload_key = upload_key
+        self.filename = filename
+
+
 class AzureRegionDto(_serialization.Model):
     """AzureRegionDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar display_name: Required.
     :vartype display_name: str
@@ -3231,14 +3257,211 @@
         :paramtype nodes: list[~ignos.api.client.models.SustainabilityNodeDto]
         """
         super().__init__(**kwargs)
         self.customer_order = customer_order
         self.nodes = nodes
 
 
+class CreateDocumentType(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """CreateDocumentType.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Required.
+    :vartype id: str
+    :ivar name: Required.
+    :vartype name: str
+    :ivar title:
+    :vartype title: str
+    :ivar desciption:
+    :vartype desciption: str
+    :ivar active: Required.
+    :vartype active: bool
+    :ivar number_key: Required. Known values are: "Multiple" and "SingleDocument".
+    :vartype number_key: str or ~ignos.api.client.models.DocumentNumberKey
+    :ivar document_number_pattern: Required.
+    :vartype document_number_pattern: str
+    :ivar workflow_type: Required. Known values are: "None", "CustomerProvided",
+     "CustomerApproval", and "InternalWithFix".
+    :vartype workflow_type: str or ~ignos.api.client.models.DocumentWorkflowType
+    :ivar file_type:
+    :vartype file_type: str
+    :ivar is_internal_document_type: Required.
+    :vartype is_internal_document_type: bool
+    :ivar is_generated_document_type: Required.
+    :vartype is_generated_document_type: bool
+    :ivar require_portable_file: Required.
+    :vartype require_portable_file: bool
+    :ivar category: Required. Known values are: "General", "Procedure", "Drawing", "Report", and
+     "Certificate".
+    :vartype category: str or ~ignos.api.client.models.DocumentTypeCategory
+    :ivar can_assign_document_number: Required.
+    :vartype can_assign_document_number: bool
+    :ivar import_tag:
+    :vartype import_tag: str
+    :ivar document_requirement_strategy: Required. Known values are: "None", "WorkOrder", "Lot",
+     "Drawing", and "CustomerOrderLine".
+    :vartype document_requirement_strategy: str or
+     ~ignos.api.client.models.DocumentRequirementStrategy
+    :ivar can_link_document: Required.
+    :vartype can_link_document: bool
+    :ivar require_dc_approval: Required.
+    :vartype require_dc_approval: bool
+    :ivar search_option: Required. Known values are: "IncludeApproved", "IncludeDraft", and
+     "Exclude".
+    :vartype search_option: str or ~ignos.api.client.models.DocumentTypeSearchOption
+    :ivar can_have_certificate: Required.
+    :vartype can_have_certificate: bool
+    :ivar sub_types: Required.
+    :vartype sub_types: list[~ignos.api.client.models.DocumentSubTypeDto]
+    """
+
+    _validation = {
+        "id": {"required": True, "min_length": 1},
+        "name": {"required": True, "min_length": 1},
+        "active": {"required": True},
+        "number_key": {"required": True},
+        "document_number_pattern": {"required": True, "min_length": 1},
+        "workflow_type": {"required": True},
+        "is_internal_document_type": {"required": True},
+        "is_generated_document_type": {"required": True},
+        "require_portable_file": {"required": True},
+        "category": {"required": True},
+        "can_assign_document_number": {"required": True},
+        "document_requirement_strategy": {"required": True},
+        "can_link_document": {"required": True},
+        "require_dc_approval": {"required": True},
+        "search_option": {"required": True},
+        "can_have_certificate": {"required": True},
+        "sub_types": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "title": {"key": "title", "type": "str"},
+        "desciption": {"key": "desciption", "type": "str"},
+        "active": {"key": "active", "type": "bool"},
+        "number_key": {"key": "numberKey", "type": "str"},
+        "document_number_pattern": {"key": "documentNumberPattern", "type": "str"},
+        "workflow_type": {"key": "workflowType", "type": "str"},
+        "file_type": {"key": "fileType", "type": "str"},
+        "is_internal_document_type": {"key": "isInternalDocumentType", "type": "bool"},
+        "is_generated_document_type": {"key": "isGeneratedDocumentType", "type": "bool"},
+        "require_portable_file": {"key": "requirePortableFile", "type": "bool"},
+        "category": {"key": "category", "type": "str"},
+        "can_assign_document_number": {"key": "canAssignDocumentNumber", "type": "bool"},
+        "import_tag": {"key": "importTag", "type": "str"},
+        "document_requirement_strategy": {"key": "documentRequirementStrategy", "type": "str"},
+        "can_link_document": {"key": "canLinkDocument", "type": "bool"},
+        "require_dc_approval": {"key": "requireDCApproval", "type": "bool"},
+        "search_option": {"key": "searchOption", "type": "str"},
+        "can_have_certificate": {"key": "canHaveCertificate", "type": "bool"},
+        "sub_types": {"key": "subTypes", "type": "[DocumentSubTypeDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: str,  # pylint: disable=redefined-builtin
+        name: str,
+        active: bool,
+        number_key: Union[str, "_models.DocumentNumberKey"],
+        document_number_pattern: str,
+        workflow_type: Union[str, "_models.DocumentWorkflowType"],
+        is_internal_document_type: bool,
+        is_generated_document_type: bool,
+        require_portable_file: bool,
+        category: Union[str, "_models.DocumentTypeCategory"],
+        can_assign_document_number: bool,
+        document_requirement_strategy: Union[str, "_models.DocumentRequirementStrategy"],
+        can_link_document: bool,
+        require_dc_approval: bool,
+        search_option: Union[str, "_models.DocumentTypeSearchOption"],
+        can_have_certificate: bool,
+        sub_types: List["_models.DocumentSubTypeDto"],
+        title: Optional[str] = None,
+        desciption: Optional[str] = None,
+        file_type: Optional[str] = None,
+        import_tag: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id: Required.
+        :paramtype id: str
+        :keyword name: Required.
+        :paramtype name: str
+        :keyword title:
+        :paramtype title: str
+        :keyword desciption:
+        :paramtype desciption: str
+        :keyword active: Required.
+        :paramtype active: bool
+        :keyword number_key: Required. Known values are: "Multiple" and "SingleDocument".
+        :paramtype number_key: str or ~ignos.api.client.models.DocumentNumberKey
+        :keyword document_number_pattern: Required.
+        :paramtype document_number_pattern: str
+        :keyword workflow_type: Required. Known values are: "None", "CustomerProvided",
+         "CustomerApproval", and "InternalWithFix".
+        :paramtype workflow_type: str or ~ignos.api.client.models.DocumentWorkflowType
+        :keyword file_type:
+        :paramtype file_type: str
+        :keyword is_internal_document_type: Required.
+        :paramtype is_internal_document_type: bool
+        :keyword is_generated_document_type: Required.
+        :paramtype is_generated_document_type: bool
+        :keyword require_portable_file: Required.
+        :paramtype require_portable_file: bool
+        :keyword category: Required. Known values are: "General", "Procedure", "Drawing", "Report", and
+         "Certificate".
+        :paramtype category: str or ~ignos.api.client.models.DocumentTypeCategory
+        :keyword can_assign_document_number: Required.
+        :paramtype can_assign_document_number: bool
+        :keyword import_tag:
+        :paramtype import_tag: str
+        :keyword document_requirement_strategy: Required. Known values are: "None", "WorkOrder", "Lot",
+         "Drawing", and "CustomerOrderLine".
+        :paramtype document_requirement_strategy: str or
+         ~ignos.api.client.models.DocumentRequirementStrategy
+        :keyword can_link_document: Required.
+        :paramtype can_link_document: bool
+        :keyword require_dc_approval: Required.
+        :paramtype require_dc_approval: bool
+        :keyword search_option: Required. Known values are: "IncludeApproved", "IncludeDraft", and
+         "Exclude".
+        :paramtype search_option: str or ~ignos.api.client.models.DocumentTypeSearchOption
+        :keyword can_have_certificate: Required.
+        :paramtype can_have_certificate: bool
+        :keyword sub_types: Required.
+        :paramtype sub_types: list[~ignos.api.client.models.DocumentSubTypeDto]
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.name = name
+        self.title = title
+        self.desciption = desciption
+        self.active = active
+        self.number_key = number_key
+        self.document_number_pattern = document_number_pattern
+        self.workflow_type = workflow_type
+        self.file_type = file_type
+        self.is_internal_document_type = is_internal_document_type
+        self.is_generated_document_type = is_generated_document_type
+        self.require_portable_file = require_portable_file
+        self.category = category
+        self.can_assign_document_number = can_assign_document_number
+        self.import_tag = import_tag
+        self.document_requirement_strategy = document_requirement_strategy
+        self.can_link_document = can_link_document
+        self.require_dc_approval = require_dc_approval
+        self.search_option = search_option
+        self.can_have_certificate = can_have_certificate
+        self.sub_types = sub_types
+
+
 class CreateElectricalIotConfig(_serialization.Model):
     """CreateElectricalIotConfig.
 
     :ivar type_id:
     :vartype type_id: str
     :ivar serial_number:
     :vartype serial_number: str
@@ -3937,14 +4160,81 @@
         :keyword unit: Required.
         :paramtype unit: str
         """
         super().__init__(**kwargs)
         self.unit = unit
 
 
+class CreateMrbTemplateRequest(_serialization.Model):
+    """CreateMrbTemplateRequest.
+
+    :ivar title:
+    :vartype title: str
+    :ivar customer_id:
+    :vartype customer_id: str
+    :ivar customer_group_id:
+    :vartype customer_group_id: str
+    :ivar customer_name:
+    :vartype customer_name: str
+    :ivar elements:
+    :vartype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+    :ivar pdf_upload_key:
+    :vartype pdf_upload_key: str
+    :ivar pdf_filename:
+    :vartype pdf_filename: str
+    """
+
+    _attribute_map = {
+        "title": {"key": "title", "type": "str"},
+        "customer_id": {"key": "customerId", "type": "str"},
+        "customer_group_id": {"key": "customerGroupId", "type": "str"},
+        "customer_name": {"key": "customerName", "type": "str"},
+        "elements": {"key": "elements", "type": "[MrbTemplateElementDto]"},
+        "pdf_upload_key": {"key": "pdfUploadKey", "type": "str"},
+        "pdf_filename": {"key": "pdfFilename", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        title: Optional[str] = None,
+        customer_id: Optional[str] = None,
+        customer_group_id: Optional[str] = None,
+        customer_name: Optional[str] = None,
+        elements: Optional[List["_models.MrbTemplateElementDto"]] = None,
+        pdf_upload_key: Optional[str] = None,
+        pdf_filename: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword title:
+        :paramtype title: str
+        :keyword customer_id:
+        :paramtype customer_id: str
+        :keyword customer_group_id:
+        :paramtype customer_group_id: str
+        :keyword customer_name:
+        :paramtype customer_name: str
+        :keyword elements:
+        :paramtype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+        :keyword pdf_upload_key:
+        :paramtype pdf_upload_key: str
+        :keyword pdf_filename:
+        :paramtype pdf_filename: str
+        """
+        super().__init__(**kwargs)
+        self.title = title
+        self.customer_id = customer_id
+        self.customer_group_id = customer_group_id
+        self.customer_name = customer_name
+        self.elements = elements
+        self.pdf_upload_key = pdf_upload_key
+        self.pdf_filename = pdf_filename
+
+
 class CreateSchemaElement(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """CreateSchemaElement.
 
     :ivar balloon_id:
     :vartype balloon_id: str
     :ivar section:
     :vartype section: str
@@ -4583,14 +4873,34 @@
         :keyword machines:
         :paramtype machines: list[~ignos.api.client.models.MachineDataHealthDto]
         """
         super().__init__(**kwargs)
         self.machines = machines
 
 
+class DeleteMrbTemplateRequest(_serialization.Model):
+    """DeleteMrbTemplateRequest.
+
+    :ivar id:
+    :vartype id: str
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+    }
+
+    def __init__(self, *, id: Optional[str] = None, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
+        """
+        :keyword id:
+        :paramtype id: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+
+
 class DeletePartDrawingRequest(_serialization.Model):
     """DeletePartDrawingRequest.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar filename: Required.
     :vartype filename: str
@@ -4629,14 +4939,298 @@
         :keyword date:
         :paramtype date: ~datetime.datetime
         """
         super().__init__(**kwargs)
         self.date = date
 
 
+class DocumentRevisionApprovalDto(_serialization.Model):
+    """DocumentRevisionApprovalDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar user: Required.
+    :vartype user: ~ignos.api.client.models.UserDto
+    :ivar approval_date: Required.
+    :vartype approval_date: ~datetime.datetime
+    """
+
+    _validation = {
+        "user": {"required": True},
+        "approval_date": {"required": True},
+    }
+
+    _attribute_map = {
+        "user": {"key": "user", "type": "UserDto"},
+        "approval_date": {"key": "approvalDate", "type": "iso-8601"},
+    }
+
+    def __init__(self, *, user: "_models.UserDto", approval_date: datetime.datetime, **kwargs: Any) -> None:
+        """
+        :keyword user: Required.
+        :paramtype user: ~ignos.api.client.models.UserDto
+        :keyword approval_date: Required.
+        :paramtype approval_date: ~datetime.datetime
+        """
+        super().__init__(**kwargs)
+        self.user = user
+        self.approval_date = approval_date
+
+
+class DocumentSubTypeDto(_serialization.Model):
+    """DocumentSubTypeDto.
+
+    :ivar name:
+    :vartype name: str
+    :ivar description:
+    :vartype description: str
+    :ivar active:
+    :vartype active: bool
+    """
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "description": {"key": "description", "type": "str"},
+        "active": {"key": "active", "type": "bool"},
+    }
+
+    def __init__(
+        self,
+        *,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        active: Optional[bool] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword name:
+        :paramtype name: str
+        :keyword description:
+        :paramtype description: str
+        :keyword active:
+        :paramtype active: bool
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.description = description
+        self.active = active
+
+
+class DocumentTagDto(_serialization.Model):
+    """DocumentTagDto.
+
+    :ivar key:
+    :vartype key: str
+    :ivar value:
+    :vartype value: str
+    """
+
+    _attribute_map = {
+        "key": {"key": "key", "type": "str"},
+        "value": {"key": "value", "type": "str"},
+    }
+
+    def __init__(self, *, key: Optional[str] = None, value: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword key:
+        :paramtype key: str
+        :keyword value:
+        :paramtype value: str
+        """
+        super().__init__(**kwargs)
+        self.key = key
+        self.value = value
+
+
+class DocumentTypeDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """DocumentTypeDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id:
+    :vartype id: str
+    :ivar name:
+    :vartype name: str
+    :ivar title:
+    :vartype title: str
+    :ivar desciption:
+    :vartype desciption: str
+    :ivar active:
+    :vartype active: bool
+    :ivar number_key: Known values are: "Multiple" and "SingleDocument".
+    :vartype number_key: str or ~ignos.api.client.models.DocumentNumberKey
+    :ivar document_number_pattern:
+    :vartype document_number_pattern: str
+    :ivar workflow_type: Known values are: "None", "CustomerProvided", "CustomerApproval", and
+     "InternalWithFix".
+    :vartype workflow_type: str or ~ignos.api.client.models.DocumentWorkflowType
+    :ivar file_type:
+    :vartype file_type: str
+    :ivar is_internal_document_type:
+    :vartype is_internal_document_type: bool
+    :ivar is_generated_document_type:
+    :vartype is_generated_document_type: bool
+    :ivar require_portable_file:
+    :vartype require_portable_file: bool
+    :ivar category: Known values are: "General", "Procedure", "Drawing", "Report", and
+     "Certificate".
+    :vartype category: str or ~ignos.api.client.models.DocumentTypeCategory
+    :ivar can_assign_document_number:
+    :vartype can_assign_document_number: bool
+    :ivar import_tag:
+    :vartype import_tag: str
+    :ivar document_requirement_strategy: Known values are: "None", "WorkOrder", "Lot", "Drawing",
+     and "CustomerOrderLine".
+    :vartype document_requirement_strategy: str or
+     ~ignos.api.client.models.DocumentRequirementStrategy
+    :ivar can_link_document:
+    :vartype can_link_document: bool
+    :ivar require_dc_approval:
+    :vartype require_dc_approval: bool
+    :ivar search_option: Known values are: "IncludeApproved", "IncludeDraft", and "Exclude".
+    :vartype search_option: str or ~ignos.api.client.models.DocumentTypeSearchOption
+    :ivar can_have_certificate:
+    :vartype can_have_certificate: bool
+    :ivar used:
+    :vartype used: bool
+    :ivar sub_types: Required.
+    :vartype sub_types: list[~ignos.api.client.models.DocumentSubTypeDto]
+    """
+
+    _validation = {
+        "sub_types": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "title": {"key": "title", "type": "str"},
+        "desciption": {"key": "desciption", "type": "str"},
+        "active": {"key": "active", "type": "bool"},
+        "number_key": {"key": "numberKey", "type": "str"},
+        "document_number_pattern": {"key": "documentNumberPattern", "type": "str"},
+        "workflow_type": {"key": "workflowType", "type": "str"},
+        "file_type": {"key": "fileType", "type": "str"},
+        "is_internal_document_type": {"key": "isInternalDocumentType", "type": "bool"},
+        "is_generated_document_type": {"key": "isGeneratedDocumentType", "type": "bool"},
+        "require_portable_file": {"key": "requirePortableFile", "type": "bool"},
+        "category": {"key": "category", "type": "str"},
+        "can_assign_document_number": {"key": "canAssignDocumentNumber", "type": "bool"},
+        "import_tag": {"key": "importTag", "type": "str"},
+        "document_requirement_strategy": {"key": "documentRequirementStrategy", "type": "str"},
+        "can_link_document": {"key": "canLinkDocument", "type": "bool"},
+        "require_dc_approval": {"key": "requireDCApproval", "type": "bool"},
+        "search_option": {"key": "searchOption", "type": "str"},
+        "can_have_certificate": {"key": "canHaveCertificate", "type": "bool"},
+        "used": {"key": "used", "type": "bool"},
+        "sub_types": {"key": "subTypes", "type": "[DocumentSubTypeDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        sub_types: List["_models.DocumentSubTypeDto"],
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        name: Optional[str] = None,
+        title: Optional[str] = None,
+        desciption: Optional[str] = None,
+        active: Optional[bool] = None,
+        number_key: Optional[Union[str, "_models.DocumentNumberKey"]] = None,
+        document_number_pattern: Optional[str] = None,
+        workflow_type: Optional[Union[str, "_models.DocumentWorkflowType"]] = None,
+        file_type: Optional[str] = None,
+        is_internal_document_type: Optional[bool] = None,
+        is_generated_document_type: Optional[bool] = None,
+        require_portable_file: Optional[bool] = None,
+        category: Optional[Union[str, "_models.DocumentTypeCategory"]] = None,
+        can_assign_document_number: Optional[bool] = None,
+        import_tag: Optional[str] = None,
+        document_requirement_strategy: Optional[Union[str, "_models.DocumentRequirementStrategy"]] = None,
+        can_link_document: Optional[bool] = None,
+        require_dc_approval: Optional[bool] = None,
+        search_option: Optional[Union[str, "_models.DocumentTypeSearchOption"]] = None,
+        can_have_certificate: Optional[bool] = None,
+        used: Optional[bool] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id:
+        :paramtype id: str
+        :keyword name:
+        :paramtype name: str
+        :keyword title:
+        :paramtype title: str
+        :keyword desciption:
+        :paramtype desciption: str
+        :keyword active:
+        :paramtype active: bool
+        :keyword number_key: Known values are: "Multiple" and "SingleDocument".
+        :paramtype number_key: str or ~ignos.api.client.models.DocumentNumberKey
+        :keyword document_number_pattern:
+        :paramtype document_number_pattern: str
+        :keyword workflow_type: Known values are: "None", "CustomerProvided", "CustomerApproval", and
+         "InternalWithFix".
+        :paramtype workflow_type: str or ~ignos.api.client.models.DocumentWorkflowType
+        :keyword file_type:
+        :paramtype file_type: str
+        :keyword is_internal_document_type:
+        :paramtype is_internal_document_type: bool
+        :keyword is_generated_document_type:
+        :paramtype is_generated_document_type: bool
+        :keyword require_portable_file:
+        :paramtype require_portable_file: bool
+        :keyword category: Known values are: "General", "Procedure", "Drawing", "Report", and
+         "Certificate".
+        :paramtype category: str or ~ignos.api.client.models.DocumentTypeCategory
+        :keyword can_assign_document_number:
+        :paramtype can_assign_document_number: bool
+        :keyword import_tag:
+        :paramtype import_tag: str
+        :keyword document_requirement_strategy: Known values are: "None", "WorkOrder", "Lot",
+         "Drawing", and "CustomerOrderLine".
+        :paramtype document_requirement_strategy: str or
+         ~ignos.api.client.models.DocumentRequirementStrategy
+        :keyword can_link_document:
+        :paramtype can_link_document: bool
+        :keyword require_dc_approval:
+        :paramtype require_dc_approval: bool
+        :keyword search_option: Known values are: "IncludeApproved", "IncludeDraft", and "Exclude".
+        :paramtype search_option: str or ~ignos.api.client.models.DocumentTypeSearchOption
+        :keyword can_have_certificate:
+        :paramtype can_have_certificate: bool
+        :keyword used:
+        :paramtype used: bool
+        :keyword sub_types: Required.
+        :paramtype sub_types: list[~ignos.api.client.models.DocumentSubTypeDto]
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.name = name
+        self.title = title
+        self.desciption = desciption
+        self.active = active
+        self.number_key = number_key
+        self.document_number_pattern = document_number_pattern
+        self.workflow_type = workflow_type
+        self.file_type = file_type
+        self.is_internal_document_type = is_internal_document_type
+        self.is_generated_document_type = is_generated_document_type
+        self.require_portable_file = require_portable_file
+        self.category = category
+        self.can_assign_document_number = can_assign_document_number
+        self.import_tag = import_tag
+        self.document_requirement_strategy = document_requirement_strategy
+        self.can_link_document = can_link_document
+        self.require_dc_approval = require_dc_approval
+        self.search_option = search_option
+        self.can_have_certificate = can_have_certificate
+        self.used = used
+        self.sub_types = sub_types
+
+
 class DownloadDto(_serialization.Model):
     """DownloadDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar url: Required.
     :vartype url: str
@@ -4765,37 +5359,51 @@
 class EmployeeDto(_serialization.Model):
     """EmployeeDto.
 
     :ivar id:
     :vartype id: str
     :ivar name:
     :vartype name: str
+    :ivar upn:
+    :vartype upn: str
+    :ivar azure_ad_object_id:
+    :vartype azure_ad_object_id: str
     """
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
+        "upn": {"key": "upn", "type": "str"},
+        "azure_ad_object_id": {"key": "azureAdObjectId", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         id: Optional[str] = None,  # pylint: disable=redefined-builtin
         name: Optional[str] = None,
+        upn: Optional[str] = None,
+        azure_ad_object_id: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id:
         :paramtype id: str
         :keyword name:
         :paramtype name: str
+        :keyword upn:
+        :paramtype upn: str
+        :keyword azure_ad_object_id:
+        :paramtype azure_ad_object_id: str
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
+        self.upn = upn
+        self.azure_ad_object_id = azure_ad_object_id
 
 
 class ExportDimensionReportRequest(_serialization.Model):
     """ExportDimensionReportRequest.
 
     :ivar tenant_id:
     :vartype tenant_id: str
@@ -5298,14 +5906,249 @@
         """
         super().__init__(**kwargs)
         self.url = url
         self.name = name
         self.thumbnail_url = thumbnail_url
 
 
+class ImportDocument(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """ImportDocument.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar document_type: Required.
+    :vartype document_type: str
+    :ivar document_sub_type:
+    :vartype document_sub_type: str
+    :ivar document_number: Required.
+    :vartype document_number: str
+    :ivar customer_document_number:
+    :vartype customer_document_number: str
+    :ivar custom_document_number:
+    :vartype custom_document_number: str
+    :ivar supplier_document_number:
+    :vartype supplier_document_number: str
+    :ivar title:
+    :vartype title: str
+    :ivar comment:
+    :vartype comment: str
+    :ivar tags: Required.
+    :vartype tags: list[~ignos.api.client.models.DocumentTagDto]
+    :ivar sequences: Required.
+    :vartype sequences: list[str]
+    :ivar internal: Required.
+    :vartype internal: bool
+    :ivar order_lines: Required.
+    :vartype order_lines: list[int]
+    :ivar lots: Required.
+    :vartype lots: list[str]
+    :ivar front_page_document_id:
+    :vartype front_page_document_id: str
+    :ivar document_source: Required. Known values are: 0, 1, 2, and 3.
+    :vartype document_source: int or ~ignos.api.client.models.DocumentSource
+    :ivar revisions: Required.
+    :vartype revisions: list[~ignos.api.client.models.ImportDocumentRevisionDto]
+    """
+
+    _validation = {
+        "document_type": {"required": True, "min_length": 1},
+        "document_number": {"required": True, "min_length": 1},
+        "tags": {"required": True},
+        "sequences": {"required": True},
+        "internal": {"required": True},
+        "order_lines": {"required": True},
+        "lots": {"required": True},
+        "document_source": {"required": True},
+        "revisions": {"required": True},
+    }
+
+    _attribute_map = {
+        "document_type": {"key": "documentType", "type": "str"},
+        "document_sub_type": {"key": "documentSubType", "type": "str"},
+        "document_number": {"key": "documentNumber", "type": "str"},
+        "customer_document_number": {"key": "customerDocumentNumber", "type": "str"},
+        "custom_document_number": {"key": "customDocumentNumber", "type": "str"},
+        "supplier_document_number": {"key": "supplierDocumentNumber", "type": "str"},
+        "title": {"key": "title", "type": "str"},
+        "comment": {"key": "comment", "type": "str"},
+        "tags": {"key": "tags", "type": "[DocumentTagDto]"},
+        "sequences": {"key": "sequences", "type": "[str]"},
+        "internal": {"key": "internal", "type": "bool"},
+        "order_lines": {"key": "orderLines", "type": "[int]"},
+        "lots": {"key": "lots", "type": "[str]"},
+        "front_page_document_id": {"key": "frontPageDocumentId", "type": "str"},
+        "document_source": {"key": "documentSource", "type": "int"},
+        "revisions": {"key": "revisions", "type": "[ImportDocumentRevisionDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        document_type: str,
+        document_number: str,
+        tags: List["_models.DocumentTagDto"],
+        sequences: List[str],
+        internal: bool,
+        order_lines: List[int],
+        lots: List[str],
+        document_source: Union[int, "_models.DocumentSource"],
+        revisions: List["_models.ImportDocumentRevisionDto"],
+        document_sub_type: Optional[str] = None,
+        customer_document_number: Optional[str] = None,
+        custom_document_number: Optional[str] = None,
+        supplier_document_number: Optional[str] = None,
+        title: Optional[str] = None,
+        comment: Optional[str] = None,
+        front_page_document_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword document_type: Required.
+        :paramtype document_type: str
+        :keyword document_sub_type:
+        :paramtype document_sub_type: str
+        :keyword document_number: Required.
+        :paramtype document_number: str
+        :keyword customer_document_number:
+        :paramtype customer_document_number: str
+        :keyword custom_document_number:
+        :paramtype custom_document_number: str
+        :keyword supplier_document_number:
+        :paramtype supplier_document_number: str
+        :keyword title:
+        :paramtype title: str
+        :keyword comment:
+        :paramtype comment: str
+        :keyword tags: Required.
+        :paramtype tags: list[~ignos.api.client.models.DocumentTagDto]
+        :keyword sequences: Required.
+        :paramtype sequences: list[str]
+        :keyword internal: Required.
+        :paramtype internal: bool
+        :keyword order_lines: Required.
+        :paramtype order_lines: list[int]
+        :keyword lots: Required.
+        :paramtype lots: list[str]
+        :keyword front_page_document_id:
+        :paramtype front_page_document_id: str
+        :keyword document_source: Required. Known values are: 0, 1, 2, and 3.
+        :paramtype document_source: int or ~ignos.api.client.models.DocumentSource
+        :keyword revisions: Required.
+        :paramtype revisions: list[~ignos.api.client.models.ImportDocumentRevisionDto]
+        """
+        super().__init__(**kwargs)
+        self.document_type = document_type
+        self.document_sub_type = document_sub_type
+        self.document_number = document_number
+        self.customer_document_number = customer_document_number
+        self.custom_document_number = custom_document_number
+        self.supplier_document_number = supplier_document_number
+        self.title = title
+        self.comment = comment
+        self.tags = tags
+        self.sequences = sequences
+        self.internal = internal
+        self.order_lines = order_lines
+        self.lots = lots
+        self.front_page_document_id = front_page_document_id
+        self.document_source = document_source
+        self.revisions = revisions
+
+
+class ImportDocumentRevisionDto(_serialization.Model):
+    """ImportDocumentRevisionDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar revistion_id: Required.
+    :vartype revistion_id: int
+    :ivar revision:
+    :vartype revision: str
+    :ivar status: Required. Known values are: 0, 1, 2, 3, 10, and 90.
+    :vartype status: int or ~ignos.api.client.models.DocumentStatus
+    :ivar status_date: Required.
+    :vartype status_date: ~datetime.datetime
+    :ivar description:
+    :vartype description: str
+    :ivar import_reference:
+    :vartype import_reference: str
+    :ivar signed_by_document_id:
+    :vartype signed_by_document_id: str
+    :ivar extensions: Required.
+    :vartype extensions: list[str]
+    :ivar approvals: Required.
+    :vartype approvals: list[~ignos.api.client.models.DocumentRevisionApprovalDto]
+    """
+
+    _validation = {
+        "revistion_id": {"required": True},
+        "status": {"required": True},
+        "status_date": {"required": True},
+        "extensions": {"required": True},
+        "approvals": {"required": True},
+    }
+
+    _attribute_map = {
+        "revistion_id": {"key": "revistionId", "type": "int"},
+        "revision": {"key": "revision", "type": "str"},
+        "status": {"key": "status", "type": "int"},
+        "status_date": {"key": "statusDate", "type": "iso-8601"},
+        "description": {"key": "description", "type": "str"},
+        "import_reference": {"key": "importReference", "type": "str"},
+        "signed_by_document_id": {"key": "signedByDocumentId", "type": "str"},
+        "extensions": {"key": "extensions", "type": "[str]"},
+        "approvals": {"key": "approvals", "type": "[DocumentRevisionApprovalDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        revistion_id: int,
+        status: Union[int, "_models.DocumentStatus"],
+        status_date: datetime.datetime,
+        extensions: List[str],
+        approvals: List["_models.DocumentRevisionApprovalDto"],
+        revision: Optional[str] = None,
+        description: Optional[str] = None,
+        import_reference: Optional[str] = None,
+        signed_by_document_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword revistion_id: Required.
+        :paramtype revistion_id: int
+        :keyword revision:
+        :paramtype revision: str
+        :keyword status: Required. Known values are: 0, 1, 2, 3, 10, and 90.
+        :paramtype status: int or ~ignos.api.client.models.DocumentStatus
+        :keyword status_date: Required.
+        :paramtype status_date: ~datetime.datetime
+        :keyword description:
+        :paramtype description: str
+        :keyword import_reference:
+        :paramtype import_reference: str
+        :keyword signed_by_document_id:
+        :paramtype signed_by_document_id: str
+        :keyword extensions: Required.
+        :paramtype extensions: list[str]
+        :keyword approvals: Required.
+        :paramtype approvals: list[~ignos.api.client.models.DocumentRevisionApprovalDto]
+        """
+        super().__init__(**kwargs)
+        self.revistion_id = revistion_id
+        self.revision = revision
+        self.status = status
+        self.status_date = status_date
+        self.description = description
+        self.import_reference = import_reference
+        self.signed_by_document_id = signed_by_document_id
+        self.extensions = extensions
+        self.approvals = approvals
+
+
 class ImportMeasurementFormInstanceRequest(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """ImportMeasurementFormInstanceRequest.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar part_info: Required.
     :vartype part_info: ~ignos.api.client.models.ImportMeasurementFormPartDto
@@ -7203,58 +8046,65 @@
     :vartype external_id: str
     :ivar name: Required.
     :vartype name: str
     :ivar description:
     :vartype description: str
     :ivar type:
     :vartype type: str
+    :ivar work_order_asset_external_id:
+    :vartype work_order_asset_external_id: str
     """
 
     _validation = {
         "id": {"required": True},
         "external_id": {"required": True, "min_length": 1},
         "name": {"required": True, "min_length": 1},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "int"},
         "external_id": {"key": "externalId", "type": "str"},
         "name": {"key": "name", "type": "str"},
         "description": {"key": "description", "type": "str"},
         "type": {"key": "type", "type": "str"},
+        "work_order_asset_external_id": {"key": "workOrderAssetExternalId", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         id: int,  # pylint: disable=redefined-builtin
         external_id: str,
         name: str,
         description: Optional[str] = None,
         type: Optional[str] = None,
+        work_order_asset_external_id: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: int
         :keyword external_id: Required.
         :paramtype external_id: str
         :keyword name: Required.
         :paramtype name: str
         :keyword description:
         :paramtype description: str
         :keyword type:
         :paramtype type: str
+        :keyword work_order_asset_external_id:
+        :paramtype work_order_asset_external_id: str
         """
         super().__init__(**kwargs)
         self.id = id
         self.external_id = external_id
         self.name = name
         self.description = description
         self.type = type
+        self.work_order_asset_external_id = work_order_asset_external_id
 
 
 class MachineGroupDto(_serialization.Model):
     """MachineGroupDto.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -7892,14 +8742,117 @@
         :paramtype name: str
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
 
 
+class MaterialConsumptionDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """MaterialConsumptionDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar operation:
+    :vartype operation: int
+    :ivar material_line:
+    :vartype material_line: int
+    :ivar material: Required.
+    :vartype material: ~ignos.api.client.models.PartDto
+    :ivar quantity: Required.
+    :vartype quantity: float
+    :ivar unit:
+    :vartype unit: str
+    :ivar trace_type: Required. Known values are: "None", "Lot", "Batch", and "SerialNumber".
+    :vartype trace_type: str or ~ignos.api.client.models.TraceType
+    :ivar lot:
+    :vartype lot: str
+    :ivar heat:
+    :vartype heat: str
+    :ivar supplier_id:
+    :vartype supplier_id: str
+    :ivar procurement_order:
+    :vartype procurement_order: str
+    :ivar procurement_order_line:
+    :vartype procurement_order_line: int
+    """
+
+    _validation = {
+        "material": {"required": True},
+        "quantity": {"required": True},
+        "trace_type": {"required": True},
+    }
+
+    _attribute_map = {
+        "operation": {"key": "operation", "type": "int"},
+        "material_line": {"key": "materialLine", "type": "int"},
+        "material": {"key": "material", "type": "PartDto"},
+        "quantity": {"key": "quantity", "type": "float"},
+        "unit": {"key": "unit", "type": "str"},
+        "trace_type": {"key": "traceType", "type": "str"},
+        "lot": {"key": "lot", "type": "str"},
+        "heat": {"key": "heat", "type": "str"},
+        "supplier_id": {"key": "supplierId", "type": "str"},
+        "procurement_order": {"key": "procurementOrder", "type": "str"},
+        "procurement_order_line": {"key": "procurementOrderLine", "type": "int"},
+    }
+
+    def __init__(
+        self,
+        *,
+        material: "_models.PartDto",
+        quantity: float,
+        trace_type: Union[str, "_models.TraceType"],
+        operation: Optional[int] = None,
+        material_line: Optional[int] = None,
+        unit: Optional[str] = None,
+        lot: Optional[str] = None,
+        heat: Optional[str] = None,
+        supplier_id: Optional[str] = None,
+        procurement_order: Optional[str] = None,
+        procurement_order_line: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword operation:
+        :paramtype operation: int
+        :keyword material_line:
+        :paramtype material_line: int
+        :keyword material: Required.
+        :paramtype material: ~ignos.api.client.models.PartDto
+        :keyword quantity: Required.
+        :paramtype quantity: float
+        :keyword unit:
+        :paramtype unit: str
+        :keyword trace_type: Required. Known values are: "None", "Lot", "Batch", and "SerialNumber".
+        :paramtype trace_type: str or ~ignos.api.client.models.TraceType
+        :keyword lot:
+        :paramtype lot: str
+        :keyword heat:
+        :paramtype heat: str
+        :keyword supplier_id:
+        :paramtype supplier_id: str
+        :keyword procurement_order:
+        :paramtype procurement_order: str
+        :keyword procurement_order_line:
+        :paramtype procurement_order_line: int
+        """
+        super().__init__(**kwargs)
+        self.operation = operation
+        self.material_line = material_line
+        self.material = material
+        self.quantity = quantity
+        self.unit = unit
+        self.trace_type = trace_type
+        self.lot = lot
+        self.heat = heat
+        self.supplier_id = supplier_id
+        self.procurement_order = procurement_order
+        self.procurement_order_line = procurement_order_line
+
+
 class MaterialMassDensityDto(_serialization.Model):
     """MaterialMassDensityDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar name: Required.
     :vartype name: str
@@ -12699,14 +13652,176 @@
         :paramtype unit: str
         """
         super().__init__(**kwargs)
         self.id = id
         self.unit = unit
 
 
+class MrbTemplateDto(_serialization.Model):
+    """MrbTemplateDto.
+
+    :ivar id:
+    :vartype id: str
+    :ivar title:
+    :vartype title: str
+    :ivar customer_id:
+    :vartype customer_id: str
+    :ivar customer_group_id:
+    :vartype customer_group_id: str
+    :ivar customer_name:
+    :vartype customer_name: str
+    :ivar url:
+    :vartype url: str
+    :ivar shared_access_uri:
+    :vartype shared_access_uri: str
+    :ivar elements:
+    :vartype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "title": {"key": "title", "type": "str"},
+        "customer_id": {"key": "customerId", "type": "str"},
+        "customer_group_id": {"key": "customerGroupId", "type": "str"},
+        "customer_name": {"key": "customerName", "type": "str"},
+        "url": {"key": "url", "type": "str"},
+        "shared_access_uri": {"key": "sharedAccessUri", "type": "str"},
+        "elements": {"key": "elements", "type": "[MrbTemplateElementDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        title: Optional[str] = None,
+        customer_id: Optional[str] = None,
+        customer_group_id: Optional[str] = None,
+        customer_name: Optional[str] = None,
+        url: Optional[str] = None,
+        shared_access_uri: Optional[str] = None,
+        elements: Optional[List["_models.MrbTemplateElementDto"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id:
+        :paramtype id: str
+        :keyword title:
+        :paramtype title: str
+        :keyword customer_id:
+        :paramtype customer_id: str
+        :keyword customer_group_id:
+        :paramtype customer_group_id: str
+        :keyword customer_name:
+        :paramtype customer_name: str
+        :keyword url:
+        :paramtype url: str
+        :keyword shared_access_uri:
+        :paramtype shared_access_uri: str
+        :keyword elements:
+        :paramtype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.title = title
+        self.customer_id = customer_id
+        self.customer_group_id = customer_group_id
+        self.customer_name = customer_name
+        self.url = url
+        self.shared_access_uri = shared_access_uri
+        self.elements = elements
+
+
+class MrbTemplateElementDto(_serialization.Model):
+    """MrbTemplateElementDto.
+
+    :ivar document_index:
+    :vartype document_index: str
+    :ivar bookmark_title:
+    :vartype bookmark_title: str
+    :ivar elements:
+    :vartype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+    :ivar empty_chapter_strategy: Known values are: 0, 1, and 2.
+    :vartype empty_chapter_strategy: int or ~ignos.api.client.models.EmptyChapterStrategy
+    :ivar template_page_number:
+    :vartype template_page_number: int
+    :ivar generated_document_types:
+    :vartype generated_document_types: list[str]
+    :ivar document_types:
+    :vartype document_types: list[str]
+    :ivar separator_format_title:
+    :vartype separator_format_title: str
+    :ivar child_document_bookmark_title:
+    :vartype child_document_bookmark_title: str
+    :ivar element_type: Known values are: 0, 1, 2, 3, and 4.
+    :vartype element_type: int or ~ignos.api.client.models.MrbElementType
+    """
+
+    _attribute_map = {
+        "document_index": {"key": "documentIndex", "type": "str"},
+        "bookmark_title": {"key": "bookmarkTitle", "type": "str"},
+        "elements": {"key": "elements", "type": "[MrbTemplateElementDto]"},
+        "empty_chapter_strategy": {"key": "emptyChapterStrategy", "type": "int"},
+        "template_page_number": {"key": "templatePageNumber", "type": "int"},
+        "generated_document_types": {"key": "generatedDocumentTypes", "type": "[str]"},
+        "document_types": {"key": "documentTypes", "type": "[str]"},
+        "separator_format_title": {"key": "separatorFormatTitle", "type": "str"},
+        "child_document_bookmark_title": {"key": "childDocumentBookmarkTitle", "type": "str"},
+        "element_type": {"key": "elementType", "type": "int"},
+    }
+
+    def __init__(
+        self,
+        *,
+        document_index: Optional[str] = None,
+        bookmark_title: Optional[str] = None,
+        elements: Optional[List["_models.MrbTemplateElementDto"]] = None,
+        empty_chapter_strategy: Optional[Union[int, "_models.EmptyChapterStrategy"]] = None,
+        template_page_number: Optional[int] = None,
+        generated_document_types: Optional[List[str]] = None,
+        document_types: Optional[List[str]] = None,
+        separator_format_title: Optional[str] = None,
+        child_document_bookmark_title: Optional[str] = None,
+        element_type: Optional[Union[int, "_models.MrbElementType"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword document_index:
+        :paramtype document_index: str
+        :keyword bookmark_title:
+        :paramtype bookmark_title: str
+        :keyword elements:
+        :paramtype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+        :keyword empty_chapter_strategy: Known values are: 0, 1, and 2.
+        :paramtype empty_chapter_strategy: int or ~ignos.api.client.models.EmptyChapterStrategy
+        :keyword template_page_number:
+        :paramtype template_page_number: int
+        :keyword generated_document_types:
+        :paramtype generated_document_types: list[str]
+        :keyword document_types:
+        :paramtype document_types: list[str]
+        :keyword separator_format_title:
+        :paramtype separator_format_title: str
+        :keyword child_document_bookmark_title:
+        :paramtype child_document_bookmark_title: str
+        :keyword element_type: Known values are: 0, 1, 2, 3, and 4.
+        :paramtype element_type: int or ~ignos.api.client.models.MrbElementType
+        """
+        super().__init__(**kwargs)
+        self.document_index = document_index
+        self.bookmark_title = bookmark_title
+        self.elements = elements
+        self.empty_chapter_strategy = empty_chapter_strategy
+        self.template_page_number = template_page_number
+        self.generated_document_types = generated_document_types
+        self.document_types = document_types
+        self.separator_format_title = separator_format_title
+        self.child_document_bookmark_title = child_document_bookmark_title
+        self.element_type = element_type
+
+
 class NumericDataPointDto(_serialization.Model):
     """NumericDataPointDto.
 
     :ivar timestamp:
     :vartype timestamp: int
     :ivar value:
     :vartype value: float
@@ -13200,36 +14315,45 @@
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: Required.
     :vartype id: str
     :ivar name: Required.
     :vartype name: str
+    :ivar selected: Required.
+    :vartype selected: bool
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "name": {"required": True, "min_length": 1},
+        "selected": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "name": {"key": "name", "type": "str"},
+        "selected": {"key": "selected", "type": "bool"},
     }
 
-    def __init__(self, *, id: str, name: str, **kwargs: Any) -> None:  # pylint: disable=redefined-builtin
+    def __init__(
+        self, *, id: str, name: str, selected: bool, **kwargs: Any  # pylint: disable=redefined-builtin
+    ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword name: Required.
         :paramtype name: str
+        :keyword selected: Required.
+        :paramtype selected: bool
         """
         super().__init__(**kwargs)
         self.id = id
         self.name = name
+        self.selected = selected
 
 
 class ProductionEmployeeDto(_serialization.Model):
     """ProductionEmployeeDto.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -13442,20 +14566,22 @@
     :vartype fixed_time: bool
     :ivar resource:
     :vartype resource: ~ignos.api.client.models.ResourceDto
     :ivar planned_start:
     :vartype planned_start: ~datetime.datetime
     :ivar planned_end:
     :vartype planned_end: ~datetime.datetime
-    :ivar status: Known values are: "NotReady", "Ready", "Ongoing", and "Completed".
+    :ivar status: Known values are: "NotReady", "Ready", "Ongoing", "Completed", and "Stopped".
     :vartype status: str or ~ignos.api.client.models.OperationStatus
     :ivar produced_quantity:
     :vartype produced_quantity: float
     :ivar scrapped_quantity:
     :vartype scrapped_quantity: float
+    :ivar quantity:
+    :vartype quantity: float
     :ivar used_production_time:
     :vartype used_production_time: float
     :ivar used_setup_time:
     :vartype used_setup_time: float
     :ivar work_instructions:
     :vartype work_instructions: str
     :ivar fixture:
@@ -13475,14 +14601,15 @@
         "fixed_time": {"key": "fixedTime", "type": "bool"},
         "resource": {"key": "resource", "type": "ResourceDto"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
+        "quantity": {"key": "quantity", "type": "float"},
         "used_production_time": {"key": "usedProductionTime", "type": "float"},
         "used_setup_time": {"key": "usedSetupTime", "type": "float"},
         "work_instructions": {"key": "workInstructions", "type": "str"},
         "fixture": {"key": "fixture", "type": "str"},
         "program": {"key": "program", "type": "str"},
         "tool_number": {"key": "toolNumber", "type": "str"},
     }
@@ -13498,14 +14625,15 @@
         fixed_time: Optional[bool] = None,
         resource: Optional["_models.ResourceDto"] = None,
         planned_start: Optional[datetime.datetime] = None,
         planned_end: Optional[datetime.datetime] = None,
         status: Optional[Union[str, "_models.OperationStatus"]] = None,
         produced_quantity: Optional[float] = None,
         scrapped_quantity: Optional[float] = None,
+        quantity: Optional[float] = None,
         used_production_time: Optional[float] = None,
         used_setup_time: Optional[float] = None,
         work_instructions: Optional[str] = None,
         fixture: Optional[str] = None,
         program: Optional[str] = None,
         tool_number: Optional[str] = None,
         **kwargs: Any
@@ -13525,20 +14653,22 @@
         :paramtype fixed_time: bool
         :keyword resource:
         :paramtype resource: ~ignos.api.client.models.ResourceDto
         :keyword planned_start:
         :paramtype planned_start: ~datetime.datetime
         :keyword planned_end:
         :paramtype planned_end: ~datetime.datetime
-        :keyword status: Known values are: "NotReady", "Ready", "Ongoing", and "Completed".
+        :keyword status: Known values are: "NotReady", "Ready", "Ongoing", "Completed", and "Stopped".
         :paramtype status: str or ~ignos.api.client.models.OperationStatus
         :keyword produced_quantity:
         :paramtype produced_quantity: float
         :keyword scrapped_quantity:
         :paramtype scrapped_quantity: float
+        :keyword quantity:
+        :paramtype quantity: float
         :keyword used_production_time:
         :paramtype used_production_time: float
         :keyword used_setup_time:
         :paramtype used_setup_time: float
         :keyword work_instructions:
         :paramtype work_instructions: str
         :keyword fixture:
@@ -13557,14 +14687,15 @@
         self.fixed_time = fixed_time
         self.resource = resource
         self.planned_start = planned_start
         self.planned_end = planned_end
         self.status = status
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
+        self.quantity = quantity
         self.used_production_time = used_production_time
         self.used_setup_time = used_setup_time
         self.work_instructions = work_instructions
         self.fixture = fixture
         self.program = program
         self.tool_number = tool_number
 
@@ -13620,16 +14751,20 @@
     :vartype status: str
     :ivar planned_hours:
     :vartype planned_hours: float
     :ivar used_hours:
     :vartype used_hours: float
     :ivar quantity: Required.
     :vartype quantity: float
-    :ivar project_name:
-    :vartype project_name: str
+    :ivar produced_quantity: Required.
+    :vartype produced_quantity: float
+    :ivar scrapped_quantity: Required.
+    :vartype scrapped_quantity: float
+    :ivar project:
+    :vartype project: ~ignos.api.client.models.WorkOrderProjectDto
     :ivar part_number: Required.
     :vartype part_number: str
     :ivar part_revision:
     :vartype part_revision: str
     :ivar part_name:
     :vartype part_name: str
     :ivar resource_id: Required.
@@ -13648,26 +14783,32 @@
     :vartype work_instructions: str
     :ivar description:
     :vartype description: str
     :ivar fixture:
     :vartype fixture: str
     :ivar program:
     :vartype program: str
+    :ivar tool_number:
+    :vartype tool_number: str
     :ivar prerequisites:
     :vartype prerequisites: ~ignos.api.client.models.OperationPrerequisitesDto
+    :ivar end_location:
+    :vartype end_location: str
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "production_order_number": {"required": True, "min_length": 1},
         "operation": {"required": True},
         "operation_name": {"required": True, "min_length": 1},
         "planned_start": {"required": True},
         "status": {"required": True, "min_length": 1},
         "quantity": {"required": True},
+        "produced_quantity": {"required": True},
+        "scrapped_quantity": {"required": True},
         "part_number": {"required": True, "min_length": 1},
         "resource_id": {"required": True, "min_length": 1},
         "resource_name": {"required": True, "min_length": 1},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
@@ -13675,58 +14816,66 @@
         "operation": {"key": "operation", "type": "int"},
         "operation_name": {"key": "operationName", "type": "str"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "planned_hours": {"key": "plannedHours", "type": "float"},
         "used_hours": {"key": "usedHours", "type": "float"},
         "quantity": {"key": "quantity", "type": "float"},
-        "project_name": {"key": "projectName", "type": "str"},
+        "produced_quantity": {"key": "producedQuantity", "type": "float"},
+        "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
+        "project": {"key": "project", "type": "WorkOrderProjectDto"},
         "part_number": {"key": "partNumber", "type": "str"},
         "part_revision": {"key": "partRevision", "type": "str"},
         "part_name": {"key": "partName", "type": "str"},
         "resource_id": {"key": "resourceId", "type": "str"},
         "resource_name": {"key": "resourceName", "type": "str"},
         "bom_position": {"key": "bomPosition", "type": "str"},
         "customer_name": {"key": "customerName", "type": "str"},
         "previous_operation": {"key": "previousOperation", "type": "SurroundingOperationDto"},
         "next_operation": {"key": "nextOperation", "type": "SurroundingOperationDto"},
         "work_instructions": {"key": "workInstructions", "type": "str"},
         "description": {"key": "description", "type": "str"},
         "fixture": {"key": "fixture", "type": "str"},
         "program": {"key": "program", "type": "str"},
+        "tool_number": {"key": "toolNumber", "type": "str"},
         "prerequisites": {"key": "prerequisites", "type": "OperationPrerequisitesDto"},
+        "end_location": {"key": "endLocation", "type": "str"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         production_order_number: str,
         operation: int,
         operation_name: str,
         planned_start: datetime.datetime,
         status: str,
         quantity: float,
+        produced_quantity: float,
+        scrapped_quantity: float,
         part_number: str,
         resource_id: str,
         resource_name: str,
         planned_hours: Optional[float] = None,
         used_hours: Optional[float] = None,
-        project_name: Optional[str] = None,
+        project: Optional["_models.WorkOrderProjectDto"] = None,
         part_revision: Optional[str] = None,
         part_name: Optional[str] = None,
         bom_position: Optional[str] = None,
         customer_name: Optional[str] = None,
         previous_operation: Optional["_models.SurroundingOperationDto"] = None,
         next_operation: Optional["_models.SurroundingOperationDto"] = None,
         work_instructions: Optional[str] = None,
         description: Optional[str] = None,
         fixture: Optional[str] = None,
         program: Optional[str] = None,
+        tool_number: Optional[str] = None,
         prerequisites: Optional["_models.OperationPrerequisitesDto"] = None,
+        end_location: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword production_order_number: Required.
         :paramtype production_order_number: str
@@ -13740,16 +14889,20 @@
         :paramtype status: str
         :keyword planned_hours:
         :paramtype planned_hours: float
         :keyword used_hours:
         :paramtype used_hours: float
         :keyword quantity: Required.
         :paramtype quantity: float
-        :keyword project_name:
-        :paramtype project_name: str
+        :keyword produced_quantity: Required.
+        :paramtype produced_quantity: float
+        :keyword scrapped_quantity: Required.
+        :paramtype scrapped_quantity: float
+        :keyword project:
+        :paramtype project: ~ignos.api.client.models.WorkOrderProjectDto
         :keyword part_number: Required.
         :paramtype part_number: str
         :keyword part_revision:
         :paramtype part_revision: str
         :keyword part_name:
         :paramtype part_name: str
         :keyword resource_id: Required.
@@ -13768,42 +14921,50 @@
         :paramtype work_instructions: str
         :keyword description:
         :paramtype description: str
         :keyword fixture:
         :paramtype fixture: str
         :keyword program:
         :paramtype program: str
+        :keyword tool_number:
+        :paramtype tool_number: str
         :keyword prerequisites:
         :paramtype prerequisites: ~ignos.api.client.models.OperationPrerequisitesDto
+        :keyword end_location:
+        :paramtype end_location: str
         """
         super().__init__(**kwargs)
         self.id = id
         self.production_order_number = production_order_number
         self.operation = operation
         self.operation_name = operation_name
         self.planned_start = planned_start
         self.status = status
         self.planned_hours = planned_hours
         self.used_hours = used_hours
         self.quantity = quantity
-        self.project_name = project_name
+        self.produced_quantity = produced_quantity
+        self.scrapped_quantity = scrapped_quantity
+        self.project = project
         self.part_number = part_number
         self.part_revision = part_revision
         self.part_name = part_name
         self.resource_id = resource_id
         self.resource_name = resource_name
         self.bom_position = bom_position
         self.customer_name = customer_name
         self.previous_operation = previous_operation
         self.next_operation = next_operation
         self.work_instructions = work_instructions
         self.description = description
         self.fixture = fixture
         self.program = program
+        self.tool_number = tool_number
         self.prerequisites = prerequisites
+        self.end_location = end_location
 
 
 class RegisterMeasuringToolCalibrationRequest(_serialization.Model):
     """RegisterMeasuringToolCalibrationRequest.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -15506,47 +16667,57 @@
     :vartype planned_end: ~datetime.datetime
     :ivar status: Required.
     :vartype status: str
     :ivar resource_id: Required.
     :vartype resource_id: str
     :ivar resource_name: Required.
     :vartype resource_name: str
+    :ivar produced_quantity: Required.
+    :vartype produced_quantity: float
+    :ivar scrapped_quantity: Required.
+    :vartype scrapped_quantity: float
     """
 
     _validation = {
         "id": {"required": True, "min_length": 1},
         "operation": {"required": True},
         "operation_name": {"required": True, "min_length": 1},
         "planned_start": {"required": True},
         "status": {"required": True, "min_length": 1},
         "resource_id": {"required": True, "min_length": 1},
         "resource_name": {"required": True, "min_length": 1},
+        "produced_quantity": {"required": True},
+        "scrapped_quantity": {"required": True},
     }
 
     _attribute_map = {
         "id": {"key": "id", "type": "str"},
         "operation": {"key": "operation", "type": "int"},
         "operation_name": {"key": "operationName", "type": "str"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "resource_id": {"key": "resourceId", "type": "str"},
         "resource_name": {"key": "resourceName", "type": "str"},
+        "produced_quantity": {"key": "producedQuantity", "type": "float"},
+        "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
     }
 
     def __init__(
         self,
         *,
         id: str,  # pylint: disable=redefined-builtin
         operation: int,
         operation_name: str,
         planned_start: datetime.datetime,
         status: str,
         resource_id: str,
         resource_name: str,
+        produced_quantity: float,
+        scrapped_quantity: float,
         planned_end: Optional[datetime.datetime] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword id: Required.
         :paramtype id: str
         :keyword operation: Required.
@@ -15559,24 +16730,30 @@
         :paramtype planned_end: ~datetime.datetime
         :keyword status: Required.
         :paramtype status: str
         :keyword resource_id: Required.
         :paramtype resource_id: str
         :keyword resource_name: Required.
         :paramtype resource_name: str
+        :keyword produced_quantity: Required.
+        :paramtype produced_quantity: float
+        :keyword scrapped_quantity: Required.
+        :paramtype scrapped_quantity: float
         """
         super().__init__(**kwargs)
         self.id = id
         self.operation = operation
         self.operation_name = operation_name
         self.planned_start = planned_start
         self.planned_end = planned_end
         self.status = status
         self.resource_id = resource_id
         self.resource_name = resource_name
+        self.produced_quantity = produced_quantity
+        self.scrapped_quantity = scrapped_quantity
 
 
 class SustainabilityCustomerOrderDto(_serialization.Model):
     """SustainabilityCustomerOrderDto.
 
     :ivar customer_id:
     :vartype customer_id: str
@@ -15777,14 +16954,304 @@
         """
         super().__init__(**kwargs)
         self.part_number = part_number
         self.part_revision = part_revision
         self.part_name = part_name
 
 
+class TraceDto(_serialization.Model):
+    """TraceDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar id: Required.
+    :vartype id: str
+    :ivar user:
+    :vartype user: ~ignos.api.client.models.UserDto
+    :ivar last_changed:
+    :vartype last_changed: ~datetime.datetime
+    :ivar part: Required.
+    :vartype part: ~ignos.api.client.models.PartDto
+    :ivar items: Required.
+    :vartype items: list[~ignos.api.client.models.TraceItemDto]
+    :ivar override_material_details:
+    :vartype override_material_details: list[~ignos.api.client.models.TraceMaterialDetailDto]
+    """
+
+    _validation = {
+        "id": {"required": True, "min_length": 1},
+        "part": {"required": True},
+        "items": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "user": {"key": "user", "type": "UserDto"},
+        "last_changed": {"key": "lastChanged", "type": "iso-8601"},
+        "part": {"key": "part", "type": "PartDto"},
+        "items": {"key": "items", "type": "[TraceItemDto]"},
+        "override_material_details": {"key": "overrideMaterialDetails", "type": "[TraceMaterialDetailDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: str,  # pylint: disable=redefined-builtin
+        part: "_models.PartDto",
+        items: List["_models.TraceItemDto"],
+        user: Optional["_models.UserDto"] = None,
+        last_changed: Optional[datetime.datetime] = None,
+        override_material_details: Optional[List["_models.TraceMaterialDetailDto"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id: Required.
+        :paramtype id: str
+        :keyword user:
+        :paramtype user: ~ignos.api.client.models.UserDto
+        :keyword last_changed:
+        :paramtype last_changed: ~datetime.datetime
+        :keyword part: Required.
+        :paramtype part: ~ignos.api.client.models.PartDto
+        :keyword items: Required.
+        :paramtype items: list[~ignos.api.client.models.TraceItemDto]
+        :keyword override_material_details:
+        :paramtype override_material_details: list[~ignos.api.client.models.TraceMaterialDetailDto]
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.user = user
+        self.last_changed = last_changed
+        self.part = part
+        self.items = items
+        self.override_material_details = override_material_details
+
+
+class TraceItemConsumptionDto(_serialization.Model):
+    """TraceItemConsumptionDto.
+
+    :ivar source_work_order:
+    :vartype source_work_order: str
+    :ivar source_sequence:
+    :vartype source_sequence: str
+    :ivar trace_number:
+    :vartype trace_number: str
+    :ivar heat:
+    :vartype heat: str
+    :ivar quantity_used:
+    :vartype quantity_used: float
+    """
+
+    _attribute_map = {
+        "source_work_order": {"key": "sourceWorkOrder", "type": "str"},
+        "source_sequence": {"key": "sourceSequence", "type": "str"},
+        "trace_number": {"key": "traceNumber", "type": "str"},
+        "heat": {"key": "heat", "type": "str"},
+        "quantity_used": {"key": "quantityUsed", "type": "float"},
+    }
+
+    def __init__(
+        self,
+        *,
+        source_work_order: Optional[str] = None,
+        source_sequence: Optional[str] = None,
+        trace_number: Optional[str] = None,
+        heat: Optional[str] = None,
+        quantity_used: Optional[float] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword source_work_order:
+        :paramtype source_work_order: str
+        :keyword source_sequence:
+        :paramtype source_sequence: str
+        :keyword trace_number:
+        :paramtype trace_number: str
+        :keyword heat:
+        :paramtype heat: str
+        :keyword quantity_used:
+        :paramtype quantity_used: float
+        """
+        super().__init__(**kwargs)
+        self.source_work_order = source_work_order
+        self.source_sequence = source_sequence
+        self.trace_number = trace_number
+        self.heat = heat
+        self.quantity_used = quantity_used
+
+
+class TraceItemDto(_serialization.Model):
+    """TraceItemDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar sequence: Required.
+    :vartype sequence: str
+    :ivar serial_number:
+    :vartype serial_number: str
+    :ivar status: Required. Known values are: "None", "OK", and "Scrap".
+    :vartype status: str or ~ignos.api.client.models.TraceItemStatus
+    :ivar quantity: Required.
+    :vartype quantity: float
+    :ivar materials: Required.
+    :vartype materials: list[~ignos.api.client.models.TraceListItemDto]
+    """
+
+    _validation = {
+        "sequence": {"required": True, "min_length": 1},
+        "status": {"required": True},
+        "quantity": {"required": True},
+        "materials": {"required": True},
+    }
+
+    _attribute_map = {
+        "sequence": {"key": "sequence", "type": "str"},
+        "serial_number": {"key": "serialNumber", "type": "str"},
+        "status": {"key": "status", "type": "str"},
+        "quantity": {"key": "quantity", "type": "float"},
+        "materials": {"key": "materials", "type": "[TraceListItemDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        sequence: str,
+        status: Union[str, "_models.TraceItemStatus"],
+        quantity: float,
+        materials: List["_models.TraceListItemDto"],
+        serial_number: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword sequence: Required.
+        :paramtype sequence: str
+        :keyword serial_number:
+        :paramtype serial_number: str
+        :keyword status: Required. Known values are: "None", "OK", and "Scrap".
+        :paramtype status: str or ~ignos.api.client.models.TraceItemStatus
+        :keyword quantity: Required.
+        :paramtype quantity: float
+        :keyword materials: Required.
+        :paramtype materials: list[~ignos.api.client.models.TraceListItemDto]
+        """
+        super().__init__(**kwargs)
+        self.sequence = sequence
+        self.serial_number = serial_number
+        self.status = status
+        self.quantity = quantity
+        self.materials = materials
+
+
+class TraceListItemDto(_serialization.Model):
+    """TraceListItemDto.
+
+    :ivar material_line:
+    :vartype material_line: int
+    :ivar operation:
+    :vartype operation: int
+    :ivar material_quantity:
+    :vartype material_quantity: float
+    :ivar part_number:
+    :vartype part_number: str
+    :ivar consumptions:
+    :vartype consumptions: list[~ignos.api.client.models.TraceItemConsumptionDto]
+    """
+
+    _attribute_map = {
+        "material_line": {"key": "materialLine", "type": "int"},
+        "operation": {"key": "operation", "type": "int"},
+        "material_quantity": {"key": "materialQuantity", "type": "float"},
+        "part_number": {"key": "partNumber", "type": "str"},
+        "consumptions": {"key": "consumptions", "type": "[TraceItemConsumptionDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        material_line: Optional[int] = None,
+        operation: Optional[int] = None,
+        material_quantity: Optional[float] = None,
+        part_number: Optional[str] = None,
+        consumptions: Optional[List["_models.TraceItemConsumptionDto"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword material_line:
+        :paramtype material_line: int
+        :keyword operation:
+        :paramtype operation: int
+        :keyword material_quantity:
+        :paramtype material_quantity: float
+        :keyword part_number:
+        :paramtype part_number: str
+        :keyword consumptions:
+        :paramtype consumptions: list[~ignos.api.client.models.TraceItemConsumptionDto]
+        """
+        super().__init__(**kwargs)
+        self.material_line = material_line
+        self.operation = operation
+        self.material_quantity = material_quantity
+        self.part_number = part_number
+        self.consumptions = consumptions
+
+
+class TraceMaterialDetailDto(_serialization.Model):
+    """TraceMaterialDetailDto.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar material_line: Required.
+    :vartype material_line: int
+    :ivar operation:
+    :vartype operation: int
+    :ivar material_part_number: Required.
+    :vartype material_part_number: str
+    :ivar status: Required. Known values are: "None", "ForceInclude", and "Exclude".
+    :vartype status: str or ~ignos.api.client.models.TraceIncludeStatus
+    """
+
+    _validation = {
+        "material_line": {"required": True},
+        "material_part_number": {"required": True, "min_length": 1},
+        "status": {"required": True},
+    }
+
+    _attribute_map = {
+        "material_line": {"key": "materialLine", "type": "int"},
+        "operation": {"key": "operation", "type": "int"},
+        "material_part_number": {"key": "materialPartNumber", "type": "str"},
+        "status": {"key": "status", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        material_line: int,
+        material_part_number: str,
+        status: Union[str, "_models.TraceIncludeStatus"],
+        operation: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword material_line: Required.
+        :paramtype material_line: int
+        :keyword operation:
+        :paramtype operation: int
+        :keyword material_part_number: Required.
+        :paramtype material_part_number: str
+        :keyword status: Required. Known values are: "None", "ForceInclude", and "Exclude".
+        :paramtype status: str or ~ignos.api.client.models.TraceIncludeStatus
+        """
+        super().__init__(**kwargs)
+        self.material_line = material_line
+        self.operation = operation
+        self.material_part_number = material_part_number
+        self.status = status
+
+
 class UnregisteredToolValueDto(_serialization.Model):
     """UnregisteredToolValueDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar unregistered_tool: Required.
     :vartype unregistered_tool: str
@@ -16957,14 +18424,81 @@
         :paramtype max_number_of_usages_between_calibration: int
         """
         super().__init__(**kwargs)
         self.calibration_interval = calibration_interval
         self.max_number_of_usages_between_calibration = max_number_of_usages_between_calibration
 
 
+class UpdateMrbTemplateRequest(_serialization.Model):
+    """UpdateMrbTemplateRequest.
+
+    :ivar id:
+    :vartype id: str
+    :ivar title:
+    :vartype title: str
+    :ivar customer_id:
+    :vartype customer_id: str
+    :ivar customer_group_id:
+    :vartype customer_group_id: str
+    :ivar customer_name:
+    :vartype customer_name: str
+    :ivar url:
+    :vartype url: str
+    :ivar elements:
+    :vartype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "title": {"key": "title", "type": "str"},
+        "customer_id": {"key": "customerId", "type": "str"},
+        "customer_group_id": {"key": "customerGroupId", "type": "str"},
+        "customer_name": {"key": "customerName", "type": "str"},
+        "url": {"key": "url", "type": "str"},
+        "elements": {"key": "elements", "type": "[MrbTemplateElementDto]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        title: Optional[str] = None,
+        customer_id: Optional[str] = None,
+        customer_group_id: Optional[str] = None,
+        customer_name: Optional[str] = None,
+        url: Optional[str] = None,
+        elements: Optional[List["_models.MrbTemplateElementDto"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id:
+        :paramtype id: str
+        :keyword title:
+        :paramtype title: str
+        :keyword customer_id:
+        :paramtype customer_id: str
+        :keyword customer_group_id:
+        :paramtype customer_group_id: str
+        :keyword customer_name:
+        :paramtype customer_name: str
+        :keyword url:
+        :paramtype url: str
+        :keyword elements:
+        :paramtype elements: list[~ignos.api.client.models.MrbTemplateElementDto]
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.title = title
+        self.customer_id = customer_id
+        self.customer_group_id = customer_group_id
+        self.customer_name = customer_name
+        self.url = url
+        self.elements = elements
+
+
 class UpdateSchemaGroupedElementDto(_serialization.Model):
     """UpdateSchemaGroupedElementDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar balloon_id: Required.
     :vartype balloon_id: str
@@ -17779,14 +19313,40 @@
         self.planned_start = planned_start
         self.planned_end = planned_end
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
         self.customer_order_reference = customer_order_reference
 
 
+class UpsertWorkOrderConsumptionsRequest(_serialization.Model):
+    """UpsertWorkOrderConsumptionsRequest.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar material_consumptions: Required.
+    :vartype material_consumptions: list[~ignos.api.client.models.MaterialConsumptionDto]
+    """
+
+    _validation = {
+        "material_consumptions": {"required": True},
+    }
+
+    _attribute_map = {
+        "material_consumptions": {"key": "materialConsumptions", "type": "[MaterialConsumptionDto]"},
+    }
+
+    def __init__(self, *, material_consumptions: List["_models.MaterialConsumptionDto"], **kwargs: Any) -> None:
+        """
+        :keyword material_consumptions: Required.
+        :paramtype material_consumptions: list[~ignos.api.client.models.MaterialConsumptionDto]
+        """
+        super().__init__(**kwargs)
+        self.material_consumptions = material_consumptions
+
+
 class UpsertWorkorderTracesRequest(_serialization.Model):
     """UpsertWorkorderTracesRequest.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar traces: Required.
     :vartype traces: list[~ignos.api.client.models.WorkorderTraceItemDto]
@@ -17805,14 +19365,185 @@
         :keyword traces: Required.
         :paramtype traces: list[~ignos.api.client.models.WorkorderTraceItemDto]
         """
         super().__init__(**kwargs)
         self.traces = traces
 
 
+class UpsertWorkorderV2(_serialization.Model):  # pylint: disable=too-many-instance-attributes
+    """UpsertWorkorderV2.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar work_order: Required.
+    :vartype work_order: str
+    :ivar company_id:
+    :vartype company_id: str
+    :ivar part: Required.
+    :vartype part: ~ignos.api.client.models.PartDto
+    :ivar quantity: Required.
+    :vartype quantity: float
+    :ivar unit:
+    :vartype unit: str
+    :ivar status: Required. Known values are: "Draft", "Ready", "Ongoing", "Completed", and
+     "Deleted".
+    :vartype status: str or ~ignos.api.client.models.WorkorderStatus
+    :ivar operations: Required.
+    :vartype operations: list[~ignos.api.client.models.WorkorderOperationDto]
+    :ivar planned_start:
+    :vartype planned_start: ~datetime.datetime
+    :ivar planned_end:
+    :vartype planned_end: ~datetime.datetime
+    :ivar produced_quantity:
+    :vartype produced_quantity: float
+    :ivar scrapped_quantity:
+    :vartype scrapped_quantity: float
+    :ivar customer_order_reference:
+    :vartype customer_order_reference: ~ignos.api.client.models.WorkorderCustomerOrderReferenceDto
+    :ivar planner:
+    :vartype planner: ~ignos.api.client.models.UserDto
+    :ivar project_leader:
+    :vartype project_leader: ~ignos.api.client.models.UserDto
+    :ivar end_location:
+    :vartype end_location: str
+    :ivar project:
+    :vartype project: ~ignos.api.client.models.WorkOrderProject
+    :ivar start_date:
+    :vartype start_date: ~datetime.datetime
+    :ivar end_date:
+    :vartype end_date: ~datetime.datetime
+    :ivar bom_position:
+    :vartype bom_position: str
+    :ivar trace_type: Known values are: "None", "Lot", "Batch", and "SerialNumber".
+    :vartype trace_type: str or ~ignos.api.client.models.TraceType
+    """
+
+    _validation = {
+        "work_order": {"required": True, "min_length": 1},
+        "part": {"required": True},
+        "quantity": {"required": True},
+        "status": {"required": True},
+        "operations": {"required": True},
+    }
+
+    _attribute_map = {
+        "work_order": {"key": "workOrder", "type": "str"},
+        "company_id": {"key": "companyId", "type": "str"},
+        "part": {"key": "part", "type": "PartDto"},
+        "quantity": {"key": "quantity", "type": "float"},
+        "unit": {"key": "unit", "type": "str"},
+        "status": {"key": "status", "type": "str"},
+        "operations": {"key": "operations", "type": "[WorkorderOperationDto]"},
+        "planned_start": {"key": "plannedStart", "type": "iso-8601"},
+        "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
+        "produced_quantity": {"key": "producedQuantity", "type": "float"},
+        "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
+        "customer_order_reference": {"key": "customerOrderReference", "type": "WorkorderCustomerOrderReferenceDto"},
+        "planner": {"key": "planner", "type": "UserDto"},
+        "project_leader": {"key": "projectLeader", "type": "UserDto"},
+        "end_location": {"key": "endLocation", "type": "str"},
+        "project": {"key": "project", "type": "WorkOrderProject"},
+        "start_date": {"key": "startDate", "type": "iso-8601"},
+        "end_date": {"key": "endDate", "type": "iso-8601"},
+        "bom_position": {"key": "bomPosition", "type": "str"},
+        "trace_type": {"key": "traceType", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        work_order: str,
+        part: "_models.PartDto",
+        quantity: float,
+        status: Union[str, "_models.WorkorderStatus"],
+        operations: List["_models.WorkorderOperationDto"],
+        company_id: Optional[str] = None,
+        unit: Optional[str] = None,
+        planned_start: Optional[datetime.datetime] = None,
+        planned_end: Optional[datetime.datetime] = None,
+        produced_quantity: Optional[float] = None,
+        scrapped_quantity: Optional[float] = None,
+        customer_order_reference: Optional["_models.WorkorderCustomerOrderReferenceDto"] = None,
+        planner: Optional["_models.UserDto"] = None,
+        project_leader: Optional["_models.UserDto"] = None,
+        end_location: Optional[str] = None,
+        project: Optional["_models.WorkOrderProject"] = None,
+        start_date: Optional[datetime.datetime] = None,
+        end_date: Optional[datetime.datetime] = None,
+        bom_position: Optional[str] = None,
+        trace_type: Optional[Union[str, "_models.TraceType"]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword work_order: Required.
+        :paramtype work_order: str
+        :keyword company_id:
+        :paramtype company_id: str
+        :keyword part: Required.
+        :paramtype part: ~ignos.api.client.models.PartDto
+        :keyword quantity: Required.
+        :paramtype quantity: float
+        :keyword unit:
+        :paramtype unit: str
+        :keyword status: Required. Known values are: "Draft", "Ready", "Ongoing", "Completed", and
+         "Deleted".
+        :paramtype status: str or ~ignos.api.client.models.WorkorderStatus
+        :keyword operations: Required.
+        :paramtype operations: list[~ignos.api.client.models.WorkorderOperationDto]
+        :keyword planned_start:
+        :paramtype planned_start: ~datetime.datetime
+        :keyword planned_end:
+        :paramtype planned_end: ~datetime.datetime
+        :keyword produced_quantity:
+        :paramtype produced_quantity: float
+        :keyword scrapped_quantity:
+        :paramtype scrapped_quantity: float
+        :keyword customer_order_reference:
+        :paramtype customer_order_reference:
+         ~ignos.api.client.models.WorkorderCustomerOrderReferenceDto
+        :keyword planner:
+        :paramtype planner: ~ignos.api.client.models.UserDto
+        :keyword project_leader:
+        :paramtype project_leader: ~ignos.api.client.models.UserDto
+        :keyword end_location:
+        :paramtype end_location: str
+        :keyword project:
+        :paramtype project: ~ignos.api.client.models.WorkOrderProject
+        :keyword start_date:
+        :paramtype start_date: ~datetime.datetime
+        :keyword end_date:
+        :paramtype end_date: ~datetime.datetime
+        :keyword bom_position:
+        :paramtype bom_position: str
+        :keyword trace_type: Known values are: "None", "Lot", "Batch", and "SerialNumber".
+        :paramtype trace_type: str or ~ignos.api.client.models.TraceType
+        """
+        super().__init__(**kwargs)
+        self.work_order = work_order
+        self.company_id = company_id
+        self.part = part
+        self.quantity = quantity
+        self.unit = unit
+        self.status = status
+        self.operations = operations
+        self.planned_start = planned_start
+        self.planned_end = planned_end
+        self.produced_quantity = produced_quantity
+        self.scrapped_quantity = scrapped_quantity
+        self.customer_order_reference = customer_order_reference
+        self.planner = planner
+        self.project_leader = project_leader
+        self.end_location = end_location
+        self.project = project
+        self.start_date = start_date
+        self.end_date = end_date
+        self.bom_position = bom_position
+        self.trace_type = trace_type
+
+
 class UptimeDowntimeDto(_serialization.Model):
     """UptimeDowntimeDto.
 
     :ivar uptime_in_seconds:
     :vartype uptime_in_seconds: int
     :ivar downtime_in_seconds:
     :vartype downtime_in_seconds: int
@@ -18892,14 +20623,16 @@
     :vartype quantity_per_part: float
     :ivar fixed_quantity: Required.
     :vartype fixed_quantity: bool
     :ivar used_quantity:
     :vartype used_quantity: float
     :ivar unit:
     :vartype unit: str
+    :ivar trace_type: Known values are: "None", "Lot", "Batch", and "SerialNumber".
+    :vartype trace_type: str or ~ignos.api.client.models.TraceType
     """
 
     _validation = {
         "status": {"required": True},
         "material": {"required": True},
         "quantity_per_part": {"required": True},
         "fixed_quantity": {"required": True},
@@ -18909,26 +20642,28 @@
         "material_line": {"key": "materialLine", "type": "int"},
         "status": {"key": "status", "type": "str"},
         "material": {"key": "material", "type": "PartDto"},
         "quantity_per_part": {"key": "quantityPerPart", "type": "float"},
         "fixed_quantity": {"key": "fixedQuantity", "type": "bool"},
         "used_quantity": {"key": "usedQuantity", "type": "float"},
         "unit": {"key": "unit", "type": "str"},
+        "trace_type": {"key": "traceType", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         status: Union[str, "_models.MaterialStatus"],
         material: "_models.PartDto",
         quantity_per_part: float,
         fixed_quantity: bool,
         material_line: Optional[int] = None,
         used_quantity: Optional[float] = None,
         unit: Optional[str] = None,
+        trace_type: Optional[Union[str, "_models.TraceType"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword material_line:
         :paramtype material_line: int
         :keyword status: Required. Known values are: "Unknown", "NotStarted", "Partial", and
          "Completed".
@@ -18939,23 +20674,26 @@
         :paramtype quantity_per_part: float
         :keyword fixed_quantity: Required.
         :paramtype fixed_quantity: bool
         :keyword used_quantity:
         :paramtype used_quantity: float
         :keyword unit:
         :paramtype unit: str
+        :keyword trace_type: Known values are: "None", "Lot", "Batch", and "SerialNumber".
+        :paramtype trace_type: str or ~ignos.api.client.models.TraceType
         """
         super().__init__(**kwargs)
         self.material_line = material_line
         self.status = status
         self.material = material
         self.quantity_per_part = quantity_per_part
         self.fixed_quantity = fixed_quantity
         self.used_quantity = used_quantity
         self.unit = unit
+        self.trace_type = trace_type
 
 
 class WorkorderOperationDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """WorkorderOperationDto.
 
     All required parameters must be populated in order to send to Azure.
 
@@ -18963,23 +20701,26 @@
     :vartype operation: int
     :ivar description:
     :vartype description: str
     :ivar planned_setup_time: Required.
     :vartype planned_setup_time: float
     :ivar planned_production_time_per_part: Required.
     :vartype planned_production_time_per_part: float
+    :ivar planned_production_time: Required.
+    :vartype planned_production_time: float
     :ivar fixed_time:
     :vartype fixed_time: bool
     :ivar resource: Required.
     :vartype resource: ~ignos.api.client.models.ResourceDto
     :ivar planned_start:
     :vartype planned_start: ~datetime.datetime
     :ivar planned_end:
     :vartype planned_end: ~datetime.datetime
-    :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", and "Completed".
+    :ivar status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
+     "Stopped".
     :vartype status: str or ~ignos.api.client.models.OperationStatus
     :ivar produced_quantity: Required.
     :vartype produced_quantity: float
     :ivar scrapped_quantity: Required.
     :vartype scrapped_quantity: float
     :ivar used_production_time: Required.
     :vartype used_production_time: float
@@ -18989,28 +20730,30 @@
     :vartype materials: list[~ignos.api.client.models.WorkorderMaterialDto]
     """
 
     _validation = {
         "operation": {"required": True},
         "planned_setup_time": {"required": True},
         "planned_production_time_per_part": {"required": True},
+        "planned_production_time": {"required": True},
         "resource": {"required": True},
         "status": {"required": True},
         "produced_quantity": {"required": True},
         "scrapped_quantity": {"required": True},
         "used_production_time": {"required": True},
         "used_setup_time": {"required": True},
         "materials": {"required": True},
     }
 
     _attribute_map = {
         "operation": {"key": "operation", "type": "int"},
         "description": {"key": "description", "type": "str"},
         "planned_setup_time": {"key": "plannedSetupTime", "type": "float"},
         "planned_production_time_per_part": {"key": "plannedProductionTimePerPart", "type": "float"},
+        "planned_production_time": {"key": "plannedProductionTime", "type": "float"},
         "fixed_time": {"key": "fixedTime", "type": "bool"},
         "resource": {"key": "resource", "type": "ResourceDto"},
         "planned_start": {"key": "plannedStart", "type": "iso-8601"},
         "planned_end": {"key": "plannedEnd", "type": "iso-8601"},
         "status": {"key": "status", "type": "str"},
         "produced_quantity": {"key": "producedQuantity", "type": "float"},
         "scrapped_quantity": {"key": "scrappedQuantity", "type": "float"},
@@ -19021,14 +20764,15 @@
 
     def __init__(
         self,
         *,
         operation: int,
         planned_setup_time: float,
         planned_production_time_per_part: float,
+        planned_production_time: float,
         resource: "_models.ResourceDto",
         status: Union[str, "_models.OperationStatus"],
         produced_quantity: float,
         scrapped_quantity: float,
         used_production_time: float,
         used_setup_time: float,
         materials: List["_models.WorkorderMaterialDto"],
@@ -19043,23 +20787,26 @@
         :paramtype operation: int
         :keyword description:
         :paramtype description: str
         :keyword planned_setup_time: Required.
         :paramtype planned_setup_time: float
         :keyword planned_production_time_per_part: Required.
         :paramtype planned_production_time_per_part: float
+        :keyword planned_production_time: Required.
+        :paramtype planned_production_time: float
         :keyword fixed_time:
         :paramtype fixed_time: bool
         :keyword resource: Required.
         :paramtype resource: ~ignos.api.client.models.ResourceDto
         :keyword planned_start:
         :paramtype planned_start: ~datetime.datetime
         :keyword planned_end:
         :paramtype planned_end: ~datetime.datetime
-        :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", and "Completed".
+        :keyword status: Required. Known values are: "NotReady", "Ready", "Ongoing", "Completed", and
+         "Stopped".
         :paramtype status: str or ~ignos.api.client.models.OperationStatus
         :keyword produced_quantity: Required.
         :paramtype produced_quantity: float
         :keyword scrapped_quantity: Required.
         :paramtype scrapped_quantity: float
         :keyword used_production_time: Required.
         :paramtype used_production_time: float
@@ -19069,14 +20816,15 @@
         :paramtype materials: list[~ignos.api.client.models.WorkorderMaterialDto]
         """
         super().__init__(**kwargs)
         self.operation = operation
         self.description = description
         self.planned_setup_time = planned_setup_time
         self.planned_production_time_per_part = planned_production_time_per_part
+        self.planned_production_time = planned_production_time
         self.fixed_time = fixed_time
         self.resource = resource
         self.planned_start = planned_start
         self.planned_end = planned_end
         self.status = status
         self.produced_quantity = produced_quantity
         self.scrapped_quantity = scrapped_quantity
@@ -19201,14 +20949,53 @@
         self.resource_id = resource_id
         self.description = description
         self.part = part
         self.workorder_description = workorder_description
         self.operation_description = operation_description
 
 
+class WorkOrderProject(_serialization.Model):
+    """WorkOrderProject.
+
+    :ivar id:
+    :vartype id: str
+    :ivar name:
+    :vartype name: str
+    :ivar project_manager:
+    :vartype project_manager: str
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "project_manager": {"key": "projectManager", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        name: Optional[str] = None,
+        project_manager: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id:
+        :paramtype id: str
+        :keyword name:
+        :paramtype name: str
+        :keyword project_manager:
+        :paramtype project_manager: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.name = name
+        self.project_manager = project_manager
+
+
 class WorkOrderProjectDto(_serialization.Model):
     """WorkOrderProjectDto.
 
     :ivar id:
     :vartype id: str
     :ivar name:
     :vartype name: str
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/models/_patch.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/operations/__init__.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ._operations import AssetsOperations
 from ._operations import AzureRegionsOperations
 from ._operations import CdfOperations
 from ._operations import CncFileTransferOperations
 from ._operations import CncSetupOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
+from ._operations import DocumentsOperations
+from ._operations import DocumentTypesOperations
 from ._operations import CustomerOrdersOperations
 from ._operations import WorkordersOperations
 from ._operations import ExternalOperations
 from ._operations import ExternalAccessOperations
 from ._operations import ExternalServicesOperations
 from ._operations import ElectricalOperations
 from ._operations import WeldingOperations
@@ -29,20 +31,22 @@
 from ._operations import MeasurementFormSchemasOperations
 from ._operations import MeasurementFormsInstancesOperations
 from ._operations import MeasuringToolsOperations
 from ._operations import MesOperations
 from ._operations import MesProductionOrderOperations
 from ._operations import MesProductionScheduleOperations
 from ._operations import MesResourceOperations
+from ._operations import MrbOperations
 from ._operations import OperatorCalculatorsOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
 from ._operations import SuppliersOperations
 from ._operations import SustainabilityOperations
 from ._operations import SystemHealthDashboardOperations
+from ._operations import TraceOperations
 from ._operations import UploadOperations
 from ._operations import UsersOperations
 from ._operations import WorkspacesOperations
 from ._operations import WorkspaceTemplatesAdminOperations
 from ._operations import WorkspaceTemplatesOperations
 
 from ._patch import __all__ as _patch_all
@@ -54,14 +58,16 @@
     "AssetsOperations",
     "AzureRegionsOperations",
     "CdfOperations",
     "CncFileTransferOperations",
     "CncSetupOperations",
     "CountriesOperations",
     "CustomersOperations",
+    "DocumentsOperations",
+    "DocumentTypesOperations",
     "CustomerOrdersOperations",
     "WorkordersOperations",
     "ExternalOperations",
     "ExternalAccessOperations",
     "ExternalServicesOperations",
     "ElectricalOperations",
     "WeldingOperations",
@@ -73,20 +79,22 @@
     "MeasurementFormSchemasOperations",
     "MeasurementFormsInstancesOperations",
     "MeasuringToolsOperations",
     "MesOperations",
     "MesProductionOrderOperations",
     "MesProductionScheduleOperations",
     "MesResourceOperations",
+    "MrbOperations",
     "OperatorCalculatorsOperations",
     "PowerOperations",
     "PresentationOperations",
     "SuppliersOperations",
     "SustainabilityOperations",
     "SystemHealthDashboardOperations",
+    "TraceOperations",
     "UploadOperations",
     "UsersOperations",
     "WorkspacesOperations",
     "WorkspaceTemplatesAdminOperations",
     "WorkspaceTemplatesOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_operations.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/operations/_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1386,14 +1386,160 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_documents_import_document_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/documents/import"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_documents_import_document_contents_request(*, json: Optional[JSON] = None, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/documents/importcontent"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, json=json, **kwargs)
+
+
+def build_document_types_list_document_types_request(*, include_inactive: bool = False, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/documenttypes"
+
+    # Construct parameters
+    if include_inactive is not None:
+        _params["includeInactive"] = _SERIALIZER.query("include_inactive", include_inactive, "bool")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_document_types_create_document_type_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/documenttypes"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_document_types_update_document_type_request(
+    id: str, *, json: Optional[JSON] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/documenttypes/{id}"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, json=json, **kwargs)
+
+
+def build_document_types_delete_document_type_request(id: str, **kwargs: Any) -> HttpRequest:
+    # Construct URL
+    _url = "/documenttypes/{id}"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    return HttpRequest(method="DELETE", url=_url, **kwargs)
+
+
+def build_document_types_active_document_type_request(id: str, **kwargs: Any) -> HttpRequest:
+    # Construct URL
+    _url = "/documenttypes/{id}/activate"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    return HttpRequest(method="POST", url=_url, **kwargs)
+
+
+def build_document_types_deactive_document_type_request(id: str, **kwargs: Any) -> HttpRequest:
+    # Construct URL
+    _url = "/documenttypes/{id}/deactivate"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    return HttpRequest(method="POST", url=_url, **kwargs)
+
+
+def build_document_types_list_available_tags_for_document_type_request(id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/documenttypes/{id}/availabletags"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_customer_orders_upsert_customer_order_request(id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     # Construct URL
     _url = "/erp/customerorders/{id}"
     path_format_arguments = {
@@ -1439,14 +1585,28 @@
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_workorders_upsert_workorder_v2_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/erp/workorders"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
 def build_workorders_list_workorders_request(
     *,
     page_size: int = 50,
     search: Optional[str] = None,
     active_orders: Optional[bool] = None,
     continuation_token_parameter: Optional[str] = None,
     **kwargs: Any
@@ -1473,14 +1633,33 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_workorders_upsert_workorder_consumption_request(id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/erp/workorders/{id}/consumptions"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
 def build_workorders_upsert_workorder_traces_request(id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     # Construct URL
     _url = "/erp/workorders/{id}/traces"
     path_format_arguments = {
@@ -5192,14 +5371,123 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
+def build_mrb_attach_pdf_request(template_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/mrb/templates/{templateId}"
+    path_format_arguments = {
+        "templateId": _SERIALIZER.url("template_id", template_id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
+def build_mrb_get_mrb_template_request(template_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/mrb/templates/{templateId}"
+    path_format_arguments = {
+        "templateId": _SERIALIZER.url("template_id", template_id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_mrb_list_mrb_templates_request(
+    *, customer_id: Optional[str] = None, customer_group_id: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/mrb/templates"
+
+    # Construct parameters
+    if customer_id is not None:
+        _params["customerId"] = _SERIALIZER.query("customer_id", customer_id, "str")
+    if customer_group_id is not None:
+        _params["customerGroupId"] = _SERIALIZER.query("customer_group_id", customer_group_id, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+def build_mrb_create_mrb_template_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/mrb/templates"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_mrb_update_mrb_template_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/mrb/templates"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+
+
+def build_mrb_delete_mrb_template_request(**kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/mrb/templates"
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
+
+
 def build_operator_calculators_calculate_spindle_and_cutting_speed_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -5527,14 +5815,33 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_trace_get_work_order_trace_request(id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/trace/{id}"
+    path_format_arguments = {
+        "id": _SERIALIZER.url("id", id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_upload_create_upload_info_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/upload"
@@ -11167,14 +11474,605 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class DocumentsOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`documents` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    def import_document(
+        self, body: Optional[_models.ImportDocument] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        """Import document with revisions from other systems.
+
+        Import document with revisions from other systems.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.ImportDocument
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def import_document(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> JSON:
+        """Import document with revisions from other systems.
+
+        Import document with revisions from other systems.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: JSON
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def import_document(self, body: Optional[Union[_models.ImportDocument, IO]] = None, **kwargs: Any) -> JSON:
+        """Import document with revisions from other systems.
+
+        Import document with revisions from other systems.
+
+        :param body: Is either a ImportDocument type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.ImportDocument or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: JSON
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "ImportDocument")
+            else:
+                _json = None
+
+        request = build_documents_import_document_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("object", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def import_document_contents(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[JSON] = None, **kwargs: Any
+    ) -> None:
+        """Register imported content for document revisions.
+
+        Register imported content for document revisions.
+
+        :param body: Default value is None.
+        :type body: JSON
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: str = kwargs.pop("content_type", _headers.pop("Content-Type", "application/json"))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        if body is not None:
+            _json = self._serialize.body(body, "object")
+        else:
+            _json = None
+
+        request = build_documents_import_document_contents_request(
+            content_type=content_type,
+            json=_json,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
+class DocumentTypesOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`document_types` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def list_document_types(self, *, include_inactive: bool = False, **kwargs: Any) -> List[_models.DocumentTypeDto]:
+        """list_document_types.
+
+        :keyword include_inactive: Default value is False.
+        :paramtype include_inactive: bool
+        :return: list of DocumentTypeDto
+        :rtype: list[~ignos.api.client.models.DocumentTypeDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.DocumentTypeDto]] = kwargs.pop("cls", None)
+
+        request = build_document_types_list_document_types_request(
+            include_inactive=include_inactive,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[DocumentTypeDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    def create_document_type(
+        self,
+        body: Optional[_models.CreateDocumentType] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """create_document_type.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateDocumentType
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_document_type(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """create_document_type.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_document_type(
+        self, body: Optional[Union[_models.CreateDocumentType, IO]] = None, **kwargs: Any
+    ) -> _models.DocumentTypeDto:
+        """create_document_type.
+
+        :param body: Is either a CreateDocumentType type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.CreateDocumentType or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.DocumentTypeDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateDocumentType")
+            else:
+                _json = None
+
+        request = build_document_types_create_document_type_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("DocumentTypeDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def update_document_type(self, id: str, body: Optional[JSON] = None, **kwargs: Any) -> _models.DocumentTypeDto:
+        """update_document_type.
+
+        :param id: Required.
+        :type id: str
+        :param body: Default value is None.
+        :type body: JSON
+        :return: DocumentTypeDto
+        :rtype: ~ignos.api.client.models.DocumentTypeDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: str = kwargs.pop("content_type", _headers.pop("Content-Type", "application/json"))
+        cls: ClsType[_models.DocumentTypeDto] = kwargs.pop("cls", None)
+
+        if body is not None:
+            _json = self._serialize.body(body, "object")
+        else:
+            _json = None
+
+        request = build_document_types_update_document_type_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("DocumentTypeDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def delete_document_type(self, id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
+        """Delete document type. Only allowed if not used.
+
+        Delete document type. Only allowed if not used.
+
+        :param id: Required.
+        :type id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_document_types_delete_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace
+    def active_document_type(self, id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
+        """active_document_type.
+
+        :param id: Required.
+        :type id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_document_types_active_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace
+    def deactive_document_type(self, id: str, **kwargs: Any) -> None:  # pylint: disable=inconsistent-return-statements
+        """deactive_document_type.
+
+        :param id: Required.
+        :type id: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_document_types_deactive_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace
+    def list_available_tags_for_document_type(self, id: str, **kwargs: Any) -> List[str]:
+        """list_available_tags_for_document_type.
+
+        :param id: Required.
+        :type id: str
+        :return: list of str
+        :rtype: list[str]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[str]] = kwargs.pop("cls", None)
+
+        request = build_document_types_list_available_tags_for_document_type_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[str]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+
 class CustomerOrdersOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.IgnosPortal`'s
@@ -11546,14 +12444,116 @@
         if response.status_code not in [204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response)
 
         if cls:
             return cls(pipeline_response, None, {})
 
+    @overload
+    def upsert_workorder_v2(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[_models.UpsertWorkorderV2] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Create or update a workorder.
+
+        Create or update a workorder.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkorderV2
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def upsert_workorder_v2(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Create or update a workorder.
+
+        Create or update a workorder.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def upsert_workorder_v2(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.UpsertWorkorderV2, IO]] = None, **kwargs: Any
+    ) -> None:
+        """Create or update a workorder.
+
+        Create or update a workorder.
+
+        :param body: Is either a UpsertWorkorderV2 type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkorderV2 or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpsertWorkorderV2")
+            else:
+                _json = None
+
+        request = build_workorders_upsert_workorder_v2_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
     @distributed_trace
     def list_workorders(
         self,
         *,
         page_size: int = 50,
         search: Optional[str] = None,
         active_orders: Optional[bool] = None,
@@ -11617,14 +12617,129 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     @overload
+    def upsert_workorder_consumption(  # pylint: disable=inconsistent-return-statements
+        self,
+        id: str,
+        body: Optional[_models.UpsertWorkOrderConsumptionsRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Update consumed materials on work order.
+
+        Update consumed materials on work order.
+
+        :param id: Work order id. Required.
+        :type id: str
+        :param body: Consumption details. Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkOrderConsumptionsRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def upsert_workorder_consumption(  # pylint: disable=inconsistent-return-statements
+        self, id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Update consumed materials on work order.
+
+        Update consumed materials on work order.
+
+        :param id: Work order id. Required.
+        :type id: str
+        :param body: Consumption details. Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def upsert_workorder_consumption(  # pylint: disable=inconsistent-return-statements
+        self, id: str, body: Optional[Union[_models.UpsertWorkOrderConsumptionsRequest, IO]] = None, **kwargs: Any
+    ) -> None:
+        """Update consumed materials on work order.
+
+        Update consumed materials on work order.
+
+        :param id: Work order id. Required.
+        :type id: str
+        :param body: Consumption details. Is either a UpsertWorkOrderConsumptionsRequest type or a IO
+         type. Default value is None.
+        :type body: ~ignos.api.client.models.UpsertWorkOrderConsumptionsRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpsertWorkOrderConsumptionsRequest")
+            else:
+                _json = None
+
+        request = build_workorders_upsert_workorder_consumption_request(
+            id=id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [204]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
     def upsert_workorder_traces(  # pylint: disable=inconsistent-return-statements
         self,
         id: str,
         body: Optional[_models.UpsertWorkorderTracesRequest] = None,
         *,
         content_type: str = "application/json",
         **kwargs: Any
@@ -25204,14 +26319,573 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class MrbOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`mrb` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    def attach_pdf(  # pylint: disable=inconsistent-return-statements
+        self,
+        template_id: str,
+        body: Optional[_models.AttachPdfRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """attach_pdf.
+
+        :param template_id: Required.
+        :type template_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.AttachPdfRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def attach_pdf(  # pylint: disable=inconsistent-return-statements
+        self, template_id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """attach_pdf.
+
+        :param template_id: Required.
+        :type template_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def attach_pdf(  # pylint: disable=inconsistent-return-statements
+        self, template_id: str, body: Optional[Union[_models.AttachPdfRequest, IO]] = None, **kwargs: Any
+    ) -> None:
+        """attach_pdf.
+
+        :param template_id: Required.
+        :type template_id: str
+        :param body: Is either a AttachPdfRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.AttachPdfRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "AttachPdfRequest")
+            else:
+                _json = None
+
+        request = build_mrb_attach_pdf_request(
+            template_id=template_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @distributed_trace
+    def get_mrb_template(self, template_id: str, **kwargs: Any) -> _models.MrbTemplateDto:
+        """Get a single MRB template by id.
+
+        Get a single MRB template by id.
+
+        :param template_id: Required.
+        :type template_id: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.MrbTemplateDto] = kwargs.pop("cls", None)
+
+        request = build_mrb_get_mrb_template_request(
+            template_id=template_id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("MrbTemplateDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def list_mrb_templates(
+        self, *, customer_id: Optional[str] = None, customer_group_id: Optional[str] = None, **kwargs: Any
+    ) -> List[_models.MrbTemplateDto]:
+        """Get a list of MRB templates.
+
+        Get a list of MRB templates.
+
+        :keyword customer_id: Default value is None.
+        :paramtype customer_id: str
+        :keyword customer_group_id: Default value is None.
+        :paramtype customer_group_id: str
+        :return: list of MrbTemplateDto
+        :rtype: list[~ignos.api.client.models.MrbTemplateDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.MrbTemplateDto]] = kwargs.pop("cls", None)
+
+        request = build_mrb_list_mrb_templates_request(
+            customer_id=customer_id,
+            customer_group_id=customer_group_id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[MrbTemplateDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    def create_mrb_template(
+        self,
+        body: Optional[_models.CreateMrbTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Create a new MRB template.
+
+        Create a new MRB template.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.CreateMrbTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def create_mrb_template(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Create a new MRB template.
+
+        Create a new MRB template.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def create_mrb_template(
+        self, body: Optional[Union[_models.CreateMrbTemplateRequest, IO]] = None, **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Create a new MRB template.
+
+        Create a new MRB template.
+
+        :param body: Is either a CreateMrbTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.CreateMrbTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MrbTemplateDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "CreateMrbTemplateRequest")
+            else:
+                _json = None
+
+        request = build_mrb_create_mrb_template_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("MrbTemplateDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    def update_mrb_template(
+        self,
+        body: Optional[_models.UpdateMrbTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Update an MRB template.
+
+        Update an MRB template.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.UpdateMrbTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def update_mrb_template(
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Update an MRB template.
+
+        Update an MRB template.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def update_mrb_template(
+        self, body: Optional[Union[_models.UpdateMrbTemplateRequest, IO]] = None, **kwargs: Any
+    ) -> _models.MrbTemplateDto:
+        """Update an MRB template.
+
+        Update an MRB template.
+
+        :param body: Is either a UpdateMrbTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.UpdateMrbTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: MrbTemplateDto
+        :rtype: ~ignos.api.client.models.MrbTemplateDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MrbTemplateDto] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "UpdateMrbTemplateRequest")
+            else:
+                _json = None
+
+        request = build_mrb_update_mrb_template_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("MrbTemplateDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    def delete_mrb_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        body: Optional[_models.DeleteMrbTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """Delete an MRB template.
+
+        Delete an MRB template.
+
+        :param body: Default value is None.
+        :type body: ~ignos.api.client.models.DeleteMrbTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def delete_mrb_template(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """Delete an MRB template.
+
+        Delete an MRB template.
+
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def delete_mrb_template(  # pylint: disable=inconsistent-return-statements
+        self, body: Optional[Union[_models.DeleteMrbTemplateRequest, IO]] = None, **kwargs: Any
+    ) -> None:
+        """Delete an MRB template.
+
+        Delete an MRB template.
+
+        :param body: Is either a DeleteMrbTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.api.client.models.DeleteMrbTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "DeleteMrbTemplateRequest")
+            else:
+                _json = None
+
+        request = build_mrb_delete_mrb_template_request(
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
 class OperatorCalculatorsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.IgnosPortal`'s
@@ -26795,14 +28469,82 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class TraceOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.api.client.IgnosPortal`'s
+        :attr:`trace` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def get_work_order_trace(self, id: str, **kwargs: Any) -> _models.TraceDto:
+        """get_work_order_trace.
+
+        :param id: Required.
+        :type id: str
+        :return: TraceDto
+        :rtype: ~ignos.api.client.models.TraceDto
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.TraceDto] = kwargs.pop("cls", None)
+
+        request = build_trace_get_work_order_trace_request(
+            id=id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("TraceDto", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+
 class UploadOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.api.client.IgnosPortal`'s
```

### Comparing `ignos-api-client-2023.6.14.5376/ignos/api/client/operations/_patch.py` & `ignos-api-client-2023.7.7.5556/ignos/api/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/ignos_api_client.egg-info/SOURCES.txt` & `ignos-api-client-2023.7.7.5556/ignos_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignos-api-client-2023.6.14.5376/setup.py` & `ignos-api-client-2023.7.7.5556/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 # coding: utf-8
 from setuptools import setup, find_packages
 
 
 PACKAGE_NAME = "ignos-api-client"
-version = "2023.6.14.5376"
+version = "2023.7.7.5556"
 setup(
     name=PACKAGE_NAME,
     version=version,
     description="ignos-api-client",
     author_email="",
     url="",
     keywords="azure, azure sdk",
```


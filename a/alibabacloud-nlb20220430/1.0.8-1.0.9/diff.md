# Comparing `tmp/alibabacloud_nlb20220430-1.0.8.tar.gz` & `tmp/alibabacloud_nlb20220430-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_nlb20220430-1.0.8.tar", last modified: Fri Dec  2 07:41:18 2022, max compression
+gzip compressed data, was "dist/alibabacloud_nlb20220430-1.0.9.tar", last modified: Fri Dec 16 03:46:14 2022, max compression
```

## Comparing `alibabacloud_nlb20220430-1.0.8.tar` & `alibabacloud_nlb20220430-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      354 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430/__init__.py
--rw-r--r--   0 root         (0) root         (0)   163655 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430/client.py
--rw-r--r--   0 root         (0) root         (0)   300787 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2022-12-02 07:41:18.000000 alibabacloud_nlb20220430-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      395 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171113 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430/client.py
+-rw-r--r--   0 root         (0) root         (0)   309114 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-12-16 03:46:14.000000 alibabacloud_nlb20220430-1.0.9/setup.py
```

### Comparing `alibabacloud_nlb20220430-1.0.8/LICENSE` & `alibabacloud_nlb20220430-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlb20220430-1.0.8/PKG-INFO` & `alibabacloud_nlb20220430-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_nlb20220430
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Nlb (20220430) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nlb20220430-1.0.8/README-CN.md` & `alibabacloud_nlb20220430-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlb20220430-1.0.8/README.md` & `alibabacloud_nlb20220430-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430/client.py` & `alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2583,14 +2583,186 @@
     async def list_tag_resources_async(
         self,
         request: nlb_20220430_models.ListTagResourcesRequest,
     ) -> nlb_20220430_models.ListTagResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
+    def load_balancer_join_security_group_with_options(
+        self,
+        request: nlb_20220430_models.LoadBalancerJoinSecurityGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlb_20220430_models.LoadBalancerJoinSecurityGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            body['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.load_balancer_id):
+            body['LoadBalancerId'] = request.load_balancer_id
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.security_group_ids):
+            body['SecurityGroupIds'] = request.security_group_ids
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='LoadBalancerJoinSecurityGroup',
+            version='2022-04-30',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlb_20220430_models.LoadBalancerJoinSecurityGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def load_balancer_join_security_group_with_options_async(
+        self,
+        request: nlb_20220430_models.LoadBalancerJoinSecurityGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlb_20220430_models.LoadBalancerJoinSecurityGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            body['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.load_balancer_id):
+            body['LoadBalancerId'] = request.load_balancer_id
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.security_group_ids):
+            body['SecurityGroupIds'] = request.security_group_ids
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='LoadBalancerJoinSecurityGroup',
+            version='2022-04-30',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlb_20220430_models.LoadBalancerJoinSecurityGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def load_balancer_join_security_group(
+        self,
+        request: nlb_20220430_models.LoadBalancerJoinSecurityGroupRequest,
+    ) -> nlb_20220430_models.LoadBalancerJoinSecurityGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.load_balancer_join_security_group_with_options(request, runtime)
+
+    async def load_balancer_join_security_group_async(
+        self,
+        request: nlb_20220430_models.LoadBalancerJoinSecurityGroupRequest,
+    ) -> nlb_20220430_models.LoadBalancerJoinSecurityGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.load_balancer_join_security_group_with_options_async(request, runtime)
+
+    def load_balancer_leave_security_group_with_options(
+        self,
+        request: nlb_20220430_models.LoadBalancerLeaveSecurityGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlb_20220430_models.LoadBalancerLeaveSecurityGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            body['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.load_balancer_id):
+            body['LoadBalancerId'] = request.load_balancer_id
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.security_group_ids):
+            body['SecurityGroupIds'] = request.security_group_ids
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='LoadBalancerLeaveSecurityGroup',
+            version='2022-04-30',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlb_20220430_models.LoadBalancerLeaveSecurityGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def load_balancer_leave_security_group_with_options_async(
+        self,
+        request: nlb_20220430_models.LoadBalancerLeaveSecurityGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> nlb_20220430_models.LoadBalancerLeaveSecurityGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.client_token):
+            body['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.dry_run):
+            body['DryRun'] = request.dry_run
+        if not UtilClient.is_unset(request.load_balancer_id):
+            body['LoadBalancerId'] = request.load_balancer_id
+        if not UtilClient.is_unset(request.region_id):
+            body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.security_group_ids):
+            body['SecurityGroupIds'] = request.security_group_ids
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='LoadBalancerLeaveSecurityGroup',
+            version='2022-04-30',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            nlb_20220430_models.LoadBalancerLeaveSecurityGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def load_balancer_leave_security_group(
+        self,
+        request: nlb_20220430_models.LoadBalancerLeaveSecurityGroupRequest,
+    ) -> nlb_20220430_models.LoadBalancerLeaveSecurityGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.load_balancer_leave_security_group_with_options(request, runtime)
+
+    async def load_balancer_leave_security_group_async(
+        self,
+        request: nlb_20220430_models.LoadBalancerLeaveSecurityGroupRequest,
+    ) -> nlb_20220430_models.LoadBalancerLeaveSecurityGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.load_balancer_leave_security_group_with_options_async(request, runtime)
+
     def remove_servers_from_server_group_with_options(
         self,
         request: nlb_20220430_models.RemoveServersFromServerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> nlb_20220430_models.RemoveServersFromServerGroupResponse:
         UtilClient.validate_model(request)
         body = {}
```

### Comparing `alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430/models.py` & `alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3493,14 +3493,15 @@
         load_balancer_status: str = None,
         load_balancer_type: str = None,
         modification_protection_config: GetLoadBalancerAttributeResponseBodyModificationProtectionConfig = None,
         operation_locks: List[GetLoadBalancerAttributeResponseBodyOperationLocks] = None,
         region_id: str = None,
         request_id: str = None,
         resource_group_id: str = None,
+        security_group_ids: List[str] = None,
         vpc_id: str = None,
         zone_mappings: List[GetLoadBalancerAttributeResponseBodyZoneMappings] = None,
     ):
         self.address_ip_version = address_ip_version
         self.address_type = address_type
         self.bandwidth_package_id = bandwidth_package_id
         self.cps = cps
@@ -3516,14 +3517,15 @@
         self.load_balancer_status = load_balancer_status
         self.load_balancer_type = load_balancer_type
         self.modification_protection_config = modification_protection_config
         self.operation_locks = operation_locks
         self.region_id = region_id
         self.request_id = request_id
         self.resource_group_id = resource_group_id
+        self.security_group_ids = security_group_ids
         self.vpc_id = vpc_id
         self.zone_mappings = zone_mappings
 
     def validate(self):
         if self.deletion_protection_config:
             self.deletion_protection_config.validate()
         if self.load_balancer_billing_config:
@@ -3583,14 +3585,16 @@
                 result['OperationLocks'].append(k.to_map() if k else None)
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
+        if self.security_group_ids is not None:
+            result['SecurityGroupIds'] = self.security_group_ids
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         result['ZoneMappings'] = []
         if self.zone_mappings is not None:
             for k in self.zone_mappings:
                 result['ZoneMappings'].append(k.to_map() if k else None)
         return result
@@ -3639,14 +3643,16 @@
                 self.operation_locks.append(temp_model.from_map(k))
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('SecurityGroupIds') is not None:
+            self.security_group_ids = m.get('SecurityGroupIds')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         self.zone_mappings = []
         if m.get('ZoneMappings') is not None:
             for k in m.get('ZoneMappings'):
                 temp_model = GetLoadBalancerAttributeResponseBodyZoneMappings()
                 self.zone_mappings.append(temp_model.from_map(k))
@@ -6442,14 +6448,270 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListTagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class LoadBalancerJoinSecurityGroupRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        dry_run: bool = None,
+        load_balancer_id: str = None,
+        region_id: str = None,
+        security_group_ids: List[str] = None,
+    ):
+        self.client_token = client_token
+        self.dry_run = dry_run
+        self.load_balancer_id = load_balancer_id
+        self.region_id = region_id
+        self.security_group_ids = security_group_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.dry_run is not None:
+            result['DryRun'] = self.dry_run
+        if self.load_balancer_id is not None:
+            result['LoadBalancerId'] = self.load_balancer_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.security_group_ids is not None:
+            result['SecurityGroupIds'] = self.security_group_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DryRun') is not None:
+            self.dry_run = m.get('DryRun')
+        if m.get('LoadBalancerId') is not None:
+            self.load_balancer_id = m.get('LoadBalancerId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SecurityGroupIds') is not None:
+            self.security_group_ids = m.get('SecurityGroupIds')
+        return self
+
+
+class LoadBalancerJoinSecurityGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        job_id: str = None,
+        request_id: str = None,
+    ):
+        self.job_id = job_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class LoadBalancerJoinSecurityGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: LoadBalancerJoinSecurityGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = LoadBalancerJoinSecurityGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class LoadBalancerLeaveSecurityGroupRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        dry_run: bool = None,
+        load_balancer_id: str = None,
+        region_id: str = None,
+        security_group_ids: List[str] = None,
+    ):
+        self.client_token = client_token
+        self.dry_run = dry_run
+        self.load_balancer_id = load_balancer_id
+        self.region_id = region_id
+        self.security_group_ids = security_group_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.dry_run is not None:
+            result['DryRun'] = self.dry_run
+        if self.load_balancer_id is not None:
+            result['LoadBalancerId'] = self.load_balancer_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.security_group_ids is not None:
+            result['SecurityGroupIds'] = self.security_group_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DryRun') is not None:
+            self.dry_run = m.get('DryRun')
+        if m.get('LoadBalancerId') is not None:
+            self.load_balancer_id = m.get('LoadBalancerId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SecurityGroupIds') is not None:
+            self.security_group_ids = m.get('SecurityGroupIds')
+        return self
+
+
+class LoadBalancerLeaveSecurityGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        job_id: str = None,
+        request_id: str = None,
+    ):
+        self.job_id = job_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.job_id is not None:
+            result['JobId'] = self.job_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('JobId') is not None:
+            self.job_id = m.get('JobId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class LoadBalancerLeaveSecurityGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: LoadBalancerLeaveSecurityGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = LoadBalancerLeaveSecurityGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RemoveServersFromServerGroupRequestServers(TeaModel):
     def __init__(
         self,
         port: int = None,
         server_id: str = None,
         server_ip: str = None,
         server_type: str = None,
```

### Comparing `alibabacloud_nlb20220430-1.0.8/alibabacloud_nlb20220430.egg-info/PKG-INFO` & `alibabacloud_nlb20220430-1.0.9/alibabacloud_nlb20220430.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-nlb20220430
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Nlb (20220430) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_nlb20220430-1.0.8/setup.py` & `alibabacloud_nlb20220430-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_nlb20220430.
 
-Created on 02/12/2022
+Created on 16/12/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_nlb20220430"
 NAME = "alibabacloud_nlb20220430" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Nlb (20220430) SDK Library for Python"
```


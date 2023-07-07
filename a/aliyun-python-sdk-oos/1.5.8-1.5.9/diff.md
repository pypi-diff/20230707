# Comparing `tmp/aliyun-python-sdk-oos-1.5.8.tar.gz` & `tmp/aliyun-python-sdk-oos-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-oos-1.5.8.tar", last modified: Wed Oct 12 15:29:51 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-oos-1.5.9.tar", last modified: Mon Nov  7 08:02:23 2022, max compression
```

## Comparing `aliyun-python-sdk-oos-1.5.8.tar` & `aliyun-python-sdk-oos-1.5.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/
--rw-r--r--   0 root         (0) root         (0)      575 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5072 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/
--rw-r--r--   0 root         (0) root         (0)     1469 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CancelExecutionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1913 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ContinueDeployApplicationGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2880 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateApplicationGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2201 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3472 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateOpsItemRequest.py
--rw-r--r--   0 root         (0) root         (0)     2710 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreatePatchBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2901 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateSecretParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3499 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateStateConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2215 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteApplicationGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1594 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1477 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteExecutionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1427 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1435 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeletePatchBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1439 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteSecretParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1746 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteStateConfigurationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1726 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1734 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeployApplicationGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1712 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GenerateExecutionPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetApplicationGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1425 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetExecutionTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetInventorySchemaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1447 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetOpsItemRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2000 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetParametersByPathRequest.py
--rw-r--r--   0 root         (0) root         (0)     1429 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1429 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetPatchBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1879 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetSecretParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2229 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetSecretParametersByPathRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetSecretParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1278 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetServiceSettingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1688 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListActionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2665 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListApplicationGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2123 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListApplicationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2245 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListExecutionLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListExecutionRiskyTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     5437 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListExecutionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1863 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListInstancePatchStatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2058 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListInstancePatchesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2725 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListInventoryEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2697 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListOpsItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListParameterVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3046 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2217 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListPatchBaselinesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListResourceExecutionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2231 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListSecretParameterVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2903 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListSecretParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2723 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListStateConfigurationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1845 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2006 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1998 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4369 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTaskExecutionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2048 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTemplateVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4211 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3069 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/NotifyExecutionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/RegisterDefaultPatchBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2615 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/SearchInventoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2752 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/SetServiceSettingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3636 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/StartExecutionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1996 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/TriggerExecutionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1986 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateApplicationGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1801 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateExecutionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3824 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateOpsItemRequest.py
--rw-r--r--   0 root         (0) root         (0)     2161 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2038 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdatePatchBaselineRequest.py
--rw-r--r--   0 root         (0) root         (0)     2173 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateSecretParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3326 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateStateConfigurationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2215 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ValidateTemplateContentRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-10-12 15:29:51.000000 aliyun-python-sdk-oos-1.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2022-10-12 15:29:50.000000 aliyun-python-sdk-oos-1.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5072 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/
+-rw-r--r--   0 root         (0) root         (0)     1469 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CancelExecutionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ContinueDeployApplicationGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateApplicationGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3472 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateOpsItemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreatePatchBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateSecretParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3499 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateStateConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteApplicationGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteExecutionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeletePatchBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteSecretParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteStateConfigurationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeployApplicationGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GenerateExecutionPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetApplicationGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetExecutionTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetInventorySchemaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetOpsItemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetParametersByPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1429 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetPatchBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetSecretParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetSecretParametersByPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetSecretParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetServiceSettingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListActionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListApplicationGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListExecutionLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListExecutionRiskyTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5437 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListExecutionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListInstancePatchStatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListInstancePatchesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListInventoryEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListOpsItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListParameterVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListPatchBaselinesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListResourceExecutionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2231 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListSecretParameterVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListSecretParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListStateConfigurationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTaskExecutionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTemplateVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/NotifyExecutionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/RegisterDefaultPatchBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/SearchInventoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/SetServiceSettingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3833 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/StartExecutionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/TriggerExecutionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateApplicationGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateExecutionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3824 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateOpsItemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdatePatchBaselineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateSecretParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3326 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateStateConfigurationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ValidateTemplateContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-11-07 08:02:23.000000 aliyun-python-sdk-oos-1.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2022-11-07 08:02:22.000000 aliyun-python-sdk-oos-1.5.9/setup.py
```

### Comparing `aliyun-python-sdk-oos-1.5.8/LICENSE` & `aliyun-python-sdk-oos-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/PKG-INFO` & `aliyun-python-sdk-oos-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-oos
-Version: 1.5.8
+Version: 1.5.9
 Summary: The oos module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-oos
```

### Comparing `aliyun-python-sdk-oos-1.5.8/README.rst` & `aliyun-python-sdk-oos-1.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/PKG-INFO` & `aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-oos
-Version: 1.5.8
+Version: 1.5.9
 Summary: The oos module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-oos
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyun_python_sdk_oos.egg-info/SOURCES.txt` & `aliyun-python-sdk-oos-1.5.9/aliyun_python_sdk_oos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/endpoint.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CancelExecutionRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CancelExecutionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ChangeResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ContinueDeployApplicationGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ContinueDeployApplicationGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateApplicationGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateApplicationGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateApplicationRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateOpsItemRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateOpsItemRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreatePatchBaselineRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreatePatchBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateSecretParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateSecretParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateStateConfigurationRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateStateConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/CreateTemplateRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/CreateTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteApplicationGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteApplicationGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteApplicationRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteExecutionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteExecutionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeletePatchBaselineRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeletePatchBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteSecretParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteSecretParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteStateConfigurationsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteStateConfigurationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteTemplateRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeleteTemplatesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeleteTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DeployApplicationGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DeployApplicationGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/DescribeRegionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GenerateExecutionPolicyRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GenerateExecutionPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetApplicationGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetApplicationGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetApplicationRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetExecutionTemplateRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetExecutionTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetInventorySchemaRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetInventorySchemaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetOpsItemRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetOpsItemRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetParametersByPathRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetParametersByPathRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetParametersRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetPatchBaselineRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetPatchBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetSecretParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetSecretParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetSecretParametersByPathRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetSecretParametersByPathRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetSecretParametersRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetSecretParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetServiceSettingsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetServiceSettingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/GetTemplateRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/GetTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListActionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListActionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListApplicationGroupsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListApplicationsRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,53 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoos.endpoint import endpoint_data
 
-class ListApplicationGroupsRequest(RpcRequest):
+class ListApplicationsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListApplicationGroups','oos')
+		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListApplications','oos')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
-	def get_ResourceId(self): # String
-		return self.get_query_params().get('ResourceId')
+	def get_Tags(self): # String
+		return self.get_query_params().get('Tags')
 
-	def set_ResourceId(self, ResourceId):  # String
-		self.add_query_param('ResourceId', ResourceId)
-	def get_Product(self): # String
-		return self.get_query_params().get('Product')
-
-	def set_Product(self, Product):  # String
-		self.add_query_param('Product', Product)
-	def get_DeployRegionId(self): # String
-		return self.get_query_params().get('DeployRegionId')
-
-	def set_DeployRegionId(self, DeployRegionId):  # String
-		self.add_query_param('DeployRegionId', DeployRegionId)
-	def get_ResourceType(self): # String
-		return self.get_query_params().get('ResourceType')
-
-	def set_ResourceType(self, ResourceType):  # String
-		self.add_query_param('ResourceType', ResourceType)
-	def get_ApplicationName(self): # String
-		return self.get_query_params().get('ApplicationName')
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_Names(self): # String
+		return self.get_query_params().get('Names')
+
+	def set_Names(self, Names):  # String
+		self.add_query_param('Names', Names)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
 
-	def set_ApplicationName(self, ApplicationName):  # String
-		self.add_query_param('ApplicationName', ApplicationName)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
 	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
 	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListApplicationsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListInstancePatchesRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,43 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoos.endpoint import endpoint_data
 
-class ListApplicationsRequest(RpcRequest):
+class ListInstancePatchesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListApplications','oos')
+		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListInstancePatches','oos')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
+
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
-	def get_Tags(self): # String
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self, Tags):  # String
-		self.add_query_param('Tags', Tags)
-	def get_Names(self): # String
-		return self.get_query_params().get('Names')
-
-	def set_Names(self, Names):  # String
-		self.add_query_param('Names', Names)
-	def get_Name(self): # String
-		return self.get_query_params().get('Name')
-
-	def set_Name(self, Name):  # String
-		self.add_query_param('Name', Name)
 	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
 	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
+	def get_PatchStatuses(self): # String
+		return self.get_query_params().get('PatchStatuses')
+
+	def set_PatchStatuses(self, PatchStatuses):  # String
+		self.add_query_param('PatchStatuses', PatchStatuses)
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListExecutionLogsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListExecutionLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListExecutionRiskyTasksRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListExecutionRiskyTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListExecutionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListExecutionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListInstancePatchStatesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListInstancePatchStatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListInstancePatchesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListResourceExecutionStatusRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,38 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoos.endpoint import endpoint_data
 
-class ListInstancePatchesRequest(RpcRequest):
+class ListResourceExecutionStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListInstancePatches','oos')
+		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListResourceExecutionStatus','oos')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
+	def get_ExecutionId(self): # String
+		return self.get_query_params().get('ExecutionId')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
+	def set_ExecutionId(self, ExecutionId):  # String
+		self.add_query_param('ExecutionId', ExecutionId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
 	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
 	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
-	def get_PatchStatuses(self): # String
-		return self.get_query_params().get('PatchStatuses')
-
-	def set_PatchStatuses(self, PatchStatuses):  # String
-		self.add_query_param('PatchStatuses', PatchStatuses)
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListInventoryEntriesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListInventoryEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListOpsItemsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListOpsItemsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListParameterVersionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListParameterVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListParametersRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListPatchBaselinesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListPatchBaselinesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListResourceExecutionStatusRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/RegisterDefaultPatchBaselineRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,33 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoos.endpoint import endpoint_data
 
-class ListResourceExecutionStatusRequest(RpcRequest):
+class RegisterDefaultPatchBaselineRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ListResourceExecutionStatus','oos')
+		RpcRequest.__init__(self, 'oos', '2019-06-01', 'RegisterDefaultPatchBaseline','oos')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ExecutionId(self): # String
-		return self.get_query_params().get('ExecutionId')
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
 
-	def set_ExecutionId(self, ExecutionId):  # String
-		self.add_query_param('ExecutionId', ExecutionId)
-	def get_NextToken(self): # String
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self, NextToken):  # String
-		self.add_query_param('NextToken', NextToken)
-	def get_MaxResults(self): # Integer
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_query_param('MaxResults', MaxResults)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListSecretParameterVersionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListSecretParameterVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListSecretParametersRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListSecretParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListStateConfigurationsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListStateConfigurationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTagKeysRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTagResourcesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTagValuesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTagValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTaskExecutionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTaskExecutionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTemplateVersionsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTemplateVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/ListTemplatesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ListTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/NotifyExecutionRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/NotifyExecutionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/RegisterDefaultPatchBaselineRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/ValidateTemplateContentRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkoos.endpoint import endpoint_data
 
-class RegisterDefaultPatchBaselineRequest(RpcRequest):
+class ValidateTemplateContentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'oos', '2019-06-01', 'RegisterDefaultPatchBaseline','oos')
+		RpcRequest.__init__(self, 'oos', '2019-06-01', 'ValidateTemplateContent','oos')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Name(self): # String
-		return self.get_query_params().get('Name')
+	def get_Content(self): # String
+		return self.get_query_params().get('Content')
 
-	def set_Name(self, Name):  # String
-		self.add_query_param('Name', Name)
+	def set_Content(self, Content):  # String
+		self.add_query_param('Content', Content)
+	def get_TemplateURL(self): # String
+		return self.get_query_params().get('TemplateURL')
+
+	def set_TemplateURL(self, TemplateURL):  # String
+		self.add_query_param('TemplateURL', TemplateURL)
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/SearchInventoryRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/SearchInventoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/SetServiceSettingsRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/SetServiceSettingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/StartExecutionRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/StartExecutionRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
 	def set_Description(self, Description):  # String
 		self.add_query_param('Description', Description)
+	def get_TemplateURL(self): # String
+		return self.get_query_params().get('TemplateURL')
+
+	def set_TemplateURL(self, TemplateURL):  # String
+		self.add_query_param('TemplateURL', TemplateURL)
 	def get_Mode(self): # String
 		return self.get_query_params().get('Mode')
 
 	def set_Mode(self, Mode):  # String
 		self.add_query_param('Mode', Mode)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
```

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/TagResourcesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/TriggerExecutionRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/TriggerExecutionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UntagResourcesRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateApplicationGroupRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateApplicationGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateApplicationRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateExecutionRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateExecutionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateOpsItemRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateOpsItemRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdatePatchBaselineRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdatePatchBaselineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateSecretParameterRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateSecretParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateStateConfigurationRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateStateConfigurationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/aliyunsdkoos/request/v20190601/UpdateTemplateRequest.py` & `aliyun-python-sdk-oos-1.5.9/aliyunsdkoos/request/v20190601/UpdateTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oos-1.5.8/setup.py` & `aliyun-python-sdk-oos-1.5.9/setup.py`

 * *Files identical despite different names*


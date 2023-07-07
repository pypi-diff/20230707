# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.929.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.929.tar", last modified: Thu Jul  6 00:26:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.930.tar", last modified: Fri Jul  7 00:23:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.929.tar` & `tencentcloud-sdk-python-essbasic-3.0.930.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/essbasic_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   375146 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52742 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:26:24.000000 tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/essbasic_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   375355 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52742 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:23:58.000000 tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.930/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.930/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.930/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,15 @@
 class ChannelBatchCancelFlowsRequest(AbstractModel):
     """ChannelBatchCancelFlows请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 签署流程Id数组，最多100个，超过100不处理
         :type FlowIds: list of str
         :param _CancelMessage: 撤销理由,不超过200个字符
         :type CancelMessage: str
         :param _CancelMessageFormat: 撤销理由自定义格式；选项：
 0 默认格式
@@ -655,15 +655,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FlowId: 签署流程编号
         :type FlowId: str
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _CancelMessage: 撤回原因，最大不超过200字符
         :type CancelMessage: str
         :param _CancelMessageFormat: 撤销理由自定义格式；选项：
 0 默认格式
 1 只保留身份信息：展示为【发起方】
 2 保留身份信息+企业名称：展示为【发起方xxx公司】
@@ -771,15 +771,15 @@
 class ChannelCancelMultiFlowSignQRCodeRequest(AbstractModel):
     """ChannelCancelMultiFlowSignQRCode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _QrCodeId: 二维码id
         :type QrCodeId: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -861,15 +861,15 @@
 class ChannelCreateBatchCancelFlowUrlRequest(AbstractModel):
     """ChannelCreateBatchCancelFlowUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 签署流程Id数组
         :type FlowIds: list of str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -1078,15 +1078,15 @@
 class ChannelCreateConvertTaskApiRequest(AbstractModel):
     """ChannelCreateConvertTaskApi请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _ResourceType: 资源类型 支持doc,docx,html,xls,xlsx,jpg,jpeg,png,bmp文件类型
         :type ResourceType: str
         :param _ResourceName: 资源名称，长度限制为256字符
         :type ResourceName: str
         :param _ResourceId: 资源Id，通过UploadFiles获取
         :type ResourceId: str
@@ -1222,15 +1222,15 @@
 class ChannelCreateEmbedWebUrlRequest(AbstractModel):
     """ChannelCreateEmbedWebUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 渠道应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 必填。
+        :param _Agent: 渠道应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _EmbedType: WEB嵌入资源类型。
 CREATE_SEAL: 创建印章
 CREATE_TEMPLATE：创建模版
 MODIFY_TEMPLATE：修改模版
 PREVIEW_TEMPLATE：预览模版
 PREVIEW_FLOW：预览合同文档
@@ -1360,15 +1360,15 @@
 class ChannelCreateFlowByFilesRequest(AbstractModel):
     """ChannelCreateFlowByFiles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 均必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowName: 签署流程名称，长度不超过200个字符
         :type FlowName: str
         :param _FlowApprovers: 签署流程签约方列表，最多不超过50个参与方
         :type FlowApprovers: list of FlowApproverInfo
         :param _FileIds: 签署文件资源Id列表，目前仅支持单个文件
         :type FileIds: list of str
@@ -1677,15 +1677,15 @@
 
     def __init__(self):
         r"""
         :param _FlowFileInfos: 每个子合同的发起所需的信息，数量限制2-100
         :type FlowFileInfos: list of FlowFileInfo
         :param _FlowGroupName: 合同组名称，长度不超过200个字符
         :type FlowGroupName: str
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _ApproverVerifyType: 签署人校验方式
 VerifyCheck: 人脸识别（默认）
 MobileCheck：手机号验证
 参数说明：若选择后者，未实名的个人签署方查看合同时，无需进行人脸识别实名认证（但签署合同时仍然需要人脸实名），该能力仅适用于个人签署方。
         :type ApproverVerifyType: str
         :param _Operator: 操作者的信息，此参数不用传
@@ -1821,15 +1821,15 @@
 class ChannelCreateFlowRemindsRequest(AbstractModel):
     """ChannelCreateFlowReminds请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 签署流程Id数组，最多100个，超过100不处理
         :type FlowIds: list of str
         """
         self._Agent = None
         self._FlowIds = None
 
@@ -1910,15 +1910,15 @@
 class ChannelCreateFlowSignReviewRequest(AbstractModel):
     """ChannelCreateFlowSignReview请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowId: 签署流程编号
         :type FlowId: str
         :param _ReviewType: 企业内部审核结果
 PASS: 通过
 REJECT: 拒绝
 SIGN_REJECT:拒签(流程结束)
@@ -2038,15 +2038,15 @@
 class ChannelCreateFlowSignUrlRequest(AbstractModel):
     """ChannelCreateFlowSignUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowId: 流程编号
         :type FlowId: str
         :param _FlowApproverInfos: 流程签署人，其中Name和Mobile必传，其他可不传，ApproverType目前只支持PERSON类型的签署人，如果不传默认为该值。还需注意签署人只能有手写签名和时间类型的签署控件，其他类型的填写控件和签署控件暂时都未支持。
         :type FlowApproverInfos: list of FlowApproverInfo
         :param _Operator: 用户信息，暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
@@ -2181,15 +2181,15 @@
     """ChannelCreateMultiFlowSignQRCode请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Agent: 应用相关信息。
-此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 必填。
+此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _TemplateId: 模版ID
         :type TemplateId: str
         :param _FlowName: 签署流程名称，最大长度200个字符。
         :type FlowName: str
         :param _MaxFlowNum: 最大可发起签署流程份数，默认5份；发起签署流程数量超过此上限后，二维码自动失效。
         :type MaxFlowNum: int
@@ -2609,15 +2609,15 @@
 class ChannelCreateReleaseFlowRequest(AbstractModel):
     """ChannelCreateReleaseFlow请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _NeedRelievedFlowId: 待解除的流程编号（即原流程的编号）
         :type NeedRelievedFlowId: str
         :param _ReliveInfo: 解除协议内容
         :type ReliveInfo: :class:`tencentcloud.essbasic.v20210526.models.RelieveInfo`
         :param _ReleasedApprovers: 非必须，解除协议的本企业签署人列表，默认使用原流程的签署人列表；当解除协议的签署人与原流程的签署人不能相同时（例如原流程签署人离职了），需要指定本企业的其他签署人来替换原流程中的原签署人，注意需要指明ApproverNumber来代表需要替换哪一个签署人，解除协议的签署人数量不能多于原流程的签署人数量
         :type ReleasedApprovers: list of ReleasedApprover
@@ -2784,15 +2784,15 @@
 class ChannelCreateSealPolicyRequest(AbstractModel):
     """ChannelCreateSealPolicy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _SealId: 指定印章ID
         :type SealId: str
         :param _UserIds: 指定待授权的用户ID数组,电子签的用户ID
 可以填写OpenId，系统会通过组织+渠道+OpenId查询得到UserId进行授权。
         :type UserIds: list of str
         :param _Operator: 操作人（用户）信息，不用传
@@ -2918,15 +2918,15 @@
 class ChannelCreateUserRolesRequest(AbstractModel):
     """ChannelCreateUserRoles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _RoleIds: 绑定角色的角色id列表
         :type RoleIds: list of str
         :param _UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数
         :type UserIds: list of str
         :param _OpenIds: 客户系统用户ID列表，与UserIds参数二选一,优先UserIds参数
         :type OpenIds: list of str
@@ -3049,15 +3049,15 @@
 class ChannelDeleteRoleUsersRequest(AbstractModel):
     """ChannelDeleteRoleUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 代理信息
+        :param _Agent: 代理信息此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _RoleId: 角色Id（非超管或法人角色Id）
         :type RoleId: str
         :param _UserIds: 电子签用户ID列表，与OpenIds参数二选一,优先UserIds参数
         :type UserIds: list of str
         :param _Operator: 操作人信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
@@ -3175,15 +3175,15 @@
 class ChannelDeleteSealPoliciesRequest(AbstractModel):
     """ChannelDeleteSealPolicies请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _SealId: 指定印章ID
         :type SealId: str
         :param _UserIds: 指定用户ID数组，电子签系统用户ID
 可以填写OpenId，系统会通过组织+渠道+OpenId查询得到UserId进行授权取消。
         :type UserIds: list of str
         :param _Organization: 组织机构信息，不用传
@@ -3298,15 +3298,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Limit: 返回最大数量，最大为20
         :type Limit: int
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _Filters: 查询过滤实名用户，Key为Status，Values为["IsVerified"]
 根据第三方系统openId过滤查询员工时,Key为StaffOpenId,Values为["OpenId","OpenId",...]
 查询离职员工时，Key为Status，Values为["QuiteJob"]
         :type Filters: list of Filter
         :param _Offset: 偏移量，默认为0，最大为20000
         :type Offset: int
@@ -3472,15 +3472,15 @@
 class ChannelDescribeFlowComponentsRequest(AbstractModel):
     """ChannelDescribeFlowComponents请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息
+        :param _Agent: 应用相关信息。此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowId: 电子签流程的Id
         :type FlowId: str
         """
         self._Agent = None
         self._FlowId = None
 
@@ -3562,15 +3562,15 @@
 class ChannelDescribeOrganizationSealsRequest(AbstractModel):
     """ChannelDescribeOrganizationSeals请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _Limit: 返回最大数量，最大为100
         :type Limit: int
         :param _Offset: 偏移量，默认为0，最大为20000
         :type Offset: int
         :param _InfoType: 查询信息类型，为1时返回授权用户，为其他值时不返回
         :type InfoType: int
@@ -3717,15 +3717,15 @@
 class ChannelDescribeRolesRequest(AbstractModel):
     """ChannelDescribeRoles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _Offset: 查询起始偏移，最大2000
         :type Offset: int
         :param _Limit: 查询数量，最大200
         :type Limit: str
         :param _Filters: 查询的关键字段:
 Key:"RoleType",Values:["1"]查询系统角色，Values:["2"]查询自定义角色
@@ -3892,15 +3892,15 @@
 class ChannelGetTaskResultApiRequest(AbstractModel):
     """ChannelGetTaskResultApi请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 均必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _TaskId: 任务Id，通过ChannelCreateConvertTaskApi接口获得
         :type TaskId: str
         :param _Operator: 操作者的信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         :param _Organization: 暂未开放
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
@@ -4138,15 +4138,15 @@
 class ChannelUpdateSealStatusRequest(AbstractModel):
     """ChannelUpdateSealStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _Status: 操作的印章状态，DISABLE-停用印章
         :type Status: str
         :param _SealId: 印章ID
         :type SealId: str
         :param _Reason: 更新印章状态原因说明
         :type Reason: str
@@ -4254,15 +4254,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FlowId: 流程ID
         :type FlowId: str
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._FlowId = None
         self._Agent = None
         self._Operator = None
@@ -5079,15 +5079,15 @@
 class CreateChannelFlowEvidenceReportRequest(AbstractModel):
     """CreateChannelFlowEvidenceReport请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowId: 签署流程编号
         :type FlowId: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -5470,15 +5470,15 @@
 class CreateFlowsByTemplatesRequest(AbstractModel):
     """CreateFlowsByTemplates请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 均必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowInfos: 多个合同（签署流程）信息，最多支持20个
         :type FlowInfos: list of FlowInfo
         :param _NeedPreview: 是否为预览模式；默认为false，即非预览模式，此时发起合同并返回FlowIds；若为预览模式，不会发起合同，会返回PreviewUrls；
 预览链接有效期300秒；
 同时，如果预览的文件中指定了动态表格控件，需要进行异步合成；此时此接口返回的是合成前的文档预览链接，而合成完成后的文档预览链接会通过：回调通知的方式、或使用返回的TaskInfo中的TaskId通过ChannelGetTaskResultApi接口查询；
         :type NeedPreview: bool
@@ -5658,15 +5658,15 @@
 class CreateSealByImageRequest(AbstractModel):
     """CreateSealByImage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _SealName: 印章名称，最大长度不超过50字符
         :type SealName: str
         :param _SealImage: 印章图片base64，大小不超过10M（原始图片不超过7.6M）
         :type SealImage: str
         :param _Operator: 操作者的信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
@@ -5772,15 +5772,15 @@
 class CreateSignUrlsRequest(AbstractModel):
     """CreateSignUrls请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 签署流程编号数组，最多支持100个。(备注：该参数和合同组编号必须二选一)
         :type FlowIds: list of str
         :param _FlowGroupId: 合同组编号(备注：该参数和合同(流程)编号数组必须二选一)
         :type FlowGroupId: str
         :param _Endpoint: 签署链接类型：“WEIXINAPP”-短链直接跳小程序；“CHANNEL”-跳转H5页面；“APP”-第三方APP或小程序跳转电子签小程序；"LONGURL2WEIXINAPP"-长链接跳转小程序；默认“WEIXINAPP”类型，即跳转至小程序；
         :type Endpoint: str
@@ -6064,15 +6064,15 @@
 class DescribeChannelFlowEvidenceReportRequest(AbstractModel):
     """DescribeChannelFlowEvidenceReport请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _ReportId: 出证报告编号
         :type ReportId: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -6181,15 +6181,15 @@
 class DescribeExtendedServiceAuthInfoRequest(AbstractModel):
     """DescribeExtendedServiceAuthInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填
 
 注: 此接口 参数Agent. ProxyOperator.OpenId 需要传递超管或者法人的OpenId
 
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         """
         self._Agent = None
 
@@ -6262,15 +6262,15 @@
 class DescribeFlowDetailInfoRequest(AbstractModel):
     """DescribeFlowDetailInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 合同(流程)编号数组，最多支持100个。
 （备注：该参数和合同组编号必须二选一）
         :type FlowIds: list of str
         :param _FlowGroupId: 合同组编号（备注：该参数和合同(流程)编号数组必须二选一）
         :type FlowGroupId: str
         :param _Operator: 暂未开放
@@ -6434,15 +6434,15 @@
     """DescribeResourceUrlsByFlows请求参数结构体
 
     """
 
     def __init__(self):
         r"""
         :param _Agent: 应用相关信息。
-此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowIds: 查询资源所对应的签署流程Id，最多支持50个
         :type FlowIds: list of str
         :param _Operator: 操作者的信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -6554,15 +6554,15 @@
 class DescribeTemplatesRequest(AbstractModel):
     """DescribeTemplates请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _TemplateId: 模板唯一标识，查询单个模板时使用
         :type TemplateId: str
         :param _ContentType: 查询内容：0-模板列表及详情（默认），1-仅模板列表
         :type ContentType: int
         :param _Limit: 查询个数，默认20，最大100；在查询列表的时候有效
         :type Limit: int
@@ -8607,15 +8607,15 @@
 class GetDownloadFlowUrlRequest(AbstractModel):
     """GetDownloadFlowUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _DownLoadFlows: 文件夹数组，签署流程总数不能超过50个，一个文件夹下，不能超过20个签署流程
         :type DownLoadFlows: list of DownloadFlowInfo
         :param _Operator: 操作者的信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self._Agent = None
@@ -8714,15 +8714,15 @@
 class ModifyExtendedServiceRequest(AbstractModel):
     """ModifyExtendedService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
 
 注: 此接口 参数Agent. ProxyOperator.OpenId 需要传递超管或者法人的OpenId
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _ServiceType:   扩展服务类型
   AUTO_SIGN             企业静默签（自动签署）
   OVERSEA_SIGN          企业与港澳台居民*签署合同
   MOBILE_CHECK_APPROVER 使用手机号验证签署方身份
@@ -8994,21 +8994,25 @@
         :type TemplateId: str
         :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据，支持多个， 用","进行分隔
         :type ProxyOrganizationOpenIds: str
         :param _AuthTag: 模板可见性, 全部可见-"all", 部分可见-"part"
         :type AuthTag: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
+        :param _Available: 当OperateType=UPADATE时，可以通过设置此字段对模板启停用状态进行操作。若此字段值为0，则不会修改模板Available，1为启用模板，2为停用模板。
+启用后模板可以正常领取。停用后，推送方式为【自动推送】的模板则无法被子客使用，推送方式为【手动领取】的模板则无法出现被模板库被子客领用。如果Available更新失败，会直接返回错误。
+        :type Available: int
         """
         self._Agent = None
         self._OperateType = None
         self._TemplateId = None
         self._ProxyOrganizationOpenIds = None
         self._AuthTag = None
         self._Operator = None
+        self._Available = None
 
     @property
     def Agent(self):
         return self._Agent
 
     @Agent.setter
     def Agent(self, Agent):
@@ -9054,26 +9058,35 @@
 
     @Operator.setter
     def Operator(self, Operator):
         warnings.warn("parameter `Operator` is deprecated", DeprecationWarning) 
 
         self._Operator = Operator
 
+    @property
+    def Available(self):
+        return self._Available
+
+    @Available.setter
+    def Available(self, Available):
+        self._Available = Available
+
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self._Agent = Agent()
             self._Agent._deserialize(params.get("Agent"))
         self._OperateType = params.get("OperateType")
         self._TemplateId = params.get("TemplateId")
         self._ProxyOrganizationOpenIds = params.get("ProxyOrganizationOpenIds")
         self._AuthTag = params.get("AuthTag")
         if params.get("Operator") is not None:
             self._Operator = UserInfo()
             self._Operator._deserialize(params.get("Operator"))
+        self._Available = params.get("Available")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -9089,15 +9102,15 @@
         r"""
         :param _AppId: 腾讯电子签颁发给第三方应用平台的应用ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type AppId: str
         :param _TemplateId: 第三方应用平台模板库模板唯一标识
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateId: str
-        :param _OperateResult: 全部成功-"all-success",部分成功-"part-success", 全部失败-"fail"失败的会在FailMessageList中展示
+        :param _OperateResult: 描述模版可见性更改的结果，和参数中Available无关，全部成功-"all-success",部分成功-"part-success", 全部失败-"fail"失败的会在FailMessageList中展示。
 注意：此字段可能返回 null，表示取不到有效值。
         :type OperateResult: str
         :param _AuthTag: 模板可见性, 全部可见-"all", 部分可见-"part"
 注意：此字段可能返回 null，表示取不到有效值。
         :type AuthTag: str
         :param _ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据
 注意：此字段可能返回 null，表示取不到有效值。
@@ -9469,15 +9482,15 @@
 class PrepareFlowsRequest(AbstractModel):
     """PrepareFlows请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param _Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param _FlowInfos: 多个合同（签署流程）信息，最大支持20个签署流程。
         :type FlowInfos: list of FlowInfo
         :param _JumpUrl: 操作完成后的跳转地址，最大长度200
         :type JumpUrl: str
         :param _Operator: 暂未开放
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.929/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.930/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.929'
+__version__ = '3.0.930'
```


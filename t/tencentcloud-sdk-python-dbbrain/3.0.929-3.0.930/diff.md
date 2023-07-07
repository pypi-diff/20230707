# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.929.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.929.tar", last modified: Thu Jul  6 00:24:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.930.tar", last modified: Fri Jul  7 00:22:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.929.tar` & `tencentcloud-sdk-python-dbbrain-3.0.930.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/setup.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   299639 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)    48612 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   183920 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)    27659 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:24:30.000000 tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   302818 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)    49641 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   183920 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:22:08.000000 tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/__init__.py
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.930/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.930/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1224,14 +1224,121 @@
 
 
     def _deserialize(self, params):
         self._AsyncRequestId = params.get("AsyncRequestId")
         self._RequestId = params.get("RequestId")
 
 
+class CreateRedisBigKeyAnalysisTaskRequest(AbstractModel):
+    """CreateRedisBigKeyAnalysisTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _Product: 服务产品类型，支持值包括 "redis" - 云数据库 Redis。
+        :type Product: str
+        :param _ShardIds: 分片节点序号列表。当列表为空时，选择所有分片节点。
+        :type ShardIds: list of int
+        :param _KeyDelimiterList: Top Key前缀的分隔符列表。
+目前仅支持以下分割符：[",", ";", ":", "_", "-", "+", "@", "=", "|", "#", "."]，当列表为空时，默认选择所有分隔符。
+        :type KeyDelimiterList: list of str
+        """
+        self._InstanceId = None
+        self._Product = None
+        self._ShardIds = None
+        self._KeyDelimiterList = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def Product(self):
+        return self._Product
+
+    @Product.setter
+    def Product(self, Product):
+        self._Product = Product
+
+    @property
+    def ShardIds(self):
+        return self._ShardIds
+
+    @ShardIds.setter
+    def ShardIds(self, ShardIds):
+        self._ShardIds = ShardIds
+
+    @property
+    def KeyDelimiterList(self):
+        return self._KeyDelimiterList
+
+    @KeyDelimiterList.setter
+    def KeyDelimiterList(self, KeyDelimiterList):
+        self._KeyDelimiterList = KeyDelimiterList
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._Product = params.get("Product")
+        self._ShardIds = params.get("ShardIds")
+        self._KeyDelimiterList = params.get("KeyDelimiterList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateRedisBigKeyAnalysisTaskResponse(AbstractModel):
+    """CreateRedisBigKeyAnalysisTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AsyncRequestId: 异步任务ID。
+        :type AsyncRequestId: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._AsyncRequestId = None
+        self._RequestId = None
+
+    @property
+    def AsyncRequestId(self):
+        return self._AsyncRequestId
+
+    @AsyncRequestId.setter
+    def AsyncRequestId(self, AsyncRequestId):
+        self._AsyncRequestId = AsyncRequestId
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._AsyncRequestId = params.get("AsyncRequestId")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateSchedulerMailProfileRequest(AbstractModel):
     """CreateSchedulerMailProfile请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateRedisBigKeyAnalysisTask(self, request):
+        """即时创建redis实例大key分析任务，限制正在运行的即时分析任务数量默认为5。
+
+        :param request: Request instance for CreateRedisBigKeyAnalysisTask.
+        :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateRedisBigKeyAnalysisTaskRequest`
+        :rtype: :class:`tencentcloud.dbbrain.v20210527.models.CreateRedisBigKeyAnalysisTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateRedisBigKeyAnalysisTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateRedisBigKeyAnalysisTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateSchedulerMailProfile(self, request):
         """该接口用于创建定期生成健康报告并邮件发送的配置，将健康报告的定期生成时间作为参数传入（周一至周日），用于设置健康报告的定期生成时间，同时保存相应的定期邮件发送的配置。
 
         :param request: Request instance for CreateSchedulerMailProfile.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.CreateSchedulerMailProfileRequest`
         :rtype: :class:`tencentcloud.dbbrain.v20210527.models.CreateSchedulerMailProfileResponse`
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.929/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.930/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*


# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.929.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.929.tar", last modified: Thu Jul  6 00:36:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.930.tar", last modified: Fri Jul  7 00:34:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.929.tar` & `tencentcloud-sdk-python-tke-3.0.930.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)    19591 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1058062 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190375 2023-07-06 00:36:52.000000 tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/tke_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)    19591 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1059071 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190375 2023-07-07 00:34:51.000000 tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/tke_client.py
```

### Comparing `tencentcloud-sdk-python-tke-3.0.929/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.930/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.929/setup.py` & `tencentcloud-sdk-python-tke-3.0.930/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.929/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.930/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.929/README.rst` & `tencentcloud-sdk-python-tke-3.0.930/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.929/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.930/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3041,27 +3041,30 @@
         :type Alias: str
         :param _NodeCount: 节点数量
         :type NodeCount: int
         :param _PodCount: Pod数量
         :type PodCount: int
         :param _ConfigMapCount: Configmap数量
         :type ConfigMapCount: int
+        :param _RSCount: ReplicaSets数量
+        :type RSCount: int
         :param _CRDCount: CRD数量
         :type CRDCount: int
         :param _Enable: 是否启用
         :type Enable: bool
         :param _OtherCount: 其他资源数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type OtherCount: int
         """
         self._Name = None
         self._Alias = None
         self._NodeCount = None
         self._PodCount = None
         self._ConfigMapCount = None
+        self._RSCount = None
         self._CRDCount = None
         self._Enable = None
         self._OtherCount = None
 
     @property
     def Name(self):
         return self._Name
@@ -3099,14 +3102,22 @@
         return self._ConfigMapCount
 
     @ConfigMapCount.setter
     def ConfigMapCount(self, ConfigMapCount):
         self._ConfigMapCount = ConfigMapCount
 
     @property
+    def RSCount(self):
+        return self._RSCount
+
+    @RSCount.setter
+    def RSCount(self, RSCount):
+        self._RSCount = RSCount
+
+    @property
     def CRDCount(self):
         return self._CRDCount
 
     @CRDCount.setter
     def CRDCount(self, CRDCount):
         self._CRDCount = CRDCount
 
@@ -3129,14 +3140,15 @@
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._Alias = params.get("Alias")
         self._NodeCount = params.get("NodeCount")
         self._PodCount = params.get("PodCount")
         self._ConfigMapCount = params.get("ConfigMapCount")
+        self._RSCount = params.get("RSCount")
         self._CRDCount = params.get("CRDCount")
         self._Enable = params.get("Enable")
         self._OtherCount = params.get("OtherCount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
@@ -18074,23 +18086,26 @@
 
     def __init__(self):
         r"""
         :param _CRDUsage: CRD使用量
         :type CRDUsage: :class:`tencentcloud.tke.v20180525.models.ResourceUsage`
         :param _PodUsage: Pod使用量
         :type PodUsage: int
+        :param _RSUsage: ReplicaSet使用量
+        :type RSUsage: int
         :param _ConfigMapUsage: ConfigMap使用量
         :type ConfigMapUsage: int
         :param _OtherUsage: 其他资源使用量
         :type OtherUsage: :class:`tencentcloud.tke.v20180525.models.ResourceUsage`
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._CRDUsage = None
         self._PodUsage = None
+        self._RSUsage = None
         self._ConfigMapUsage = None
         self._OtherUsage = None
         self._RequestId = None
 
     @property
     def CRDUsage(self):
         return self._CRDUsage
@@ -18104,14 +18119,22 @@
         return self._PodUsage
 
     @PodUsage.setter
     def PodUsage(self, PodUsage):
         self._PodUsage = PodUsage
 
     @property
+    def RSUsage(self):
+        return self._RSUsage
+
+    @RSUsage.setter
+    def RSUsage(self, RSUsage):
+        self._RSUsage = RSUsage
+
+    @property
     def ConfigMapUsage(self):
         return self._ConfigMapUsage
 
     @ConfigMapUsage.setter
     def ConfigMapUsage(self, ConfigMapUsage):
         self._ConfigMapUsage = ConfigMapUsage
 
@@ -18133,14 +18156,15 @@
 
 
     def _deserialize(self, params):
         if params.get("CRDUsage") is not None:
             self._CRDUsage = ResourceUsage()
             self._CRDUsage._deserialize(params.get("CRDUsage"))
         self._PodUsage = params.get("PodUsage")
+        self._RSUsage = params.get("RSUsage")
         self._ConfigMapUsage = params.get("ConfigMapUsage")
         if params.get("OtherUsage") is not None:
             self._OtherUsage = ResourceUsage()
             self._OtherUsage._deserialize(params.get("OtherUsage"))
         self._RequestId = params.get("RequestId")
 
 
@@ -26467,24 +26491,27 @@
         r"""
         :param _ClusterId: 集群ID
         :type ClusterId: str
         :param _NodePoolId: 节点池ID
         :type NodePoolId: str
         :param _Name: 节点池名称
         :type Name: str
+        :param _SecurityGroupIds: 安全组ID列表
+        :type SecurityGroupIds: list of str
         :param _Labels: 虚拟节点label
         :type Labels: list of Label
         :param _Taints: 虚拟节点taint
         :type Taints: list of Taint
         :param _DeletionProtection: 删除保护开关
         :type DeletionProtection: bool
         """
         self._ClusterId = None
         self._NodePoolId = None
         self._Name = None
+        self._SecurityGroupIds = None
         self._Labels = None
         self._Taints = None
         self._DeletionProtection = None
 
     @property
     def ClusterId(self):
         return self._ClusterId
@@ -26506,14 +26533,22 @@
         return self._Name
 
     @Name.setter
     def Name(self, Name):
         self._Name = Name
 
     @property
+    def SecurityGroupIds(self):
+        return self._SecurityGroupIds
+
+    @SecurityGroupIds.setter
+    def SecurityGroupIds(self, SecurityGroupIds):
+        self._SecurityGroupIds = SecurityGroupIds
+
+    @property
     def Labels(self):
         return self._Labels
 
     @Labels.setter
     def Labels(self, Labels):
         self._Labels = Labels
 
@@ -26534,14 +26569,15 @@
         self._DeletionProtection = DeletionProtection
 
 
     def _deserialize(self, params):
         self._ClusterId = params.get("ClusterId")
         self._NodePoolId = params.get("NodePoolId")
         self._Name = params.get("Name")
+        self._SecurityGroupIds = params.get("SecurityGroupIds")
         if params.get("Labels") is not None:
             self._Labels = []
             for item in params.get("Labels"):
                 obj = Label()
                 obj._deserialize(item)
                 self._Labels.append(obj)
         if params.get("Taints") is not None:
```

### Comparing `tencentcloud-sdk-python-tke-3.0.929/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.930/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*


# Comparing `tmp/tencentcloud-sdk-python-tcr-3.0.928.tar.gz` & `tmp/tencentcloud-sdk-python-tcr-3.0.929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.928.tar", last modified: Wed Jul  5 00:34:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcr-3.0.929.tar", last modified: Thu Jul  6 00:35:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcr-3.0.928.tar` & `tencentcloud-sdk-python-tcr-3.0.929.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud_sdk_python_tcr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/
--rw-r--r--   0 root         (0) root         (0)     8520 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   424696 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100588 2023-07-05 00:34:28.000000 tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/tcr_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud_sdk_python_tcr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud_sdk_python_tcr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud_sdk_python_tcr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud_sdk_python_tcr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/
+-rw-r--r--   0 root         (0) root         (0)     8520 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   425647 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100588 2023-07-06 00:35:13.000000 tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/tcr_client.py
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/setup.py` & `tencentcloud-sdk-python-tcr-3.0.929/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.929/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/README.rst` & `tencentcloud-sdk-python-tcr-3.0.929/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcr-3.0.929/tencentcloud_sdk_python_tcr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcr
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Tcr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.928'
+__version__ = '3.0.929'
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/errorcodes.py` & `tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/models.py` & `tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1221,22 +1221,25 @@
         :type RegistryChargeType: int
         :param _RegistryChargePrepaid: 预付费自动续费标识和购买时长
         :type RegistryChargePrepaid: :class:`tencentcloud.tcr.v20190924.models.RegistryChargePrepaid`
         :param _SyncTag: 是否同步TCR云标签至生成的COS Bucket
         :type SyncTag: bool
         :param _EnableCosMAZ: 是否开启Cos桶多AZ特性
         :type EnableCosMAZ: bool
+        :param _DeletionProtection: 是否开启实例删除保护
+        :type DeletionProtection: bool
         """
         self._RegistryName = None
         self._RegistryType = None
         self._TagSpecification = None
         self._RegistryChargeType = None
         self._RegistryChargePrepaid = None
         self._SyncTag = None
         self._EnableCosMAZ = None
+        self._DeletionProtection = None
 
     @property
     def RegistryName(self):
         return self._RegistryName
 
     @RegistryName.setter
     def RegistryName(self, RegistryName):
@@ -1286,27 +1289,36 @@
     def EnableCosMAZ(self):
         return self._EnableCosMAZ
 
     @EnableCosMAZ.setter
     def EnableCosMAZ(self, EnableCosMAZ):
         self._EnableCosMAZ = EnableCosMAZ
 
+    @property
+    def DeletionProtection(self):
+        return self._DeletionProtection
+
+    @DeletionProtection.setter
+    def DeletionProtection(self, DeletionProtection):
+        self._DeletionProtection = DeletionProtection
+
 
     def _deserialize(self, params):
         self._RegistryName = params.get("RegistryName")
         self._RegistryType = params.get("RegistryType")
         if params.get("TagSpecification") is not None:
             self._TagSpecification = TagSpecification()
             self._TagSpecification._deserialize(params.get("TagSpecification"))
         self._RegistryChargeType = params.get("RegistryChargeType")
         if params.get("RegistryChargePrepaid") is not None:
             self._RegistryChargePrepaid = RegistryChargePrepaid()
             self._RegistryChargePrepaid._deserialize(params.get("RegistryChargePrepaid"))
         self._SyncTag = params.get("SyncTag")
         self._EnableCosMAZ = params.get("EnableCosMAZ")
+        self._DeletionProtection = params.get("DeletionProtection")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -10604,19 +10616,25 @@
 
     """
 
     def __init__(self):
         r"""
         :param _RegistryId: 实例ID
         :type RegistryId: str
-        :param _RegistryType: 实例的规格
+        :param _RegistryType: 实例的规格,
+基础版：basic
+标准版：standard
+高级版：premium
         :type RegistryType: str
+        :param _DeletionProtection: 实例删除保护，false为关闭
+        :type DeletionProtection: bool
         """
         self._RegistryId = None
         self._RegistryType = None
+        self._DeletionProtection = None
 
     @property
     def RegistryId(self):
         return self._RegistryId
 
     @RegistryId.setter
     def RegistryId(self, RegistryId):
@@ -10626,18 +10644,27 @@
     def RegistryType(self):
         return self._RegistryType
 
     @RegistryType.setter
     def RegistryType(self, RegistryType):
         self._RegistryType = RegistryType
 
+    @property
+    def DeletionProtection(self):
+        return self._DeletionProtection
+
+    @DeletionProtection.setter
+    def DeletionProtection(self, DeletionProtection):
+        self._DeletionProtection = DeletionProtection
+
 
     def _deserialize(self, params):
         self._RegistryId = params.get("RegistryId")
         self._RegistryType = params.get("RegistryType")
+        self._DeletionProtection = params.get("DeletionProtection")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcr-3.0.928/tencentcloud/tcr/v20190924/tcr_client.py` & `tencentcloud-sdk-python-tcr-3.0.929/tencentcloud/tcr/v20190924/tcr_client.py`

 * *Files identical despite different names*


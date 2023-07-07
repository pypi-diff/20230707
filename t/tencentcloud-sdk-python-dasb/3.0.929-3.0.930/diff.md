# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.929.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.929.tar", last modified: Thu Jul  6 00:24:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.930.tar", last modified: Fri Jul  7 00:21:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.929.tar` & `tencentcloud-sdk-python-dasb-3.0.930.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/setup.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)    45577 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   259484 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:24:14.000000 tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)    45577 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   259761 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:21:52.000000 tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/__init__.py
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/setup.py` & `tencentcloud-sdk-python-dasb-3.0.930/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.930/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.930/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/README.rst` & `tencentcloud-sdk-python-dasb-3.0.930/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.929/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.930/tencentcloud/dasb/v20191018/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4828,27 +4828,30 @@
         :param _Limit: 每页条目数量，默认20, 最大500
         :type Limit: int
         :param _UserName: 精确查询，IdSet为空时才生效
         :type UserName: str
         :param _Phone: 精确查询，IdSet、UserName为空时才生效。
 大陆手机号直接填写，如果是其他国家、地区号码,按照"国家地区代码|手机号"的格式输入。如: "+852|xxxxxxxx"
         :type Phone: str
+        :param _Email: 邮箱，精确查询
+        :type Email: str
         :param _AuthorizedDeviceIdSet: 查询具有指定资产ID访问权限的用户
         :type AuthorizedDeviceIdSet: list of int non-negative
         :param _AuthTypeSet: 认证方式，0 - 本地, 1 - LDAP, 2 - OAuth, 不传为全部
         :type AuthTypeSet: list of int non-negative
         :param _DepartmentId: 部门ID，用于过滤属于某个部门的用户
         :type DepartmentId: str
         """
         self._IdSet = None
         self._Name = None
         self._Offset = None
         self._Limit = None
         self._UserName = None
         self._Phone = None
+        self._Email = None
         self._AuthorizedDeviceIdSet = None
         self._AuthTypeSet = None
         self._DepartmentId = None
 
     @property
     def IdSet(self):
         return self._IdSet
@@ -4894,14 +4897,22 @@
         return self._Phone
 
     @Phone.setter
     def Phone(self, Phone):
         self._Phone = Phone
 
     @property
+    def Email(self):
+        return self._Email
+
+    @Email.setter
+    def Email(self, Email):
+        self._Email = Email
+
+    @property
     def AuthorizedDeviceIdSet(self):
         return self._AuthorizedDeviceIdSet
 
     @AuthorizedDeviceIdSet.setter
     def AuthorizedDeviceIdSet(self, AuthorizedDeviceIdSet):
         self._AuthorizedDeviceIdSet = AuthorizedDeviceIdSet
 
@@ -4925,14 +4936,15 @@
     def _deserialize(self, params):
         self._IdSet = params.get("IdSet")
         self._Name = params.get("Name")
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
         self._UserName = params.get("UserName")
         self._Phone = params.get("Phone")
+        self._Email = params.get("Email")
         self._AuthorizedDeviceIdSet = params.get("AuthorizedDeviceIdSet")
         self._AuthTypeSet = params.get("AuthTypeSet")
         self._DepartmentId = params.get("DepartmentId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
@@ -9323,18 +9335,18 @@
 
     def __init__(self):
         r"""
         :param _UserName: 用户名, 3-20个字符 必须以英文字母开头，且不能包含字母、数字、.、_、-以外的字符
         :type UserName: str
         :param _RealName: 用户姓名， 最大20个字符，不能包含空白字符
         :type RealName: str
-        :param _Phone: 手机号码， 大陆手机号直接填写，如果是其他国家、地区号码,按照"国家地区代码|手机号"的格式输入。如: "+852|xxxxxxxx"
-        :type Phone: str
         :param _Id: 用户ID
         :type Id: int
+        :param _Phone: 手机号码， 大陆手机号直接填写，如果是其他国家、地区号码,按照"国家地区代码|手机号"的格式输入。如: "+852|xxxxxxxx"
+        :type Phone: str
         :param _Email: 电子邮件
         :type Email: str
         :param _ValidateFrom: 用户生效时间，如:"2021-09-22T00:00:00+00:00"
 生效、失效时间不填则用户长期有效
         :type ValidateFrom: str
         :param _ValidateTo: 用户失效时间，如:"2021-09-22T00:00:00+00:00"
 生效、失效时间不填则用户长期有效
@@ -9350,16 +9362,16 @@
         :type Department: :class:`tencentcloud.dasb.v20191018.models.Department`
         :param _DepartmentId: 用户所属部门（用于入参）
 注意：此字段可能返回 null，表示取不到有效值。
         :type DepartmentId: str
         """
         self._UserName = None
         self._RealName = None
-        self._Phone = None
         self._Id = None
+        self._Phone = None
         self._Email = None
         self._ValidateFrom = None
         self._ValidateTo = None
         self._GroupSet = None
         self._AuthType = None
         self._ValidateTime = None
         self._Department = None
@@ -9378,30 +9390,30 @@
         return self._RealName
 
     @RealName.setter
     def RealName(self, RealName):
         self._RealName = RealName
 
     @property
-    def Phone(self):
-        return self._Phone
-
-    @Phone.setter
-    def Phone(self, Phone):
-        self._Phone = Phone
-
-    @property
     def Id(self):
         return self._Id
 
     @Id.setter
     def Id(self, Id):
         self._Id = Id
 
     @property
+    def Phone(self):
+        return self._Phone
+
+    @Phone.setter
+    def Phone(self, Phone):
+        self._Phone = Phone
+
+    @property
     def Email(self):
         return self._Email
 
     @Email.setter
     def Email(self, Email):
         self._Email = Email
 
@@ -9461,16 +9473,16 @@
     def DepartmentId(self, DepartmentId):
         self._DepartmentId = DepartmentId
 
 
     def _deserialize(self, params):
         self._UserName = params.get("UserName")
         self._RealName = params.get("RealName")
-        self._Phone = params.get("Phone")
         self._Id = params.get("Id")
+        self._Phone = params.get("Phone")
         self._Email = params.get("Email")
         self._ValidateFrom = params.get("ValidateFrom")
         self._ValidateTo = params.get("ValidateTo")
         if params.get("GroupSet") is not None:
             self._GroupSet = []
             for item in params.get("GroupSet"):
                 obj = Group()
```


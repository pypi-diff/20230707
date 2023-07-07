# Comparing `tmp/tencentcloud-sdk-python-iotcloud-3.0.929.tar.gz` & `tmp/tencentcloud-sdk-python-iotcloud-3.0.930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.929.tar", last modified: Thu Jul  6 00:28:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.930.tar", last modified: Fri Jul  7 00:26:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotcloud-3.0.929.tar` & `tencentcloud-sdk-python-iotcloud-3.0.930.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/
--rw-r--r--   0 root         (0) root         (0)    12668 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   281180 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64286 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/iotcloud_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/
--rw-r--r--   0 root         (0) root         (0)    12818 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   278249 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66885 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:28:28.000000 tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   281180 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64286 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/iotcloud_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/
+-rw-r--r--   0 root         (0) root         (0)    12818 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   278249 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66885 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:26:06.000000 tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/setup.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.930/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/README.rst` & `tencentcloud-sdk-python-iotcloud-3.0.930/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20180614/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20180614/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/iotcloud/v20210408/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/iotcloud/v20210408/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.929/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotcloud-3.0.930/tencentcloud/__init__.py`

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


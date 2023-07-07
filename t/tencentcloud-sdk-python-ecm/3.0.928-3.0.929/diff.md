# Comparing `tmp/tencentcloud-sdk-python-ecm-3.0.928.tar.gz` & `tmp/tencentcloud-sdk-python-ecm-3.0.929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.928.tar", last modified: Wed Jul  5 00:25:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.929.tar", last modified: Thu Jul  6 00:25:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecm-3.0.928.tar` & `tencentcloud-sdk-python-ecm-3.0.929.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud_sdk_python_ecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/
--rw-r--r--   0 root         (0) root         (0)   126245 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/ecm_client.py
--rw-r--r--   0 root         (0) root         (0)    23407 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   697430 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 00:25:23.000000 tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud_sdk_python_ecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/
+-rw-r--r--   0 root         (0) root         (0)   126245 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/ecm_client.py
+-rw-r--r--   0 root         (0) root         (0)    23407 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   697430 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:25:48.000000 tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/__init__.py
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/setup.py` & `tencentcloud-sdk-python-ecm-3.0.929/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.929/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/README.rst` & `tencentcloud-sdk-python-ecm-3.0.929/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.929/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.928
+Version: 3.0.929
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/ecm_client.py` & `tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/ecm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/errorcodes.py` & `tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.928/tencentcloud/ecm/v20190719/models.py` & `tencentcloud-sdk-python-ecm-3.0.929/tencentcloud/ecm/v20190719/models.py`

 * *Files identical despite different names*


# Comparing `tmp/tencentcloud-sdk-python-partners-3.0.929.tar.gz` & `tmp/tencentcloud-sdk-python-partners-3.0.930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.929.tar", last modified: Thu Jul  6 00:31:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.930.tar", last modified: Fri Jul  7 00:29:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-partners-3.0.929.tar` & `tencentcloud-sdk-python-partners-3.0.930.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud_sdk_python_partners.egg-info/
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud_sdk_python_partners.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)      885 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   107514 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19334 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-06 00:31:41.000000 tencentcloud-sdk-python-partners-3.0.929/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud_sdk_python_partners.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud_sdk_python_partners.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)      885 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   107514 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19334 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-07 00:29:13.000000 tencentcloud-sdk-python-partners-3.0.930/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-partners-3.0.929/tencentcloud_sdk_python_partners.egg-info/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.930/tencentcloud_sdk_python_partners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.929/setup.py` & `tencentcloud-sdk-python-partners-3.0.930/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.929/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.930/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.929
+Version: 3.0.930
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.929/README.rst` & `tencentcloud-sdk-python-partners-3.0.930/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.929/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-partners-3.0.930/tencentcloud/partners/v20180321/partners_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.929/tencentcloud/__init__.py` & `tencentcloud-sdk-python-partners-3.0.930/tencentcloud/__init__.py`

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


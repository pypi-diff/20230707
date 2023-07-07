# Comparing `tmp/tclab-sdk-1.3.tar.gz` & `tmp/tclab-sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclab-sdk-1.3.tar", last modified: Fri Jul  7 03:17:44 2023, max compression
+gzip compressed data, was "tclab-sdk-1.3.1.tar", last modified: Fri Jul  7 05:44:05 2023, max compression
```

## Comparing `tclab-sdk-1.3.tar` & `tclab-sdk-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 03:17:44.852584 tclab-sdk-1.3/
--rw-rw-rw-   0        0        0      886 2023-07-07 03:17:44.850582 tclab-sdk-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 03:17:44.853589 tclab-sdk-1.3/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-07-07 03:17:30.000000 tclab-sdk-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:17:44.805582 tclab-sdk-1.3/tclab/
--rw-rw-rw-   0        0        0    16492 2023-07-07 02:49:58.000000 tclab-sdk-1.3/tclab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:17:44.847581 tclab-sdk-1.3/tclab_sdk.egg-info/
--rw-rw-rw-   0        0        0      886 2023-07-07 03:17:44.000000 tclab-sdk-1.3/tclab_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-07 03:17:44.000000 tclab-sdk-1.3/tclab_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 03:17:44.000000 tclab-sdk-1.3/tclab_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-07 03:17:44.000000 tclab-sdk-1.3/tclab_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 03:17:44.000000 tclab-sdk-1.3/tclab_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 05:44:05.407477 tclab-sdk-1.3.1/
+-rw-rw-rw-   0        0        0      888 2023-07-07 05:44:05.406480 tclab-sdk-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 05:44:05.408482 tclab-sdk-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-07-07 05:44:02.000000 tclab-sdk-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:44:05.375478 tclab-sdk-1.3.1/tclab/
+-rw-rw-rw-   0        0        0    16593 2023-07-07 05:43:34.000000 tclab-sdk-1.3.1/tclab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:44:05.403482 tclab-sdk-1.3.1/tclab_sdk.egg-info/
+-rw-rw-rw-   0        0        0      888 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 05:44:05.000000 tclab-sdk-1.3.1/tclab_sdk.egg-info/top_level.txt
```

### Comparing `tclab-sdk-1.3/PKG-INFO` & `tclab-sdk-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3
+Version: 1.3.1
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tclab-sdk-1.3/setup.py` & `tclab-sdk-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tclab-sdk",  # 模块名称
-    version="1.3",  # 当前版本
+    version="1.3.1",  # 当前版本
     author="Haotian Yang",  # 作者
     author_email="yht1592754117@126.com",  # 作者邮箱
     description="TC Laboratory Central_Management_System Client Module",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
```

### Comparing `tclab-sdk-1.3/tclab/__init__.py` & `tclab-sdk-1.3.1/tclab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             key (str): 密钥
 
         Returns:
             str: 解密的数据
         """
         try:
             key = key.encode()
-            data = _base64.b64edecode(data)
+            data = _base64.b64decode(data)
             cryptor = _AES.new(key, _AES.MODE_ECB)
             text = cryptor.decrypt(data)
             text = _unpad(text, _AES.block_size).decode()
             return text
         except:
             return False
     
@@ -116,14 +116,19 @@
         try:
             d._map()
         except:
             pass
         return d
 
     def status(self):
+        """查询系统状态
+
+        Returns:
+            dict: 状态信息
+        """
         return self.request('/status',{})
         
     def list_devices(self):
         """列出所有设备
 
         Returns:
             dict: 设备信息
@@ -457,14 +462,15 @@
         
         def download(self):
             res = self._request('/file/download', {"path": self.path})
             if res:
                 src=res['base64']
                 return _base64.b64edecode(src)
             raise Exception('unkown error')
+    
     class _keys:
         """
         密钥管理类
         """
         def list(self):
             """列出密钥
```

### Comparing `tclab-sdk-1.3/tclab_sdk.egg-info/PKG-INFO` & `tclab-sdk-1.3.1/tclab_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.3
+Version: 1.3.1
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```


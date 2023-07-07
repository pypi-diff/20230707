# Comparing `tmp/TSMasterAPI-2.1.2.tar.gz` & `tmp/TSMasterAPI-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.1.2.tar", last modified: Fri Jul  7 10:26:06 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.1.3.tar", last modified: Fri Jul  7 14:18:36 2023, max compression
```

## Comparing `TSMasterAPI-2.1.2.tar` & `TSMasterAPI-2.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:26:06.068251 TSMasterAPI-2.1.2/
--rw-rw-rw-   0        0        0     1024 2023-07-07 10:26:06.067235 TSMasterAPI-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-07 10:26:06.056648 TSMasterAPI-2.1.2/TSMasterAPI/
--rw-rw-rw-   0        0        0    42874 2023-07-07 07:59:38.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    72160 2023-07-07 05:19:25.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0    24356 2023-07-07 02:04:02.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSFibex_parse.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    32023 2023-07-07 02:04:02.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.2/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:26:06.066219 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 10:26:06.068251 TSMasterAPI-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-07-07 10:25:50.000000 TSMasterAPI-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:18:36.827619 TSMasterAPI-2.1.3/
+-rw-rw-rw-   0        0        0     1024 2023-07-07 14:18:36.826619 TSMasterAPI-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 14:18:36.809859 TSMasterAPI-2.1.3/TSMasterAPI/
+-rw-rw-rw-   0        0        0    42874 2023-07-07 07:59:38.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    72392 2023-07-07 14:16:58.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0    24356 2023-07-07 02:04:02.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    32023 2023-07-07 02:04:02.000000 TSMasterAPI-2.1.3/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.3/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:18:36.825618 TSMasterAPI-2.1.3/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-07-07 14:18:36.000000 TSMasterAPI-2.1.3/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-07-07 14:18:36.000000 TSMasterAPI-2.1.3/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:18:36.000000 TSMasterAPI-2.1.3/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 14:18:36.000000 TSMasterAPI-2.1.3/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.3/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 14:18:36.827619 TSMasterAPI-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-07-07 14:17:51.000000 TSMasterAPI-2.1.3/setup.py
```

### Comparing `TSMasterAPI-2.1.2/PKG-INFO` & `TSMasterAPI-2.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.1.2
+Version: 2.1.3
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSBUSDriver.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSBUSDriver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSCommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-07-07 12:22:46
+LastEditTime: 2023-07-07 22:16:58
 '''
 from .TSDirver import *
 from .TSStructure import *  
 from .TSEnumdefine import *  
 from .TSFibex_parse import * 
 
 # Common Functions
@@ -989,14 +989,19 @@
 
 
 # 获取报文中信号值
 tscom_get_flexray_signal_value = dll.tscom_get_flexray_signal_value #函数对象
 tscom_get_flexray_signal_value.argtypes = [PFlexRaySignal,pu8] #指定参数类型
 tscom_get_flexray_signal_value.restype = c_double 
 
+#获取报文原始值
+get_flexray_signal_raw_value = dll.get_flexray_signal_raw_value #函数对象
+get_flexray_signal_raw_value.argtypes = [PFlexRaySignal,pu8] #指定参数类型
+get_flexray_signal_raw_value.restype = s64 
+
 # 设置报文中的信号值
 tscom_set_flexray_signal_value = dll.tscom_set_flexray_signal_value #函数对象
 tscom_set_flexray_signal_value.argtypes = [PFlexRaySignal,pu8,double] #指定参数类型
 tscom_set_flexray_signal_value.restype = TS_ReturnType 
 tscom_set_flexray_signal_value.errcheck = check_status_operation
 
 # RBS
```

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSEnumdefine.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSFibex_parse.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSFibex_parse.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.1.3/TSMasterAPI/TSStructure.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.1.3/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.1.2
+Version: 2.1.3
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.1.2/license.txt` & `TSMasterAPI-2.1.3/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.2/setup.py` & `TSMasterAPI-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-07-07 18:25:50
+LastEditTime: 2023-07-07 22:17:51
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.1.2',  # 版本号
+      version='2.1.3',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```


# Comparing `tmp/tclab-sdk-1.1.tar.gz` & `tmp/tclab-sdk-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclab-sdk-1.1.tar", last modified: Fri Jul  7 03:07:11 2023, max compression
+gzip compressed data, was "tclab-sdk-1.2.tar", last modified: Fri Jul  7 03:15:29 2023, max compression
```

## Comparing `tclab-sdk-1.1.tar` & `tclab-sdk-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 03:07:11.455923 tclab-sdk-1.1/
--rw-rw-rw-   0        0        0      886 2023-07-07 03:07:11.451923 tclab-sdk-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 03:07:11.455923 tclab-sdk-1.1/setup.cfg
--rw-rw-rw-   0        0        0      920 2023-07-07 03:06:42.000000 tclab-sdk-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:07:11.420095 tclab-sdk-1.1/tclab/
--rw-rw-rw-   0        0        0    16492 2023-07-07 02:49:58.000000 tclab-sdk-1.1/tclab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 03:07:11.446040 tclab-sdk-1.1/tclab_sdk.egg-info/
--rw-rw-rw-   0        0        0      886 2023-07-07 03:07:11.000000 tclab-sdk-1.1/tclab_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-07-07 03:07:11.000000 tclab-sdk-1.1/tclab_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 03:07:11.000000 tclab-sdk-1.1/tclab_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-07 03:07:11.000000 tclab-sdk-1.1/tclab_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 03:07:11.000000 tclab-sdk-1.1/tclab_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 03:15:29.882213 tclab-sdk-1.2/
+-rw-rw-rw-   0        0        0      886 2023-07-07 03:15:29.881213 tclab-sdk-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-07-07 03:03:35.000000 tclab-sdk-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 03:15:29.883221 tclab-sdk-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-07-07 03:14:23.000000 tclab-sdk-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:15:29.832221 tclab-sdk-1.2/tclab/
+-rw-rw-rw-   0        0        0    16492 2023-07-07 02:49:58.000000 tclab-sdk-1.2/tclab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 03:15:29.878214 tclab-sdk-1.2/tclab_sdk.egg-info/
+-rw-rw-rw-   0        0        0      886 2023-07-07 03:15:29.000000 tclab-sdk-1.2/tclab_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-07-07 03:15:29.000000 tclab-sdk-1.2/tclab_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 03:15:29.000000 tclab-sdk-1.2/tclab_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-07 03:15:29.000000 tclab-sdk-1.2/tclab_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 03:15:29.000000 tclab-sdk-1.2/tclab_sdk.egg-info/top_level.txt
```

### Comparing `tclab-sdk-1.1/PKG-INFO` & `tclab-sdk-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.1
+Version: 1.2
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tclab-sdk-1.1/setup.py` & `tclab-sdk-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tclab-sdk",  # 模块名称
-    version="1.1",  # 当前版本
+    version="1.2",  # 当前版本
     author="Haotian Yang",  # 作者
     author_email="yht1592754117@126.com",  # 作者邮箱
     description="TC Laboratory Central_Management_System Client Module",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据
@@ -15,10 +15,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     # 依赖模块
     install_requires=[
         'requests',
+        'base64',
+        'hashlab',
+        'pycryptodome',
+        'platform'
     ],
     python_requires='>=3',
 )
```

### Comparing `tclab-sdk-1.1/tclab/__init__.py` & `tclab-sdk-1.2/tclab/__init__.py`

 * *Files identical despite different names*

### Comparing `tclab-sdk-1.1/tclab_sdk.egg-info/PKG-INFO` & `tclab-sdk-1.2/tclab_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclab-sdk
-Version: 1.1
+Version: 1.2
 Summary: TC Laboratory Central_Management_System Client Module
 Home-page: UNKNOWN
 Author: Haotian Yang
 Author-email: yht1592754117@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```


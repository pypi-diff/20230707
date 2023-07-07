# Comparing `tmp/ectool-1.1.0.tar.gz` & `tmp/ectool-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.1.0.tar", last modified: Fri Jul  7 07:01:39 2023, max compression
+gzip compressed data, was "ectool-1.1.1.tar", last modified: Fri Jul  7 07:21:03 2023, max compression
```

## Comparing `ectool-1.1.0.tar` & `ectool-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.768663 ectool-1.1.0/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1585 2023-07-07 07:01:39.768663 ectool-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-07-07 06:59:20.000000 ectool-1.1.0/README.md
--rw-rw-rw-   0        0        0      113 2023-07-07 07:01:39.769663 ectool-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     7895 2023-07-07 06:56:02.000000 ectool-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.746662 ectool-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.759663 ectool-1.1.0/src/ectool/
--rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.0/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    15521 2023-07-07 06:53:51.000000 ectool-1.1.0/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.0/src/ectool/ecag.py
--rw-rw-rw-   0        0        0     5069 2023-07-07 07:00:17.000000 ectool-1.1.0/src/ectool/eccli.py
--rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.0/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.0/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     3790 2023-07-07 06:32:49.000000 ectool-1.1.0/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-07 07:01:39.767662 ectool-1.1.0/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     1585 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 07:01:39.000000 ectool-1.1.0/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.383125 ectool-1.1.1/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2018 2023-07-07 07:21:03.383125 ectool-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2023-07-07 07:20:11.000000 ectool-1.1.1/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-07 07:21:03.384125 ectool-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     7947 2023-07-07 07:18:53.000000 ectool-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.360127 ectool-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.374126 ectool-1.1.1/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.1/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    15521 2023-07-07 06:53:51.000000 ectool-1.1.1/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0    71158 2023-07-07 06:43:13.000000 ectool-1.1.1/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0     4947 2023-07-07 07:19:15.000000 ectool-1.1.1/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1663 2023-07-07 06:43:10.000000 ectool-1.1.1/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.1/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3790 2023-07-07 06:32:49.000000 ectool-1.1.1/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-07 07:21:03.382125 ectool-1.1.1/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-07 07:21:03.000000 ectool-1.1.1/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.1.0/LICENSE` & `ectool-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.1.0/PKG-INFO` & `ectool-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tools for EC modules, like EC618/EC616/EC718
-Home-page: https://github.com/openLuat/ectools2py
+Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
-Author-email: vt400@qq.com
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
@@ -47,7 +47,24 @@
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
+
+## TODO List
+
+* [ ] 完整的注释
+* [ ] 测试Linux下的兼容性
+* [ ] 测试Mac下的兼容性
+* [ ] 支持刷LuatOS的script.bin
+* [ ] 支持只刷AP
+
+## 参考链接
+
+* 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
+* beanio走的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
+
+## 开源协议
+
+MIT
```

### Comparing `ectool-1.1.0/setup.py` & `ectool-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.1.0",  # Required
+    version="1.1.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -57,21 +57,21 @@
     # This field corresponds to the "Description-Content-Type" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url="https://github.com/openLuat/ectools2py",  # Optional
+    url="https://github.com/openLuat/ectool2py",  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
     author="Wendal Chen",  # Optional
     # This should be a valid email address corresponding to the author listed
     # above.
-    author_email="vt400@qq.com",  # Optional
+    # author_email="vt400@qq.com",  # Optional
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
@@ -86,14 +86,15 @@
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
```

### Comparing `ectool-1.1.0/src/ectool/ecaction.py` & `ectool-1.1.1/src/ectool/ecaction.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.0/src/ectool/ecag.py` & `ectool-1.1.1/src/ectool/ecag.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.0/src/ectool/eccli.py` & `ectool-1.1.1/src/ectool/eccli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 from ectool.ecaction import *
 
 import ectool.ecag as ecag
 
 ecargs = None
 logger = None
 
-# 参考文件 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
-
 def ecburn_auto_select() :
     for item in serial.tools.list_ports.comports():
         if not item.pid or not item.location :
             continue
         if item.vid == 0x17D1 and item.pid == 0x0001 :
             return item.name
     return None
```

### Comparing `ectool-1.1.0/src/ectool/ecconst.py` & `ectool-1.1.1/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.0/src/ectool/ecstruct.py` & `ectool-1.1.1/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.0/src/ectool/unpkg.py` & `ectool-1.1.1/src/ectool/unpkg.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.0/src/ectool.egg-info/PKG-INFO` & `ectool-1.1.1/src/ectool.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tools for EC modules, like EC618/EC616/EC718
-Home-page: https://github.com/openLuat/ectools2py
+Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
-Author-email: vt400@qq.com
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
@@ -47,7 +47,24 @@
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件, 但暂不支持LuatOS的脚本刷机
 
 ```bash
 ectool burn -f example.binpkg
 # 启动后, 按住BOOT键, 复位模块, 或模块开机
 ```
+
+## TODO List
+
+* [ ] 完整的注释
+* [ ] 测试Linux下的兼容性
+* [ ] 测试Mac下的兼容性
+* [ ] 支持刷LuatOS的script.bin
+* [ ] 支持只刷AP
+
+## 参考链接
+
+* 流程参考 https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=483a9555e446577cefc31b5629e843cc814b83cb
+* beanio走的逆向版本 https://github.com/beanjs/beanio-ec618-downloader
+
+## 开源协议
+
+MIT
```


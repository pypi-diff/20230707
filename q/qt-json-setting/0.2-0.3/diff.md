# Comparing `tmp/qt-json-setting-0.2.tar.gz` & `tmp/qt-json-setting-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt-json-setting-0.2.tar", last modified: Fri Jun 30 02:52:20 2023, max compression
+gzip compressed data, was "qt-json-setting-0.3.tar", last modified: Fri Jul  7 01:38:55 2023, max compression
```

## Comparing `qt-json-setting-0.2.tar` & `qt-json-setting-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:52:20.802761 qt-json-setting-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-30 02:52:03.000000 qt-json-setting-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 02:52:20.802761 qt-json-setting-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-30 02:52:03.000000 qt-json-setting-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:52:20.802761 qt-json-setting-0.2/qt-json-setting/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-30 02:52:03.000000 qt-json-setting-0.2/qt-json-setting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 02:52:20.802761 qt-json-setting-0.2/qt_json_setting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-30 02:52:20.000000 qt-json-setting-0.2/qt_json_setting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-30 02:52:20.000000 qt-json-setting-0.2/qt_json_setting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 02:52:20.000000 qt-json-setting-0.2/qt_json_setting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-30 02:52:20.000000 qt-json-setting-0.2/qt_json_setting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 02:52:20.000000 qt-json-setting-0.2/qt_json_setting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 02:52:20.802761 qt-json-setting-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-30 02:52:03.000000 qt-json-setting-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:38:55.278487 qt-json-setting-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-07 01:38:45.000000 qt-json-setting-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 01:38:55.278487 qt-json-setting-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-07 01:38:45.000000 qt-json-setting-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:38:55.278487 qt-json-setting-0.3/qt_json_setting/
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-07-07 01:38:45.000000 qt-json-setting-0.3/qt_json_setting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 01:38:55.278487 qt-json-setting-0.3/qt_json_setting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 01:38:55.000000 qt-json-setting-0.3/qt_json_setting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 01:38:55.278487 qt-json-setting-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-07 01:38:45.000000 qt-json-setting-0.3/setup.py
```

### Comparing `qt-json-setting-0.2/LICENSE` & `qt-json-setting-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qt-json-setting-0.2/PKG-INFO` & `qt-json-setting-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.2
+Version: 0.3
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.2/qt-json-setting/__init__.py` & `qt-json-setting-0.3/qt_json_setting/__init__.py`

 * *Files identical despite different names*

### Comparing `qt-json-setting-0.2/qt_json_setting.egg-info/PKG-INFO` & `qt-json-setting-0.3/qt_json_setting.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-json-setting
-Version: 0.2
+Version: 0.3
 Summary: 根据json schema生成设置界面
 Home-page: https://github.com/ovo-Tim/pyqt-json-settingt
 Author: ovo-tim
 Author-email: ovo-tim@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `qt-json-setting-0.2/setup.py` & `qt-json-setting-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qt-json-setting",
-    version="0.2",
+    version="0.3",
     author="ovo-tim",
     author_email="ovo-tim@qq.com",
     description="根据json schema生成设置界面",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ovo-Tim/pyqt-json-settingt",
     packages=setuptools.find_packages(),
```


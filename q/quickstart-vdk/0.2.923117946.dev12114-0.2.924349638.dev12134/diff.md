# Comparing `tmp/quickstart-vdk-0.2.923117946.dev12114.tar.gz` & `tmp/quickstart-vdk-0.2.924349638.dev12134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.923117946.dev12114.tar", last modified: Thu Jul  6 11:37:14 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.924349638.dev12134.tar", last modified: Fri Jul  7 12:08:48 2023, max compression
```

## Comparing `quickstart-vdk-0.2.923117946.dev12114.tar` & `quickstart-vdk-0.2.924349638.dev12134.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:37:14.240036 quickstart-vdk-0.2.923117946.dev12114/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-06 11:37:14.240036 quickstart-vdk-0.2.923117946.dev12114/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-06 11:36:53.000000 quickstart-vdk-0.2.923117946.dev12114/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:37:14.240036 quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-06 11:37:14.000000 quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-06 11:37:14.000000 quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 11:37:14.000000 quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 11:37:14.000000 quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 11:37:14.000000 quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 11:37:14.240036 quickstart-vdk-0.2.923117946.dev12114/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-06 11:37:03.000000 quickstart-vdk-0.2.923117946.dev12114/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:37:14.240036 quickstart-vdk-0.2.923117946.dev12114/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-06 11:36:53.000000 quickstart-vdk-0.2.923117946.dev12114/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:08:48.711053 quickstart-vdk-0.2.924349638.dev12134/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-07 12:08:48.711053 quickstart-vdk-0.2.924349638.dev12134/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-07 12:08:27.000000 quickstart-vdk-0.2.924349638.dev12134/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:08:48.711053 quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-07 12:08:48.000000 quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-07 12:08:48.000000 quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 12:08:48.000000 quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-07 12:08:48.000000 quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-07 12:08:48.000000 quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 12:08:48.711053 quickstart-vdk-0.2.924349638.dev12134/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-07 12:08:37.000000 quickstart-vdk-0.2.924349638.dev12134/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 12:08:48.711053 quickstart-vdk-0.2.924349638.dev12134/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-07 12:08:27.000000 quickstart-vdk-0.2.924349638.dev12134/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.923117946.dev12114/PKG-INFO` & `quickstart-vdk-0.2.924349638.dev12134/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.923117946.dev12114
+Version: 0.2.924349638.dev12134
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.923117946.dev12114/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.924349638.dev12134/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.923117946.dev12114
+Version: 0.2.924349638.dev12134
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.923117946.dev12114/setup.py` & `quickstart-vdk-0.2.924349638.dev12134/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.923117946.dev12114"
+__version__ = "0.2.924349638.dev12134"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```


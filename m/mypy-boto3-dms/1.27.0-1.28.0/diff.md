# Comparing `tmp/mypy-boto3-dms-1.27.0.tar.gz` & `tmp/mypy-boto3-dms-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dms-1.27.0.tar", last modified: Mon Jul  3 19:50:40 2023, max compression
+gzip compressed data, was "mypy-boto3-dms-1.28.0.tar", last modified: Thu Jul  6 20:59:26 2023, max compression
```

## Comparing `mypy-boto3-dms-1.27.0.tar` & `mypy-boto3-dms-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26839 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.339140 mypy-boto3-dms-1.27.0/mypy_boto3_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66105 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66008 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    92957 2023-07-03 19:35:45.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92906 2023-07-03 19:35:44.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-03 19:35:42.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:40.000000 mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:40.351140 mypy-boto3-dms-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-03 19:35:41.000000 mypy-boto3-dms-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.078282 mypy-boto3-dms-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-07-06 20:59:26.078282 mypy-boto3-dms-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26839 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.066282 mypy-boto3-dms-1.28.0/mypy_boto3_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66105 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66008 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    92957 2023-07-06 20:38:05.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92906 2023-07-06 20:38:04.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-06 20:38:01.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.078282 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28329 2023-07-06 20:59:25.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:25.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:25.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:25.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:25.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:25.000000 mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:26.078282 mypy-boto3-dms-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-06 20:38:00.000000 mypy-boto3-dms-1.28.0/setup.py
```

### Comparing `mypy-boto3-dms-1.27.0/LICENSE` & `mypy-boto3-dms-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/PKG-INFO` & `mypy-boto3-dms-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.27.0
-Summary: Type annotations for boto3.DatabaseMigrationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dms-1.27.0/README.md` & `mypy-boto3-dms-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.py` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/__init__.pyi` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.py` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/client.pyi` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.py` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/literals.pyi` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.py` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/paginator.pyi` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.py` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/type_defs.pyi` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.py` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms/waiter.pyi` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/PKG-INFO` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dms
-Version: 1.27.0
-Summary: Type annotations for boto3.DatabaseMigrationService 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.DatabaseMigrationService 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dms.svg?color=blue)](https://pypi.org/project/mypy-boto3-dms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dms?color=blue)](https://pypistats.org/packages/mypy-boto3-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DatabaseMigrationService 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
+[boto3.DatabaseMigrationService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dms-1.27.0/mypy_boto3_dms.egg-info/SOURCES.txt` & `mypy-boto3-dms-1.28.0/mypy_boto3_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dms-1.27.0/setup.py` & `mypy-boto3-dms-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dms",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DatabaseMigrationService 1.27.0 service generated with"
+        "Type annotations for boto3.DatabaseMigrationService 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```


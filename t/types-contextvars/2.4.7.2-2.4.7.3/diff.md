# Comparing `tmp/types-contextvars-2.4.7.2.tar.gz` & `tmp/types-contextvars-2.4.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-contextvars-2.4.7.2.tar", last modified: Mon Mar 27 18:22:54 2023, max compression
+gzip compressed data, was "types-contextvars-2.4.7.3.tar", last modified: Fri Jul  7 09:16:37 2023, max compression
```

## Comparing `types-contextvars-2.4.7.2.tar` & `types-contextvars-2.4.7.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:54.958243 types-contextvars-2.4.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:22:54.954243 types-contextvars-2.4.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:54.954243 types-contextvars-2.4.7.2/contextvars-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/contextvars-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/contextvars-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:54.958243 types-contextvars-2.4.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:54.954243 types-contextvars-2.4.7.2/types_contextvars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/types_contextvars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/types_contextvars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/types_contextvars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:22:54.000000 types-contextvars-2.4.7.2/types_contextvars.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:16:37.409886 types-contextvars-2.4.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-07 09:16:34.000000 types-contextvars-2.4.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 09:16:34.000000 types-contextvars-2.4.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-07 09:16:37.409886 types-contextvars-2.4.7.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:16:37.409886 types-contextvars-2.4.7.3/contextvars-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 09:16:34.000000 types-contextvars-2.4.7.3/contextvars-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-07 09:16:34.000000 types-contextvars-2.4.7.3/contextvars-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:16:37.409886 types-contextvars-2.4.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-07 09:16:34.000000 types-contextvars-2.4.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:16:37.409886 types-contextvars-2.4.7.3/types_contextvars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-07 09:16:37.000000 types-contextvars-2.4.7.3/types_contextvars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 09:16:37.000000 types-contextvars-2.4.7.3/types_contextvars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:16:37.000000 types-contextvars-2.4.7.3/types_contextvars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 09:16:37.000000 types-contextvars-2.4.7.3/types_contextvars.egg-info/top_level.txt
```

### Comparing `types-contextvars-2.4.7.2/CHANGELOG.md` & `types-contextvars-2.4.7.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.4.7.3 (2023-07-07)
+
+Mark contextvars stubs as no longer updated (#10419)
+
 ## 2.4.7.2 (2023-03-27)
 
 contextvars: widen return value of ContextVar.get(default) (#9953)
 
 ## 2.4.7.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-contextvars-2.4.7.2/PKG-INFO` & `types-contextvars-2.4.7.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-contextvars
-Version: 2.4.7.2
+Version: 2.4.7.3
 Summary: Typing stubs for contextvars
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/contextvars.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `contextvars`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/contextvars. All fixes for
 types and metadata should be contributed there.
 
+*Note:* `types-contextvars` is unmaintained and won't be updated.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `5ad520e27b5e206213dbe209e87c46c483aae7ec` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

### Comparing `types-contextvars-2.4.7.2/contextvars-stubs/__init__.pyi` & `types-contextvars-2.4.7.3/contextvars-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-contextvars-2.4.7.2/setup.py` & `types-contextvars-2.4.7.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `contextvars`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/contextvars. All fixes for
 types and metadata should be contributed there.
 
+*Note:* `types-contextvars` is unmaintained and won't be updated.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `5ad520e27b5e206213dbe209e87c46c483aae7ec` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.4.7.2",
+      version="2.4.7.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/contextvars.md",
```

### Comparing `types-contextvars-2.4.7.2/types_contextvars.egg-info/PKG-INFO` & `types-contextvars-2.4.7.3/types_contextvars.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-contextvars
-Version: 2.4.7.2
+Version: 2.4.7.3
 Summary: Typing stubs for contextvars
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/contextvars.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `contextvars`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/contextvars. All fixes for
 types and metadata should be contributed there.
 
+*Note:* `types-contextvars` is unmaintained and won't be updated.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `5ad520e27b5e206213dbe209e87c46c483aae7ec` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```


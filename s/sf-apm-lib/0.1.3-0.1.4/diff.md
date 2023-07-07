# Comparing `tmp/sf_apm_lib-0.1.3.tar.gz` & `tmp/sf_apm_lib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf_apm_lib-0.1.3.tar", last modified: Wed Feb 23 14:07:25 2022, max compression
+gzip compressed data, was "sf_apm_lib-0.1.4.tar", last modified: Fri Jul  7 04:43:54 2023, max compression
```

## Comparing `sf_apm_lib-0.1.3.tar` & `sf_apm_lib-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 14:07:25.322078 sf_apm_lib-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (116)     1075 2022-02-23 14:07:15.000000 sf_apm_lib-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1613 2022-02-23 14:07:25.322078 sf_apm_lib-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      924 2022-02-23 14:07:15.000000 sf_apm_lib-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-02-23 14:07:25.322078 sf_apm_lib-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1252 2022-02-23 14:07:15.000000 sf_apm_lib-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 14:07:25.322078 sf_apm_lib-0.1.3/sf_apm_lib/
--rw-r--r--   0 runner    (1001) docker     (116)      135 2022-02-23 14:07:15.000000 sf_apm_lib-0.1.3/sf_apm_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2882 2022-02-23 14:07:15.000000 sf_apm_lib-0.1.3/sf_apm_lib/snappyflow.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-23 14:07:25.322078 sf_apm_lib-0.1.3/sf_apm_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1613 2022-02-23 14:07:24.000000 sf_apm_lib-0.1.3/sf_apm_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      243 2022-02-23 14:07:25.000000 sf_apm_lib-0.1.3/sf_apm_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-23 14:07:25.000000 sf_apm_lib-0.1.3/sf_apm_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       61 2022-02-23 14:07:25.000000 sf_apm_lib-0.1.3/sf_apm_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-02-23 14:07:25.000000 sf_apm_lib-0.1.3/sf_apm_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 04:43:54.139555 sf_apm_lib-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-07-07 04:43:43.000000 sf_apm_lib-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-07 04:43:54.135555 sf_apm_lib-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-07 04:43:43.000000 sf_apm_lib-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 04:43:54.139555 sf_apm_lib-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1252 2023-07-07 04:43:43.000000 sf_apm_lib-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 04:43:54.135555 sf_apm_lib-0.1.4/sf_apm_lib/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-07 04:43:43.000000 sf_apm_lib-0.1.4/sf_apm_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5187 2023-07-07 04:43:43.000000 sf_apm_lib-0.1.4/sf_apm_lib/snappyflow.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 04:43:54.135555 sf_apm_lib-0.1.4/sf_apm_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-07 04:43:54.000000 sf_apm_lib-0.1.4/sf_apm_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-07 04:43:54.000000 sf_apm_lib-0.1.4/sf_apm_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 04:43:54.000000 sf_apm_lib-0.1.4/sf_apm_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-07 04:43:54.000000 sf_apm_lib-0.1.4/sf_apm_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-07 04:43:54.000000 sf_apm_lib-0.1.4/sf_apm_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 04:43:54.135555 sf_apm_lib-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       98 2023-07-07 04:43:43.000000 sf_apm_lib-0.1.4/tests/test_sample.py
```

### Comparing `sf_apm_lib-0.1.3/LICENSE` & `sf_apm_lib-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sf_apm_lib-0.1.3/PKG-INFO` & `sf_apm_lib-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sf_apm_lib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Snappyflow pip package
 Home-page: https://github.com/snappyflow/py_snappyflow
 Author: Maplelabs
 Author-email: pradeep.jaiswar@maplelabs.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -50,9 +49,7 @@
 sf.init(profile_key, project_name, app_name)
 # End of manual configuration
 
 trace_config = sf.get_trace_config() # Returns trace config
 
 print(trace_config)
 ```
-
-
```

### Comparing `sf_apm_lib-0.1.3/README.md` & `sf_apm_lib-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sf_apm_lib-0.1.3/setup.py` & `sf_apm_lib-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="sf_apm_lib",
-    version="0.1.3",
+    version="0.1.4",
     url="https://github.com/snappyflow/py_snappyflow",
     license='MIT',
 
     author="Maplelabs",
     author_email="pradeep.jaiswar@maplelabs.com",
 
     description="Snappyflow pip package",
```

### Comparing `sf_apm_lib-0.1.3/sf_apm_lib.egg-info/PKG-INFO` & `sf_apm_lib-0.1.4/sf_apm_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sf-apm-lib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Snappyflow pip package
 Home-page: https://github.com/snappyflow/py_snappyflow
 Author: Maplelabs
 Author-email: pradeep.jaiswar@maplelabs.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -50,9 +49,7 @@
 sf.init(profile_key, project_name, app_name)
 # End of manual configuration
 
 trace_config = sf.get_trace_config() # Returns trace config
 
 print(trace_config)
 ```
-
-
```


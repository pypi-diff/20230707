# Comparing `tmp/internetarchive-deriver-module-1.0.8.tar.gz` & `tmp/internetarchive-deriver-module-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetarchive-deriver-module-1.0.8.tar", last modified: Mon Nov  7 23:10:36 2022, max compression
+gzip compressed data, was "internetarchive-deriver-module-1.0.9.tar", last modified: Sun Nov 13 14:07:21 2022, max compression
```

## Comparing `internetarchive-deriver-module-1.0.8.tar` & `internetarchive-deriver-module-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2022-11-07 23:10:36.751030 internetarchive-deriver-module-1.0.8/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       82 2020-10-24 10:25:12.000000 internetarchive-deriver-module-1.0.8/AUTHORS
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2017-09-30 07:16:25.000000 internetarchive-deriver-module-1.0.8/COPYING
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2017-09-30 07:16:25.000000 internetarchive-deriver-module-1.0.8/LICENSE.TXT
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      746 2022-11-07 23:10:36.751030 internetarchive-deriver-module-1.0.8/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      293 2021-10-22 11:09:21.000000 internetarchive-deriver-module-1.0.8/README.rst
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2022-11-07 23:10:36.751030 internetarchive-deriver-module-1.0.8/derivermodule/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      166 2021-01-26 10:07:38.000000 internetarchive-deriver-module-1.0.8/derivermodule/__init__.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      387 2021-01-15 18:03:55.000000 internetarchive-deriver-module-1.0.8/derivermodule/const.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      589 2022-09-14 11:42:22.000000 internetarchive-deriver-module-1.0.8/derivermodule/files.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     8352 2022-11-04 12:46:15.000000 internetarchive-deriver-module-1.0.8/derivermodule/imagestack.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1109 2021-01-15 18:16:09.000000 internetarchive-deriver-module-1.0.8/derivermodule/logger.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10759 2022-11-07 23:09:43.000000 internetarchive-deriver-module-1.0.8/derivermodule/metadata.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4173 2022-11-04 12:49:38.000000 internetarchive-deriver-module-1.0.8/derivermodule/scandata.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     2734 2021-01-29 18:32:38.000000 internetarchive-deriver-module-1.0.8/derivermodule/task.py
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       22 2022-11-07 23:10:09.000000 internetarchive-deriver-module-1.0.8/derivermodule/version.py
-drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2022-11-07 23:10:36.751030 internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      746 2022-11-07 23:10:36.000000 internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/PKG-INFO
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)      549 2022-11-07 23:10:36.000000 internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/SOURCES.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2022-11-07 23:10:36.000000 internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/dependency_links.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       18 2022-11-07 23:10:36.000000 internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/requires.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       14 2022-11-07 23:10:36.000000 internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/top_level.txt
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)       80 2022-11-07 23:10:36.751030 internetarchive-deriver-module-1.0.8/setup.cfg
--rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1081 2021-10-04 23:34:37.000000 internetarchive-deriver-module-1.0.8/setup.py
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2022-11-13 14:07:21.476619 internetarchive-deriver-module-1.0.9/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       82 2020-10-24 10:25:12.000000 internetarchive-deriver-module-1.0.9/AUTHORS
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2017-09-30 07:16:25.000000 internetarchive-deriver-module-1.0.9/COPYING
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    34523 2017-09-30 07:16:25.000000 internetarchive-deriver-module-1.0.9/LICENSE.TXT
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      746 2022-11-13 14:07:21.476619 internetarchive-deriver-module-1.0.9/PKG-INFO
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      293 2021-10-22 11:09:21.000000 internetarchive-deriver-module-1.0.9/README.rst
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2022-11-13 14:07:21.476619 internetarchive-deriver-module-1.0.9/derivermodule/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      166 2021-01-26 10:07:38.000000 internetarchive-deriver-module-1.0.9/derivermodule/__init__.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      387 2021-01-15 18:03:55.000000 internetarchive-deriver-module-1.0.9/derivermodule/const.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      589 2022-09-14 11:42:22.000000 internetarchive-deriver-module-1.0.9/derivermodule/files.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     8352 2022-11-13 14:07:16.000000 internetarchive-deriver-module-1.0.9/derivermodule/imagestack.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1109 2021-01-15 18:16:09.000000 internetarchive-deriver-module-1.0.9/derivermodule/logger.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)    10759 2022-11-07 23:09:43.000000 internetarchive-deriver-module-1.0.9/derivermodule/metadata.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     4173 2022-11-04 12:49:38.000000 internetarchive-deriver-module-1.0.9/derivermodule/scandata.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     3317 2022-11-13 14:06:19.000000 internetarchive-deriver-module-1.0.9/derivermodule/task.py
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       22 2022-11-13 14:06:49.000000 internetarchive-deriver-module-1.0.9/derivermodule/version.py
+drwxr-xr-x   0 merlijn   (1000) merlijn   (1000)        0 2022-11-13 14:07:21.476619 internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      746 2022-11-13 14:07:21.000000 internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/PKG-INFO
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)      549 2022-11-13 14:07:21.000000 internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/SOURCES.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)        1 2022-11-13 14:07:21.000000 internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/dependency_links.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       18 2022-11-13 14:07:21.000000 internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/requires.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       14 2022-11-13 14:07:21.000000 internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/top_level.txt
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)       80 2022-11-13 14:07:21.479952 internetarchive-deriver-module-1.0.9/setup.cfg
+-rw-r--r--   0 merlijn   (1000) merlijn   (1000)     1081 2021-10-04 23:34:37.000000 internetarchive-deriver-module-1.0.9/setup.py
```

### Comparing `internetarchive-deriver-module-1.0.8/COPYING` & `internetarchive-deriver-module-1.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/LICENSE.TXT` & `internetarchive-deriver-module-1.0.9/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/PKG-INFO` & `internetarchive-deriver-module-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: internetarchive-deriver-module
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python derivermodule package
 Home-page: https://git.archive.org/merlijn/python-derivermodule
 Author: Merlijn Boris Wolf Wajer
 Author-email: merlijn@archive.org
 License: AGPL-3.0
-Download-URL: https://git.archive.org/merlijn/python-derivermodule/-/archive/1.0.0/python-derivermodule-1.0.8.tar.gz
+Download-URL: https://git.archive.org/merlijn/python-derivermodule/-/archive/1.0.0/python-derivermodule-1.0.9.tar.gz
 Keywords: Deriver,Internet Archive
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `internetarchive-deriver-module-1.0.8/derivermodule/files.py` & `internetarchive-deriver-module-1.0.9/derivermodule/files.py`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/derivermodule/imagestack.py` & `internetarchive-deriver-module-1.0.9/derivermodule/imagestack.py`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/derivermodule/logger.py` & `internetarchive-deriver-module-1.0.9/derivermodule/logger.py`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/derivermodule/metadata.py` & `internetarchive-deriver-module-1.0.9/derivermodule/metadata.py`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/derivermodule/scandata.py` & `internetarchive-deriver-module-1.0.9/derivermodule/scandata.py`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/derivermodule/task.py` & `internetarchive-deriver-module-1.0.9/derivermodule/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,41 @@
     """
     extra_targets_file = join(PB_TASK, 'extra_targets.json')
     fp = open(extra_targets_file, 'w+')
     dump(extra_targets, fp)
     fp.close()
 
 
+def write_extra_tasks(extra_tasks):
+    """
+    Create /task/extra_tasks.json file based on `extra_tasks`.
+
+    Args:
+
+    * `extra_tasks`: A list of lists with each two items. The first item being
+      the name (string) of the task, and the second item being a dictionary of
+      arguments for this task.
+
+    Returns:
+
+    * Nothing
+
+    Example:
+
+    >>> write_extra_tasks([
+    >>>     ['book_op.php', {'op1': 'VirusCheck'}]
+    >>> ])
+
+
+    """
+    extra_tasks_file = join(PB_TASK, 'extra_tasks.json')
+    with open(extra_tasks_file, 'w') as f:
+        dump(extra_tasks, f)
+
+
 def get_task_args(task_info):
     """
     Args:
 
     * task_info (dict): task_info as returned by get_task_info()
 
     Returns:
```

### Comparing `internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/PKG-INFO` & `internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: internetarchive-deriver-module
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python derivermodule package
 Home-page: https://git.archive.org/merlijn/python-derivermodule
 Author: Merlijn Boris Wolf Wajer
 Author-email: merlijn@archive.org
 License: AGPL-3.0
-Download-URL: https://git.archive.org/merlijn/python-derivermodule/-/archive/1.0.0/python-derivermodule-1.0.8.tar.gz
+Download-URL: https://git.archive.org/merlijn/python-derivermodule/-/archive/1.0.0/python-derivermodule-1.0.9.tar.gz
 Keywords: Deriver,Internet Archive
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `internetarchive-deriver-module-1.0.8/internetarchive_deriver_module.egg-info/SOURCES.txt` & `internetarchive-deriver-module-1.0.9/internetarchive_deriver_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetarchive-deriver-module-1.0.8/setup.py` & `internetarchive-deriver-module-1.0.9/setup.py`

 * *Files identical despite different names*


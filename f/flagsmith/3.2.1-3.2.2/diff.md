# Comparing `tmp/flagsmith-3.2.1.tar.gz` & `tmp/flagsmith-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-3.2.1.tar", max compression
+gzip compressed data, was "flagsmith-3.2.2.tar", max compression
```

## Comparing `flagsmith-3.2.1.tar` & `flagsmith-3.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1476 2023-05-19 09:21:37.241623 flagsmith-3.2.1/LICENSE
--rw-r--r--   0        0        0     1118 2023-05-19 09:21:37.241623 flagsmith-3.2.1/Readme.md
--rw-r--r--   0        0        0       41 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/__init__.py
--rw-r--r--   0        0        0     2008 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/analytics.py
--rw-r--r--   0        0        0      106 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/exceptions.py
--rw-r--r--   0        0        0    11054 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/flagsmith.py
--rw-r--r--   0        0        0     4633 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/models.py
--rw-r--r--   0        0        0      758 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/polling_manager.py
--rw-r--r--   0        0        0        0 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/utils/__init__.py
--rw-r--r--   0        0        0      204 2023-05-19 09:21:37.241623 flagsmith-3.2.1/flagsmith/utils/identities.py
--rw-r--r--   0        0        0      724 2023-05-19 09:21:37.245623 flagsmith-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1476 2023-07-07 12:56:39.339852 flagsmith-3.2.2/LICENSE
+-rw-r--r--   0        0        0     1118 2023-07-07 12:56:39.339852 flagsmith-3.2.2/Readme.md
+-rw-r--r--   0        0        0       41 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/analytics.py
+-rw-r--r--   0        0        0      106 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/exceptions.py
+-rw-r--r--   0        0        0    11095 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/flagsmith.py
+-rw-r--r--   0        0        0     4633 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/models.py
+-rw-r--r--   0        0        0      822 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/polling_manager.py
+-rw-r--r--   0        0        0        0 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/utils/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-07 12:56:39.343852 flagsmith-3.2.2/flagsmith/utils/identities.py
+-rw-r--r--   0        0        0      724 2023-07-07 12:56:39.343852 flagsmith-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1935 1970-01-01 00:00:00.000000 flagsmith-3.2.2/PKG-INFO
```

### Comparing `flagsmith-3.2.1/LICENSE` & `flagsmith-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.1/Readme.md` & `flagsmith-3.2.2/Readme.md`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.1/flagsmith/analytics.py` & `flagsmith-3.2.2/flagsmith/analytics.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.1/flagsmith/flagsmith.py` & `flagsmith-3.2.2/flagsmith/flagsmith.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                     "in the environment settings page."
                 )
 
             self.environment_data_polling_manager_thread = (
                 EnvironmentDataPollingManager(
                     main=self,
                     refresh_interval_seconds=environment_refresh_interval_seconds,
+                    daemon=True,  # noqa
                 )
             )
             self.environment_data_polling_manager_thread.start()
 
         self._analytics_processor = (
             AnalyticsProcessor(
                 environment_key, self.api_url, timeout=self.request_timeout_seconds
```

### Comparing `flagsmith-3.2.1/flagsmith/models.py` & `flagsmith-3.2.2/flagsmith/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-3.2.1/pyproject.toml` & `flagsmith-3.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flagsmith"
-version = "3.2.1"
+version = "3.2.2"
 description = "Flagsmith Python SDK"
 authors = ["Flagsmith <support@flagsmith.com>"]
 license = "BSD3"
 readme = "Readme.md"
 keywords = ["feature", "flag", "flagsmith", "remote", "config"]
 documentation = "https://docs.flagsmith.com"
 packages = [
```

### Comparing `flagsmith-3.2.1/PKG-INFO` & `flagsmith-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith
-Version: 3.2.1
+Version: 3.2.2
 Summary: Flagsmith Python SDK
 License: BSD3
 Keywords: feature,flag,flagsmith,remote,config
 Author: Flagsmith
 Author-email: support@flagsmith.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flagsmith Version: 3.2.1 Summary: Flagsmith Python
+Metadata-Version: 2.1 Name: flagsmith Version: 3.2.2 Summary: Flagsmith Python
 SDK License: BSD3 Keywords: feature,flag,flagsmith,remote,config Author:
 Flagsmith Author-email: support@flagsmith.com Requires-Python: >=3.7.0,<4
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: flagsmith-
```


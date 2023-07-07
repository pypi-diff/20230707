# Comparing `tmp/lifeguard-1.2.0.tar.gz` & `tmp/lifeguard-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-1.2.0.tar", last modified: Tue Jun 13 13:06:43 2023, max compression
+gzip compressed data, was "lifeguard-1.3.0.tar", last modified: Fri Jul  7 16:48:55 2023, max compression
```

## Comparing `lifeguard-1.2.0.tar` & `lifeguard-1.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.089350 lifeguard-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-13 13:06:43.089350 lifeguard-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-13 13:06:33.000000 lifeguard-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-13 13:06:33.000000 lifeguard-1.2.0/bin/lifeguard
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/controllers/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 13:06:43.089350 lifeguard-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 13:06:33.000000 lifeguard-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/tests/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/controllers/test_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.089350 lifeguard-1.2.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-07 16:48:55.952991 lifeguard-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-07 16:48:43.000000 lifeguard-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-07-07 16:48:43.000000 lifeguard-1.3.0/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/controllers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-07 16:48:43.000000 lifeguard-1.3.0/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.948991 lifeguard-1.3.0/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 16:48:55.000000 lifeguard-1.3.0/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-07 16:48:55.952991 lifeguard-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 16:48:43.000000 lifeguard-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/controllers/test_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:55.952991 lifeguard-1.3.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-07 16:48:43.000000 lifeguard-1.3.0/tests/test_validations.py
```

### Comparing `lifeguard-1.2.0/PKG-INFO` & `lifeguard-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.2.0
+Version: 1.3.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `lifeguard-1.2.0/README.md` & `lifeguard-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/bin/lifeguard` & `lifeguard-1.3.0/bin/lifeguard`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/__init__.py` & `lifeguard-1.3.0/lifeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/actions/email.py` & `lifeguard-1.3.0/lifeguard/actions/email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/actions/notifications.py` & `lifeguard-1.3.0/lifeguard/actions/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/auth.py` & `lifeguard-1.3.0/lifeguard/auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/context.py` & `lifeguard-1.3.0/lifeguard/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/controllers/__init__.py` & `lifeguard-1.3.0/lifeguard/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/controllers/assets.py` & `lifeguard-1.3.0/lifeguard/controllers/assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/http_client.py` & `lifeguard-1.3.0/lifeguard/http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/logger.py` & `lifeguard-1.3.0/lifeguard/logger.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/notifications.py` & `lifeguard-1.3.0/lifeguard/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/repositories.py` & `lifeguard-1.3.0/lifeguard/repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/scheduler.py` & `lifeguard-1.3.0/lifeguard/scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/server.py` & `lifeguard-1.3.0/lifeguard/server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/settings.py` & `lifeguard-1.3.0/lifeguard/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/lifeguard/validations.py` & `lifeguard-1.3.0/lifeguard/validations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
+import yaml
 import sys
 import traceback
+from os.path import join
 from json import JSONEncoder
 from functools import wraps
 
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.settings import (
     LIFEGUARD_DIRECTORY,
     LIFEGUARD_RUN_ONLY_VALIDATIONS,
@@ -22,14 +24,59 @@
             "executing action %s with result %s...",
             str(action.__name__),
             str(result),
         )
         action(result, settings)
 
 
+def __load_function_from_module(module_name_with_function_name):
+    module_path, function_name = module_name_with_function_name.rsplit(".", 1)
+
+    function = __import__(module_path)
+
+    module_path = module_path.split(".")
+    for module in module_path[1:]:
+        function = getattr(function, module)
+
+    return getattr(function, function_name)
+
+
+def __build_validation_function(command_function, args):
+    def validation_function():
+        command = __load_function_from_module(command_function)
+        return command(args)
+
+    return validation_function
+
+
+def __build_validation_from_settings(validation_yaml_file):
+    with open(validation_yaml_file) as file:
+        validation_list_from_file = yaml.load(file, Loader=yaml.FullLoader)
+
+    for validation_settings in validation_list_from_file["validations"]:
+        logger.info(
+            "loading validation %s from yaml file",
+            validation_settings["validation_name"],
+        )
+        validation_settings["actions"] = [
+            __load_function_from_module(action)
+            for action in validation_settings["actions"]
+        ]
+
+        command_settings = validation_settings.pop("execute")
+
+        validation_function = __build_validation_function(
+            command_settings["command"], *command_settings["args"]
+        )
+
+        validation_function.__name__ = validation_settings.pop("validation_name")
+
+        validation(**validation_settings)(validation_function)
+
+
 class ValidationResponse:
     """
     Represents the result of a validation
     """
 
     def __init__(
         self, status, details, settings=None, last_execution=None, validation_name=None
@@ -129,26 +176,29 @@
 
 
 def load_validations():
     """
     Load validations from application path
     """
     for root, _dirs, files in os.walk(os.path.join(LIFEGUARD_DIRECTORY, "validations")):
-        root = os.path.relpath(root, os.path.join(LIFEGUARD_DIRECTORY))
+        relative_path = os.path.relpath(root, os.path.join(LIFEGUARD_DIRECTORY))
         for validation_file in files:
             if validation_file.endswith("_validation.py"):
                 validation_module_name = (
-                    f'{build_import(root, validation_file.replace(".py", ""))}'
+                    f'{build_import(relative_path, validation_file.replace(".py", ""))}'
                 )
                 logger.info("loading validation %s", validation_file.replace(".py", ""))
 
                 module = "%s" % (validation_module_name)
                 if module not in sys.modules:
                     __import__(module)
 
+            if validation_file.endswith("_validation.yaml"):
+                __build_validation_from_settings(join(root, validation_file))
+
 
 def validation(
     description=None, actions=None, schedule=None, settings=None, actions_on_error=None
 ):
     """
     Decorator to configure a validation
     """
@@ -185,28 +235,31 @@
             except Exception as exception:
                 logger.error(
                     "validation error %s: %s",
                     str(decorated.__name__),
                     str(exception),
                     extra={"traceback": traceback.format_exc()},
                 )
+                validation_response_error = ValidationResponse(
+                    PROBLEM,
+                    {
+                        "exception": str(exception),
+                        "traceback": traceback.format_exc(),
+                        "use_error_template": True,
+                    },
+                    validation_name=decorated.__name__,
+                )
                 __execute_actions(
                     actions_on_error,
-                    ValidationResponse(
-                        PROBLEM,
-                        {
-                            "exception": str(exception),
-                            "traceback": traceback.format_exc(),
-                            "use_error_template": True,
-                        },
-                        validation_name=decorated.__name__,
-                    ),
+                    validation_response_error,
                     settings,
                 )
 
+                return validation_response_error
+
         VALIDATIONS[decorated.__name__] = {
             "ref": wrapped,
             "description": description,
             "actions": actions,
             "schedule": schedule,
             "settings": settings,
         }
```

### Comparing `lifeguard-1.2.0/lifeguard.egg-info/PKG-INFO` & `lifeguard-1.3.0/lifeguard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.2.0
+Version: 1.3.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `lifeguard-1.2.0/lifeguard.egg-info/SOURCES.txt` & `lifeguard-1.3.0/lifeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/setup.py` & `lifeguard-1.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard",
-    version="1.2.0",
+    version="1.3.0",
     url="https://github.com/LifeguardSystem/lifeguard",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=["bin/lifeguard"],
     include_package_data=True,
     description="Application to monitor your systems and give you the security to sleep peacefully at night",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["flask", "schedule", "gunicorn", "requests", "tabulate"],
+    install_requires=[
+        "flask",
+        "schedule",
+        "gunicorn",
+        "requests",
+        "tabulate",
+        "PyYAML",
+    ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: System :: Monitoring",
```

### Comparing `lifeguard-1.2.0/tests/actions/test_database.py` & `lifeguard-1.3.0/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/actions/test_email.py` & `lifeguard-1.3.0/tests/actions/test_email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/actions/test_notification.py` & `lifeguard-1.3.0/tests/actions/test_notification.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/controllers/test_assets.py` & `lifeguard-1.3.0/tests/controllers/test_assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_auth.py` & `lifeguard-1.3.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_bootstrap.py` & `lifeguard-1.3.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_controllers.py` & `lifeguard-1.3.0/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_http_client.py` & `lifeguard-1.3.0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_lifeguard_core.py` & `lifeguard-1.3.0/tests/test_lifeguard_core.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_notifications.py` & `lifeguard-1.3.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_repositories.py` & `lifeguard-1.3.0/tests/test_repositories.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_scheduler.py` & `lifeguard-1.3.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_server.py` & `lifeguard-1.3.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_settings.py` & `lifeguard-1.3.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.2.0/tests/test_validations.py` & `lifeguard-1.3.0/tests/test_validations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
-from unittest.mock import patch
+from unittest.mock import patch, call
 
-from lifeguard import NORMAL
+from lifeguard import NORMAL, PROBLEM
 from lifeguard.validations import (
     ValidationResponse,
     load_validations,
     VALIDATIONS,
 )
 
 from tests.fixtures.validations.simple_validation_with_action_on_errors import (
@@ -73,14 +73,41 @@
         mock_logger.info.assert_called_with(
             "executing action %s with result %s...",
             "simple_action",
             "{'validation_name': 'simple_with_action_validation', 'status': 'NORMAL', 'details': {}, 'settings': None}",
         )
 
     @patch("lifeguard.validations.LIFEGUARD_DIRECTORY", "tests/fixtures")
+    @patch("tests.fixtures.validations.shared.common_validation.logger")
+    def test_execute_validation_with_action_defined_from_yaml(self, mock_logger):
+        load_validations()
+        response = VALIDATIONS["simple_validation_with_action_in_yaml"]["ref"]()
+        self.assertEqual(response.status, NORMAL)
+        self.assertEqual(response.details, {"arg": "arg"})
+        self.assertEqual(
+            VALIDATIONS["simple_validation_with_action_in_yaml"]["settings"],
+            {"notification": {"update_thread_interval": 3600}},
+        )
+        self.assertEqual(
+            VALIDATIONS["simple_validation_with_action_in_yaml"]["schedule"],
+            {"every": {"minutes": 1}},
+        )
+        mock_logger.info.assert_has_calls(
+            [
+                call("common action executed"),
+            ]
+        )
+
+    @patch("lifeguard.validations.LIFEGUARD_DIRECTORY", "tests/fixtures")
+    def test_execute_validation_with_action_defined_from_yaml_when_error(self):
+        load_validations()
+        response = VALIDATIONS["simple_validation_with_error_in_yaml"]["ref"]()
+        self.assertEqual(response.status, PROBLEM)
+
+    @patch("lifeguard.validations.LIFEGUARD_DIRECTORY", "tests/fixtures")
     @patch(
         "lifeguard.validations.LIFEGUARD_RUN_ONLY_VALIDATIONS",
         ["simple_with_action_validation"],
     )
     @patch("lifeguard.validations.logger")
     def test_execute_validation_because_in_list(self, mock_logger):
         load_validations()
@@ -143,15 +170,15 @@
         result = VALIDATIONS["simple_with_invalid_action_validation"]["ref"]()
         mock_logger.error.assert_called_with(
             "validation error %s: %s",
             "simple_with_invalid_action_validation",
             "invalid_action() takes 0 positional arguments but 2 were given",
             extra={"traceback": "traceback"},
         )
-        self.assertIsNone(result)
+        self.assertEqual(result.status, PROBLEM)
 
     @patch("lifeguard.validations.LIFEGUARD_DIRECTORY", "tests/fixtures")
     @patch("lifeguard.validations.logger")
     @patch("lifeguard.validations.traceback")
     def test_execute_validation_with_error_and_error_actions(
         self, mock_traceback, mock_logger
     ):
```


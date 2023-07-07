# Comparing `tmp/fabman-1.2.10.tar.gz` & `tmp/fabman-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabman-1.2.10.tar", last modified: Fri Jul  7 19:55:54 2023, max compression
+gzip compressed data, was "fabman-1.2.9.tar", last modified: Fri Jul  7 19:24:40 2023, max compression
```

## Comparing `fabman-1.2.10.tar` & `fabman-1.2.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:55:54.122261 fabman-1.2.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 19:55:44.000000 fabman-1.2.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-07 19:55:54.122261 fabman-1.2.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-07 19:55:44.000000 fabman-1.2.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:55:54.118261 fabman-1.2.10/fabman/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/deleted_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/embedded_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25890 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/fabman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/fabman_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    27464 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/resource_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/training_course.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-07 19:55:44.000000 fabman-1.2.10/fabman/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:55:54.118261 fabman-1.2.10/fabman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-07 19:55:54.000000 fabman-1.2.10/fabman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-07 19:55:54.000000 fabman-1.2.10/fabman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:55:54.000000 fabman-1.2.10/fabman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 19:55:54.000000 fabman-1.2.10/fabman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 19:55:54.000000 fabman-1.2.10/fabman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-07 19:55:44.000000 fabman-1.2.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 19:55:54.122261 fabman-1.2.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 19:55:44.000000 fabman-1.2.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:55:54.122261 fabman-1.2.10/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_embedded_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_fabman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_resource_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_training_course.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-07 19:55:44.000000 fabman-1.2.10/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:24:40.027936 fabman-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 19:24:27.000000 fabman-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-07 19:24:40.027936 fabman-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-07 19:24:27.000000 fabman-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:24:40.023936 fabman-1.2.9/fabman/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/deleted_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/embedded_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25890 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/fabman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/fabman_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27053 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/resource_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/training_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-07 19:24:27.000000 fabman-1.2.9/fabman/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:24:40.023936 fabman-1.2.9/fabman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-07 19:24:40.000000 fabman-1.2.9/fabman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-07 19:24:40.000000 fabman-1.2.9/fabman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:24:40.000000 fabman-1.2.9/fabman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 19:24:40.000000 fabman-1.2.9/fabman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 19:24:40.000000 fabman-1.2.9/fabman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-07 19:24:27.000000 fabman-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 19:24:40.027936 fabman-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 19:24:27.000000 fabman-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:24:40.027936 fabman-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_embedded_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_fabman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_resource_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_training_course.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-07 19:24:27.000000 fabman-1.2.9/tests/test_webhook.py
```

### Comparing `fabman-1.2.10/LICENSE` & `fabman-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/PKG-INFO` & `fabman-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fabman
-Version: 1.2.10
+Version: 1.2.9
 Summary: Python wrappers for interacting with the Fabman API
 Author: Davin Lawrence
-Author-email: Davin Lawrence <davin.lawrence@utexas.edu>, Texas Inventionworks <tiw@utexas.edu>
+Author-email: Davin Lawrence <davin.lawrence@utexas.edu>
 Project-URL: Homepage, https://github.com/utexas-engr-tiw/fabman-api
 Project-URL: Documentation, https://fabman-api.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/utexas-engr-tiw/fabman-api/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `fabman-1.2.10/README.md` & `fabman-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/account.py` & `fabman-1.2.9/fabman/account.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/api_key.py` & `fabman-1.2.9/fabman/api_key.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/booking.py` & `fabman-1.2.9/fabman/booking.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/charge.py` & `fabman-1.2.9/fabman/charge.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/embedded_list.py` & `fabman-1.2.9/fabman/embedded_list.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/exceptions.py` & `fabman-1.2.9/fabman/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/fabman.py` & `fabman-1.2.9/fabman/fabman.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/fabman_object.py` & `fabman-1.2.9/fabman/fabman_object.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/invoice.py` & `fabman-1.2.9/fabman/invoice.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/member.py` & `fabman-1.2.9/fabman/member.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,27 +367,14 @@
 
         response = self._requester.request(
             "POST", f"/members/{self.id}/key", _kwargs=kwargs
         )
 
         return MemberKey(self._requester, response.json())
 
-    def create_training(self, **kwargs) -> MemberTraining:
-        """Creates a Training object which links a member to a training course.
-
-        :return: MemberTraining object
-        :rtype: MemberTraining
-        """
-
-        response = self._requester.request(
-            "POST", f"/members/{self.id}/trainings", _kwargs=kwargs
-        )
-
-        return MemberTraining(self._requester, response.json())
-
     def delete(self, **kwargs) -> requests.Response:
         """
         Deletes a member
         
         :calls: "DELETE /members/{id}" \
 		<https://fabman.io/api/v1/documentation#/members/deleteMembersId>
```

### Comparing `fabman-1.2.10/fabman/package.py` & `fabman-1.2.9/fabman/package.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/paginated_list.py` & `fabman-1.2.9/fabman/paginated_list.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/payment.py` & `fabman-1.2.9/fabman/payment.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/requester.py` & `fabman-1.2.9/fabman/requester.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/resource.py` & `fabman-1.2.9/fabman/resource.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/resource_log.py` & `fabman-1.2.9/fabman/resource_log.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/resource_type.py` & `fabman-1.2.9/fabman/resource_type.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/space.py` & `fabman-1.2.9/fabman/space.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/training_course.py` & `fabman-1.2.9/fabman/training_course.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/util.py` & `fabman-1.2.9/fabman/util.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman/webhook.py` & `fabman-1.2.9/fabman/webhook.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/fabman.egg-info/PKG-INFO` & `fabman-1.2.9/fabman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fabman
-Version: 1.2.10
+Version: 1.2.9
 Summary: Python wrappers for interacting with the Fabman API
 Author: Davin Lawrence
-Author-email: Davin Lawrence <davin.lawrence@utexas.edu>, Texas Inventionworks <tiw@utexas.edu>
+Author-email: Davin Lawrence <davin.lawrence@utexas.edu>
 Project-URL: Homepage, https://github.com/utexas-engr-tiw/fabman-api
 Project-URL: Documentation, https://fabman-api.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/utexas-engr-tiw/fabman-api/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `fabman-1.2.10/fabman.egg-info/SOURCES.txt` & `fabman-1.2.9/fabman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/pyproject.toml` & `fabman-1.2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel>=0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fabman"
-version = "1.2.10"
+version = "1.2.9"
 authors = [
     {name = "Davin Lawrence", email="davin.lawrence@utexas.edu"},
-    {name = "Texas Inventionworks", email="tiw@utexas.edu"}
 ]
 dependencies = [
     "requests>=2.31.0",
     "arrow>=1.2.3",
     "pytz==2023.3"
 ]
 description = "Python wrappers for interacting with the Fabman API"
```

### Comparing `fabman-1.2.10/setup.py` & `fabman-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_account.py` & `fabman-1.2.9/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_api_key.py` & `fabman-1.2.9/tests/test_api_key.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_booking.py` & `fabman-1.2.9/tests/test_booking.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_charge.py` & `fabman-1.2.9/tests/test_charge.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_embedded_list.py` & `fabman-1.2.9/tests/test_embedded_list.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_fabman.py` & `fabman-1.2.9/tests/test_fabman.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_invoice.py` & `fabman-1.2.9/tests/test_invoice.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_job.py` & `fabman-1.2.9/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_member.py` & `fabman-1.2.9/tests/test_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,14 @@
         register_uris({"member": ["create_key"]}, m)
 
         key = self.member.create_key(type="em4102", token="12345678")
         self.assertIsInstance(key, MemberKey)
         self.assertTrue(hasattr(key, "type"))
         self.assertTrue(key.type == "em4102")
 
-    def test_create_training(self, m):
-        register_uris({"member": ["create_training"]}, m)
-
-        training = self.member.create_training(account="1", training_course="1")
-        self.assertIsInstance(training, MemberTraining)
-        self.assertTrue(hasattr(training, "id"))
-
     def test_delete(self, m):
         register_uris({"member": ["delete"]}, m)
 
         resp = self.member.delete()
         self.assertTrue(m.called)
         self.assertTrue(resp.status_code == 204)
```

### Comparing `fabman-1.2.10/tests/test_package.py` & `fabman-1.2.9/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_paginated_list.py` & `fabman-1.2.9/tests/test_paginated_list.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_payment.py` & `fabman-1.2.9/tests/test_payment.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_requester.py` & `fabman-1.2.9/tests/test_requester.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_resource.py` & `fabman-1.2.9/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_resource_log.py` & `fabman-1.2.9/tests/test_resource_log.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_resource_type.py` & `fabman-1.2.9/tests/test_resource_type.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_sanity.py` & `fabman-1.2.9/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_space.py` & `fabman-1.2.9/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_training_course.py` & `fabman-1.2.9/tests/test_training_course.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_util.py` & `fabman-1.2.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `fabman-1.2.10/tests/test_webhook.py` & `fabman-1.2.9/tests/test_webhook.py`

 * *Files identical despite different names*


# Comparing `tmp/fabman-1.1.20.tar.gz` & `tmp/fabman-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabman-1.1.20.tar", last modified: Fri Jun 30 23:11:11 2023, max compression
+gzip compressed data, was "fabman-1.2.9.tar", last modified: Fri Jul  7 19:24:40 2023, max compression
```

## Comparing `fabman-1.1.20.tar` & `fabman-1.2.9.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.561270 fabman-1.1.20/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-30 23:10:59.000000 fabman-1.1.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-30 23:11:11.561270 fabman-1.1.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-30 23:10:59.000000 fabman-1.1.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.557270 fabman-1.1.20/fabman/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25890 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/fabman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/fabman_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    23297 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/resource_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/training_course.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-30 23:10:59.000000 fabman-1.1.20/fabman/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.557270 fabman-1.1.20/fabman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 23:11:11.000000 fabman-1.1.20/fabman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-30 23:10:59.000000 fabman-1.1.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-30 23:11:11.561270 fabman-1.1.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-30 23:10:59.000000 fabman-1.1.20/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 23:11:11.561270 fabman-1.1.20/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_fabman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14450 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_resource_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_training_course.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-30 23:10:59.000000 fabman-1.1.20/tests/test_webhook.py
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

### Comparing `fabman-1.1.20/LICENSE` & `fabman-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/PKG-INFO` & `fabman-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabman
-Version: 1.1.20
+Version: 1.2.9
 Summary: Python wrappers for interacting with the Fabman API
 Author: Davin Lawrence
 Author-email: Davin Lawrence <davin.lawrence@utexas.edu>
 Project-URL: Homepage, https://github.com/utexas-engr-tiw/fabman-api
 Project-URL: Documentation, https://fabman-api.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/utexas-engr-tiw/fabman-api/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fabman-1.1.20/README.md` & `fabman-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/account.py` & `fabman-1.2.9/fabman/account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Defines the Account object"""
 
-import requests
-
 from fabman.fabman_object import FabmanObject
 
 
+class PaymentInfo(FabmanObject):
+    """Holds PaymentInfo as returned from the accounts endpoint."""
+
+    def __str__(self):
+        return f"PaymentInfo for Account #{self.account_id}: {self.paymentMethod}"
+
+
 class Account(FabmanObject):
     """Handles Account objects from the Fabman API. In most cases, this only
     returns information about the API key holders account. Since most API endpoints
     in this object require superuser privileges, they are not implemented.
     """
 
     def __str__(self):
@@ -32,22 +37,24 @@
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
-    def get_payment_info(self, **kwargs) -> requests.Response:
+    def get_payment_info(self, **kwargs) -> PaymentInfo:
         """
         Get information about the payment plan of the account.
 
         :calls: "GET /accounts/{id}/payment-info" \
         <https://fabman.io/api/v1/documentation#/accounts/getAccountsIdPaymentinfo>
         
         :returns: Information about the payment plan of the account.
-        :rtype: dict
+        :rtype: fabman.account.PaymentInfo
         """
         uri = f"/accounts/{self.id}/payment-info"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
+        data = response.json()
+        data.update({"account_id": self.id})
 
-        return response.json()
+        return PaymentInfo(self._requester, data)
```

### Comparing `fabman-1.1.20/fabman/api_key.py` & `fabman-1.2.9/fabman/api_key.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Defines the ApiKey class"""
 
 import requests
 
 from fabman.fabman_object import FabmanObject
 
 
+class ApiKeyToken(FabmanObject):
+    """Simple Class to hold the token for an api-key"""
+
+    def __str__(self):
+        return f"ApiKeyToken #{self.api_key_id}: {self.token}"
+
+
 class ApiKey(FabmanObject):
     """
     Class for interacting with the api-keys endpoints on the Fabman API
     """
 
     def __str__(self):
         return f"ApiKey #{self.id}: {self.label}"
@@ -26,30 +33,33 @@
 
         uri = f"/api-keys/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
-    def get_token(self, **kwargs) -> requests.Response:
+    def get_token(self, **kwargs) -> ApiKeyToken:
         """
         Returns the token for an api-key. Must be called with a valid api-key.
 
         :calls: "GET /api-keys/{apiKeyId}/token" \
 		<https://fabman.io/api/v1/documentation#/api-keys/getApiKeysIdToken>
   
         :returns: Response from the API with status code 200 (OK) if successful
         :rtype: requests.Response
         """
 
         uri = f"/api-keys/{self.id}/token"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
+        data = response.json()
+
+        data.update({"api_key_id": self.id})
 
-        return response.json()
+        return ApiKeyToken(self._requester, data)
 
     def update(self, **kwargs) -> None:
         """
         Updates the api-key. Attributes are updated in place with new information
         returned by the API.
 
         :calls: "PUT /api-keys/{apiKeyId}" \
```

### Comparing `fabman-1.1.20/fabman/booking.py` & `fabman-1.2.9/fabman/booking.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/charge.py` & `fabman-1.2.9/fabman/charge.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/exceptions.py` & `fabman-1.2.9/fabman/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/fabman.py` & `fabman-1.2.9/fabman/fabman.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/fabman_object.py` & `fabman-1.2.9/fabman/fabman_object.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/invoice.py` & `fabman-1.2.9/fabman/invoice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Define the Invoice Object"""
 
 import requests
 
 from fabman.fabman_object import FabmanObject
 
 
+class InvoiceDetails(FabmanObject):
+    """Simple Class to handle Invoice Details"""
+
+    def __str__(self):
+        return f"Invoice #{self.id}: {self.totalExcludingTax} # Charges: {len(self.charges)}"
+
+
 class Invoice(FabmanObject):
     """Simple Class to handle Invoices"""
 
     def __str__(self):
         return f"Invoice #{self.id}: {self.total} {self.state}"
 
     def cancel(self) -> requests.Response:
@@ -25,35 +32,37 @@
         data = {"lockVersion": self.lockVersion}
 
         uri = f"/invoices/{self.id}/cancel"
         response = self._requester.request("POST", uri, _kwargs=data)
 
         return response.json()
 
-    def details(self, **kwargs) -> requests.Response:
+    def details(self, **kwargs) -> InvoiceDetails:
         """
         Returns details about the invoice. Takes no arguments.
 
         :calls: "GET /invoices/{id}/details" \
 		<https://fabman.io/api/v1/documentation>
   
         :returns: A dict containing details about the invoice.
         :rtype: dict
         """
 
         if "details" in self._embedded:
-            return self._embedded["details"]
+            self._embedded["details"].update({"invoice_id": self.id})
+            return InvoiceDetails(self._requester, self._embedded["details"])
 
         uri = f"/invoices/{self.id}/details"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
-
+        data = response.json()
         self._embedded["details"] = response.json()
 
-        return response.json()
+        data.update({"invoice_id": self.id})
+        return InvoiceDetails(self._requester, data)
 
     def update(self, **kwargs) -> None:
         """
         Updates the invoice. Attributes are updated in place with new information
         provided by the API
 
         :calls: "PUT /invoices/{id}" \
```

### Comparing `fabman-1.1.20/fabman/member.py` & `fabman-1.2.9/fabman/member.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,55 @@
 """Defines and handles the Member object returned by the API"""
 # pylint: disable=too-many-public-methods, line-too-long
-from typing import Union
+from typing import List, Optional, Union
 
 import requests
 
+from fabman.embedded_list import EmbeddedList
 from fabman.fabman_object import FabmanObject
 from fabman.package import Package
 from fabman.paginated_list import PaginatedList
 
 
+class MemberBalanceItems(FabmanObject):
+    """Simple Class to handle Member Balance Items"""
+
+
+class MemberChange(FabmanObject):
+    """Simple class to hold Member Changes"""
+
+    def __str__(self):
+        return f"Change #{self.id} for member #{self.member_id}"
+
+    def delete(self, **kwargs) -> requests.Response:
+        """
+        Deletes a member change given change ID
+        
+        :calls: "DELETE /members/{id}/changes/{changeId}" \
+        <https://fabman.io/api/v1/documentation#/members/deleteMembersIdChangesChangeid>
+        
+        :return: Response information of delete call
+        :rtype: requests.Response
+        """
+
+        return self._requester.request(
+            "DELETE", f"/members/{self.member_id}/changes/{self.id}", _kwargs=kwargs
+        )
+
+
+class MemberCreditUse(FabmanObject):
+    """
+    Simple class to hold Credit Use
+    """
+
+    def __str__(self):
+        # TODO: Test this method. No current way of applying credits with account available to developers
+        return f"{self.id}: {self.amount} - {self.description}"
+
+
 class MemberCredit(FabmanObject):
     """
     Simple Class to handle operations on MemberCredits
     """
 
     def __str__(self):
         return f"{self.id}: {self.scope} - {self.amount}"
@@ -29,29 +66,30 @@
         """
         response = self._requester.request(
             "DELETE", f"/members/{self.member_id}/credits/{self.id}", _kwargs=kwargs
         )
 
         return response
 
-    def get_uses(self, **kwargs) -> requests.Response:
+    def get_uses(self, **kwargs) -> List[MemberCreditUse]:
         """
         Retrieves a list of uses of the credit.
 
         :calls: "GET /members/{member_id}/credits/{credit_id}/uses" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdCreditsCreditidUses>
   
         :return: A list of uses of the credit.
         :rtype: list
         """
         response = self._requester.request(
             "GET", f"/members/{self.member_id}/credits/{self.id}/uses", _kwargs=kwargs
         )
 
-        return response.json()
+        data = response.json()
+        return [MemberCreditUse(self._requester, use) for use in data]
 
     def update(self, **kwargs) -> None:
         """
         Updates an existing credit in place
 
         :calls: "PUT /members/{id}/credits/{creditId}" \
 		<https://fabman.io/api/v1/documentation#/members/putMembersIdCreditsCreditid>
@@ -66,14 +104,48 @@
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
 
+class MemberDevice(FabmanObject):
+    """Simple Class to represent a Member Device"""
+
+    def __str__(self):
+        return f"Device: {self.name}"
+
+
+class MemberDeviceChange(FabmanObject):
+    """Simple class to represent a Member Device Change"""
+
+    def __str__(self) -> str:
+        return f"DeviceChange #{self.id} for member #{self.member_id}"
+
+    def delete(self, **kwargs) -> requests.Response:
+        """
+        Deletes a member device change given change ID
+        
+        :calls: "DELETE /members/{id}/device/changes/{changeId}" \
+        <https://fabman.io/api/v1/documentation#/members/deleteMembersIdDeviceChangesChangeid>
+        
+        :returns: Response information of delete call
+        :rtype: requests.Response
+        """
+        return self._requester.request(
+            "DELETE",
+            f"/members/{self.member_id}/device/changes/{self.id}",
+            _kwargs=kwargs,
+        )
+
+
+class MemberInvitation(FabmanObject):
+    """Simple class to represent a MemberInvitation"""
+
+
 class MemberKey(FabmanObject):
     """
     Manage a member keycard object
     """
 
     def __str__(self):
         return f"{self.member} - {self.type}"
@@ -181,14 +253,78 @@
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
 
+class MemberPaymentAccount(FabmanObject):
+    """Simple object to hold Member Payment Accounts"""
+
+
+class MemberPaymentMethod(FabmanObject):
+    """Simple object to hold Member Payment Methods"""
+
+    def __str__(self):
+        return f"Member #{self.member_id} has a {self.type} payment method"
+
+    def delete(self, **kwargs):
+        """Deletes a member payment method
+        
+        :calls: "DELETE /members/{id}/payment-method" \
+        <https://fabman.io/api/v1/documentation#/members/deleteMembersIdPaymentmethod>
+        
+        :return: Response information of the delete call
+        :rtype: requests.Response
+        """
+
+        return self._requester.request(
+            "DELETE", f"/members/{self.member_id}/payment-method", _kwargs=kwargs
+        )
+
+
+class MemberPaymentMethodMandatePreview(FabmanObject):
+    """Simple object to hold Member Payment Method Mandate Previews"""
+
+
+class MemberPrivileges(FabmanObject):
+    """Simple object to hold Member Privileges"""
+
+    def __str__(self):
+        return f"Member #{self.member_id} is {self.privileges}"
+
+
+class MemberTrainedResources(FabmanObject):
+    """Simple object to hold Member Trained Resources"""
+
+    def __str__(self):
+        return f"Member #{self.member_id} is trained on {len(self.resources)} resources"
+
+
+class MemberTraining(FabmanObject):
+    """Simple object to handle Member Trainings"""
+
+    def __str__(self):
+        return f"MemberTraining #{self.id} for member #{self.member_id}"
+
+    def delete(self, **kwargs):
+        """Deletes a member training
+
+        :calls: "DELETE /members/{id}/trainings/{trainingId}" \
+        <https://fabman.io/api/v1/documentation#/members/deleteMembersIdTrainingsTrainingid>
+        
+        :return: Response Information of delete call
+        :rtype: requests.Response
+        """
+
+        return self._requester.request(
+            "DELETE", f"/members/{self.member_id}/trainings/{self.id}", _kwargs=kwargs
+        )
+
+
 class Member(FabmanObject):
     """
     Member object returned by the API. Provides access to all API calls that operate on a single member.
     """
 
     def __str__(self):
         return f"{self.id}: {self.firstName} {self.lastName}"
@@ -247,119 +383,55 @@
         """
         return self._requester.request(
             "DELETE",
             f"/members/{self.id}",
             _kwargs=kwargs,
         )
 
-    def delete_change(self, change_id: int, **kwargs) -> requests.Response:
-        """
-        Deletes a member change given change ID
-        
-        :calls: "DELETE /members/{id}/changes/{changeId}" \
-		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdChangesChangeid>
-
-        :param change_id: ID of the change to delete
-        :type change_id: int
-        :return: Response information of delete call
-        :rtype: requests.Response
-        """
-        return self._requester.request(
-            "DELETE",
-            f"/members/{self.id}/changes/{change_id}",
-            _kwargs=kwargs,
-        )
-
-    def delete_device_change(self, change_id: int, **kwargs) -> requests.Response:
-        """
-        Deletes a member device change given change ID
-        
-        :calls: "DELETE /members/{id}/device/changes/{changeId}" \
-		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdDeviceChangesChangeid>
-
-        :param change_id: ID of the change to delete
-        :type change_id: int
-        :returns: Response information of delete call
-        :rtype: requests.Response
-        """
-        return self._requester.request(
-            "DELETE",
-            f"/members/{self.id}/device/changes/{change_id}",
-            _kwargs=kwargs,
-        )
-
-    def delete_payment_method(self, **kwargs) -> requests.Response:
-        """
-        Deletes a member payment method
-        
-        :calls: "DELETE /members/{id}/payment-method" \
-		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdPaymentmethod>
-  
-        :returns: Response information of delete call
-        :rtype: requests.Response
-        """
-        return self._requester.request(
-            "DELETE",
-            f"/members/{self.id}/payment-method",
-            _kwargs=kwargs,
-        )
-
-    def delete_training(self, training_id: int, **kwargs) -> requests.Response:
-        """
-        Deletes a member training given training ID
-        
-        :calls: "DELETE /members/{id}/trainings/{trainingId}" \
-		<https://fabman.io/api/v1/documentation#/members/deleteMembersIdTrainingsTrainingid>
-
-        :param training_id: ID of the training to delete
-        :type training_id: int
-        :returns: Response information of delete call
-        :rtype: requests.Response
-        """
-        return self._requester.request(
-            "DELETE",
-            f"/members/{self.id}/trainings/{training_id}",
-            _kwargs=kwargs,
-        )
-
-    def get_balance_items(self, **kwargs) -> requests.Response:
+    def get_balance_items(self, **kwargs) -> MemberBalanceItems:
         """
         Retrieves the balance items of a member
         
         :calls: "GET /members/{id}/balance-items" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdBalanceitems>
   
         :returns: Response information of get call
-        :rtype: requests.Response
+        :rtype: MemberBalanceItems
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/balance-items",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = response.json()
+        data.update({"member_id": self.id})
+
+        return MemberBalanceItems(self._requester, data)
 
-    def get_changes(self, **kwargs) -> requests.Response:
+    def get_changes(self, **kwargs) -> List[MemberChange]:
         """
         Retrieves the changes of a member
         
         :calls: "GET /members/{id}/changes" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdChanges>
   
         :returns: List of changes of a member
-        :rtype: list
+        :rtype: list[MemberChange]
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/changes",
             _kwargs=kwargs,
         )
+        data = response.json()
+        for change in data:
+            change.update({"member_id": self.id})
 
-        return response.json()
+        return [MemberChange(self._requester, x) for x in data]
 
     def get_credits(self, **kwargs) -> PaginatedList:
         """
         Retrieves the credits of a member
         :calls: "GET /members/{id}/credits" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdCredits>
   
@@ -394,54 +466,60 @@
         )
 
         data = response.json()
         data.update({"member_id": self.id})
 
         return MemberCredit(self._requester, data)
 
-    def get_device(self, **kwargs) -> requests.Response:
+    def get_device(self, **kwargs) -> MemberDevice:
         """
         Retrieves the device of a member used to authenticate on a bridge.
         
         :calls: "GET /members/{id}/devices" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdDevice>
   
         :returns: Device information
         :rtype: dict
         """
         if "device" in self._embedded:
-            return self._embedded["device"]
+            data = self._embedded["device"]
+        else:
+            response = self._requester.request(
+                "GET",
+                f"/members/{self.id}/device",
+                _kwargs=kwargs,
+            )
 
-        response = self._requester.request(
-            "GET",
-            f"/members/{self.id}/device",
-            _kwargs=kwargs,
-        )
+            data = response.json()
+        data.update({"member_id": self.id})
 
-        return response.json()
+        return MemberDevice(self._requester, data)
 
-    def get_device_changes(self, **kwargs) -> requests.Response:
+    def get_device_changes(self, **kwargs) -> List[MemberDeviceChange]:
         """
         Retrieves the device changes of a member
         
         :calls: "GET /members/{id}/device/changes" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdDeviceChanges>
 
         :returns: List of device changes of a member
-        :rtype: list
+        :rtype: list[MemberDeviceChange]
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/device/changes",
             _kwargs=kwargs,
         )
+        data = response.json()
+        for el in data:
+            el.update({"member_id": self.id})
 
-        return response.json()
+        return [MemberDeviceChange(self._requester, change) for change in data]
 
-    def get_device_change(self, change_id: int, **kwargs) -> requests.Response:
+    def get_device_change(self, change_id: int, **kwargs) -> MemberDeviceChange:
         """
         Retrieves a device change of a member given the change ID
         
         :calls: "GET /members/{id}/device/changes/{changeId}" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdDeviceChangesChangeId>
   
         :param change_id: ID of the change to retrieve
@@ -451,28 +529,31 @@
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/device/changes/{change_id}",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = response.json()
+        data.update({"member_id": self.id})
+
+        return MemberDeviceChange(self._requester, data)
 
     def get_export(self, **kwargs) -> requests.Response:
         """
         Retrieves the export of a member. This is a placeholder for future functionality.
         
         :calls: "GET /members/{id}/export" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdExport>
   
         :raises: NotImplementedError
         """
         raise NotImplementedError("get_export not implemented yet")
 
-    def get_invitation(self, **kwargs) -> requests.Response:
+    def get_invitation(self, **kwargs) -> MemberInvitation:
         """
         Retrieves the invitation status of a member
         
         :calls: "GET /members/{id}/invitations" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdInvitation>
   
         :returns: Invitation status of a member
@@ -480,53 +561,61 @@
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/invitation",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = response.json()
+        data.update({"member_id": self.id})
+
+        return MemberInvitation(self._requester, data)
 
     def get_key(self, **kwargs) -> MemberKey:
         """
         Retrieves the keycard number of a member
         
         :calls: "GET /members/{id}/key" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdKey>
   
         :returns: :code:`fabman.member.MemberKey` object with key details
         :rtype: fabman.member.MemberKey
         """
         if "key" in self._embedded:
-            return MemberKey(self._requester, self._embedded["key"])
-
-        response = self._requester.request(
-            "GET",
-            f"/members/{self.id}/key",
-            _kwargs=kwargs,
-        )
+            data = self._embedded["key"]
+        else:
+            response = self._requester.request(
+                "GET",
+                f"/members/{self.id}/key",
+                _kwargs=kwargs,
+            )
+            data = response.json()
+        data.update({"member_id": self.id})
 
-        return MemberKey(self._requester, response.json())
+        return MemberKey(self._requester, data)
 
-    def get_packages(self, **kwargs) -> Union[list, PaginatedList]:
+    def get_packages(self, **kwargs) -> Union[EmbeddedList, PaginatedList]:
         """
         Retrieves the packages of a member
 
         :calls: "GET /members/{id}/packages" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdPackages>
   
         :returns: List of packages of a member
         :rtype: fabman.paginated_list.PaginatedList
         """
         if "memberPackages" in self._embedded:
-            out = []
-            for package in self._embedded["memberPackages"]:
-                package.update({"member_id": self.id})
-                out.append(MemberPackage(self._requester, package))
-            return out
+            return EmbeddedList(
+                MemberPackage,
+                self._embedded["memberPackages"],
+                self._requester,
+                "GET",
+                f"/members/{self.id}/packages",
+                extra_attribs={"member_id": self.id},
+            )
 
         return PaginatedList(
             MemberPackage,
             self._requester,
             "GET",
             f"/members/{self.id}/packages",
             extra_attribs={"member_id": self.id},
@@ -541,31 +630,32 @@
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdPackagesMemberpackageid>
   
         :param member_package_id: ID of the package to retrieve
         :type member_package_id: int
         :returns: :code:`fabman.member.MemberPackage` object with package details
         :rtype: fabman.member.MemberPackage
         """
+        data = dict()
         if "memberPackages" in self._embedded:
             for package in self._embedded["memberPackages"]:
                 if package["id"] == member_package_id:
-                    return MemberPackage(self._requester, package)
-
-        response = self._requester.request(
-            "GET",
-            f"/members/{self.id}/packages/{member_package_id}",
-            _kwargs=kwargs,
-        )
+                    data = package
+        if len(data) == 0:
+            response = self._requester.request(
+                "GET",
+                f"/members/{self.id}/packages/{member_package_id}",
+                _kwargs=kwargs,
+            )
 
-        data = response.json()
+            data = response.json()
         data.update({"member_id": self.id})
 
         return MemberPackage(self._requester, data)
 
-    def get_payment_account(self, **kwargs) -> requests.Response:
+    def get_payment_account(self, **kwargs) -> MemberPaymentAccount:
         """
         Retrieves the payment account of a member
         
         :calls: "GET /members/{id}/payment-account" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentaccount>
   
         :returns: Payment account information
@@ -573,34 +663,42 @@
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/payment-account",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = {"payments": response.json()}
+        data.update({"member_id": self.id})
+
+        return MemberPaymentAccount(self._requester, data)
 
-    def get_payment_method(self, **kwargs) -> requests.Response:
+    def get_payment_method(self, **kwargs) -> MemberPaymentMethod:
         """
         Retrieves the payment method of a member
         :calls: "GET /members/{id}/payment-method" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentmethod>
   
         :returns: Payment method information
         :rtype: dict
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/payment-method",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = response.json()
+        data.update({"member_id": self.id})
 
-    def get_payment_method_mandate_preview(self, **kwargs) -> requests.Response:
+        return MemberPaymentMethod(self._requester, data)
+
+    def get_payment_method_mandate_preview(
+        self, **kwargs
+    ) -> MemberPaymentMethodMandatePreview:
         """
         Retrieves the payment method mandate preview of a member
         
         :calls: "GET /members/{id}/payment-method-mandate-preview" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdPaymentmethodmandatepreview>
   
         :returns: Payment method mandate preview information
@@ -608,99 +706,119 @@
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/payment-method-mandate-preview",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = response.json()
+        data.update({"member_id": self.id})
+
+        return MemberPaymentMethodMandatePreview(self._requester, data)
 
-    def get_privileges(self, **kwargs) -> requests.Response:
+    def get_privileges(self, **kwargs) -> MemberPrivileges:
         """
         Retrieves the privileges of a member
         :calls: "GET /members/{id}/privileges" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdPrivileges>
   
         :returns: privileges of a member
         :rtype: dict
         """
         if "privileges" in self._embedded:
-            return self._embedded["privileges"]
+            data = self._embedded["privileges"]
+        else:
+            response = self._requester.request(
+                "GET",
+                f"/members/{self.id}/privileges",
+                _kwargs=kwargs,
+            )
 
-        response = self._requester.request(
-            "GET",
-            f"/members/{self.id}/privileges",
-            _kwargs=kwargs,
-        )
+            data = response.json()
+        data.update({"member_id": self.id})
 
-        return response.json()
+        return MemberPrivileges(self._requester, data)
 
-    def get_trained_resources(self, **kwargs) -> requests.Response:
+    def get_trained_resources(self, **kwargs) -> MemberTrainedResources:
         """
         Retrieves the trained resources of a member
         :calls: "GET /members/{id}/trained-resources" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdTrainedResources>
   
         :return: Trained resources of a member
         :rtype: list
         """
         response = self._requester.request(
             "GET",
             f"/members/{self.id}/trained-resources",
             _kwargs=kwargs,
         )
 
-        return response.json()
+        data = {"resources": response.json()}
+        data.update({"member_id": self.id})
+
+        return MemberTrainedResources(self._requester, data)
 
-    def get_trainings(self, **kwargs) -> requests.Response:
+    def get_trainings(
+        self, ignore_embeds: Optional[bool] = False, **kwargs
+    ) -> Union[PaginatedList, EmbeddedList]:
         """
-        TODO: Move to MemberTrainings object
         
         Retrieves the trainings of a member
         :calls: "GET /members/{id}/trainings" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdTrainings>
 
         :return: List of trainings of a member
-        :rtype: list
+        :rtype: Union[PaginatedList, EmbeddedList]
         """
-        if "trainings" in self._embedded:
-            return self._embedded["trainings"]
+        if "trainings" in self._embedded and not ignore_embeds:
+            return EmbeddedList(
+                MemberTraining,
+                self._embedded["trainings"],
+                self._requester,
+                "GET",
+                f"/members/{self.id}/trainings",
+                extra_attribs={"member_id": self.id},
+            )
 
-        response = self._requester.request(
+        return PaginatedList(
+            MemberTraining,
+            self._requester,
             "GET",
             f"/members/{self.id}/trainings",
-            _kwargs=kwargs,
+            extra_attribs={"member_id": self.id},
         )
 
-        return response.json()
-
-    def get_training(self, training_id: int, **kwargs) -> requests.Response:
+    def get_training(self, training_id: int, **kwargs) -> MemberTraining:
         """
-        TODO: Move this to MemberTraining Object
         Retrieves a training of a member
         :calls: "GET /members/{id}/trainings/{trainingId}" \
 		<https://fabman.io/api/v1/documentation#/members/getMembersIdTrainingstrainingid>
         
         :param training_id: ID of the training to retrieve
         :type training_id: int
         :return: Training information
         :rtype: dict
         """
+        data = {}
         if "trainings" in self._embedded:
             for training in self._embedded["trainings"]:
                 if training["id"] == training_id:
-                    return training
+                    data = training
+        if len(data) == 0:
+            response = self._requester.request(
+                "GET",
+                f"/members/{self.id}/trainings/{training_id}",
+                _kwargs=kwargs,
+            )
 
-        response = self._requester.request(
-            "GET",
-            f"/members/{self.id}/trainings/{training_id}",
-            _kwargs=kwargs,
-        )
+            data = response.json()
+        data.update({"member_id": self.id})
 
-        return response.json()
+        return MemberTraining(self._requester, data)
 
     def refresh(self) -> None:
         """
         Updates the objects with more recent data from the API. Needs to be called
         when update() fails for lockVersioning.
 
         :calls: "GET /members/{id}" \
```

### Comparing `fabman-1.1.20/fabman/package.py` & `fabman-1.2.9/fabman/package.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/paginated_list.py` & `fabman-1.2.9/fabman/paginated_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Handles pagination of the api"""
-from typing import Optional, Type
+from typing import List, Optional, Type
 
 from requests.structures import CaseInsensitiveDict
 
 from fabman.fabman_object import FabmanObject
 from fabman.requester import Requester
 
 
@@ -20,26 +20,44 @@
         ), "Index must be an integer, slicing and keys are \
             not supported"
         if index < 0:
             raise IndexError("Cannot use negative indexing on PaginatedList")
         self._get_up_to_index(index)
         return self._elements[index]
 
-    def __init__(
-        self,  # pylint: disable=too-many-arguments
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
         content_class: Type[FabmanObject],
         requester: Requester,
         request_method: str,
         first_url: str,
         extra_attribs: Optional[dict] = None,
-        _root=None,
-        url_override=None,
+        _root: Optional[str] = None,
+        url_override: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """Initializes the PaginatedList class with the given parameters."""
+        """Abstracts pagination of the Fabman API. Provides a simple interface to work with
+        objects and requests new objects from the API as needed.
+
+        :param content_class: Class of the stored objects. Must inherit from FabmanObject
+        :type content_class: Type[fabman.fabman_object.FabmanObject]
+        :param requester: Requester for refreshing the API
+        :type requester: fabman.requester.Requester
+        :param request_method: One of "GET", "POST", "PUT", "DELETE"
+        :type request_method: str
+        :param first_url: endpoint to be called for the first page
+        :type first_url: str
+        :param extra_attribs: Extra attributes to be added to :code:`content_class`, defaults to None
+        :type extra_attribs: Optional[dict], optional
+        :param _root: Root endpoint without parameters, defaults to None
+        :type _root: str, optional
+        :param url_override: Override the base_url, defaults to None
+        :type url_override: str, optional
+        """
+
         self._elements = []
 
         self._content_class = content_class
         self._requester = requester
         self._first_url = first_url
         self._first_params = kwargs or {}
         self._next_url = first_url
```

### Comparing `fabman-1.1.20/fabman/payment.py` & `fabman-1.2.9/fabman/payment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """Defines the Payment object"""
 
 import requests
 
 from fabman.fabman_object import FabmanObject
 
 
+class PaymentRequest(FabmanObject):
+    """Simple class to hold payment request information"""
+
+    def __str__(self):
+        return f"PaymentRequest for Payment #{self.payment_id}"
+
+
 class Payment(FabmanObject):
     """Defines the Payment object for interacting with payments on the Fabman API"""
 
     def __str__(self) -> str:
         return f"Payment #{self.id}: {self.notes}"
 
     def delete(self, **kwargs) -> requests.Response:
@@ -23,29 +30,32 @@
         """
         uri = f"/payments/{self.id}"
 
         response = self._requester.request("DELETE", uri, _kwargs=kwargs)
 
         return response
 
-    def request_payment(self, **kwargs) -> requests.Response:
+    def request_payment(self, **kwargs) -> PaymentRequest:
         """
         Requests a payment from the customer.
 
         :calls: "POST /payments/{id}/request-payment" \
 		<https://fabman.io/api/v1/documentation#/payments/postPaymentsIdRequestpayment>
         
         :return: response information of the call
-        :rtype: requests.Response
+        :rtype: PaymentRequest
         """
         uri = f"/payments/{self.id}/request-payment"
 
         response = self._requester.request("POST", uri, _kwargs=kwargs)
 
-        return response
+        data = response.json()
+        data.update({"payment_id": self.id})
+
+        return PaymentRequest(self._requester, data)
 
     def update(self, **kwargs) -> None:
         """
         Updates a payment. Attributes are modified in place using updated information
         from the API.
 
         :calls: "PUT /payments/{id}" \
```

### Comparing `fabman-1.1.20/fabman/requester.py` & `fabman-1.2.9/fabman/requester.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/resource.py` & `fabman-1.2.9/fabman/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
 
+class ResourceBridgeApiKey(FabmanObject):
+    """Simple class to hold Bridge API key information"""
+
+    def __str__(self):
+        api_key = "xxxx" + self.apiKey[-4:]
+        return f"Resource #{self.resource_id}: {api_key}"
+
+
 class Resource(FabmanObject):
     """
     Resource object returned by the API. Provides access to all API calls that
     operate on a single Resource.
     """
 
     def __str__(self):
@@ -93,31 +101,34 @@
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"resource_id": self.id})
 
         return ResourceBridge(self._requester, data)
 
-    def get_bridge_api_key(self, **kwargs) -> requests.Response:
+    def get_bridge_api_key(self, **kwargs) -> ResourceBridgeApiKey:
         """
         Get the API key for the bridge that is currently connected to this resource.
         For most users, this will return a 204 code with an empty body. Only superusers
         or users who have created a custom bridge should be able to access this endpoint.
 
         :calls: "GET /resources/{id}/bridge/api-key" \
 		<https://fabman.io/api/v1/documentation#/resources/getResourcesIdBridgeApikey>
 
         :return: response information of call
-        :rtype: dict
+        :rtype: ResourceBridgeApiKey
         """
         uri = f"/resources/{self.id}/bridge/api-key"
 
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
-        return response.json()
+        data = response.json()
+        data.update({"resource_id": self.id})
+
+        return ResourceBridgeApiKey(self._requester, data)
 
     def switch_on(self, **kwargs) -> requests.Response:
         """
         Switch on the resource. Requires "code" field to be in the data packet.
         Does not seem to work without the proper code, which is undocumented.
 
         :calls: "POST /resources/{id}/switch-on" \
```

### Comparing `fabman-1.1.20/fabman/resource_log.py` & `fabman-1.2.9/fabman/resource_log.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/resource_type.py` & `fabman-1.2.9/fabman/resource_type.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/space.py` & `fabman-1.2.9/fabman/space.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Defines the Space class and other Space-related classes"""
 
 from typing import Union
 
 import requests
 
+from fabman.embedded_list import EmbeddedList
 from fabman.fabman_object import FabmanObject
 from fabman.paginated_list import PaginatedList
 
 
 class SpaceBillingSettings(FabmanObject):
     """Class for interacting with the space-billing-settings endpoint on the Fabman API"""
 
@@ -111,14 +112,26 @@
 
         data = response.json()
 
         for attr, val in data.items():
             setattr(self, attr, val)
 
 
+class SpaceOpeningHours(FabmanObject):
+    """Class for holding Opening Hours requests"""
+
+    def __str__(self):
+        out = f"Space #{self.space_id} Opening Hours:\n"
+        out += "+-----------------+-----------------+\n"
+        for day in self.days:
+            out += f"{day['dayOfWeek']}: {day['fromTime']} - {day['untilTime']}\n"
+
+        return out
+
+
 class Space(FabmanObject):
     """Class for interacting with the Space endpoint on the Fabman API"""
 
     def __str__(self):
         return f"Space #{self.id}: {self.name}"
 
     def create_holiday(self, **kwargs) -> SpaceHoliday:
@@ -214,60 +227,67 @@
         response = self._requester.request("GET", uri, _kwargs=kwargs)
 
         data = response.json()
         data.update({"space_id": self.id})
 
         return SpaceHoliday(self._requester, data)
 
-    def get_holidays(self, **kwargs) -> Union[list, PaginatedList]:
+    def get_holidays(self, **kwargs) -> Union[EmbeddedList, PaginatedList]:
         """
         Returns a list of holidays for the space. If the information is cached from an embedded call, 
         a list of SpaceHoliday objects is returned. Otherwise, a PaginatedList will be returned.
 
         :calls: "GET /spaces/{spaceId}/holidays" \
 		<https://fabman.io/api/v1/documentation#/spaces/getSpacesIdHolidays>
   
         :return: List of SpaceHoliday Objects
         :rtype: list[fabman.space.SpaceHoliday] or fabman.paginated_list.PaginatedList
         """
         if "holidays" in self._embedded:
             out = []
-            for holiday in self._embedded["holidays"]:
-                holiday.update({"space_id": self.id})
-                out.append(SpaceHoliday(self._requester, holiday))
-            return out
+            return EmbeddedList(
+                SpaceHoliday,
+                self._embedded["holidays"],
+                self._requester,
+                "GET",
+                f"/spaces/{self.id}/holidays",
+                extra_attribs={"space_id": self.id},
+                kwargs=kwargs,
+            )
 
         return PaginatedList(
             SpaceHoliday,
             self._requester,
             "GET",
             f"/spaces/{self.id}/holidays",
             extra_attribs={"space_id": self.id},
             kwargs=kwargs,
         )
 
-    def get_opening_hours(self, **kwargs) -> Union[list, requests.Response]:
+    def get_opening_hours(self, **kwargs) -> SpaceOpeningHours:
         """
         Get the opening hours for the space.
 
         :calls: "GET /spaces/{spaceId}/opening-hours" \
 		<https://fabman.io/api/v1/documentation#/spaces/getSpacesIdOpeninghours>
 
         :return: List of opening hours
         :rtype: list
         """
 
         if "openingHours" in self._embedded:
-            return self._embedded["openingHours"]
-
-        uri = f"/spaces/{self.id}/opening-hours"
+            data = {"days": self._embedded["openingHours"]}
+        else:
+            uri = f"/spaces/{self.id}/opening-hours"
 
-        response = self._requester.request("GET", uri, _kwargs=kwargs)
+            response = self._requester.request("GET", uri, _kwargs=kwargs)
+            data = {"days": response.json()}
 
-        return response
+        data.update({"space_id": self.id})
+        return SpaceOpeningHours(self._requester, data)
 
     def update(self, **kwargs) -> None:
         """
         Updates the space. Attributes are updated in place with new information
         from the API.
 
         :calls: "PUT /spaces/{spaceId}" \
@@ -308,28 +328,29 @@
 
         token = data["calendarUrl"].split("/")[-1].split(".")[0]
         setattr(self, "calendarToken", token)
         setattr(self, "calendarUrl", data["calendarUrl"])
 
         return response
 
-    def update_opening_hours(self, **kwargs) -> requests.Response:
+    def update_opening_hours(self, **kwargs) -> SpaceOpeningHours:
         """
         Updates the opening hours of a space. If the the openingHours key is
         present in the _embedded attribute, the opening hours are updated in
         place with information returned by the api.
 
         :calls: "PUT /spaces/{spaceId}/opening-hours" \
 		<https://fabman.io/api/v1/documentation#/spaces/putSpacesIdOpeninghours>
   
         :return: response information of call
-        :rtype: requests.Response
+        :rtype: SpaceOpeningHours
         """
 
         uri = f"/spaces/{self.id}/opening-hours"
 
         response = self._requester.request("PUT", uri, _kwargs=kwargs)
 
-        if "openingHours" in self._embedded:
-            self._embedded["openingHours"] = self.get_opening_hours()
+        data = response.json()
+        out = {"days": data}
+        out.update({"space_id": self.id})
 
-        return response
+        return SpaceOpeningHours(self._requester, out)
```

### Comparing `fabman-1.1.20/fabman/training_course.py` & `fabman-1.2.9/fabman/training_course.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/util.py` & `fabman-1.2.9/fabman/util.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman/webhook.py` & `fabman-1.2.9/fabman/webhook.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/fabman.egg-info/PKG-INFO` & `fabman-1.2.9/fabman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabman
-Version: 1.1.20
+Version: 1.2.9
 Summary: Python wrappers for interacting with the Fabman API
 Author: Davin Lawrence
 Author-email: Davin Lawrence <davin.lawrence@utexas.edu>
 Project-URL: Homepage, https://github.com/utexas-engr-tiw/fabman-api
 Project-URL: Documentation, https://fabman-api.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/utexas-engr-tiw/fabman-api/issues
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `fabman-1.1.20/fabman.egg-info/SOURCES.txt` & `fabman-1.2.9/fabman.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 setup.cfg
 setup.py
 fabman/__init__.py
 fabman/account.py
 fabman/api_key.py
 fabman/booking.py
 fabman/charge.py
+fabman/deleted_object.py
+fabman/embedded_list.py
 fabman/exceptions.py
 fabman/fabman.py
 fabman/fabman_object.py
 fabman/invoice.py
 fabman/job.py
 fabman/member.py
 fabman/package.py
@@ -30,14 +32,15 @@
 fabman.egg-info/dependency_links.txt
 fabman.egg-info/requires.txt
 fabman.egg-info/top_level.txt
 tests/test_account.py
 tests/test_api_key.py
 tests/test_booking.py
 tests/test_charge.py
+tests/test_embedded_list.py
 tests/test_fabman.py
 tests/test_invoice.py
 tests/test_job.py
 tests/test_member.py
 tests/test_package.py
 tests/test_paginated_list.py
 tests/test_payment.py
```

### Comparing `fabman-1.1.20/pyproject.toml` & `fabman-1.2.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel>=0.37.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fabman"
-version = "1.1.20"
+version = "1.2.9"
 authors = [
     {name = "Davin Lawrence", email="davin.lawrence@utexas.edu"},
 ]
 dependencies = [
     "requests>=2.31.0",
     "arrow>=1.2.3",
     "pytz==2023.3"
```

### Comparing `fabman-1.1.20/setup.py` & `fabman-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_account.py` & `fabman-1.2.9/tests/test_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=missing-docstring, invalid-name, unused-argument
 
 import unittest
 
 import requests_mock
 
 from fabman import Fabman
-from fabman.account import Account
+from fabman.account import Account, PaymentInfo
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
 class TestAccount(unittest.TestCase):
     def setUp(self) -> None:
@@ -28,16 +28,19 @@
         string = str(self.account)
         self.assertTrue(string == "Account #1: Tarok Nor")
 
     def test_get_payment_info(self, m):
         register_uris({"accounts": ["get_payment_info"]}, m)
 
         info = self.account.get_payment_info()
-        self.assertIsInstance(info, dict)
-        self.assertTrue(info["id"] == 1)
+        self.assertIsInstance(info, PaymentInfo)
+        self.assertEqual(info.id, 1)
+        self.assertEqual(info.account_id, 1)
+
+        self.assertEqual(str(info), "PaymentInfo for Account #1: stripe")
 
     def test_update(self, m):
         m.register_uri(
             "PUT",
             f"{settings.BASE_URL_WITH_VERSION}/accounts/1",
             text=validate_update,
             status_code=200,
```

### Comparing `fabman-1.1.20/tests/test_api_key.py` & `fabman-1.2.9/tests/test_api_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import unittest
 
 import requests
 import requests_mock
 
 from fabman import Fabman
-from fabman.api_key import ApiKey
+from fabman.api_key import ApiKey, ApiKeyToken
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
 class TestMembers(unittest.TestCase):
     def setUp(self):
@@ -37,16 +37,18 @@
         self.assertIsInstance(resp, requests.Response)
         self.assertTrue(resp.status_code == 204)
 
     def test_get_token(self, m):
         register_uris({"api_key": ["get_token"]}, m)
 
         tok = self.api_key.get_token()
-        self.assertIsInstance(tok, dict)
-        self.assertTrue(tok["token"] == "123")
+        self.assertIsInstance(tok, ApiKeyToken)
+        self.assertTrue(tok.token == "123")
+
+        self.assertEqual(str(tok), "ApiKeyToken #1: 123")
 
     def test_update(self, m):
         m.register_uri(
             "PUT",
             f"{settings.BASE_URL_WITH_VERSION}/api-keys/1",
             text=validate_update,
             status_code=200,
```

### Comparing `fabman-1.1.20/tests/test_booking.py` & `fabman-1.2.9/tests/test_booking.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_charge.py` & `fabman-1.2.9/tests/test_charge.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_fabman.py` & `fabman-1.2.9/tests/test_fabman.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_invoice.py` & `fabman-1.2.9/tests/test_invoice.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=missing-docstring, invalid-name, unused-argument
 
 import unittest
 
 import requests_mock
 
 from fabman import Fabman
-from fabman.invoice import Invoice
+from fabman.invoice import Invoice, InvoiceDetails
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
 class TestInvoice(unittest.TestCase):
     def setUp(self):
@@ -41,16 +41,29 @@
         self.assertTrue(m.called)
 
     def test_details(self, m):
         register_uris({"invoice": ["details"]}, m)
 
         details = self.invoice.details()
         self.assertTrue(m.called)
-        self.assertIsInstance(details, dict)
-        self.assertTrue(details["id"] == 1)
+        self.assertIsInstance(details, InvoiceDetails)
+        self.assertTrue(details.id == 1)
+
+        self.assertEqual(str(details), "Invoice #1: 12.34 # Charges: 1")
+
+    def test_details_embedded(self, m):
+        register_uris({"fabman": ["get_invoice_embedded_detail"]}, m)
+        invoice = self.fabman.get_invoice(1)
+
+        details = invoice.details()
+        self.assertTrue(m.called)
+        self.assertIsInstance(details, InvoiceDetails)
+        self.assertEqual(details.id, 2)
+
+        self.assertEqual(str(details), "Invoice #2: 45.67 # Charges: 1")
 
     def test_update(self, m):
         m.register_uri(
             "PUT",
             f"{settings.BASE_URL_WITH_VERSION}/invoices/1",
             text=validate_update,
             status_code=200,
```

### Comparing `fabman-1.1.20/tests/test_job.py` & `fabman-1.2.9/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_member.py` & `fabman-1.2.9/tests/test_member.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,34 @@
 
 import unittest
 import warnings
 
 import requests_mock
 
 from fabman import Fabman
+from fabman.embedded_list import EmbeddedList
 from fabman.exceptions import ResourceDoesNotExist
-from fabman.member import Member, MemberCredit, MemberKey, MemberPackage
+from fabman.member import (
+    Member,
+    MemberBalanceItems,
+    MemberChange,
+    MemberCredit,
+    MemberCreditUse,
+    MemberDevice,
+    MemberDeviceChange,
+    MemberInvitation,
+    MemberKey,
+    MemberPackage,
+    MemberPaymentAccount,
+    MemberPaymentMethod,
+    MemberPaymentMethodMandatePreview,
+    MemberPrivileges,
+    MemberTrainedResources,
+    MemberTraining,
+)
 from fabman.package import Package
 from fabman.paginated_list import PaginatedList
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
@@ -52,48 +70,20 @@
     def test_delete(self, m):
         register_uris({"member": ["delete"]}, m)
 
         resp = self.member.delete()
         self.assertTrue(m.called)
         self.assertTrue(resp.status_code == 204)
 
-    def test_delete_change(self, m):
-        register_uris({"member": ["delete_change"]}, m)
-
-        resp = self.member.delete_change(1)
-        self.assertTrue(m.called)
-        self.assertTrue(resp.status_code == 204)
-
-    def test_delete_device_change(self, m):
-        register_uris({"member": ["delete_device_change"]}, m)
-
-        resp = self.member.delete_device_change(1)
-        self.assertTrue(m.called)
-        self.assertTrue(resp.status_code == 204)
-
-    def test_delete_payment_method(self, m):
-        register_uris({"member": ["delete_payment_method"]}, m)
-
-        resp = self.member.delete_payment_method()
-        self.assertTrue(m.called)
-        self.assertTrue(resp.status_code == 204)
-
-    def test_delete_training(self, m):
-        register_uris({"member": ["delete_training"]}, m)
-
-        resp = self.member.delete_training(1)
-        self.assertTrue(m.called)
-        self.assertTrue(resp.status_code == 204)
-
     def test_get_balance_items(self, m):
         register_uris({"member": ["get_balance_items"]}, m)
 
         balance_items = self.member.get_balance_items()
 
-        self.assertIsInstance(balance_items, dict)
+        self.assertIsInstance(balance_items, MemberBalanceItems)
 
     def test_get_get_changes(self, m):
         register_uris({"member": ["get_changes"]}, m)
 
         changes = self.member.get_changes()
         self.assertIsInstance(changes, list)
 
@@ -109,39 +99,42 @@
         credit = self.member.get_credit(1)
         self.assertIsInstance(credit, MemberCredit)
 
     def test_get_device(self, m):
         register_uris({"member": ["get_device"]}, m)
 
         device = self.member.get_device()
-        self.assertIsInstance(device, dict)
-        self.assertEqual(device["name"], "Starfleet Tricorder")
+        self.assertIsInstance(device, MemberDevice)
+        self.assertEqual(device.name, "Starfleet Tricorder")
+
+        self.assertEqual(str(device), "Device: Starfleet Tricorder")
 
     def test_get_device_embeded(self, m):
         register_uris({"fabman": ["get_member_by_id_device_embed"]}, m)
 
         member = self.fabman.get_member(1, embed=["device"])
 
         self.assertIsInstance(member, Member)
         device = member.get_device()
-        self.assertTrue(device["name"] == "Device 1")
+        self.assertTrue(device.name == "Device 1")
 
     def test_get_device_changes(self, m):
         register_uris({"member": ["get_device_changes"]}, m)
         changes = self.member.get_device_changes()
 
         self.assertIsInstance(changes, list)
+        self.assertIsInstance(changes[0], MemberDeviceChange)
         self.assertEqual(len(changes), 2)
 
     def test_get_device_changes_by_id(self, m):
         register_uris({"member": ["get_device_change_by_id"]}, m)
 
         change = self.member.get_device_change(1)
 
-        self.assertIsInstance(change, dict)
+        self.assertIsInstance(change, MemberDeviceChange)
 
     def test_get_embeds(self, m):
         register_uris({"member": ["get_embeds"]}, m)
 
         member = self.fabman.get_member(
             1, embed=["memberPackages", "trainings", "key", "privileges", "device"]
         )
@@ -151,49 +144,57 @@
         self.assertTrue("trainings" in member._embedded)
         self.assertTrue("key" in member._embedded)
         self.assertTrue("privileges" in member._embedded)
         self.assertTrue("device" in member._embedded)
 
         # memberPackages
         packages = member.get_packages()
-        self.assertIsInstance(packages, list)
+        self.assertIsInstance(packages, EmbeddedList)
         self.assertIsInstance(packages[0], MemberPackage)
+        self.assertEqual(packages[0].member_id, 1)
 
         package = member.get_package(1)
         self.assertIsInstance(package, MemberPackage)
+        self.assertEqual(package.member_id, 1)
 
         # trainings
         trainings = member.get_trainings()
-        self.assertIsInstance(trainings, list)
-        self.assertTrue(trainings[0]["id"] == 2)
+        self.assertIsInstance(trainings, EmbeddedList)
+        self.assertIsInstance(trainings[0], MemberTraining)
+        self.assertTrue(trainings[0].id == 2)
+        self.assertTrue(trainings[0].member_id == 1)
 
         training = member.get_training(2)
-        self.assertIsInstance(training, dict)
-        self.assertTrue(training["id"] == 2)
+        self.assertIsInstance(training, MemberTraining)
+        self.assertTrue(training.id == 2)
+        self.assertTrue(training.member_id == 1)
 
         # key
         key = member.get_key()
         self.assertIsInstance(key, MemberKey)
         self.assertTrue(key.lockVersion == 4)
+        self.assertTrue(key.member_id == 1)
 
         # privileges
         privileges = member.get_privileges()
-        self.assertIsInstance(privileges, dict)
-        self.assertTrue(privileges["privileges"] == "member")
+        self.assertIsInstance(privileges, MemberPrivileges)
+        self.assertTrue(privileges.privileges == "member")
+        self.assertEqual(privileges.member_id, 1)
 
         # device
         device = member.get_device()
-        self.assertIsInstance(device, dict)
-        self.assertTrue(device["name"] == "Starfleet Communicator")
+        self.assertIsInstance(device, MemberDevice)
+        self.assertTrue(device.name == "Starfleet Tricorder")
 
     def test_get_invitation(self, m):
         register_uris({"member": ["get_invitation"]}, m)
 
         invitation = self.member.get_invitation()
-        self.assertIsInstance(invitation, dict)
+        self.assertIsInstance(invitation, MemberInvitation)
+        self.assertEqual(invitation.member_id, 1)
 
     def test_get_key_empty(self, m):
         register_uris({"member": ["get_key_empty"]}, m)
         with warnings.catch_warnings(record=True):
             key = self.member.get_key()  # pylint: disable=unused-variable
             self.assertRaises(
                 UserWarning,
@@ -228,21 +229,23 @@
         self.assertRaises(ResourceDoesNotExist, self.member.get_package, 2)
 
     def test_get_payment_account(self, m):
         register_uris({"member": ["get_payment_account"]}, m)
 
         payment_acct = self.member.get_payment_account()
 
-        self.assertIsInstance(payment_acct, list)
+        self.assertIsInstance(payment_acct, MemberPaymentAccount)
+        self.assertEqual(payment_acct.member_id, 1)
 
     def test_get_payment_methods_exists(self, m):
         register_uris({"member": ["get_payment_method_exists"]}, m)
 
         payment_method = self.member.get_payment_method()
-        self.assertIsInstance(payment_method, dict)
+        self.assertIsInstance(payment_method, MemberPaymentMethod)
+        self.assertEqual(payment_method.member_id, 1)
 
     def test_get_payment_method_doesnt_exist(self, m):
         register_uris({"member": ["get_payment_method_doesnt_exist"]}, m)
         with warnings.catch_warnings(record=True):  # pylint: disable=unused-variable
             self.assertRaises(
                 UserWarning,
                 msg=(
@@ -251,40 +254,47 @@
                 ),
             )
 
     def test_get_payment_method_mandate_preview(self, m):
         register_uris({"member": ["get_payment_method_mandate_preview"]}, m)
 
         mandate_preview = self.member.get_payment_method_mandate_preview()
-        self.assertIsInstance(mandate_preview, dict)
+        self.assertIsInstance(mandate_preview, MemberPaymentMethodMandatePreview)
+        self.assertEqual(mandate_preview.member_id, 1)
 
     def test_get_privileges(self, m):
         register_uris({"member": ["get_privileges"]}, m)
 
         priv = self.member.get_privileges()
-        self.assertIsInstance(priv, dict)
-        self.assertEqual(priv["privileges"], "admin")
+        self.assertIsInstance(priv, MemberPrivileges)
+        self.assertEqual(priv.privileges, "admin")
+        self.assertEqual(priv.member_id, 1)
+        self.assertTrue(str(priv) == "Member #1 is admin")
 
     def test_get_trained_resources(self, m):
         register_uris({"member": ["get_trained_resources"]}, m)
 
         train_res = self.member.get_trained_resources()
-        self.assertIsInstance(train_res, list)
+        self.assertIsInstance(train_res, MemberTrainedResources)
+        self.assertEqual(train_res.member_id, 1)
+        self.assertTrue(str(train_res) == "Member #1 is trained on 3 resources")
+        self.assertListEqual(train_res.resources, [1, 2, 3])
 
     def test_get_trainings(self, m):
         register_uris({"member": ["get_trainings"]}, m)
 
         trainings = self.member.get_trainings()
-        self.assertIsInstance(trainings, list)
+        self.assertIsInstance(trainings, PaginatedList)
+        self.assertIsInstance(trainings[0], MemberTraining)
 
     def test_get_training_by_id(self, m):
         register_uris({"member": ["get_training_by_id"]}, m)
 
         training = self.member.get_training(1)
-        self.assertIsInstance(training, dict)
+        self.assertIsInstance(training, MemberTraining)
 
     def test_refresh(self, m):
         register_uris({"fabman": ["get_member_by_id"]}, m)
 
         before = self.member.id
         self.member.refresh()
         self.assertTrue(m.called)
@@ -299,14 +309,41 @@
         )
 
         self.member.update(firstName="John", lastName="Doe")
         self.assertTrue(m.called)
 
 
 @requests_mock.Mocker()
+class TestMemberChange(unittest.TestCase):
+    def setUp(self):
+        self.fabman = Fabman(settings.API_KEY)
+
+        with requests_mock.Mocker() as m:
+            register_uris({"fabman": ["get_member_by_id"]}, m)
+            register_uris({"member": ["get_changes"]}, m)
+
+            self.member: Member = self.fabman.get_member(1)
+            self.changes: list = self.member.get_changes()
+            self.change = self.changes[0]
+
+    def test_instance(self, m):
+        self.assertIsInstance(self.change, MemberChange)
+
+    def test_string(self, m):
+        self.assertEqual(str(self.change), "Change #1 for member #1")
+
+    def test_delete(self, m):
+        register_uris({"member": ["delete_change"]}, m)
+
+        resp = self.change.delete()
+        self.assertTrue(m.called)
+        self.assertTrue(resp.status_code == 204)
+
+
+@requests_mock.Mocker()
 class TestMemberCredit(unittest.TestCase):
     def setUp(self):
         self.fabman = Fabman(settings.API_KEY)
 
         with requests_mock.Mocker() as m:
             register_uris({"fabman": ["get_member_by_id"]}, m)
             register_uris({"member": ["get_credit_by_id"]}, m)
@@ -330,29 +367,85 @@
         self.assertTrue(resp.status_code == 204)
 
     def test_get_uses(self, m):
         register_uris({"member": ["get_credit_uses"]}, m)
 
         uses = self.credit.get_uses()
         self.assertIsInstance(uses, list)
-        self.assertTrue(uses[0]["id"] == 1)
+        self.assertIsInstance(uses[0], MemberCreditUse)
+        self.assertTrue(uses[0].id == 1)
 
     def test_update(self, m):
         m.register_uri(
             "PUT",
             "https://fabman.io/api/v1/members/1/credits/1",
             text=validate_update,
             status_code=200,
         )
 
         self.credit.update(amount=12.34)
         self.assertTrue(m.called)
 
 
 @requests_mock.Mocker()
+class TestMemberDeviceChange(unittest.TestCase):
+    def setUp(self):
+        self.fabman = Fabman(settings.API_KEY)
+
+        with requests_mock.Mocker() as m:
+            register_uris({"fabman": ["get_member_by_id"]}, m)
+            register_uris({"member": ["get_device_changes"]}, m)
+
+            self.member: Member = self.fabman.get_member(1)
+            self.device_changes: list = self.member.get_device_changes()
+            self.device_change = self.device_changes[0]
+
+    def test_instance(self, m):
+        self.assertIsInstance(self.device_change, MemberDeviceChange)
+
+    def test_str(self, m):
+        self.assertEqual(str(self.device_change), "DeviceChange #1 for member #1")
+
+    def test_delete(self, m):
+        register_uris({"member": ["delete_device_change"]}, m)
+
+        resp = self.device_change.delete()
+        self.assertTrue(m.called)
+        self.assertTrue(resp.status_code == 204)
+
+
+@requests_mock.Mocker()
+class TestMemberPaymentMethod(unittest.TestCase):
+    def setUp(self):
+        self.fabman = Fabman(settings.API_KEY)
+
+        with requests_mock.Mocker() as m:
+            register_uris({"fabman": ["get_member_by_id"]}, m)
+            register_uris({"member": ["get_payment_method_exists"]}, m)
+
+            self.member: Member = self.fabman.get_member(1)
+            self.payment_method: MemberPaymentMethod = self.member.get_payment_method()
+
+    def test_instance(self, m):
+        self.assertIsInstance(self.payment_method, MemberPaymentMethod)
+
+    def test_str(self, m):
+        self.assertEqual(
+            str(self.payment_method), "Member #1 has a stripe payment method"
+        )
+
+    def test_delete(self, m):
+        register_uris({"member": ["delete_payment_method"]}, m)
+
+        resp = self.payment_method.delete()
+        self.assertTrue(m.called)
+        self.assertTrue(resp.status_code == 204)
+
+
+@requests_mock.Mocker()
 class TestMemberKey(unittest.TestCase):
     def setUp(self):
         self.fabman: Fabman = Fabman(settings.API_KEY)
 
         with requests_mock.Mocker() as m:
             register_uris(
                 {"member": ["get_key_data"], "fabman": ["get_member_by_id"]}, m
@@ -434,7 +527,34 @@
             "https://fabman.io/api/v1/members/1/packages/1",
             text=validate_update,
             status_code=200,
         )
 
         self.package.update()
         self.assertTrue(m.called)
+
+
+@requests_mock.Mocker()
+class TestMemberTraining(unittest.TestCase):
+    def setUp(self) -> None:
+        self.fabman = Fabman(settings.API_KEY)
+
+        with requests_mock.Mocker() as m:
+            register_uris(
+                {"fabman": ["get_member_by_id"], "member": ["get_training_by_id"]}, m
+            )
+
+            self.member = self.fabman.get_member(1)
+            self.training = self.member.get_training(1)
+
+    def test_instance(self, m):
+        self.assertIsInstance(self.training, MemberTraining)
+
+    def test_str(self, m):
+        self.assertTrue(str(self.training) == "MemberTraining #1 for member #1")
+
+    def test_delete(self, m):
+        register_uris({"member": ["delete_training"]}, m)
+
+        resp = self.training.delete()
+        self.assertTrue(m.called)
+        self.assertTrue(resp.status_code == 204)
```

### Comparing `fabman-1.1.20/tests/test_package.py` & `fabman-1.2.9/tests/test_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         )
 
         self.package.update(name="Test Package")
         self.assertTrue(m.called)
 
 
 @requests_mock.Mocker()
-class TestMemberCredit(unittest.TestCase):
+class TestPackageCredit(unittest.TestCase):
     def setUp(self) -> None:
         self.fabman = Fabman(settings.API_KEY)
 
         with requests_mock.Mocker() as m:
             register_uris(
                 {"fabman": ["get_package_by_id"], "package": ["get_credit"]}, m
             )
```

### Comparing `fabman-1.1.20/tests/test_paginated_list.py` & `fabman-1.2.9/tests/test_paginated_list.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_payment.py` & `fabman-1.2.9/tests/test_payment.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import unittest
 
 import requests
 import requests_mock
 
 from fabman import Fabman
-from fabman.payment import Payment
+from fabman.payment import Payment, PaymentRequest
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
 class TestPayment(unittest.TestCase):
     """
@@ -45,16 +45,18 @@
         self.assertTrue(resp.status_code == 204)
 
     def test_request_payment(self, m):
         register_uris({"payment": ["request_payment"]}, m)
 
         resp = self.payment.request_payment()
         self.assertTrue(m.called)
-        self.assertIsInstance(resp, requests.Response)
-        self.assertTrue(resp.status_code == 201)
+        self.assertIsInstance(resp, PaymentRequest)
+        self.assertTrue(resp.payment_id == 1)
+
+        self.assertEqual(str(resp), "PaymentRequest for Payment #1")
 
     def test_update(self, m):
         """Checks to ensure lockVersion is added and used"""
         m.register_uri(
             "PUT",
             f"{settings.BASE_URL_WITH_VERSION}/payments/1",
             text=validate_update,
```

### Comparing `fabman-1.1.20/tests/test_requester.py` & `fabman-1.2.9/tests/test_requester.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_resource.py` & `fabman-1.2.9/tests/test_resource.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import unittest
 
 import requests
 import requests_mock
 
 from fabman import Fabman
-from fabman.resource import Resource, ResourceBridge
+from fabman.resource import Resource, ResourceBridge, ResourceBridgeApiKey
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
 class TestResource(unittest.TestCase):
     """Test Cases for the Resource class."""
@@ -54,15 +54,18 @@
         self.assertIsInstance(bridge, ResourceBridge)
         self.assertTrue(hasattr(bridge, "serialNumber"))
 
     def test_get_bridge_api_key(self, m):
         register_uris({"resource": ["get_bridge_api_key"]}, m)
         api_key = self.resource.get_bridge_api_key()
 
-        self.assertIsInstance(api_key, dict)
+        self.assertIsInstance(api_key, ResourceBridgeApiKey)
+        self.assertTrue(api_key.resource_id == 1)
+
+        self.assertEqual(str(api_key), "Resource #1: xxxx3456")
 
     def test_switch_on(self, m):
         register_uris({"resource": ["switch_on"]}, m)
 
         resp = self.resource.switch_on()
         self.assertTrue(m.called)
         self.assertIsInstance(resp, requests.Response)
```

### Comparing `fabman-1.1.20/tests/test_resource_log.py` & `fabman-1.2.9/tests/test_resource_log.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_resource_type.py` & `fabman-1.2.9/tests/test_resource_type.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_sanity.py` & `fabman-1.2.9/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_space.py` & `fabman-1.2.9/tests/test_space.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 import unittest
 
 import requests
 import requests_mock
 
 from fabman import Fabman
+from fabman.embedded_list import EmbeddedList
 from fabman.paginated_list import PaginatedList
-from fabman.space import Space, SpaceBillingSettings, SpaceHoliday
+from fabman.space import Space, SpaceBillingSettings, SpaceHoliday, SpaceOpeningHours
 from tests import settings
 from tests.util import register_uris, validate_update
 
 
 @requests_mock.Mocker()
 class TestSpace(unittest.TestCase):
     def setUp(self):
@@ -81,23 +82,23 @@
         billing = space.get_billing_settings()
         self.assertIsInstance(billing, SpaceBillingSettings)
         self.assertTrue(hasattr(billing, "space_id"))
 
         # holidays
         self.assertTrue("holidays" in space._embedded)
         holidays = space.get_holidays()
-        self.assertIsInstance(holidays, list)
-        self.assertTrue(len(holidays) == 3)
+        self.assertIsInstance(holidays, EmbeddedList)
         self.assertIsInstance(holidays[0], SpaceHoliday)
         self.assertTrue(hasattr(holidays[0], "space_id"))
 
         # openingHours
         self.assertTrue("openingHours" in space._embedded)
         opening_hours = space.get_opening_hours()
-        self.assertIsInstance(opening_hours, list)
+        self.assertIsInstance(opening_hours, SpaceOpeningHours)
+        self.assertEqual(opening_hours.space_id, 1)
 
     def test_get_holiday(self, m):
         register_uris({"space": ["get_holiday"]}, m)
 
         holiday = self.space.get_holiday(1)
         self.assertIsInstance(holiday, SpaceHoliday)
         self.assertTrue(hasattr(holiday, "id"))
@@ -113,16 +114,18 @@
         self.assertTrue(holiday[0].id == 1)
 
     def test_get_opening_hours(self, m):
         register_uris({"space": ["get_opening_hours"]}, m)
 
         resp = self.space.get_opening_hours()
         self.assertTrue(m.called)
-        self.assertIsInstance(resp, requests.Response)
-        self.assertTrue(resp.status_code == 200)
+        self.assertIsInstance(resp, SpaceOpeningHours)
+        self.assertTrue(resp.space_id == 1)
+
+        self.assertTrue("Space #1 Opening Hours" in str(resp))
 
     def test_update_calendar_token(self, m):
         register_uris({"space": ["update_calendar_token"]}, m)
 
         resp = self.space.update_calendar_token()
         self.assertTrue(m.called)
         self.assertIsInstance(resp, requests.Response)
@@ -131,16 +134,16 @@
         self.assertTrue(self.space.calendarToken == "abcdef-1234-5678")
 
     def test_update_hours(self, m):
         register_uris({"space": ["update_opening_hours"]}, m)
 
         resp = self.space.update_opening_hours()
         self.assertTrue(m.called)
-        self.assertIsInstance(resp, requests.Response)
-        self.assertTrue(resp.status_code == 200)
+        self.assertIsInstance(resp, SpaceOpeningHours)
+        self.assertTrue(resp.space_id == 1)
 
     def test_update(self, m):
         m.register_uri(
             "PUT",
             f"{settings.BASE_URL_WITH_VERSION}/spaces/1",
             text=validate_update,
             status_code=200,
```

### Comparing `fabman-1.1.20/tests/test_training_course.py` & `fabman-1.2.9/tests/test_training_course.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_util.py` & `fabman-1.2.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `fabman-1.1.20/tests/test_webhook.py` & `fabman-1.2.9/tests/test_webhook.py`

 * *Files identical despite different names*


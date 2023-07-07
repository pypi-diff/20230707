# Comparing `tmp/py_clob_client-0.7.0.tar.gz` & `tmp/py_clob_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_clob_client-0.7.0.tar", last modified: Fri May  5 23:14:19 2023, max compression
+gzip compressed data, was "py_clob_client-0.8.0.tar", last modified: Fri Jul  7 15:49:45 2023, max compression
```

## Comparing `py_clob_client-0.7.0.tar` & `py_clob_client-0.8.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.806583 py_clob_client-0.7.0/
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1067 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/LICENSE
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-05-05 23:14:19.806450 py_clob_client-0.7.0/PKG-INFO
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2304 2023-02-01 18:41:38.000000 py_clob_client-0.7.0/README.md
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.802968 py_clob_client-0.7.0/py_clob_client/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/py_clob_client/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    16135 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/client.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2531 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/clob_types.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      453 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/constants.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      713 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/endpoints.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      871 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/exceptions.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.803665 py_clob_client-0.7.0/py_clob_client/headers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/headers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1473 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/headers/headers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.803844 py_clob_client-0.7.0/py_clob_client/http_helpers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/py_clob_client/http_helpers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     4213 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/py_clob_client/http_helpers/helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.804451 py_clob_client-0.7.0/py_clob_client/order_builder/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/order_builder/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3995 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/py_clob_client/order_builder/builder.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)       26 2023-01-26 15:15:34.000000 py_clob_client-0.7.0/py_clob_client/order_builder/constants.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      629 2023-01-27 20:18:52.000000 py_clob_client-0.7.0/py_clob_client/order_builder/helpers.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      583 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signer.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.804951 py_clob_client-0.7.0/py_clob_client/signing/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.7.0/py_clob_client/signing/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      795 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signing/eip712.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      708 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signing/hmac.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      186 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/py_clob_client/signing/model.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1040 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/py_clob_client/utilities.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.803469 py_clob_client-0.7.0/py_clob_client.egg-info/
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/PKG-INFO
--rw-r--r--   0 poly-rodr   (505) staff       (20)     1226 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/SOURCES.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/dependency_links.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       36 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/requires.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2023-05-05 23:14:19.000000 py_clob_client-0.7.0/py_clob_client.egg-info/top_level.txt
--rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2023-05-05 23:14:19.806636 py_clob_client-0.7.0/setup.cfg
--rw-r--r--   0 poly-rodr   (505) staff       (20)      963 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/setup.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805189 py_clob_client-0.7.0/tests/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/__init__.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805465 py_clob_client-0.7.0/tests/headers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/headers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     3256 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/headers/test_headers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805677 py_clob_client-0.7.0/tests/http_helpers/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/http_helpers/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)     2759 2023-05-05 23:11:51.000000 py_clob_client-0.7.0/tests/http_helpers/test_helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.805997 py_clob_client-0.7.0/tests/order_builder/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/order_builder/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    30909 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/tests/order_builder/test_builder.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      274 2023-01-27 20:18:52.000000 py_clob_client-0.7.0/tests/order_builder/test_helpers.py
-drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-05-05 23:14:19.806292 py_clob_client-0.7.0/tests/signing/
--rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/signing/__init__.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      757 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/signing/test_eip712.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)      536 2022-09-23 20:43:25.000000 py_clob_client-0.7.0/tests/signing/test_hmac.py
--rw-r--r--   0 poly-rodr   (505) staff       (20)    33747 2023-04-19 16:44:09.000000 py_clob_client-0.7.0/tests/test_utilities.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.484612 py_clob_client-0.8.0/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1067 2022-05-27 21:15:08.000000 py_clob_client-0.8.0/LICENSE
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-07-07 15:49:45.484454 py_clob_client-0.8.0/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2304 2023-02-01 18:41:38.000000 py_clob_client-0.8.0/README.md
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.480585 py_clob_client-0.8.0/py_clob_client/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.8.0/py_clob_client/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    17410 2023-07-07 15:49:34.000000 py_clob_client-0.8.0/py_clob_client/client.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2531 2023-05-05 23:11:51.000000 py_clob_client-0.8.0/py_clob_client/clob_types.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      453 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/constants.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      918 2023-07-07 15:49:34.000000 py_clob_client-0.8.0/py_clob_client/endpoints.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      871 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/exceptions.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.481339 py_clob_client-0.8.0/py_clob_client/headers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/headers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1473 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/headers/headers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.481538 py_clob_client-0.8.0/py_clob_client/http_helpers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.8.0/py_clob_client/http_helpers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     4213 2023-05-05 23:11:51.000000 py_clob_client-0.8.0/py_clob_client/http_helpers/helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.482013 py_clob_client-0.8.0/py_clob_client/order_builder/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/order_builder/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3995 2023-04-19 16:44:09.000000 py_clob_client-0.8.0/py_clob_client/order_builder/builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       26 2023-01-26 15:15:34.000000 py_clob_client-0.8.0/py_clob_client/order_builder/constants.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      629 2023-01-27 20:18:52.000000 py_clob_client-0.8.0/py_clob_client/order_builder/helpers.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      583 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/signer.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.482447 py_clob_client-0.8.0/py_clob_client/signing/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-05-27 21:15:08.000000 py_clob_client-0.8.0/py_clob_client/signing/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      795 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/signing/eip712.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      708 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/signing/hmac.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      186 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/py_clob_client/signing/model.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1040 2023-04-19 16:44:09.000000 py_clob_client-0.8.0/py_clob_client/utilities.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.481140 py_clob_client-0.8.0/py_clob_client.egg-info/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2930 2023-07-07 15:49:45.000000 py_clob_client-0.8.0/py_clob_client.egg-info/PKG-INFO
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     1226 2023-07-07 15:49:45.000000 py_clob_client-0.8.0/py_clob_client.egg-info/SOURCES.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        1 2023-07-07 15:49:45.000000 py_clob_client-0.8.0/py_clob_client.egg-info/dependency_links.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       36 2023-07-07 15:49:45.000000 py_clob_client-0.8.0/py_clob_client.egg-info/requires.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       21 2023-07-07 15:49:45.000000 py_clob_client-0.8.0/py_clob_client.egg-info/top_level.txt
+-rw-r--r--   0 poly-rodr   (505) staff       (20)       38 2023-07-07 15:49:45.484663 py_clob_client-0.8.0/setup.cfg
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      963 2023-07-07 15:49:34.000000 py_clob_client-0.8.0/setup.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.482669 py_clob_client-0.8.0/tests/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/__init__.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.482901 py_clob_client-0.8.0/tests/headers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/headers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     3256 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/headers/test_headers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.483296 py_clob_client-0.8.0/tests/http_helpers/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/http_helpers/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)     2759 2023-05-05 23:11:51.000000 py_clob_client-0.8.0/tests/http_helpers/test_helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.483678 py_clob_client-0.8.0/tests/order_builder/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/order_builder/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    30909 2023-04-19 16:44:09.000000 py_clob_client-0.8.0/tests/order_builder/test_builder.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      274 2023-07-03 17:15:49.000000 py_clob_client-0.8.0/tests/order_builder/test_helpers.py
+drwxr-xr-x   0 poly-rodr   (505) staff       (20)        0 2023-07-07 15:49:45.484132 py_clob_client-0.8.0/tests/signing/
+-rw-r--r--   0 poly-rodr   (505) staff       (20)        0 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/signing/__init__.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      757 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/signing/test_eip712.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)      536 2022-09-23 20:43:25.000000 py_clob_client-0.8.0/tests/signing/test_hmac.py
+-rw-r--r--   0 poly-rodr   (505) staff       (20)    33747 2023-04-19 16:44:09.000000 py_clob_client-0.8.0/tests/test_utilities.py
```

### Comparing `py_clob_client-0.7.0/LICENSE` & `py_clob_client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/PKG-INFO` & `py_clob_client-0.8.0/py_clob_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_clob_client
-Version: 0.7.0
+Name: py-clob-client
+Version: 0.8.0
 Summary: Python client for the Polymarket CLOB
 Home-page: https://github.com/Polymarket/py-clob-client
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
 Project-URL: Bug Tracker, https://github.com/Polymarket/py-clob-client/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py_clob_client Version: 0.7.0 Summary: Python
+Metadata-Version: 2.1 Name: py-clob-client Version: 0.8.0 Summary: Python
 client for the Polymarket CLOB Home-page: https://github.com/Polymarket/py-
 clob-client Author: Polymarket Engineering Author-email:
 engineering@polymarket.com Maintainer: Polymarket Engineering Maintainer-email:
 engineering@polymarket.com Project-URL: Bug Tracker, https://github.com/
 Polymarket/py-clob-client/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9.10 Description-Content-Type:
```

### Comparing `py_clob_client-0.7.0/README.md` & `py_clob_client-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/client.py` & `py_clob_client-0.8.0/py_clob_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,19 @@
     TRADES,
     GET_TRADE_NOTIFICATIONS,
     DROP_TRADE_NOTIFICATIONS,
     GET_BALANCE_ALLOWANCE,
     IS_ORDER_SCORING,
     GET_TICK_SIZE,
     ARE_ORDERS_SCORING,
+    GET_SIMPLIFIED_MARKETS,
+    GET_MARKETS,
+    GET_MARKET,
+    GET_SAMPLING_SIMPLIFIED_MARKETS,
+    GET_SAMPLING_MARKETS,
 )
 from .clob_types import (
     ApiCreds,
     FilterParams,
     OrderArgs,
     RequestArgs,
     TradeNotificationParams,
@@ -476,7 +481,45 @@
         self.assert_level_2_auth()
         request_args = RequestArgs(method="GET", request_path=ARE_ORDERS_SCORING)
         headers = create_level_2_headers(self.signer, self.creds, request_args)
         url = add_orders_scoring_params_to_url(
             "{}{}".format(self.host, ARE_ORDERS_SCORING), params
         )
         return get(url, headers=headers)
+
+    def get_sampling_markets(self, next_cursor="MA=="):
+        """
+        Get the current sampling markets
+        """
+        return get(
+            "{}{}?next_cursor={}".format(self.host, GET_SAMPLING_MARKETS, next_cursor)
+        )
+
+    def get_sampling_simplified_markets(self, next_cursor="MA=="):
+        """
+        Get the current sampling simplified markets
+        """
+        return get(
+            "{}{}?next_cursor={}".format(
+                self.host, GET_SAMPLING_SIMPLIFIED_MARKETS, next_cursor
+            )
+        )
+
+    def get_markets(self, next_cursor="MA=="):
+        """
+        Get the current markets
+        """
+        return get("{}{}?next_cursor={}".format(self.host, GET_MARKETS, next_cursor))
+
+    def get_simplified_markets(self, next_cursor="MA=="):
+        """
+        Get the current simplified markets
+        """
+        return get(
+            "{}{}?next_cursor={}".format(self.host, GET_SIMPLIFIED_MARKETS, next_cursor)
+        )
+
+    def get_market(self, condition_id):
+        """
+        Get a market by condition_id
+        """
+        return get("{}{}{}".format(self.host, GET_MARKET, condition_id))
```

### Comparing `py_clob_client-0.7.0/py_clob_client/clob_types.py` & `py_clob_client-0.8.0/py_clob_client/clob_types.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/endpoints.py` & `py_clob_client-0.8.0/py_clob_client/endpoints.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,7 +17,12 @@
 GET_LAST_TRADE_PRICE = "/last-trade-price"
 GET_TRADE_NOTIFICATIONS = "/trade-notifications"
 DROP_TRADE_NOTIFICATIONS = "/drop-trade-notifications"
 GET_BALANCE_ALLOWANCE = "/balance-allowance"
 IS_ORDER_SCORING = "/order-scoring"
 ARE_ORDERS_SCORING = "/orders-scoring"
 GET_TICK_SIZE = "/tick-size"
+GET_SAMPLING_SIMPLIFIED_MARKETS = "/sampling-simplified-markets"
+GET_SAMPLING_MARKETS = "/sampling-markets"
+GET_SIMPLIFIED_MARKETS = "/simplified-markets"
+GET_MARKETS = "/markets"
+GET_MARKET = "/markets/"
```

### Comparing `py_clob_client-0.7.0/py_clob_client/exceptions.py` & `py_clob_client-0.8.0/py_clob_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/headers/headers.py` & `py_clob_client-0.8.0/py_clob_client/headers/headers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/http_helpers/helpers.py` & `py_clob_client-0.8.0/py_clob_client/http_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/order_builder/builder.py` & `py_clob_client-0.8.0/py_clob_client/order_builder/builder.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/order_builder/helpers.py` & `py_clob_client-0.8.0/py_clob_client/order_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/signer.py` & `py_clob_client-0.8.0/py_clob_client/signer.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/signing/eip712.py` & `py_clob_client-0.8.0/py_clob_client/signing/eip712.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/signing/hmac.py` & `py_clob_client-0.8.0/py_clob_client/signing/hmac.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client/utilities.py` & `py_clob_client-0.8.0/py_clob_client/utilities.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/py_clob_client.egg-info/PKG-INFO` & `py_clob_client-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-clob-client
-Version: 0.7.0
+Name: py_clob_client
+Version: 0.8.0
 Summary: Python client for the Polymarket CLOB
 Home-page: https://github.com/Polymarket/py-clob-client
 Author: Polymarket Engineering
 Author-email: engineering@polymarket.com
 Maintainer: Polymarket Engineering
 Maintainer-email: engineering@polymarket.com
 Project-URL: Bug Tracker, https://github.com/Polymarket/py-clob-client/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-clob-client Version: 0.7.0 Summary: Python
+Metadata-Version: 2.1 Name: py_clob_client Version: 0.8.0 Summary: Python
 client for the Polymarket CLOB Home-page: https://github.com/Polymarket/py-
 clob-client Author: Polymarket Engineering Author-email:
 engineering@polymarket.com Maintainer: Polymarket Engineering Maintainer-email:
 engineering@polymarket.com Project-URL: Bug Tracker, https://github.com/
 Polymarket/py-clob-client/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.9.10 Description-Content-Type:
```

### Comparing `py_clob_client-0.7.0/py_clob_client.egg-info/SOURCES.txt` & `py_clob_client-0.8.0/py_clob_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/setup.py` & `py_clob_client-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_clob_client",
-    version="0.7.0",
+    version="0.8.0",
     author="Polymarket Engineering",
     author_email="engineering@polymarket.com",
     maintainer="Polymarket Engineering",
     maintainer_email="engineering@polymarket.com",
     description="Python client for the Polymarket CLOB",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `py_clob_client-0.7.0/tests/headers/test_headers.py` & `py_clob_client-0.8.0/tests/headers/test_headers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/tests/http_helpers/test_helpers.py` & `py_clob_client-0.8.0/tests/http_helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/tests/order_builder/test_builder.py` & `py_clob_client-0.8.0/tests/order_builder/test_builder.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/tests/signing/test_eip712.py` & `py_clob_client-0.8.0/tests/signing/test_eip712.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/tests/signing/test_hmac.py` & `py_clob_client-0.8.0/tests/signing/test_hmac.py`

 * *Files identical despite different names*

### Comparing `py_clob_client-0.7.0/tests/test_utilities.py` & `py_clob_client-0.8.0/tests/test_utilities.py`

 * *Files identical despite different names*


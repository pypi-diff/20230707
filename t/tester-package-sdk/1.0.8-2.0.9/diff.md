# Comparing `tmp/tester-package-sdk-1.0.8.tar.gz` & `tmp/tester-package-sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tester-package-sdk-1.0.8.tar", last modified: Fri Jul  7 10:08:14 2023, max compression
+gzip compressed data, was "tester-package-sdk-2.0.9.tar", last modified: Tue Jun 13 12:23:15 2023, max compression
```

## Comparing `tester-package-sdk-1.0.8.tar` & `tester-package-sdk-2.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.798979 tester-package-sdk-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5478 2023-07-07 10:08:14.798979 tester-package-sdk-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5253 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-07 10:08:14.799979 tester-package-sdk-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.769979 tester-package-sdk-1.0.8/swaggerpetstore/
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.772979 tester-package-sdk-1.0.8/swaggerpetstore/controllers/
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/controllers/pet_controller.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/controllers/store_controller.py
--rw-r--r--   0 root         (0) root         (0)    10595 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.774979 tester-package-sdk-1.0.8/swaggerpetstore/exceptions/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/exceptions/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/exceptions/o_auth_provider_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.778979 tester-package-sdk-1.0.8/swaggerpetstore/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.793979 tester-package-sdk-1.0.8/swaggerpetstore/models/
--rw-r--r--   0 root         (0) root         (0)      249 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2232 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/api_response.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/category.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/o_auth_provider_error_enum.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/o_auth_scope_enum.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/o_auth_token.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/order.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/pet.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/status_1_enum.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/status_2_enum.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/status_enum.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     4034 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/models/user.py
--rw-r--r--   0 root         (0) root         (0)     3644 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/swaggerpetstore_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.795979 tester-package-sdk-1.0.8/swaggerpetstore/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-07 10:07:29.000000 tester-package-sdk-1.0.8/swaggerpetstore/utilities/file_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:08:14.798979 tester-package-sdk-1.0.8/tester_package_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5478 2023-07-07 10:08:14.000000 tester-package-sdk-1.0.8/tester_package_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1517 2023-07-07 10:08:14.000000 tester-package-sdk-1.0.8/tester_package_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 10:08:14.000000 tester-package-sdk-1.0.8/tester_package_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-07 10:08:14.000000 tester-package-sdk-1.0.8/tester_package_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-07 10:08:14.000000 tester-package-sdk-1.0.8/tester_package_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.032098 tester-package-sdk-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-06-13 12:23:15.032098 tester-package-sdk-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5281 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      653 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-13 12:23:15.032098 tester-package-sdk-2.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.007098 tester-package-sdk-2.0.9/swaggerpetstore/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.011098 tester-package-sdk-2.0.9/swaggerpetstore/controllers/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/controllers/pet_controller.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/controllers/store_controller.py
+-rw-r--r--   0 root         (0) root         (0)    10595 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/controllers/user_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.013098 tester-package-sdk-2.0.9/swaggerpetstore/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/exceptions/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/exceptions/o_auth_provider_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.018098 tester-package-sdk-2.0.9/swaggerpetstore/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.027098 tester-package-sdk-2.0.9/swaggerpetstore/models/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/api_response.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/category.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/o_auth_provider_error_enum.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/o_auth_scope_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/o_auth_token.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/order.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/pet.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/status_1_enum.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/status_2_enum.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/status_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/swaggerpetstore_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.028098 tester-package-sdk-2.0.9/swaggerpetstore/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-13 12:22:48.000000 tester-package-sdk-2.0.9/swaggerpetstore/utilities/file_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:23:15.031098 tester-package-sdk-2.0.9/tester_package_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-06-13 12:23:14.000000 tester-package-sdk-2.0.9/tester_package_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-13 12:23:14.000000 tester-package-sdk-2.0.9/tester_package_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:23:14.000000 tester-package-sdk-2.0.9/tester_package_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-06-13 12:23:14.000000 tester-package-sdk-2.0.9/tester_package_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-13 12:23:14.000000 tester-package-sdk-2.0.9/tester_package_sdk.egg-info/top_level.txt
```

### Comparing `tester-package-sdk-1.0.8/LICENSE` & `tester-package-sdk-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/PKG-INFO` & `tester-package-sdk-2.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tester-package-sdk
-Version: 1.0.8
+Version: 2.0.9
 Summary: this is testing please ignore
 Author-email: Subtain <Subtain@gmail.com>
 Project-URL: Documentation, https://subtain.com
 Keywords: this,is
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -21,23 +21,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install tester-package-sdk==1.0.8
+pip install tester-package-sdk==2.0.9
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/tester-package-sdk/1.0.8
+https://pypi.python.org/pypi/tester-package-sdk/2.0.9
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -103,17 +103,17 @@
 | Scope Name | Description |
 |  --- | --- |
 | `READPETS` | read your pets |
 | `WRITEPETS` | modify pets in your account |
 
 ## List of APIs
 
-* [Pet](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/store.md)
-* [User](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/http-request.md)
```

### Comparing `tester-package-sdk-1.0.8/README.md` & `tester-package-sdk-2.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install tester-package-sdk==1.0.8
+pip install tester-package-sdk==2.0.9
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/tester-package-sdk/1.0.8
+https://pypi.python.org/pypi/tester-package-sdk/2.0.9
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -91,17 +91,17 @@
 | Scope Name | Description |
 |  --- | --- |
 | `READPETS` | read your pets |
 | `WRITEPETS` | modify pets in your account |
 
 ## List of APIs
 
-* [Pet](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/store.md)
-* [User](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/http-request.md)
```

### Comparing `tester-package-sdk-1.0.8/pyproject.toml` & `tester-package-sdk-2.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "tester-package-sdk"
 description = "this is testing please ignore"
-version = "1.0.8"
+version = "2.0.9"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["this", "is"]
 authors = [{name = "Subtain", email = "Subtain@gmail.com"}]
 urls = {Documentation = "https://subtain.com"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10", "deprecation~=2.1"]
 classifiers = []
```

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/api_helper.py` & `tester-package-sdk-2.0.9/swaggerpetstore/api_helper.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/configuration.py` & `tester-package-sdk-2.0.9/swaggerpetstore/configuration.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/controllers/base_controller.py` & `tester-package-sdk-2.0.9/swaggerpetstore/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/controllers/pet_controller.py` & `tester-package-sdk-2.0.9/swaggerpetstore/controllers/pet_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,75 @@
 from apimatic_core.request_builder import RequestBuilder
 from apimatic_core.response_handler import ResponseHandler
 from apimatic_core.types.parameter import Parameter
 from swaggerpetstore.http.http_method_enum import HttpMethodEnum
 from apimatic_core.authentication.multiple.single_auth import Single
 from apimatic_core.authentication.multiple.and_auth_group import And
 from apimatic_core.authentication.multiple.or_auth_group import Or
-from swaggerpetstore.models.pet import Pet
 from swaggerpetstore.models.api_response import ApiResponse
+from swaggerpetstore.models.pet import Pet
 from swaggerpetstore.exceptions.api_exception import APIException
 
 
 class PetController(BaseController):
 
     """A Controller to access Endpoints in the swaggerpetstore API."""
     def __init__(self, config):
         super(PetController, self).__init__(config)
 
+    def upload_file(self,
+                    pet_id,
+                    additional_metadata=None,
+                    file=None):
+        """Does a POST request to /pet/{petId}/uploadImage.
+
+        uploads an image
+
+        Args:
+            pet_id (long|int): ID of pet to update
+            additional_metadata (string, optional): Additional data to pass to
+                server
+            file (typing.BinaryIO, optional): file to upload
+
+        Returns:
+            ApiResponse: Response from the API. successful operation
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        return super().new_api_call_builder.request(
+            RequestBuilder().server(Server.SERVER1)
+            .path('/pet/{petId}/uploadImage')
+            .http_method(HttpMethodEnum.POST)
+            .template_param(Parameter()
+                            .key('petId')
+                            .value(pet_id)
+                            .should_encode(True))
+            .form_param(Parameter()
+                        .key('additionalMetadata')
+                        .value(additional_metadata))
+            .multipart_param(Parameter()
+                             .key('file')
+                             .value(file)
+                             .default_content_type('application/octet-stream'))
+            .header_param(Parameter()
+                          .key('accept')
+                          .value('application/json'))
+            .auth(Single('global'))
+        ).response(
+            ResponseHandler()
+            .deserializer(APIHelper.json_deserialize)
+            .deserialize_into(ApiResponse.from_dictionary)
+        ).execute()
+
     def add_pet(self,
                 body):
         """Does a POST request to /pet.
 
         Add a new pet to the store
 
         Args:
@@ -92,14 +142,53 @@
             .header_param(Parameter()
                           .key('Content-Type')
                           .value('application/json'))
             .body_serializer(APIHelper.json_serialize)
             .auth(Single('global'))
         ).execute()
 
+    def find_pets_by_status(self,
+                            status):
+        """Does a GET request to /pet/findByStatus.
+
+        Multiple status values can be provided with comma separated strings
+
+        Args:
+            status (list of Status2Enum): Status values that need to be
+                considered for filter
+
+        Returns:
+            list of Pet: Response from the API. successful operation
+
+        Raises:
+            APIException: When an error occurs while fetching the data from
+                the remote API. This exception includes the HTTP Response
+                code, an error message, and the HTTP body that was received in
+                the request.
+
+        """
+
+        return super().new_api_call_builder.request(
+            RequestBuilder().server(Server.SERVER1)
+            .path('/pet/findByStatus')
+            .http_method(HttpMethodEnum.GET)
+            .query_param(Parameter()
+                         .key('status')
+                         .value(status))
+            .header_param(Parameter()
+                          .key('accept')
+                          .value('application/json'))
+            .auth(Single('global'))
+        ).response(
+            ResponseHandler()
+            .deserializer(APIHelper.json_deserialize)
+            .deserialize_into(Pet.from_dictionary)
+            .local_error('400', 'Invalid status value', APIException)
+        ).execute()
+
     @deprecated()
     def find_pets_by_tags(self,
                           tags):
         """Does a GET request to /pet/findByTags.
 
         Multiple tags can be provided with comma separated strings. Use tag1,
         tag2, tag3 for testing.
@@ -172,24 +261,26 @@
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
             .deserialize_into(Pet.from_dictionary)
             .local_error('400', 'Invalid ID supplied', APIException)
             .local_error('404', 'Pet not found', APIException)
         ).execute()
 
-    def delete_pet(self,
-                   pet_id,
-                   api_key=None):
-        """Does a DELETE request to /pet/{petId}.
+    def update_pet_with_form(self,
+                             pet_id,
+                             name=None,
+                             status=None):
+        """Does a POST request to /pet/{petId}.
 
-        Deletes a pet
+        Updates a pet in the store with form data
 
         Args:
-            pet_id (long|int): Pet id to delete
-            api_key (string, optional): TODO: type description here.
+            pet_id (long|int): ID of pet that needs to be updated
+            name (string, optional): Updated name of the pet
+            status (string, optional): Updated status of the pet
 
         Returns:
             void: Response from the API.
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
@@ -197,126 +288,41 @@
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
             .path('/pet/{petId}')
-            .http_method(HttpMethodEnum.DELETE)
-            .template_param(Parameter()
-                            .key('petId')
-                            .value(pet_id)
-                            .should_encode(True))
-            .header_param(Parameter()
-                          .key('api_key')
-                          .value(api_key))
-            .auth(Single('global'))
-        ).execute()
-
-    def upload_file(self,
-                    pet_id,
-                    additional_metadata=None,
-                    file=None):
-        """Does a POST request to /pet/{petId}/uploadImage.
-
-        uploads an image
-
-        Args:
-            pet_id (long|int): ID of pet to update
-            additional_metadata (string, optional): Additional data to pass to
-                server
-            file (typing.BinaryIO, optional): file to upload
-
-        Returns:
-            ApiResponse: Response from the API. successful operation
-
-        Raises:
-            APIException: When an error occurs while fetching the data from
-                the remote API. This exception includes the HTTP Response
-                code, an error message, and the HTTP body that was received in
-                the request.
-
-        """
-
-        return super().new_api_call_builder.request(
-            RequestBuilder().server(Server.SERVER1)
-            .path('/pet/{petId}/uploadImage')
             .http_method(HttpMethodEnum.POST)
             .template_param(Parameter()
                             .key('petId')
                             .value(pet_id)
                             .should_encode(True))
             .form_param(Parameter()
-                        .key('additionalMetadata')
-                        .value(additional_metadata))
-            .multipart_param(Parameter()
-                             .key('file')
-                             .value(file)
-                             .default_content_type('application/octet-stream'))
-            .header_param(Parameter()
-                          .key('accept')
-                          .value('application/json'))
-            .auth(Single('global'))
-        ).response(
-            ResponseHandler()
-            .deserializer(APIHelper.json_deserialize)
-            .deserialize_into(ApiResponse.from_dictionary)
-        ).execute()
-
-    def find_pets_by_status(self,
-                            status):
-        """Does a GET request to /pet/findByStatus.
-
-        Multiple status values can be provided with comma separated strings
-
-        Args:
-            status (list of Status2Enum): Status values that need to be
-                considered for filter
-
-        Returns:
-            list of Pet: Response from the API. successful operation
-
-        Raises:
-            APIException: When an error occurs while fetching the data from
-                the remote API. This exception includes the HTTP Response
-                code, an error message, and the HTTP body that was received in
-                the request.
-
-        """
-
-        return super().new_api_call_builder.request(
-            RequestBuilder().server(Server.SERVER1)
-            .path('/pet/findByStatus')
-            .http_method(HttpMethodEnum.GET)
-            .query_param(Parameter()
-                         .key('status')
-                         .value(status))
+                        .key('name')
+                        .value(name))
+            .form_param(Parameter()
+                        .key('status')
+                        .value(status))
             .header_param(Parameter()
-                          .key('accept')
-                          .value('application/json'))
+                          .key('content-type')
+                          .value('application/x-www-form-urlencoded'))
             .auth(Single('global'))
-        ).response(
-            ResponseHandler()
-            .deserializer(APIHelper.json_deserialize)
-            .deserialize_into(Pet.from_dictionary)
-            .local_error('400', 'Invalid status value', APIException)
         ).execute()
 
-    def update_pet_with_form(self,
-                             pet_id,
-                             name=None,
-                             status=None):
-        """Does a POST request to /pet/{petId}.
+    def delete_pet(self,
+                   pet_id,
+                   api_key=None):
+        """Does a DELETE request to /pet/{petId}.
 
-        Updates a pet in the store with form data
+        Deletes a pet
 
         Args:
-            pet_id (long|int): ID of pet that needs to be updated
-            name (string, optional): Updated name of the pet
-            status (string, optional): Updated status of the pet
+            pet_id (long|int): Pet id to delete
+            api_key (string, optional): TODO: type description here.
 
         Returns:
             void: Response from the API.
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
@@ -324,23 +330,17 @@
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
             .path('/pet/{petId}')
-            .http_method(HttpMethodEnum.POST)
+            .http_method(HttpMethodEnum.DELETE)
             .template_param(Parameter()
                             .key('petId')
                             .value(pet_id)
                             .should_encode(True))
-            .form_param(Parameter()
-                        .key('name')
-                        .value(name))
-            .form_param(Parameter()
-                        .key('status')
-                        .value(status))
             .header_param(Parameter()
-                          .key('content-type')
-                          .value('application/x-www-form-urlencoded'))
+                          .key('api_key')
+                          .value(api_key))
             .auth(Single('global'))
         ).execute()
```

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/controllers/store_controller.py` & `tester-package-sdk-2.0.9/swaggerpetstore/controllers/store_controller.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/controllers/user_controller.py` & `tester-package-sdk-2.0.9/swaggerpetstore/controllers/user_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,92 +56,86 @@
             .header_param(Parameter()
                           .key('Content-Type')
                           .value('application/json'))
             .body_serializer(APIHelper.json_serialize)
             .auth(Single('global'))
         ).execute()
 
-    def get_user_by_name(self,
-                         username):
-        """Does a GET request to /user/{username}.
+    def create_users_with_list_input(self,
+                                     body):
+        """Does a POST request to /user/createWithList.
 
-        Get user by user name
+        Creates list of users with given input array
 
         Args:
-            username (string): The name that needs to be fetched. Use user1
-                for testing.
+            body (list of User): List of user object
 
         Returns:
-            User: Response from the API. successful operation
+            void: Response from the API.
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
                 code, an error message, and the HTTP body that was received in
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
-            .path('/user/{username}')
-            .http_method(HttpMethodEnum.GET)
-            .template_param(Parameter()
-                            .key('username')
-                            .value(username)
-                            .should_encode(True))
+            .path('/user/createWithList')
+            .http_method(HttpMethodEnum.POST)
+            .body_param(Parameter()
+                        .value(body))
             .header_param(Parameter()
-                          .key('accept')
+                          .key('Content-Type')
                           .value('application/json'))
+            .body_serializer(APIHelper.json_serialize)
             .auth(Single('global'))
-        ).response(
-            ResponseHandler()
-            .deserializer(APIHelper.json_deserialize)
-            .deserialize_into(User.from_dictionary)
-            .local_error('400', 'Invalid username supplied', APIException)
-            .local_error('404', 'User not found', APIException)
         ).execute()
 
-    def login_user(self,
-                   username,
-                   password):
-        """Does a GET request to /user/login.
+    def get_user_by_name(self,
+                         username):
+        """Does a GET request to /user/{username}.
 
-        Logs user into the system
+        Get user by user name
 
         Args:
-            username (string): The user name for login
-            password (string): The password for login in clear text
+            username (string): The name that needs to be fetched. Use user1
+                for testing.
 
         Returns:
-            string: Response from the API. successful operation
+            User: Response from the API. successful operation
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
                 code, an error message, and the HTTP body that was received in
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
-            .path('/user/login')
+            .path('/user/{username}')
             .http_method(HttpMethodEnum.GET)
-            .query_param(Parameter()
-                         .key('username')
-                         .value(username))
-            .query_param(Parameter()
-                         .key('password')
-                         .value(password))
+            .template_param(Parameter()
+                            .key('username')
+                            .value(username)
+                            .should_encode(True))
+            .header_param(Parameter()
+                          .key('accept')
+                          .value('application/json'))
             .auth(Single('global'))
         ).response(
             ResponseHandler()
             .deserializer(APIHelper.json_deserialize)
-            .local_error('400', 'Invalid username/password supplied', APIException)
+            .deserialize_into(User.from_dictionary)
+            .local_error('400', 'Invalid username supplied', APIException)
+            .local_error('404', 'User not found', APIException)
         ).execute()
 
     def update_user(self,
                     username,
                     body):
         """Does a PUT request to /user/{username}.
 
@@ -206,45 +200,51 @@
             .template_param(Parameter()
                             .key('username')
                             .value(username)
                             .should_encode(True))
             .auth(Single('global'))
         ).execute()
 
-    def create_users_with_list_input(self,
-                                     body):
-        """Does a POST request to /user/createWithList.
+    def login_user(self,
+                   username,
+                   password):
+        """Does a GET request to /user/login.
 
-        Creates list of users with given input array
+        Logs user into the system
 
         Args:
-            body (list of User): List of user object
+            username (string): The user name for login
+            password (string): The password for login in clear text
 
         Returns:
-            void: Response from the API.
+            string: Response from the API. successful operation
 
         Raises:
             APIException: When an error occurs while fetching the data from
                 the remote API. This exception includes the HTTP Response
                 code, an error message, and the HTTP body that was received in
                 the request.
 
         """
 
         return super().new_api_call_builder.request(
             RequestBuilder().server(Server.SERVER1)
-            .path('/user/createWithList')
-            .http_method(HttpMethodEnum.POST)
-            .body_param(Parameter()
-                        .value(body))
-            .header_param(Parameter()
-                          .key('Content-Type')
-                          .value('application/json'))
-            .body_serializer(APIHelper.json_serialize)
+            .path('/user/login')
+            .http_method(HttpMethodEnum.GET)
+            .query_param(Parameter()
+                         .key('username')
+                         .value(username))
+            .query_param(Parameter()
+                         .key('password')
+                         .value(password))
             .auth(Single('global'))
+        ).response(
+            ResponseHandler()
+            .deserializer(APIHelper.json_deserialize)
+            .local_error('400', 'Invalid username/password supplied', APIException)
         ).execute()
 
     def logout_user(self):
         """Does a GET request to /user/logout.
 
         Logs out current logged in user session
```

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/exceptions/api_exception.py` & `tester-package-sdk-2.0.9/swaggerpetstore/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/exceptions/o_auth_provider_exception.py` & `tester-package-sdk-2.0.9/swaggerpetstore/exceptions/o_auth_provider_exception.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/http/http_request.py` & `tester-package-sdk-2.0.9/swaggerpetstore/http/http_request.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/http/http_response.py` & `tester-package-sdk-2.0.9/swaggerpetstore/http/http_response.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/api_response.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/api_response.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/category.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/category.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/o_auth_provider_error_enum.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/o_auth_provider_error_enum.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/o_auth_token.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/o_auth_token.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/order.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/order.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/pet.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/pet.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/status_2_enum.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/status_2_enum.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/tag.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/tag.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/models/user.py` & `tester-package-sdk-2.0.9/swaggerpetstore/models/user.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/swaggerpetstore/swaggerpetstore_client.py` & `tester-package-sdk-2.0.9/swaggerpetstore/swaggerpetstore_client.py`

 * *Files identical despite different names*

### Comparing `tester-package-sdk-1.0.8/tester_package_sdk.egg-info/PKG-INFO` & `tester-package-sdk-2.0.9/tester_package_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tester-package-sdk
-Version: 1.0.8
+Version: 2.0.9
 Summary: this is testing please ignore
 Author-email: Subtain <Subtain@gmail.com>
 Project-URL: Documentation, https://subtain.com
 Keywords: this,is
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -21,23 +21,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install tester-package-sdk==1.0.8
+pip install tester-package-sdk==2.0.9
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/tester-package-sdk/1.0.8
+https://pypi.python.org/pypi/tester-package-sdk/2.0.9
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
 | `http_client_instance` | `HttpClient` | The Http Client passed from the sdk user for making requests |
@@ -103,17 +103,17 @@
 | Scope Name | Description |
 |  --- | --- |
 | `READPETS` | read your pets |
 | `WRITEPETS` | modify pets in your account |
 
 ## List of APIs
 
-* [Pet](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/pet.md)
-* [Store](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/store.md)
-* [User](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/controllers/user.md)
+* [Pet](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/pet.md)
+* [Store](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/store.md)
+* [User](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/controllers/user.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/http-response.md)
-* [HttpRequest](https://www.github.com/sdks-io/new-repository-python/tree/1.0.8/doc/http-request.md)
+* [Utility Classes](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/http-response.md)
+* [HttpRequest](https://www.github.com/Syed-Subtain/sync-pack-python-sdk/tree/2.0.9/doc/http-request.md)
```

### Comparing `tester-package-sdk-1.0.8/tester_package_sdk.egg-info/SOURCES.txt` & `tester-package-sdk-2.0.9/tester_package_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


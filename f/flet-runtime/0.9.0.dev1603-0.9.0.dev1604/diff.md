# Comparing `tmp/flet_runtime-0.9.0.dev1603.tar.gz` & `tmp/flet_runtime-0.9.0.dev1604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_runtime-0.9.0.dev1603.tar", max compression
+gzip compressed data, was "flet_runtime-0.9.0.dev1604.tar", max compression
```

## Comparing `flet_runtime-0.9.0.dev1603.tar` & `flet_runtime-0.9.0.dev1604.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      204 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/README.md
--rw-r--r--   0        0        0      747 2023-07-06 01:34:09.953677 flet_runtime-0.9.0.dev1603/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    23719 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/app.py
--rw-r--r--   0        0        0     6309 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/async_local_socket_connection.py
--rw-r--r--   0        0        0      252 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0     9107 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1515 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0    10255 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/pubsub.py
--rw-r--r--   0        0        0     6934 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/sync_local_socket_connection.py
--rw-r--r--   0        0        0     3593 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/utils.py
--rw-r--r--   0        0        0      103 2023-07-06 01:33:30.014795 flet_runtime-0.9.0.dev1603/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.9.0.dev1603/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/README.md
+-rw-r--r--   0        0        0      747 2023-07-06 16:34:12.868829 flet_runtime-0.9.0.dev1604/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    23719 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/app.py
+-rw-r--r--   0        0        0     6309 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/async_local_socket_connection.py
+-rw-r--r--   0        0        0      252 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0     9107 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1515 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0    10255 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/pubsub.py
+-rw-r--r--   0        0        0     6934 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     3593 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/utils.py
+-rw-r--r--   0        0        0      103 2023-07-06 16:33:37.320957 flet_runtime-0.9.0.dev1604/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 flet_runtime-0.9.0.dev1604/PKG-INFO
```

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/app.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/app.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/async_local_socket_connection.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/authorization.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/oauth_provider.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/oauth_token.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/pubsub.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/sync_local_socket_connection.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/src/flet_runtime/utils.py` & `flet_runtime-0.9.0.dev1604/src/flet_runtime/utils.py`

 * *Files identical despite different names*

### Comparing `flet_runtime-0.9.0.dev1603/PKG-INFO` & `flet_runtime-0.9.0.dev1604/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-runtime
-Version: 0.9.0.dev1603
+Version: 0.9.0.dev1604
 Summary: Flet Runtime - a base package for Flet desktop and Flet mobile.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.9.0.dev1603)
+Requires-Dist: flet-core (==0.9.0.dev1604)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0) ; python_version < "3.8"
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
```


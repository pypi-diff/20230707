# Comparing `tmp/splight-lib-3.1.0.dev2.tar.gz` & `tmp/splight-lib-3.1.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.1.0.dev2.tar", last modified: Tue Jul  4 20:19:06 2023, max compression
+gzip compressed data, was "splight-lib-3.1.0.dev3.tar", last modified: Thu Jul  6 14:51:07 2023, max compression
```

## Comparing `splight-lib-3.1.0.dev2.tar` & `splight-lib-3.1.0.dev3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.058694 splight-lib-3.1.0.dev2/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/grpc/reflector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/log_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.062694 splight-lib-3.1.0.dev2/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.066694 splight-lib-3.1.0.dev2/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 20:19:05.000000 splight-lib-3.1.0.dev2/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 20:19:06.054694 splight-lib-3.1.0.dev2/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-04 20:19:06.000000 splight-lib-3.1.0.dev2/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.399278 splight-lib-3.1.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 14:51:07.399278 splight-lib-3.1.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:51:07.399278 splight-lib-3.1.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.387277 splight-lib-3.1.0.dev3/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib/client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/grpc/reflector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/component/log_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.395278 splight-lib-3.1.0.dev3/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 14:51:06.000000 splight-lib-3.1.0.dev3/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:51:07.391278 splight-lib-3.1.0.dev3/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 14:51:07.000000 splight-lib-3.1.0.dev3/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-06 14:51:07.000000 splight-lib-3.1.0.dev3/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:51:07.000000 splight-lib-3.1.0.dev3/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:51:07.000000 splight-lib-3.1.0.dev3/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-06 14:51:07.000000 splight-lib-3.1.0.dev3/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 14:51:07.000000 splight-lib-3.1.0.dev3/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.1.0.dev2/PKG-INFO` & `splight-lib-3.1.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.0.dev2
+Version: 3.1.0.dev3
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.0.dev2/setup.py` & `splight-lib-3.1.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.1.0.dev2",
+    version="3.1.0.dev3",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.1.0.dev2/splight_lib/abstract/client.py` & `splight-lib-3.1.0.dev3/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/auth/mac_auth.py` & `splight-lib-3.1.0.dev3/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/communication/abstract.py` & `splight-lib-3.1.0.dev3/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/communication/remote_client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/database/abstract.py` & `splight-lib-3.1.0.dev3/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/database/builder.py` & `splight-lib-3.1.0.dev3/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/database/classmap.py` & `splight-lib-3.1.0.dev3/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/database/local_client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/database/remote_client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/datalake/abstract.py` & `splight-lib-3.1.0.dev3/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/datalake/builder.py` & `splight-lib-3.1.0.dev3/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/datalake/local_client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/exceptions.py` & `splight-lib-3.1.0.dev3/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/file_handler.py` & `splight-lib-3.1.0.dev3/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/filter.py` & `splight-lib-3.1.0.dev3/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/grpc/client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/grpc/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/grpc/reflector.py` & `splight-lib-3.1.0.dev3/splight_lib/client/grpc/reflector.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/hub/abstract.py` & `splight-lib-3.1.0.dev3/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/client/hub/client.py` & `splight-lib-3.1.0.dev3/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/communication/event_handler.py` & `splight-lib-3.1.0.dev3/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/component/abstract.py` & `splight-lib-3.1.0.dev3/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/component/exceptions.py` & `splight-lib-3.1.0.dev3/splight_lib/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/component/log_streamer.py` & `splight-lib-3.1.0.dev3/splight_lib/component/log_streamer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,21 @@
     def start(self):
         self._run()
 
     def stop(self):
         self._thread.stop()
 
     def _run(self):
-        # for msg in self.logs_iterator():
-        #     continue
         self._client.stream_logs(self.logs_iterator, self._component_id)
 
     def logs_iterator(self) -> Generator:
         self._message_buffer = []
         reader = iter(self._process.stdout.readline, "")
         for new_line in reader:
             if self._process.poll() is not None:
-                print("CRASHED")
                 msg = "".join(self._message_buffer)
                 sys.stdout.write(msg)
                 yield msg
                 output, error = self._process.communicate()
                 output_msg = output.decode("utf-8")
                 error_msg = error.decode("utf-8")
                 sys.stdout.write(output_msg)
```

### Comparing `splight-lib-3.1.0.dev2/splight_lib/component/spec.py` & `splight-lib-3.1.0.dev3/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/encryption.py` & `splight-lib-3.1.0.dev3/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/execution.py` & `splight-lib-3.1.0.dev3/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/logging/component.py` & `splight-lib-3.1.0.dev3/splight_lib/logging/component.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import os
-from logging import INFO, Formatter, Handler  # , basicConfig
+from logging import INFO, Formatter, Handler
 from typing import Optional
 
 from concurrent_log_handler import ConcurrentRotatingFileHandler
-# from splight_lib.logging.constants import LOGGING_COMPONENTS
 from splight_lib.logging.logging import (
-    # ElasticDocumentFormatter,
     SplightFormatter,
     SplightLogger,
-    # elastic_document_handler,
     standard_output_handler,
 )
 
 
 def component_file_handler(
     formatter: Optional[Formatter] = SplightFormatter(),
     log_level: Optional[str] = INFO,
@@ -35,19 +32,14 @@
         name = "component"
     logger = SplightLogger(name=name)
     logger.propagate = False
     stdout_handler = standard_output_handler(log_level=logger.level)
     logger.addHandler(stdout_handler)
     file_handler = component_file_handler(log_level=logger.level)
     logger.addHandler(file_handler)
-    # es_handler = elastic_document_handler(
-    #     formatter=ElasticDocumentFormatter(type=LOGGING_COMPONENTS),
-    #     log_level=logger.level,
-    # )
-    # logger.addHandler(es_handler)
 
     # Add logger.level to root logger
     logger.setLevel(logger.level)
     return logger
 
 
 def getLogger(name: Optional[str] = None):
```

### Comparing `splight-lib-3.1.0.dev2/splight_lib/logging/logging.py` & `splight-lib-3.1.0.dev3/splight_lib/logging/logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-# import json
+import time
 import os
 import sys
-# import time
 from logging import (
     CRITICAL,
     DEBUG,
     ERROR,
     INFO,
-    NOTSET,
     WARNING,
     Formatter,
     Handler,
     Logger,
     StreamHandler,
 )
 from logging import root as rootLogger
 from typing import Dict, Optional
 
-# from concurrent_log_handler import ConcurrentRotatingFileHandler
-# from pydantic import BaseSettings
-# from splight_lib.logging.constants import LOGGING_DEV, LogType
-
 TAGS_KEY = "tags"
 
 
 class SplightFormatter(Formatter):
     DEFAULT_FMT: str = (
         "%(levelname)s | %(asctime)s | %(filename)s:%(lineno)d | %(message)s"
     )
@@ -32,43 +26,19 @@
     def format(self, record):
         fmt = self.DEFAULT_FMT
         try:
             if record.tags is not None:
                 fmt = " | ".join([fmt, "%(tags)s"])
         except AttributeError:
             pass  # tags aren't present
-        formatter = Formatter(fmt=fmt, datefmt="%Y-%m-%dT%H:%M:%S%z")
-        # formatter.converter = time.gmtime
+        formatter = Formatter(fmt=fmt, datefmt="%Y-%m-%dT%H:%M:%SZ")
+        formatter.converter = time.gmtime
         return formatter.format(record)
 
 
-# class SplightExceptionFormatter(SplightFormatter):
-#     def format(self, record):
-#         fmt = self.DEFAULT_FMT
-#
-#         __import__('ipdb').set_trace()
-#         formatter = Formatter(fmt=fmt, datefmt="%Y-%m-%dT%H:%M:%S%z")
-#         return formatter.format(record)
-
-
-# class ElasticDocumentFormatter(Formatter):
-#     def __init__(self, fmt: str = None, type: LogType = LOGGING_DEV) -> None:
-#         super().__init__(fmt=fmt)
-#         self.type = type
-#
-#     @property
-#     def _extra_fields(self) -> Dict:
-#         return {
-#             "type": self.type,
-#         }
-#
-#     def format(self, record):
-#         return json.dumps({**record.__dict__, **self._extra_fields})
-
-
 class SplightLogger(Logger):
     def __init__(self, name: str = None) -> None:
         # this is to avoid adding handlers to root logger
         # and interfering with third party app logs
         self.name = name if name is not None else "splight"
         level = int(os.getenv("LOG_LEVEL", INFO))
         super().__init__(name, level)
@@ -170,34 +140,7 @@
     formatter: Optional[Formatter] = SplightFormatter(),
     log_level: Optional[str] = INFO,
 ) -> Handler:
     handler = StreamHandler(sys.stdout)
     handler.setFormatter(formatter)
     handler.setLevel(log_level)
     return handler
-
-
-# class ElasticDocumentHandlerSettings(BaseSettings):
-#     splight_elastic_logs_filename: str = "/tmp/splight_elastic_logs.log"
-#     splight_elastic_logs_max_bytes: int = 5e6
-#     splight_elastic_logs_backup_count: int = 5
-#
-#     @property
-#     def file_handler_settings(self) -> Dict:
-#         return {
-#             "filename": self.splight_elastic_logs_filename,
-#             "maxBytes": self.splight_elastic_logs_max_bytes,
-#             "backupCount": self.splight_elastic_logs_backup_count,
-#             "encoding": "utf-8",
-#         }
-#
-#
-# def elastic_document_handler(
-#     formatter: Optional[Formatter] = SplightFormatter(),
-#     log_level: Optional[str] = INFO,
-# ) -> Handler:
-#     settings = ElasticDocumentHandlerSettings()
-#     handler = ConcurrentRotatingFileHandler(**settings.file_handler_settings)
-#
-#     handler.setFormatter(formatter)
-#     handler.setLevel(log_level)
-#     return handler
```

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/__init__.py` & `splight-lib-3.1.0.dev3/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/alert.py` & `splight-lib-3.1.0.dev3/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/asset.py` & `splight-lib-3.1.0.dev3/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/base.py` & `splight-lib-3.1.0.dev3/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/communication.py` & `splight-lib-3.1.0.dev3/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/component.py` & `splight-lib-3.1.0.dev3/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/dashboard.py` & `splight-lib-3.1.0.dev3/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/event.py` & `splight-lib-3.1.0.dev3/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/file.py` & `splight-lib-3.1.0.dev3/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/hub.py` & `splight-lib-3.1.0.dev3/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/native.py` & `splight-lib-3.1.0.dev3/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/query.py` & `splight-lib-3.1.0.dev3/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/models/setpoint.py` & `splight-lib-3.1.0.dev3/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/restclient/client.py` & `splight-lib-3.1.0.dev3/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/restclient/exceptions.py` & `splight-lib-3.1.0.dev3/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/restclient/types.py` & `splight-lib-3.1.0.dev3/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/settings.py` & `splight-lib-3.1.0.dev3/splight_lib/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     return config
 
 
 class SplightSettings(BaseSettings, Singleton):
     SPLIGHT_ACCESS_ID: str = ""
     SPLIGHT_SECRET_KEY: str = ""
     SPLIGHT_PLATFORM_API_HOST: str = "https://api.splight-ai.com"
-    SPLIGHT_GRPC_HOST: str = "integrationgrpc.splight-ai.com:443"
-    # SPLIGHT_GRPC_HOST: str = "grpc.splight-ai.com:443"
+    SPLIGHT_GRPC_HOST: str = "grpc.splight-ai.com:443"
 
     # Parameters for local environment
     LOCAL_ENVIRONMENT: bool = False
     CURRENT_DIR: Optional[str]
 
     @root_validator(allow_reuse=True)
     def validate_local_environment(cls, values: Dict):
```

### Comparing `splight-lib-3.1.0.dev2/splight_lib/testing/__init__.py` & `splight-lib-3.1.0.dev3/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/utils/custom_model.py` & `splight-lib-3.1.0.dev3/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/utils/hub.py` & `splight-lib-3.1.0.dev3/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib/webhook.py` & `splight-lib-3.1.0.dev3/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.1.0.dev3/splight_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.0.dev2
+Version: 3.1.0.dev3
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.0.dev2/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.1.0.dev3/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.0.dev2/splight_lib.egg-info/requires.txt` & `splight-lib-3.1.0.dev3/splight_lib.egg-info/requires.txt`

 * *Files identical despite different names*


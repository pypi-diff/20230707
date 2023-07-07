# Comparing `tmp/apexpro-1.1.4.tar.gz` & `tmp/apexpro-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apexpro-1.1.4.tar", last modified: Wed Jul  5 05:58:16 2023, max compression
+gzip compressed data, was "apexpro-1.1.5.tar", last modified: Fri Jul  7 07:02:45 2023, max compression
```

## Comparing `apexpro-1.1.4.tar` & `apexpro-1.1.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.712233 apexpro-1.1.4/
--rw-r--r--   0 dl00015ml   (502) staff       (20)      363 2022-07-15 03:54:05.000000 apexpro-1.1.4/CHANGELOG.md
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1218 2022-11-25 01:02:08.000000 apexpro-1.1.4/LICENSE
--rw-r--r--   0 dl00015ml   (502) staff       (20)       83 2022-07-15 03:54:05.000000 apexpro-1.1.4/MANIFEST.in
--rw-r--r--   0 dl00015ml   (502) staff       (20)     9088 2023-07-05 05:58:16.712335 apexpro-1.1.4/PKG-INFO
--rw-r--r--   0 dl00015ml   (502) staff       (20)     8344 2022-12-09 13:23:37.000000 apexpro-1.1.4/README.md
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.699748 apexpro-1.1.4/apexpro/
--rw-r--r--   0 dl00015ml   (502) staff       (20)    14806 2022-12-22 07:57:17.000000 apexpro-1.1.4/apexpro/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     9982 2022-09-16 09:30:41.000000 apexpro-1.1.4/apexpro/_websocket_stream.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1591 2022-09-29 09:49:57.000000 apexpro-1.1.4/apexpro/constants.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      874 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/errors.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    16581 2022-12-22 07:57:17.000000 apexpro-1.1.4/apexpro/eth.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.702950 apexpro-1.1.4/apexpro/eth_signing/
--rw-r--r--   0 dl00015ml   (502) staff       (20)      246 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/eth_signing/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1812 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/eth_signing/eth_prive_action.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2617 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/eth_signing/onboarding_action.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3896 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/eth_signing/sign_off_chain_action.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3334 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/eth_signing/signers.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2749 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/eth_signing/util.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1318 2022-11-25 01:02:08.000000 apexpro-1.1.4/apexpro/exceptions.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.704353 apexpro-1.1.4/apexpro/helpers/
--rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/helpers/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      348 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/helpers/db.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2570 2022-09-16 09:30:41.000000 apexpro-1.1.4/apexpro/helpers/request_helpers.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1077 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/helpers/requests.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      840 2023-07-05 05:49:58.000000 apexpro-1.1.4/apexpro/helpers/util.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    19983 2023-07-05 05:49:58.000000 apexpro-1.1.4/apexpro/http_private.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    16177 2023-05-24 06:10:59.000000 apexpro-1.1.4/apexpro/http_private_stark_key_sign.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3245 2023-07-05 05:49:58.000000 apexpro-1.1.4/apexpro/http_public.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      127 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/models.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.706373 apexpro-1.1.4/apexpro/starkex/
--rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     4238 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/conditional_transfer.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1558 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/constants.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     5844 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/helpers.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     6588 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/order.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1124 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/signable.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.708020 apexpro-1.1.4/apexpro/starkex/starkex_resources/
--rw-r--r--   0 dl00015ml   (502) staff       (20)      285 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/starkex_resources/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3089 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/starkex_resources/cpp_signature.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3627 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/starkex_resources/math_utils.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)   102708 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/starkex_resources/pedersen_params.json
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1346 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/starkex_resources/proxy.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    10414 2022-07-15 03:54:05.000000 apexpro-1.1.4/apexpro/starkex/starkex_resources/python_signature.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3812 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/transfer.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2631 2022-08-25 03:55:08.000000 apexpro-1.1.4/apexpro/starkex/withdrawal.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     4578 2023-05-24 06:10:59.000000 apexpro-1.1.4/apexpro/websocket_api.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.701246 apexpro-1.1.4/apexpro.egg-info/
--rw-r--r--   0 dl00015ml   (502) staff       (20)     9088 2023-07-05 05:58:16.000000 apexpro-1.1.4/apexpro.egg-info/PKG-INFO
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1658 2023-07-05 05:58:16.000000 apexpro-1.1.4/apexpro.egg-info/SOURCES.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2023-07-05 05:58:16.000000 apexpro-1.1.4/apexpro.egg-info/dependency_links.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2022-07-15 06:12:12.000000 apexpro-1.1.4/apexpro.egg-info/not-zip-safe
--rw-r--r--   0 dl00015ml   (502) staff       (20)      245 2023-07-05 05:58:16.000000 apexpro-1.1.4/apexpro.egg-info/requires.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)       14 2023-07-05 05:58:16.000000 apexpro-1.1.4/apexpro.egg-info/top_level.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)      131 2023-07-05 05:58:16.712783 apexpro-1.1.4/setup.cfg
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1656 2023-07-05 05:56:24.000000 apexpro-1.1.4/setup.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-05 05:58:16.711903 apexpro-1.1.4/tests/
--rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.4/tests/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     5582 2022-11-27 04:45:32.000000 apexpro-1.1.4/tests/account_value.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      147 2022-07-15 03:54:05.000000 apexpro-1.1.4/tests/constants.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1904 2022-12-22 07:57:17.000000 apexpro-1.1.4/tests/demo_deposit.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2817 2023-02-09 06:01:49.000000 apexpro-1.1.4/tests/demo_private.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      844 2022-09-16 09:30:41.000000 apexpro-1.1.4/tests/demo_public.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1433 2022-12-22 07:57:17.000000 apexpro-1.1.4/tests/demo_register.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1503 2022-11-23 00:41:45.000000 apexpro-1.1.4/tests/demo_register_mul_address.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      583 2022-09-29 09:49:57.000000 apexpro-1.1.4/tests/demo_sign.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2927 2023-05-24 06:10:59.000000 apexpro-1.1.4/tests/demo_stark_key_sign.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      962 2022-12-09 13:23:37.000000 apexpro-1.1.4/tests/demo_ws.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     5573 2022-08-25 03:55:08.000000 apexpro-1.1.4/tests/test_onboarding.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.454831 apexpro-1.1.5/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      363 2022-07-15 03:54:05.000000 apexpro-1.1.5/CHANGELOG.md
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1218 2022-11-25 01:02:08.000000 apexpro-1.1.5/LICENSE
+-rw-r--r--   0 dl00015ml   (502) staff       (20)       83 2022-07-15 03:54:05.000000 apexpro-1.1.5/MANIFEST.in
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     9088 2023-07-07 07:02:45.454911 apexpro-1.1.5/PKG-INFO
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     8344 2022-12-09 13:23:37.000000 apexpro-1.1.5/README.md
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.444125 apexpro-1.1.5/apexpro/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    14806 2022-12-22 07:57:17.000000 apexpro-1.1.5/apexpro/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     9982 2022-09-16 09:30:41.000000 apexpro-1.1.5/apexpro/_websocket_stream.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1591 2022-09-29 09:49:57.000000 apexpro-1.1.5/apexpro/constants.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      874 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/errors.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    16581 2022-12-22 07:57:17.000000 apexpro-1.1.5/apexpro/eth.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.447121 apexpro-1.1.5/apexpro/eth_signing/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      246 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/eth_signing/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1812 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/eth_signing/eth_prive_action.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2617 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/eth_signing/onboarding_action.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3896 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/eth_signing/sign_off_chain_action.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3334 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/eth_signing/signers.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2749 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/eth_signing/util.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1318 2022-11-25 01:02:08.000000 apexpro-1.1.5/apexpro/exceptions.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.448320 apexpro-1.1.5/apexpro/helpers/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/helpers/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      348 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/helpers/db.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2570 2022-09-16 09:30:41.000000 apexpro-1.1.5/apexpro/helpers/request_helpers.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1077 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/helpers/requests.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      840 2023-07-05 05:49:58.000000 apexpro-1.1.5/apexpro/helpers/util.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    19984 2023-07-07 06:56:13.000000 apexpro-1.1.5/apexpro/http_private.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    16177 2023-05-24 06:10:59.000000 apexpro-1.1.5/apexpro/http_private_stark_key_sign.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3245 2023-07-05 05:49:58.000000 apexpro-1.1.5/apexpro/http_public.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      127 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/models.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.449724 apexpro-1.1.5/apexpro/starkex/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     4238 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/conditional_transfer.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1558 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/constants.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     5844 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/helpers.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     6588 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/order.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1124 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/signable.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.451040 apexpro-1.1.5/apexpro/starkex/starkex_resources/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      285 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/starkex_resources/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3089 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/starkex_resources/cpp_signature.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3627 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/starkex_resources/math_utils.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)   102708 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/starkex_resources/pedersen_params.json
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1346 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/starkex_resources/proxy.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    10414 2022-07-15 03:54:05.000000 apexpro-1.1.5/apexpro/starkex/starkex_resources/python_signature.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3812 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/transfer.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2631 2022-08-25 03:55:08.000000 apexpro-1.1.5/apexpro/starkex/withdrawal.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     4578 2023-05-24 06:10:59.000000 apexpro-1.1.5/apexpro/websocket_api.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.445493 apexpro-1.1.5/apexpro.egg-info/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     9088 2023-07-07 07:02:45.000000 apexpro-1.1.5/apexpro.egg-info/PKG-INFO
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1658 2023-07-07 07:02:45.000000 apexpro-1.1.5/apexpro.egg-info/SOURCES.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2023-07-07 07:02:45.000000 apexpro-1.1.5/apexpro.egg-info/dependency_links.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2022-07-15 06:12:12.000000 apexpro-1.1.5/apexpro.egg-info/not-zip-safe
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      245 2023-07-07 07:02:45.000000 apexpro-1.1.5/apexpro.egg-info/requires.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)       14 2023-07-07 07:02:45.000000 apexpro-1.1.5/apexpro.egg-info/top_level.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      131 2023-07-07 07:02:45.456240 apexpro-1.1.5/setup.cfg
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1656 2023-07-07 06:59:08.000000 apexpro-1.1.5/setup.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-07-07 07:02:45.454581 apexpro-1.1.5/tests/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.5/tests/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     5582 2022-11-27 04:45:32.000000 apexpro-1.1.5/tests/account_value.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      147 2022-07-15 03:54:05.000000 apexpro-1.1.5/tests/constants.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1904 2022-12-22 07:57:17.000000 apexpro-1.1.5/tests/demo_deposit.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2817 2023-02-09 06:01:49.000000 apexpro-1.1.5/tests/demo_private.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      844 2022-09-16 09:30:41.000000 apexpro-1.1.5/tests/demo_public.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1433 2022-12-22 07:57:17.000000 apexpro-1.1.5/tests/demo_register.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1503 2022-11-23 00:41:45.000000 apexpro-1.1.5/tests/demo_register_mul_address.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      583 2022-09-29 09:49:57.000000 apexpro-1.1.5/tests/demo_sign.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2927 2023-05-24 06:10:59.000000 apexpro-1.1.5/tests/demo_stark_key_sign.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      962 2022-12-09 13:23:37.000000 apexpro-1.1.5/tests/demo_ws.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     5573 2022-08-25 03:55:08.000000 apexpro-1.1.5/tests/test_onboarding.py
```

### Comparing `apexpro-1.1.4/LICENSE` & `apexpro-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/PKG-INFO` & `apexpro-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apexpro
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python3 Apexpro HTTP/WebSocket API Connector
 Home-page: https://github.com/xxx
 Author: Dexter Dickinson
 Author-email: xxx@apexpro.com
 License: MIT License
 Keywords: apexpro api connector
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apexpro-1.1.4/README.md` & `apexpro-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/__init__.py` & `apexpro-1.1.5/apexpro/__init__.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/_websocket_stream.py` & `apexpro-1.1.5/apexpro/_websocket_stream.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/constants.py` & `apexpro-1.1.5/apexpro/constants.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/errors.py` & `apexpro-1.1.5/apexpro/errors.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/eth.py` & `apexpro-1.1.5/apexpro/eth.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/eth_signing/eth_prive_action.py` & `apexpro-1.1.5/apexpro/eth_signing/eth_prive_action.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/eth_signing/onboarding_action.py` & `apexpro-1.1.5/apexpro/eth_signing/onboarding_action.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/eth_signing/sign_off_chain_action.py` & `apexpro-1.1.5/apexpro/eth_signing/sign_off_chain_action.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/eth_signing/signers.py` & `apexpro-1.1.5/apexpro/eth_signing/signers.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/eth_signing/util.py` & `apexpro-1.1.5/apexpro/eth_signing/util.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/exceptions.py` & `apexpro-1.1.5/apexpro/exceptions.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/helpers/request_helpers.py` & `apexpro-1.1.5/apexpro/helpers/request_helpers.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/helpers/requests.py` & `apexpro-1.1.5/apexpro/helpers/requests.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/helpers/util.py` & `apexpro-1.1.5/apexpro/helpers/util.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/http_private.py` & `apexpro-1.1.5/apexpro/http_private.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             ),
             msg=message_string.encode(encoding='utf-8'),
             digestmod=hashlib.sha256,
         )
         return base64.standard_b64encode(hashed.digest()).decode()
 
     def generate_nonce(self, starkKey, ethAddress, chainId,
-                       refresh="true"
+                       refresh="false"
                        ):
         """"
         POST: Generate nonce.
         :param kwargs: See
         https://api-docs.pro.apex.exchange/#privateapi-post-generate-nonce
         :returns: Request results as dictionary.
         """
```

### Comparing `apexpro-1.1.4/apexpro/http_private_stark_key_sign.py` & `apexpro-1.1.5/apexpro/http_private_stark_key_sign.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/http_public.py` & `apexpro-1.1.5/apexpro/http_public.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/conditional_transfer.py` & `apexpro-1.1.5/apexpro/starkex/conditional_transfer.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/constants.py` & `apexpro-1.1.5/apexpro/starkex/constants.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/helpers.py` & `apexpro-1.1.5/apexpro/starkex/helpers.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/order.py` & `apexpro-1.1.5/apexpro/starkex/order.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/signable.py` & `apexpro-1.1.5/apexpro/starkex/signable.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/starkex_resources/cpp_signature.py` & `apexpro-1.1.5/apexpro/starkex/starkex_resources/cpp_signature.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/starkex_resources/math_utils.py` & `apexpro-1.1.5/apexpro/starkex/starkex_resources/math_utils.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/starkex_resources/pedersen_params.json` & `apexpro-1.1.5/apexpro/starkex/starkex_resources/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/starkex_resources/proxy.py` & `apexpro-1.1.5/apexpro/starkex/starkex_resources/proxy.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/starkex_resources/python_signature.py` & `apexpro-1.1.5/apexpro/starkex/starkex_resources/python_signature.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/transfer.py` & `apexpro-1.1.5/apexpro/starkex/transfer.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/starkex/withdrawal.py` & `apexpro-1.1.5/apexpro/starkex/withdrawal.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro/websocket_api.py` & `apexpro-1.1.5/apexpro/websocket_api.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/apexpro.egg-info/PKG-INFO` & `apexpro-1.1.5/apexpro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apexpro
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python3 Apexpro HTTP/WebSocket API Connector
 Home-page: https://github.com/xxx
 Author: Dexter Dickinson
 Author-email: xxx@apexpro.com
 License: MIT License
 Keywords: apexpro api connector
 Classifier: Development Status :: 4 - Beta
```

### Comparing `apexpro-1.1.4/apexpro.egg-info/SOURCES.txt` & `apexpro-1.1.5/apexpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/setup.py` & `apexpro-1.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='apexpro',
-    version='1.1.4',
+    version='1.1.5',
     packages=find_packages(),
     description='Python3 Apexpro HTTP/WebSocket API Connector',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/xxx',
     license='MIT License',
     author='Dexter Dickinson',
```

### Comparing `apexpro-1.1.4/tests/account_value.py` & `apexpro-1.1.5/tests/account_value.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_deposit.py` & `apexpro-1.1.5/tests/demo_deposit.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_private.py` & `apexpro-1.1.5/tests/demo_private.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_public.py` & `apexpro-1.1.5/tests/demo_public.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_register.py` & `apexpro-1.1.5/tests/demo_register.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_register_mul_address.py` & `apexpro-1.1.5/tests/demo_register_mul_address.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_sign.py` & `apexpro-1.1.5/tests/demo_sign.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_stark_key_sign.py` & `apexpro-1.1.5/tests/demo_stark_key_sign.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/demo_ws.py` & `apexpro-1.1.5/tests/demo_ws.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.4/tests/test_onboarding.py` & `apexpro-1.1.5/tests/test_onboarding.py`

 * *Files identical despite different names*


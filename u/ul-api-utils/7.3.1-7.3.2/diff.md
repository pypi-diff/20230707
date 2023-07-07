# Comparing `tmp/ul-api-utils-7.3.1.tar.gz` & `tmp/ul-api-utils-7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.3.1.tar", last modified: Mon Jul  3 18:46:26 2023, max compression
+gzip compressed data, was "ul-api-utils-7.3.2.tar", last modified: Fri Jul  7 17:43:53 2023, max compression
```

## Comparing `ul-api-utils-7.3.1.tar` & `ul-api-utils-7.3.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.195166 ul-api-utils-7.3.1/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13527 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12938 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.119164 ul-api-utils-7.3.1/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.119164 ul-api-utils-7.3.1/example/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/pure_flask_example.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/rate_limit_load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.127164 ul-api-utils-7.3.1/example/routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11237 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/routes/api_some.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.127164 ul-api-utils-7.3.1/example/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 12:26:49.000000 ul-api-utils-7.3.1/example/workers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/example/workers/worker.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 18:46:26.195166 ul-api-utils-7.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.131164 ul-api-utils-7.3.1/ul_api_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.131164 ul-api-utils-7.3.1/ul_api_utils/access/
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.155165 ul-api-utils-7.3.1/ul_api_utils/api_resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17185 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_config.py
--rw-rw-rw-   0 root         (0) root         (0)    17241 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_fn_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_db.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_payload_alias.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/db_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/api_resource/signature_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.159165 ul-api-utils-7.3.1/ul_api_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_enc_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_api_user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_new_api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     4453 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_start.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/cmd_worker_start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.159165 ul-api-utils-7.3.1/ul_api_utils/commands/start/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/start/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/start/gunicorn.conf.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/commands/start/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.159165 ul-api-utils-7.3.1/ul_api_utils/conf/
--rw-rw-rw-   0 root         (0) root         (0)   999747 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-main.js
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-ui.js
--rw-rw-rw-   0 root         (0) root         (0)     3008 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.163165 ul-api-utils-7.3.1/ul_api_utils/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/malloc.py
--rw-rw-rw-   0 root         (0) root         (0)    14591 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/debug/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.163165 ul-api-utils-7.3.1/ul_api_utils/encrypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/encrypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.167165 ul-api-utils-7.3.1/ul_api_utils/internal_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.167165 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14067 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_check_context.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_error.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.171165 ul-api-utils-7.3.1/ul_api_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.171165 ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)    20862 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/intermediate_state.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/worker_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4620 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/worker_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/modules/worker_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.175166 ul-api-utils-7.3.1/ul_api_utils/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5077 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/debugger_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.175166 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/const.py
--rw-rw-rw-   0 root         (0) root         (0)    18739 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/health_check/resource.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/not_implemented.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3358 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/rate_limitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5142 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/resources/swagger.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.183166 ul-api-utils-7.3.1/ul_api_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.183166 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/api_request_info.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/avro.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/cached_per_request.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/decode_base64.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/deprecated.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.187166 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.187166 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)    28921 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/t_url_for.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/jinja/to_pretty_json.py
--rw-rw-rw-   0 root         (0) root         (0)     4123 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/load_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/token_check.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/token_check_through_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/utils/uuid_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.191166 ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/test_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4023 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/validate_empty_object.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-07-03 18:46:24.000000 ul-api-utils-7.3.1/ul_api_utils/validators/validate_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 18:46:26.131164 ul-api-utils-7.3.1/ul_api_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13527 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      430 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-03 18:46:25.000000 ul-api-utils-7.3.1/ul_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2022-02-13 16:08:16.000000 ul-api-utils-7.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13527 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2023-05-22 07:34:36.000000 ul-api-utils-7.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.426891 ul-api-utils-7.3.2/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-16 22:18:47.000000 ul-api-utils-7.3.2/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/example/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/example/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/example/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-05 10:42:34.000000 ul-api-utils-7.3.2/example/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/example/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-16 22:18:47.000000 ul-api-utils-7.3.2/example/pure_flask_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-11 15:03:47.000000 ul-api-utils-7.3.2/example/rate_limit_load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/example/routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-08 15:26:45.000000 ul-api-utils-7.3.2/example/routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11237 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/example/routes/api_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/example/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-19 07:17:32.000000 ul-api-utils-7.3.2/example/workers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/example/workers/worker.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/ul_api_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/ul_api_utils/access/
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/ul_api_utils/api_resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17185 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    17241 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource_fn_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_response_db.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/api_response_payload_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/db_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/api_resource/signature_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/ul_api_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/cmd_enc_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/cmd_gen_api_user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/cmd_gen_new_api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4453 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/cmd_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/cmd_worker_start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.434892 ul-api-utils-7.3.2/ul_api_utils/commands/start/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/start/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/start/gunicorn.conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/commands/start/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.434892 ul-api-utils-7.3.2/ul_api_utils/conf/
+-rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/conf/ul-debugger-main.js
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/conf/ul-debugger-ui.js
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.434892 ul-api-utils-7.3.2/ul_api_utils/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/debug/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/debug/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/debug/malloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/debug/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.434892 ul-api-utils-7.3.2/ul_api_utils/encrypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/encrypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.434892 ul-api-utils-7.3.2/ul_api_utils/internal_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.434892 ul-api-utils-7.3.2/ul_api_utils/internal_api/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/__tests__/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api_check_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.438892 ul-api-utils-7.3.2/ul_api_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.438892 ul-api-utils-7.3.2/ul_api_utils/modules/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    21828 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/modules/api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/intermediate_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/worker_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/modules/worker_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/modules/worker_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.438892 ul-api-utils-7.3.2/ul_api_utils/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/resources/debugger_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.438892 ul-api-utils-7.3.2/ul_api_utils/resources/health_check/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/health_check/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/health_check/const.py
+-rw-rw-rw-   0 root         (0) root         (0)    18739 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/health_check/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/health_check/health_check_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/health_check/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/not_implemented.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/rate_limitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5142 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/resources/swagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/__tests__/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/__tests__/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/api_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/api_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/api_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/api_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/api_request_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/avro.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/cached_per_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/decode_base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/deprecated.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    28921 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/utils/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/jinja/t_url_for.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/jinja/to_pretty_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/utils/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/load_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-07 17:43:51.000000 ul-api-utils-7.3.2/ul_api_utils/utils/token_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/token_check_through_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/utils/uuid_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/validators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.442892 ul-api-utils-7.3.2/ul_api_utils/validators/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/validators/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/validators/__tests__/test_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/validators/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/validators/validate_empty_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 12:21:54.000000 ul-api-utils-7.3.2/ul_api_utils/validators/validate_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 17:43:53.430891 ul-api-utils-7.3.2/ul_api_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13527 2023-07-07 17:43:53.000000 ul-api-utils-7.3.2/ul_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-07 17:43:53.000000 ul-api-utils-7.3.2/ul_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 17:43:53.000000 ul-api-utils-7.3.2/ul_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-07 17:43:53.000000 ul-api-utils-7.3.2/ul_api_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2023-07-07 17:43:53.000000 ul-api-utils-7.3.2/ul_api_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 17:43:53.000000 ul-api-utils-7.3.2/ul_api_utils.egg-info/top_level.txt
```

### Comparing `ul-api-utils-7.3.1/LICENSE` & `ul-api-utils-7.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/PKG-INFO` & `ul-api-utils-7.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.3.1
+Version: 7.3.2
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.3.1/README.md` & `ul-api-utils-7.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/example/conf.py` & `ul-api-utils-7.3.2/example/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/example/pure_flask_example.py` & `ul-api-utils-7.3.2/example/pure_flask_example.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/example/routes/api_some.py` & `ul-api-utils-7.3.2/example/routes/api_some.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/example/workers/worker.py` & `ul-api-utils-7.3.2/example/workers/worker.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/setup.py` & `ul-api-utils-7.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-api-utils',
-    version='7.3.1',
+    version='7.3.2',
     description='Python api utils',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='',
     packages=find_packages(),
     package_data={
```

### Comparing `ul-api-utils-7.3.1/ul_api_utils/access/__init__.py` & `ul-api-utils-7.3.2/ul_api_utils/access/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_request.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_config.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_resource_fn_typing.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_resource_fn_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_db.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_response_db.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/api_response_payload_alias.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/api_response_payload_alias.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/api_resource/signature_check.py` & `ul-api-utils-7.3.2/ul_api_utils/api_resource/signature_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_enc_keys.py` & `ul-api-utils-7.3.2/ul_api_utils/commands/cmd_enc_keys.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_api_user_token.py` & `ul-api-utils-7.3.2/ul_api_utils/commands/cmd_gen_api_user_token.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_gen_new_api_user.py` & `ul-api-utils-7.3.2/ul_api_utils/commands/cmd_gen_new_api_user.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_start.py` & `ul-api-utils-7.3.2/ul_api_utils/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/commands/cmd_worker_start.py` & `ul-api-utils-7.3.2/ul_api_utils/commands/cmd_worker_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/commands/start/wsgi.py` & `ul-api-utils-7.3.2/ul_api_utils/commands/start/wsgi.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-main.js` & `ul-api-utils-7.3.2/ul_api_utils/conf/ul-debugger-main.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/conf/ul-debugger-ui.js` & `ul-api-utils-7.3.2/ul_api_utils/conf/ul-debugger-ui.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/conf.py` & `ul-api-utils-7.3.2/ul_api_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/const.py` & `ul-api-utils-7.3.2/ul_api_utils/const.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/debug/debugger.py` & `ul-api-utils-7.3.2/ul_api_utils/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/debug/malloc.py` & `ul-api-utils-7.3.2/ul_api_utils/debug/malloc.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/debug/stat.py` & `ul-api-utils-7.3.2/ul_api_utils/debug/stat.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py` & `ul-api-utils-7.3.2/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/errors.py` & `ul-api-utils-7.3.2/ul_api_utils/errors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api.py` & `ul-api-utils-7.3.2/ul_api_utils/internal_api/__tests__/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/internal_api/__tests__/internal_api_content_type.py` & `ul-api-utils-7.3.2/ul_api_utils/internal_api/__tests__/internal_api_content_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api.py` & `ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_check_context.py` & `ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api_check_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/internal_api/internal_api_response.py` & `ul-api-utils-7.3.2/ul_api_utils/internal_api/internal_api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/main.py` & `ul-api-utils-7.3.2/ul_api_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/api_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 import traceback
 from base64 import b64decode
 from datetime import datetime
 from functools import wraps
 from typing import List, Union, Callable, Tuple, Any, Optional, TypeVar, cast, Set, TYPE_CHECKING
 
 from flask import Response, request, Flask, url_for as flask_url_for, _app_ctx_stack
+from pydantic import BaseModel
 from ul_py_tool.utils.arg_files_glob import arg_files_print
 from werkzeug import Response as BaseResponse
 
 from ul_api_utils.access import PermissionDefinition, GLOBAL_PERMISSION__PRIVATE, GLOBAL_PERMISSION__PRIVATE_RT, \
     GLOBAL_PERMISSION__PUBLIC, PermissionRegistry
 from ul_api_utils.api_resource.api_resource import ApiResource
 from ul_api_utils.api_resource.api_resource_config import ApiResourceConfig
 from ul_api_utils.api_resource.api_resource_fn_typing import ApiResourceFnTyping
 from ul_api_utils.api_resource.api_resource_type import ApiResourceType
-from ul_api_utils.api_resource.api_response import ApiResponse, JsonApiResponse, RootJsonApiResponse, ProxyJsonApiResponse
+from ul_api_utils.api_resource.api_response import ApiResponse, JsonApiResponse, RootJsonApiResponse, ProxyJsonApiResponse, AnyJsonApiResponse
 from ul_api_utils.conf import APPLICATION_DEBUGGER_PIN, APPLICATION_DEBUG, APPLICATION_DIR, APPLICATION_ENV_IS_LOCAL, \
     APPLICATION_START_DT
 from ul_api_utils.const import REQUEST_HEADER__DEBUGGER, REQUEST_HEADER__INTERNAL
 from ul_api_utils.debug import stat
 from ul_api_utils.debug.debugger import Debugger
 from ul_api_utils.errors import UserAbstractApiError, ResourceRuntimeApiError, ResponseTypeRuntimeApiError
 from ul_api_utils.internal_api.internal_api_check_context import internal_api_check_context
@@ -72,14 +73,28 @@
         try:
             os.unlink(f)
         except Exception as e:  # noqa: B902
             logger.warning(f'file {f} deleted before clean :: {e}')
     files.clear()
 
 
+def _get_error_types(response: ApiResponse) -> List[str]:
+    res = []
+    if isinstance(response, AnyJsonApiResponse) and isinstance(response.errors, (list, tuple)) and len(response.errors) > 0:
+        for err in response.errors:
+            err_t = None
+            if isinstance(err, BaseModel):  # type: ignore
+                err_t = getattr(err, 'error_type', None)  # type: ignore
+            elif isinstance(err, dict):
+                err_t = err.get('error_type', None)
+            if isinstance(err_t, str):
+                res.append(err_t)
+    return res
+
+
 class ApiSdk:
     ACCESS_PUBLIC = GLOBAL_PERMISSION__PUBLIC
     ACCESS_PRIVATE = GLOBAL_PERMISSION__PRIVATE
     ACCESS_PRIVATE_RT = GLOBAL_PERMISSION__PRIVATE_RT
 
     __slots__ = (
         '_config',
@@ -288,14 +303,17 @@
 
         flask_methods, enum_methods = ApiMethod.compile_methods(method)
 
         def wrap(fn: TFn) -> TFn:
             assert self._initialized_flask_name is not None, 'app must be initialized'
             assert fn.__module__, 'empty __module__ of function'
 
+            fn_module = fn.__module__
+            fn_name = fn.__name__
+
             logger = logging.getLogger(fn.__module__)
 
             fn_typing = ApiResourceFnTyping.parse_fn(api_type, enum_methods, fn)
 
             @wraps(fn)
             def wrapper(**kwargs: TKwargs) -> Tuple[BaseResponse, int]:
                 now = time.time()
@@ -317,19 +335,21 @@
 
                 assert self._initialized_flask_name is not None  # just for mypy
                 d = Debugger(self._initialized_flask_name, debugger_enabled, ApiMethod(request.method), request.url)
 
                 scope_user_id = None
                 scope_token_id = None
 
+                res: Optional[Tuple[BaseResponse, int]] = None
+
                 with sentry.configure_scope() as sentry_scope:
                     sentry_scope.set_tag('app_name', self._initialized_flask_name)
                     sentry_scope.set_tag('app_type', 'api')
                     sentry_scope.set_tag('app_uptime', f'{(datetime.now() - APPLICATION_START_DT).seconds // 60}s')
-                    sentry_scope.set_tag('app_api_name', fn.__name__)
+                    sentry_scope.set_tag('app_api_name', fn_name)
                     sentry_scope.set_tag('app_api_access', access.id)
 
                     try:
                         with internal_api_check_context():
                             result = None
 
                             if result is None:
@@ -406,14 +426,18 @@
                     'user_id': str(scope_user_id),
                     'token_id': str(scope_token_id),
                     'method': request.method,
                     'url': request.url,
                     'ipv4': ri.ipv4,
                     'user_agent': ri.user_agent,
                     'duration': time.time() - now,
+                    'status_code': res[1] if res is not None else 500,
+                    'fn_id': fn_name,
+                    'fn_mdl': fn_module,
+                    'error_codes': _get_error_types(result),
                 }))
 
                 return res
 
             assert access is not None  # for mypy
             self._fn_registry.append(ApiSdkResource(
                 path=path,
```

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_config.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/api_sdk_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/api_sdk_jwt.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/intermediate_state.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/intermediate_state.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/worker_context.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/worker_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/modules/worker_sdk.py` & `ul-api-utils-7.3.2/ul_api_utils/modules/worker_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/debugger_scripts.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/debugger_scripts.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/health_check/health_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/health_check/health_check_template.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/health_check/health_check_template.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/health_check/resource.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/health_check/resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/not_implemented.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/not_implemented.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/permissions.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/rate_limitter.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/rate_limitter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/resources/swagger.py` & `ul-api-utils-7.3.2/ul_api_utils/resources/swagger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/sentry.py` & `ul-api-utils-7.3.2/ul_api_utils/sentry.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/api_path_version.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/__tests__/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/__tests__/unwrap_typing.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/__tests__/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/api_encoding.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/api_encoding.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/api_format.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/api_format.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/api_method.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/api_method.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/api_pagination.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/api_pagination.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/api_path_version.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/avro.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/avro.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/cached_per_request.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/cached_per_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/colors.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/deprecated.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/json_encoder.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/load_modules.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/load_modules.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/token_check_through_request.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/token_check_through_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/unwrap_typing.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/utils/uuid_converter.py` & `ul-api-utils-7.3.2/ul_api_utils/utils/uuid_converter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/validators/__tests__/test_custom_fields.py` & `ul-api-utils-7.3.2/ul_api_utils/validators/__tests__/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils/validators/custom_fields.py` & `ul-api-utils-7.3.2/ul_api_utils/validators/custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.3.1/ul_api_utils.egg-info/PKG-INFO` & `ul-api-utils-7.3.2/ul_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.3.1
+Version: 7.3.2
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.3.1/ul_api_utils.egg-info/SOURCES.txt` & `ul-api-utils-7.3.2/ul_api_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


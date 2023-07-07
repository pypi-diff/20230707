# Comparing `tmp/aiobotocore-2.5.1.tar.gz` & `tmp/aiobotocore-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobotocore-2.5.1.tar", last modified: Tue Jun 27 23:46:23 2023, max compression
+gzip compressed data, was "aiobotocore-2.5.2.tar", last modified: Fri Jul  7 06:10:40 2023, max compression
```

## Comparing `aiobotocore-2.5.1.tar` & `aiobotocore-2.5.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:46:23.716825 aiobotocore-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-06-27 23:46:23.716825 aiobotocore-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:46:23.712825 aiobotocore-2.5.1/aiobotocore/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/_endpoint_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/awsrequest.py
--rw-r--r--   0 runner    (1001) docker     (123)    22830 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/configprovider.py
--rw-r--r--   0 runner    (1001) docker     (123)    38986 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/httpchecksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/httpsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/paginate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:46:23.716825 aiobotocore-2.5.1/aiobotocore/retries/
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/retries/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/retries/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/retries/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/retries/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/retryhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/signers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/aiobotocore/waiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:46:23.716825 aiobotocore-2.5.1/aiobotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-06-27 23:46:23.000000 aiobotocore-2.5.1/aiobotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-27 23:46:23.000000 aiobotocore-2.5.1/aiobotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:46:23.000000 aiobotocore-2.5.1/aiobotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-27 23:46:23.000000 aiobotocore-2.5.1/aiobotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 23:46:23.000000 aiobotocore-2.5.1/aiobotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 23:46:23.716825 aiobotocore-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:46:23.716825 aiobotocore-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_basic_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_eventstreams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-27 23:46:18.000000 aiobotocore-2.5.1/tests/test_waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/aiobotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/_endpoint_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/awsrequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22830 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/configprovider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/httpchecksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/httpsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/paginate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/aiobotocore/retries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/retries/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/retries/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/retries/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/retries/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/retryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/signers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/aiobotocore/waiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/aiobotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-07-07 06:10:40.000000 aiobotocore-2.5.2/aiobotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-07 06:10:40.000000 aiobotocore-2.5.2/aiobotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:10:40.000000 aiobotocore-2.5.2/aiobotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 06:10:40.000000 aiobotocore-2.5.2/aiobotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 06:10:40.000000 aiobotocore-2.5.2/aiobotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:10:40.145985 aiobotocore-2.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_basic_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_eventstreams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26368 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 06:10:35.000000 aiobotocore-2.5.2/tests/test_waiter.py
```

### Comparing `aiobotocore-2.5.1/CHANGES.rst` & `aiobotocore-2.5.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 Changes
 -------
+2.5.2 (2023-07-06)
+^^^^^^^^^^^^^^^^^^
+* fix issue #1020
+
 2.5.1 (2023-06-27)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore to 1.29.161
 
 2.5.0 (2023-03-06)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore to 1.29.76 (thanks @jakob-keller #999)
```

### Comparing `aiobotocore-2.5.1/LICENSE` & `aiobotocore-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/PKG-INFO` & `aiobotocore-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobotocore
-Version: 2.5.1
+Version: 2.5.2
 Summary: Async client for aws services using botocore and aiohttp
 Home-page: https://github.com/aio-libs/aiobotocore
 Download-URL: https://pypi.python.org/pypi/aiobotocore
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
@@ -267,14 +267,18 @@
     pip install -U 'aiobotocore[awscli,boto3]'
 
 If you only need awscli and not boto3 (or vice versa) you can just install one extra or
 the other.
 
 Changes
 -------
+2.5.2 (2023-07-06)
+^^^^^^^^^^^^^^^^^^
+* fix issue #1020
+
 2.5.1 (2023-06-27)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore to 1.29.161
 
 2.5.0 (2023-03-06)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore to 1.29.76 (thanks @jakob-keller #999)
```

### Comparing `aiobotocore-2.5.1/README.rst` & `aiobotocore-2.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/_endpoint_helpers.py` & `aiobotocore-2.5.2/aiobotocore/_endpoint_helpers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/args.py` & `aiobotocore-2.5.2/aiobotocore/args.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/awsrequest.py` & `aiobotocore-2.5.2/aiobotocore/awsrequest.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/client.py` & `aiobotocore-2.5.2/aiobotocore/client.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/config.py` & `aiobotocore-2.5.2/aiobotocore/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self._validate_connector_args(connector_args)
         self.connector_args = copy.copy(connector_args)
         if not self.connector_args:
             self.connector_args = dict()
 
         if 'keepalive_timeout' not in self.connector_args:
             # AWS has a 20 second idle timeout:
-            # https://forums.aws.amazon.com/message.jspa?messageID=215367
+            #   https://web.archive.org/web/20150926192339/https://forums.aws.amazon.com/message.jspa?messageID=215367
             # and aiohttp default timeout is 30s so we set it to something
             # reasonable here
             self.connector_args['keepalive_timeout'] = 12
 
     def merge(self, other_config):
         # Adapted from parent class
         config_options = copy.copy(self._user_provided_options)
```

### Comparing `aiobotocore-2.5.1/aiobotocore/configprovider.py` & `aiobotocore-2.5.2/aiobotocore/configprovider.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/credentials.py` & `aiobotocore-2.5.2/aiobotocore/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     _parse_if_needed,
     _serialize_if_needed,
     parse,
     resolve_imds_endpoint_mode,
 )
 from dateutil.tz import tzutc
 
+from aiobotocore._helpers import resolve_awaitable
 from aiobotocore.config import AioConfig
 from aiobotocore.tokens import AioSSOTokenProvider
 from aiobotocore.utils import (
     AioContainerMetadataFetcher,
     AioInstanceMetadataFetcher,
 )
 
@@ -320,15 +321,16 @@
                 # Might have refreshed by now
                 if not self.refresh_needed(self._mandatory_refresh_timeout):
                     return
                 await self._protected_refresh(is_mandatory=True)
 
     async def _protected_refresh(self, is_mandatory):
         try:
-            metadata = await self._refresh_using()
+            # AioEnvProvider._create_credentials_fetcher is not and does not need async
+            metadata = await resolve_awaitable(self._refresh_using())
         except Exception:
             period_name = 'mandatory' if is_mandatory else 'advisory'
             logger.warning(
                 "Refreshing temporary credentials failed "
                 "during %s refresh period.",
                 period_name,
                 exc_info=True,
@@ -432,14 +434,15 @@
             'sts',
             aws_access_key_id=frozen_credentials.access_key,
             aws_secret_access_key=frozen_credentials.secret_key,
             aws_session_token=frozen_credentials.token,
         )
 
 
+# black: # fmt: skip (ing) this line triggers internal black error
 class AioAssumeRoleWithWebIdentityCredentialFetcher(
     AioBaseAssumeRoleCredentialFetcher
 ):
     def __init__(
         self,
         client_creator,
         web_identity_token_loader,
```

### Comparing `aiobotocore-2.5.1/aiobotocore/discovery.py` & `aiobotocore-2.5.2/aiobotocore/discovery.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/endpoint.py` & `aiobotocore-2.5.2/aiobotocore/endpoint.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/eventstream.py` & `aiobotocore-2.5.2/aiobotocore/eventstream.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/handlers.py` & `aiobotocore-2.5.2/aiobotocore/handlers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/hooks.py` & `aiobotocore-2.5.2/aiobotocore/hooks.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/httpchecksum.py` & `aiobotocore-2.5.2/aiobotocore/httpchecksum.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/httpsession.py` & `aiobotocore-2.5.2/aiobotocore/httpsession.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         elif isinstance(client_cert, tuple):
             self._cert_file, self._key_file = client_cert
 
         self._timeout = timeout
         self._connector_args = connector_args
         if self._connector_args is None:
             # AWS has a 20 second idle timeout:
-            #   https://forums.aws.amazon.com/message.jspa?messageID=215367
+            #   https://web.archive.org/web/20150926192339/https://forums.aws.amazon.com/message.jspa?messageID=215367
             # aiohttp default timeout is 30s so set something reasonable here
             self._connector_args = dict(keepalive_timeout=12)
 
         self._max_pool_connections = max_pool_connections
         self._socket_options = socket_options
         if socket_options is None:
             self._socket_options = []
```

### Comparing `aiobotocore-2.5.1/aiobotocore/paginate.py` & `aiobotocore-2.5.2/aiobotocore/paginate.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/parsers.py` & `aiobotocore-2.5.2/aiobotocore/parsers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/regions.py` & `aiobotocore-2.5.2/aiobotocore/regions.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/response.py` & `aiobotocore-2.5.2/aiobotocore/response.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/retries/adaptive.py` & `aiobotocore-2.5.2/aiobotocore/retries/adaptive.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/retries/bucket.py` & `aiobotocore-2.5.2/aiobotocore/retries/bucket.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/retries/special.py` & `aiobotocore-2.5.2/aiobotocore/retries/special.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/retries/standard.py` & `aiobotocore-2.5.2/aiobotocore/retries/standard.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/retryhandler.py` & `aiobotocore-2.5.2/aiobotocore/retryhandler.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/session.py` & `aiobotocore-2.5.2/aiobotocore/session.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/signers.py` & `aiobotocore-2.5.2/aiobotocore/signers.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/tokens.py` & `aiobotocore-2.5.2/aiobotocore/tokens.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/utils.py` & `aiobotocore-2.5.2/aiobotocore/utils.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore/waiter.py` & `aiobotocore-2.5.2/aiobotocore/waiter.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/aiobotocore.egg-info/PKG-INFO` & `aiobotocore-2.5.2/aiobotocore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobotocore
-Version: 2.5.1
+Version: 2.5.2
 Summary: Async client for aws services using botocore and aiohttp
 Home-page: https://github.com/aio-libs/aiobotocore
 Download-URL: https://pypi.python.org/pypi/aiobotocore
 Author: Nikolay Novik
 Author-email: nickolainovik@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
@@ -267,14 +267,18 @@
     pip install -U 'aiobotocore[awscli,boto3]'
 
 If you only need awscli and not boto3 (or vice versa) you can just install one extra or
 the other.
 
 Changes
 -------
+2.5.2 (2023-07-06)
+^^^^^^^^^^^^^^^^^^
+* fix issue #1020
+
 2.5.1 (2023-06-27)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore to 1.29.161
 
 2.5.0 (2023-03-06)
 ^^^^^^^^^^^^^^^^^^
 * bump botocore to 1.29.76 (thanks @jakob-keller #999)
```

### Comparing `aiobotocore-2.5.1/aiobotocore.egg-info/SOURCES.txt` & `aiobotocore-2.5.2/aiobotocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/setup.py` & `aiobotocore-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_adaptive.py` & `aiobotocore-2.5.2/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_basic_s3.py` & `aiobotocore-2.5.2/tests/test_basic_s3.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_config.py` & `aiobotocore-2.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_dynamodb.py` & `aiobotocore-2.5.2/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_ec2.py` & `aiobotocore-2.5.2/tests/test_ec2.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_eventstreams.py` & `aiobotocore-2.5.2/tests/test_eventstreams.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_lambda.py` & `aiobotocore-2.5.2/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_monitor.py` & `aiobotocore-2.5.2/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_mturk.py` & `aiobotocore-2.5.2/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_patches.py` & `aiobotocore-2.5.2/tests/test_patches.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_response.py` & `aiobotocore-2.5.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_session.py` & `aiobotocore-2.5.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_sns.py` & `aiobotocore-2.5.2/tests/test_sns.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_sqs.py` & `aiobotocore-2.5.2/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_version.py` & `aiobotocore-2.5.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `aiobotocore-2.5.1/tests/test_waiter.py` & `aiobotocore-2.5.2/tests/test_waiter.py`

 * *Files identical despite different names*


# Comparing `tmp/splitapiclient-3.1.7.tar.gz` & `tmp/splitapiclient-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitapiclient-3.1.7.tar", last modified: Thu Mar  2 19:07:08 2023, max compression
+gzip compressed data, was "splitapiclient-3.1.8.tar", last modified: Thu Jun 29 20:54:23 2023, max compression
```

## Comparing `splitapiclient-3.1.7.tar` & `splitapiclient-3.1.8.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.485640 splitapiclient-3.1.7/
--rw-r--r--   0 joshuaklein   (503) staff       (20)     8445 2023-03-02 19:07:08.485828 splitapiclient-3.1.7/PKG-INFO
--rw-r--r--   0 joshuaklein   (503) staff       (20)     7613 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/README.md
--rw-r--r--   0 joshuaklein   (503) staff       (20)      688 2023-03-02 19:07:08.486503 splitapiclient-3.1.7/setup.cfg
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3513 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/setup.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.421083 splitapiclient-3.1.7/splitapiclient/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/__init__.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.425775 splitapiclient-3.1.7/splitapiclient/http_clients/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/http_clients/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5008 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/http_clients/base_client.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4344 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/http_clients/sync_client.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.427977 splitapiclient-3.1.7/splitapiclient/main/
--rw-r--r--   0 joshuaklein   (503) staff       (20)      293 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/main/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1180 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/main/apiclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4378 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/main/sync_apiclient.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.441493 splitapiclient-3.1.7/splitapiclient/microclients/
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1176 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2255 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/apikey_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5185 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/attribute_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5332 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/change_request_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4644 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/environment_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3954 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/group_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     6565 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/identity_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2750 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/restriction_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5681 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/segment_definition_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5619 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/segment_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5116 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/split_definition_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     8767 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/split_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2381 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/traffic_type_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5417 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/user_microclient.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5119 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/microclients/workspace_microclient.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.458170 splitapiclient-3.1.7/splitapiclient/resources/
--rw-r--r--   0 joshuaklein   (503) staff       (20)      825 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1497 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/apikey.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2619 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/attribute.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1934 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/base_resource.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      510 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/bucket.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4027 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/change_request.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1154 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/condition.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      519 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/default_rule.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4884 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/environment.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      816 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/group.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2689 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/identity.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2276 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/matcher.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1519 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/restriction.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1376 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/rule.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2420 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/segment.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4752 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/segment_definition.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3887 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/split.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     6682 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/split_definition.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4548 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/traffic_type.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1335 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/treatment.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1444 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/user.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4749 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/resources/workspace.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.458866 splitapiclient-3.1.7/splitapiclient/tests/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/__init__.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.460291 splitapiclient-3.1.7/splitapiclient/tests/e2e/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/e2e/__init__.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.461829 splitapiclient-3.1.7/splitapiclient/tests/e2e/backend/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/e2e/backend/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3421 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/e2e/backend/handlers.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1668 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/e2e/backend/responses.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5608 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/e2e/e2etests.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1053 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/e2e/server.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.464574 splitapiclient-3.1.7/splitapiclient/tests/http_clients/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/http_clients/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4009 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/http_clients/test_base_http_client.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     7872 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/http_clients/test_sync_http_client.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.477200 splitapiclient-3.1.7/splitapiclient/tests/resources/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4978 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_attribute.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      671 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_base_resource.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      421 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_bucket.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      871 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_condition.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      440 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_default_rule.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)    10004 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_environment.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1314 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_group.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5569 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_identity.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     1129 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_rule.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2981 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_segment.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5683 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_segment_definition.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     5492 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_split.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     7214 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_split_definition.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)    13958 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_traffic_type.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      545 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_treatment.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3423 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_user.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     7418 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/resources/test_workspace.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.480234 splitapiclient-3.1.7/splitapiclient/tests/util/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/util/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2036 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/util/test_camelcase.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3776 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/tests/util/test_helpers.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.485184 splitapiclient-3.1.7/splitapiclient/util/
--rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/__init__.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      833 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/abstract_extra.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      506 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/bulk_result.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      649 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/camelcase.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     2584 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/exceptions.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)     4534 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/helpers.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      596 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/logger.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)      742 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/util/validation.py
--rw-r--r--   0 joshuaklein   (503) staff       (20)       22 2023-03-02 19:05:08.000000 splitapiclient-3.1.7/splitapiclient/version.py
-drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-03-02 19:07:08.424517 splitapiclient-3.1.7/splitapiclient.egg-info/
--rw-r--r--   0 joshuaklein   (503) staff       (20)     8445 2023-03-02 19:07:08.000000 splitapiclient-3.1.7/splitapiclient.egg-info/PKG-INFO
--rw-r--r--   0 joshuaklein   (503) staff       (20)     3844 2023-03-02 19:07:08.000000 splitapiclient-3.1.7/splitapiclient.egg-info/SOURCES.txt
--rw-r--r--   0 joshuaklein   (503) staff       (20)        1 2023-03-02 19:07:08.000000 splitapiclient-3.1.7/splitapiclient.egg-info/dependency_links.txt
--rw-r--r--   0 joshuaklein   (503) staff       (20)       43 2023-03-02 19:07:08.000000 splitapiclient-3.1.7/splitapiclient.egg-info/requires.txt
--rw-r--r--   0 joshuaklein   (503) staff       (20)       15 2023-03-02 19:07:08.000000 splitapiclient-3.1.7/splitapiclient.egg-info/top_level.txt
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.232666 splitapiclient-3.1.8/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     8445 2023-06-29 20:54:23.232933 splitapiclient-3.1.8/PKG-INFO
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     7613 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/README.md
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      688 2023-06-29 20:54:23.233914 splitapiclient-3.1.8/setup.cfg
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3513 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/setup.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.137521 splitapiclient-3.1.8/splitapiclient/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/__init__.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.143910 splitapiclient-3.1.8/splitapiclient/http_clients/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/http_clients/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5008 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/http_clients/base_client.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4344 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/http_clients/sync_client.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.148784 splitapiclient-3.1.8/splitapiclient/main/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      293 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/main/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1180 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/main/apiclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4378 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/main/sync_apiclient.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.167750 splitapiclient-3.1.8/splitapiclient/microclients/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1176 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2255 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/apikey_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5185 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/attribute_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5332 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/change_request_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4644 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/environment_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3954 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/group_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     6565 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/identity_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2750 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/restriction_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5681 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/segment_definition_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5619 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/segment_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5116 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/split_definition_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     8767 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/split_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2381 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/traffic_type_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5417 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/user_microclient.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5119 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/microclients/workspace_microclient.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.189004 splitapiclient-3.1.8/splitapiclient/resources/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      825 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1497 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/apikey.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2803 2023-06-29 20:27:55.000000 splitapiclient-3.1.8/splitapiclient/resources/attribute.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1934 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/base_resource.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      510 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/bucket.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4027 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/change_request.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1154 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/condition.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      519 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/default_rule.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4884 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/environment.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      816 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/group.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2689 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/identity.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2276 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/matcher.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1519 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/restriction.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1376 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/rule.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2420 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/segment.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4752 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/segment_definition.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3887 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/split.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     6682 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/split_definition.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4548 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/traffic_type.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1335 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/treatment.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1444 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/user.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4749 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/resources/workspace.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.189991 splitapiclient-3.1.8/splitapiclient/tests/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/__init__.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.192010 splitapiclient-3.1.8/splitapiclient/tests/e2e/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/e2e/__init__.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.196656 splitapiclient-3.1.8/splitapiclient/tests/e2e/backend/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/e2e/backend/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3421 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/e2e/backend/handlers.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1668 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/e2e/backend/responses.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5608 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/e2e/e2etests.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1053 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/e2e/server.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.200406 splitapiclient-3.1.8/splitapiclient/tests/http_clients/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/http_clients/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4009 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/http_clients/test_base_http_client.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     7872 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/http_clients/test_sync_http_client.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.221126 splitapiclient-3.1.8/splitapiclient/tests/resources/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5062 2023-06-29 20:10:49.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_attribute.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      671 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_base_resource.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      421 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_bucket.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      871 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_condition.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      440 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_default_rule.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)    10004 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_environment.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1314 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_group.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5569 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_identity.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     1129 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_rule.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2981 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_segment.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5683 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_segment_definition.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     5492 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_split.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     7214 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_split_definition.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)    14370 2023-06-29 20:22:49.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_traffic_type.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      545 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_treatment.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3423 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_user.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     7418 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/resources/test_workspace.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.223352 splitapiclient-3.1.8/splitapiclient/tests/util/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/util/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2036 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/util/test_camelcase.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3776 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/tests/util/test_helpers.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.231550 splitapiclient-3.1.8/splitapiclient/util/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        0 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/__init__.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      833 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/abstract_extra.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      506 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/bulk_result.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      649 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/camelcase.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     2584 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/exceptions.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     4534 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/helpers.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      596 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/logger.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)      742 2023-06-29 19:41:48.000000 splitapiclient-3.1.8/splitapiclient/util/validation.py
+-rw-r--r--   0 joshuaklein   (503) staff       (20)       22 2023-06-29 20:23:26.000000 splitapiclient-3.1.8/splitapiclient/version.py
+drwxr-xr-x   0 joshuaklein   (503) staff       (20)        0 2023-06-29 20:54:23.141147 splitapiclient-3.1.8/splitapiclient.egg-info/
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     8445 2023-06-29 20:54:23.000000 splitapiclient-3.1.8/splitapiclient.egg-info/PKG-INFO
+-rw-r--r--   0 joshuaklein   (503) staff       (20)     3844 2023-06-29 20:54:23.000000 splitapiclient-3.1.8/splitapiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuaklein   (503) staff       (20)        1 2023-06-29 20:54:23.000000 splitapiclient-3.1.8/splitapiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuaklein   (503) staff       (20)       43 2023-06-29 20:54:23.000000 splitapiclient-3.1.8/splitapiclient.egg-info/requires.txt
+-rw-r--r--   0 joshuaklein   (503) staff       (20)       15 2023-06-29 20:54:23.000000 splitapiclient-3.1.8/splitapiclient.egg-info/top_level.txt
```

### Comparing `splitapiclient-3.1.7/PKG-INFO` & `splitapiclient-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: splitapiclient
-Version: 3.1.7
+Version: 3.1.8
 Summary: This Python Library provide full support for Split REST Admin API
 Home-page: https://github.com/splitio/python-api
-Download-URL: https://github.com/splitio/python-api/tarball/3.1.7
+Download-URL: https://github.com/splitio/python-api/tarball/3.1.8
 Author: Patricio Echague, Sebastian Arrubia, Martin Redolatti
 Author-email: pato@split.io, sebastian@split.io, martin@split.io
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/splitio/python-api/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `splitapiclient-3.1.7/README.md` & `splitapiclient-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/setup.cfg` & `splitapiclient-3.1.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 test = pytest
 
 [tool:pytest]
 addopts = --verbose
 
 [metadata]
 name = splitapiclient
-version = 3.1.7
+version = 3.1.8
 description = This Python Library provide full support for Split REST Admin API, allow creating, deleting and editing Environments, Splits, Split Definitions, Segments, Segment Keys, Users, Groups, API Keys, Change Requests, Attributes and Identities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/splitio/python-api
 project_urls = 
 	Bug Tracker = https://github.com/splitio/python-api/issues
 classifiers =
```

### Comparing `splitapiclient-3.1.7/setup.py` & `splitapiclient-3.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/http_clients/base_client.py` & `splitapiclient-3.1.8/splitapiclient/http_clients/base_client.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/http_clients/sync_client.py` & `splitapiclient-3.1.8/splitapiclient/http_clients/sync_client.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/main/apiclient.py` & `splitapiclient-3.1.8/splitapiclient/main/apiclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/main/sync_apiclient.py` & `splitapiclient-3.1.8/splitapiclient/main/sync_apiclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/__init__.py` & `splitapiclient-3.1.8/splitapiclient/microclients/__init__.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/apikey_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/apikey_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/attribute_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/attribute_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/change_request_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/change_request_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/environment_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/environment_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/group_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/group_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/identity_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/identity_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/restriction_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/restriction_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/segment_definition_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/segment_definition_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/segment_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/segment_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/split_definition_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/split_definition_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/split_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/split_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/traffic_type_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/traffic_type_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/user_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/user_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/microclients/workspace_microclient.py` & `splitapiclient-3.1.8/splitapiclient/microclients/workspace_microclient.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/__init__.py` & `splitapiclient-3.1.8/splitapiclient/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/apikey.py` & `splitapiclient-3.1.8/splitapiclient/resources/apikey.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/attribute.py` & `splitapiclient-3.1.8/splitapiclient/resources/attribute.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         'id': 'string',
         'trafficTypeId': 'string',
         'displayName': 'string',
         'description': 'string',
         'dataType': 'string',
         'isSearchable': 'bool',
         'workspaceId' : 'string',
+        'suggestedValues': ['string']
     }
 
     def __init__(self, data=None, client=None):
         '''
         '''
         if not data:
             data = {}
@@ -26,14 +27,15 @@
         self._id = data.get('id')
         self._traffic_type_id = data.get('trafficTypeId')
         self._display_name = data.get('displayName')
         self._description = data.get('description')
         self._data_type = data.get('dataType')
         self._is_searchable = data.get('isSearchable')
         self._workspace_id = data.get('workspaceId')
+        self._suggested_values = data.get('suggestedValues')
 
     @property
     def traffic_type_id(self):
         return self._traffic_type_id
 
     @property
     def display_name(self):
@@ -47,14 +49,18 @@
     def data_type(self):
         return self._data_type
 
     @property
     def is_searchable(self):
         return self._is_searchable
 
+    @property
+    def suggested_values(self):
+        return self._suggested_values
+
     @traffic_type_id.setter
     def traffic_type_id(self, new):
         self._traffic_type_id = new
 
     @display_name.setter
     def display_name(self, new):
         self._display_name = new
```

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/base_resource.py` & `splitapiclient-3.1.8/splitapiclient/resources/base_resource.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/change_request.py` & `splitapiclient-3.1.8/splitapiclient/resources/change_request.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/condition.py` & `splitapiclient-3.1.8/splitapiclient/resources/condition.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/default_rule.py` & `splitapiclient-3.1.8/splitapiclient/resources/default_rule.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/environment.py` & `splitapiclient-3.1.8/splitapiclient/resources/environment.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/group.py` & `splitapiclient-3.1.8/splitapiclient/resources/group.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/identity.py` & `splitapiclient-3.1.8/splitapiclient/resources/identity.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/matcher.py` & `splitapiclient-3.1.8/splitapiclient/resources/matcher.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/restriction.py` & `splitapiclient-3.1.8/splitapiclient/resources/restriction.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/rule.py` & `splitapiclient-3.1.8/splitapiclient/resources/rule.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/segment.py` & `splitapiclient-3.1.8/splitapiclient/resources/segment.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/segment_definition.py` & `splitapiclient-3.1.8/splitapiclient/resources/segment_definition.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/split.py` & `splitapiclient-3.1.8/splitapiclient/resources/split.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/split_definition.py` & `splitapiclient-3.1.8/splitapiclient/resources/split_definition.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/traffic_type.py` & `splitapiclient-3.1.8/splitapiclient/resources/traffic_type.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/treatment.py` & `splitapiclient-3.1.8/splitapiclient/resources/treatment.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/user.py` & `splitapiclient-3.1.8/splitapiclient/resources/user.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/resources/workspace.py` & `splitapiclient-3.1.8/splitapiclient/resources/workspace.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/e2e/backend/handlers.py` & `splitapiclient-3.1.8/splitapiclient/tests/e2e/backend/handlers.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/e2e/backend/responses.py` & `splitapiclient-3.1.8/splitapiclient/tests/e2e/backend/responses.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/e2e/e2etests.py` & `splitapiclient-3.1.8/splitapiclient/tests/e2e/e2etests.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/e2e/server.py` & `splitapiclient-3.1.8/splitapiclient/tests/e2e/server.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/http_clients/test_base_http_client.py` & `splitapiclient-3.1.8/splitapiclient/tests/http_clients/test_base_http_client.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/http_clients/test_sync_http_client.py` & `splitapiclient-3.1.8/splitapiclient/tests/http_clients/test_sync_http_client.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_attribute.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_attribute.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         '''
         attr_data = {
             'id': '1',
             'displayName': 'n1',
             'description': 'asd',
             'trafficTypeId': '111',
             'dataType': 'string',
+            'suggestedValues': ['string']
         }
         http_client_mock = mocker.Mock(spec=BaseHttpClient)
         http_client_mock.make_request.return_value = attr_data
         a1 = Attribute(attr_data, http_client_mock)
 
         res = a1.save()
 
@@ -83,14 +84,15 @@
 
         attr_data = {
             'id': '1',
             'displayName': 'n1',
             'description': 'asd',
             'trafficTypeId': '111',
             'dataType': 'string',
+            'suggestedValues': ['string']
         }
         mocker.patch('splitapiclient.http_clients.sync_client.SyncHttpClient.make_request')
         SyncHttpClient.make_request.return_value = attr_data
         ic = get_client({'base_url': 'http://test', 'apikey': '123'})
         a2 = Attribute(attr_data)
         res = a2.save(ic)
         http_client_mock.make_request.assert_called_once_with(
```

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_base_resource.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_base_resource.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_condition.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_condition.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_environment.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_environment.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_group.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_group.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_identity.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_identity.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_rule.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_rule.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_segment.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_segment.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_segment_definition.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_segment_definition.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_split.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_split.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_split_definition.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_split_definition.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_traffic_type.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_traffic_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,23 +54,26 @@
         data = [{
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'description': 'd1',
             'dataType': 'string',
             'isSearchable': False,
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
         }, {
             'id': 'a2',
             'trafficTypeId': '1',
             'displayName': 'dn2',
             'description': 'd1',
             'dataType': 'string',
             'isSearchable': False,
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
+            
         }]
         http_client_mock = mocker.Mock(spec=BaseHttpClient)
         http_client_mock.make_request.return_value = data
         tt1 = TrafficType(
             {
                 'id': '1',
                 'displayAttributeId': 'asd',
@@ -90,23 +93,25 @@
         data = [{
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'description': 'd1',
             'dataType': 'string',
             'isSearchable': False,
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
         }, {
             'id': 'a2',
             'trafficTypeId': '1',
             'displayName': 'dn2',
             'description': 'd1',
             'dataType': 'string',
             'isSearchable': False,
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
         }]
         assert attrs[0].to_dict() == data[0]
         assert attrs[1].to_dict() == data[1]
 
         mocker.patch('splitapiclient.http_clients.sync_client.SyncHttpClient.make_request')
         SyncHttpClient.make_request.return_value = data
         ic = get_client({'base_url': 'http://test', 'apikey': '123'})
@@ -126,38 +131,41 @@
         data = [{
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'description': 'd1',
             'dataType': 'string',
             'isSearchable': False,
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
         }, {
             'id': 'a2',
             'trafficTypeId': '1',
             'displayName': 'dn2',
             'description': 'd1',
             'dataType': 'string',
             'isSearchable': False,
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
         }]
         assert attrs[0].to_dict() == data[0]
         assert attrs[1].to_dict() == data[1]
 
     def test_add_attribute(self, mocker):
         '''
         '''
         data = {
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'isSearchable': None,
             'dataType': 'string',
             'description': 'd1',
-            'workspaceId': None
+            'workspaceId': None,
+            'suggestedValues': []
         }
         http_client_mock = mocker.Mock(spec=BaseHttpClient)
         http_client_mock.make_request.return_value = data
         tt1 = TrafficType(
             {
                 'id': '1',
                 'displayAttributeId': 'asd',
@@ -167,24 +175,27 @@
             http_client_mock
         )
         attrib_data = {'id': 'a1',
                 'displayName': 'dn1',
                 'description': 'd1',
                 'dataType': 'string',
                 'trafficTypeId': '1',
-                'workspaceId': 'ws_id'
+                'workspaceId': 'ws_id',
+                'suggestedValues': []
         }
 
         attr = tt1.add_attribute(attrib_data)
         data = {
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'dataType': 'string',
             'description': 'd1',
+            'suggestedValues': []
+            
         }
 
         http_client_mock.make_request.assert_called_once_with(
             AttributeMicroClient._endpoint['create'],
             data,
             trafficTypeId = data['trafficTypeId'],
             workspaceId = 'ws_id'
@@ -197,14 +208,15 @@
         # Test adding an attribute instance
         data = {
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'dataType': 'string',
             'description': 'd1',
+            'suggestedValues': []
         }
         atinstance = Attribute(data)
         http_client_mock.reset_mock()
         attr = tt1.add_attribute(atinstance)
         http_client_mock.make_request.assert_called_once_with(
             AttributeMicroClient._endpoint['create'],
             data,
@@ -228,14 +240,15 @@
         attr = tt2.add_attribute(data, ic)
         data = {
             'id': 'a1',
             'trafficTypeId': '1',
             'displayName': 'dn1',
             'dataType': 'string',
             'description': 'd1',
+            'suggestedValues': []
         }
 
         http_client_mock.make_request.assert_called_once_with(
             AttributeMicroClient._endpoint['create'],
             data,
             trafficTypeId=data['trafficTypeId'],
             workspaceId=None
```

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_treatment.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_treatment.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_user.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_user.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/resources/test_workspace.py` & `splitapiclient-3.1.8/splitapiclient/tests/resources/test_workspace.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/util/test_camelcase.py` & `splitapiclient-3.1.8/splitapiclient/tests/util/test_camelcase.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/tests/util/test_helpers.py` & `splitapiclient-3.1.8/splitapiclient/tests/util/test_helpers.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/util/abstract_extra.py` & `splitapiclient-3.1.8/splitapiclient/util/abstract_extra.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/util/camelcase.py` & `splitapiclient-3.1.8/splitapiclient/util/camelcase.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/util/exceptions.py` & `splitapiclient-3.1.8/splitapiclient/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/util/helpers.py` & `splitapiclient-3.1.8/splitapiclient/util/helpers.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/util/logger.py` & `splitapiclient-3.1.8/splitapiclient/util/logger.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient/util/validation.py` & `splitapiclient-3.1.8/splitapiclient/util/validation.py`

 * *Files identical despite different names*

### Comparing `splitapiclient-3.1.7/splitapiclient.egg-info/PKG-INFO` & `splitapiclient-3.1.8/splitapiclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: splitapiclient
-Version: 3.1.7
+Version: 3.1.8
 Summary: This Python Library provide full support for Split REST Admin API
 Home-page: https://github.com/splitio/python-api
-Download-URL: https://github.com/splitio/python-api/tarball/3.1.7
+Download-URL: https://github.com/splitio/python-api/tarball/3.1.8
 Author: Patricio Echague, Sebastian Arrubia, Martin Redolatti
 Author-email: pato@split.io, sebastian@split.io, martin@split.io
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/splitio/python-api/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `splitapiclient-3.1.7/splitapiclient.egg-info/SOURCES.txt` & `splitapiclient-3.1.8/splitapiclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*


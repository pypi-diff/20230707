# Comparing `tmp/predibase-2023.5.8.tar.gz` & `tmp/predibase-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/predibase-2023.5.8.tar", last modified: Tue May 30 16:42:34 2023, max compression
+gzip compressed data, was "predibase-2023.7.1.tar", last modified: Thu Jul  6 22:09:27 2023, max compression
```

## Comparing `predibase-2023.5.8.tar` & `predibase-2023.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.844697 predibase-2023.5.8/
--rw-r--r--   0 tgaddair   (501) staff       (20)       60 2023-02-15 19:35:43.000000 predibase-2023.5.8/MANIFEST.in
--rw-r--r--   0 tgaddair   (501) staff       (20)      222 2023-05-30 16:42:34.844061 predibase-2023.5.8/PKG-INFO
--rw-r--r--   0 tgaddair   (501) staff       (20)      468 2023-05-30 16:42:03.000000 predibase-2023.5.8/README.md
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.823414 predibase-2023.5.8/predibase/
--rw-r--r--   0 tgaddair   (501) staff       (20)      194 2023-03-29 04:10:48.000000 predibase-2023.5.8/predibase/__init__.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1157 2023-05-19 21:42:34.000000 predibase-2023.5.8/predibase/cli.py
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.829795 predibase-2023.5.8/predibase/cli_commands/
--rw-r--r--   0 tgaddair   (501) staff       (20)        0 2023-04-12 17:19:59.000000 predibase-2023.5.8/predibase/cli_commands/__init__.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      484 2023-05-29 04:04:31.000000 predibase-2023.5.8/predibase/cli_commands/delete.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1526 2023-05-29 04:04:31.000000 predibase-2023.5.8/predibase/cli_commands/deploy.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     2546 2023-05-19 21:42:34.000000 predibase-2023.5.8/predibase/cli_commands/prompt.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     2116 2023-04-12 17:19:59.000000 predibase-2023.5.8/predibase/cli_commands/settings.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1553 2023-04-12 17:19:59.000000 predibase-2023.5.8/predibase/cli_commands/utils.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1204 2023-05-19 21:42:34.000000 predibase-2023.5.8/predibase/client.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     2346 2023-02-28 05:17:35.000000 predibase-2023.5.8/predibase/connection.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     7289 2023-04-28 17:54:01.000000 predibase-2023.5.8/predibase/connection_mixin.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     6933 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/dataset_mixin.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     6352 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/deployment_mixin.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     6663 2023-05-22 17:59:53.000000 predibase-2023.5.8/predibase/engine_mixin.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     2408 2023-05-29 04:04:31.000000 predibase-2023.5.8/predibase/llm_mixin.py
--rw-r--r--   0 tgaddair   (501) staff       (20)    14732 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/model_mixin.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     2492 2022-11-08 22:44:48.000000 predibase-2023.5.8/predibase/permission_mixin.py
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.831498 predibase-2023.5.8/predibase/pql/
--rw-r--r--   0 tgaddair   (501) staff       (20)     2537 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/pql/__init__.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      548 2022-06-02 03:41:43.000000 predibase-2023.5.8/predibase/pql/adapter.py
--rw-r--r--   0 tgaddair   (501) staff       (20)    10954 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/pql/api.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     4181 2023-04-19 22:05:00.000000 predibase-2023.5.8/predibase/pql/utils.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     9237 2023-05-30 16:36:55.000000 predibase-2023.5.8/predibase/predictor.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1971 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/query_mixin.py
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.841843 predibase-2023.5.8/predibase/resource/
--rw-r--r--   0 tgaddair   (501) staff       (20)        0 2022-05-15 20:13:38.000000 predibase-2023.5.8/predibase/resource/__init__.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1014 2023-03-01 23:15:07.000000 predibase-2023.5.8/predibase/resource/config.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     4804 2023-04-28 17:54:01.000000 predibase-2023.5.8/predibase/resource/connection.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      635 2023-02-28 05:17:35.000000 predibase-2023.5.8/predibase/resource/connection_object.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     2630 2023-03-08 18:21:54.000000 predibase-2023.5.8/predibase/resource/connection_properties.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     7268 2023-04-27 03:58:16.000000 predibase-2023.5.8/predibase/resource/dataset.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      930 2023-02-28 05:17:35.000000 predibase-2023.5.8/predibase/resource/dataset_info.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     4262 2023-03-29 04:10:48.000000 predibase-2023.5.8/predibase/resource/deployment.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     4512 2023-05-19 21:42:34.000000 predibase-2023.5.8/predibase/resource/engine.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      699 2023-05-27 18:33:43.000000 predibase-2023.5.8/predibase/resource/llm.py
--rw-r--r--   0 tgaddair   (501) staff       (20)    37134 2023-05-19 21:42:34.000000 predibase-2023.5.8/predibase/resource/model.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     3478 2023-02-28 05:17:35.000000 predibase-2023.5.8/predibase/resource/query.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     3018 2023-04-25 21:59:22.000000 predibase-2023.5.8/predibase/resource/user.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      200 2022-07-12 20:45:22.000000 predibase-2023.5.8/predibase/resource/viz.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1410 2023-02-03 23:02:11.000000 predibase-2023.5.8/predibase/resource_util.py
--rw-r--r--   0 tgaddair   (501) staff       (20)    10310 2023-03-29 04:10:48.000000 predibase-2023.5.8/predibase/triton_util.py
--rw-r--r--   0 tgaddair   (501) staff       (20)     1892 2023-04-19 22:05:00.000000 predibase-2023.5.8/predibase/util.py
--rw-r--r--   0 tgaddair   (501) staff       (20)       25 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase/version.py
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.827007 predibase-2023.5.8/predibase.egg-info/
--rw-r--r--   0 tgaddair   (501) staff       (20)      222 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase.egg-info/PKG-INFO
--rw-r--r--   0 tgaddair   (501) staff       (20)     1554 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase.egg-info/SOURCES.txt
--rw-r--r--   0 tgaddair   (501) staff       (20)        1 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase.egg-info/dependency_links.txt
--rw-r--r--   0 tgaddair   (501) staff       (20)       46 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase.egg-info/entry_points.txt
--rw-r--r--   0 tgaddair   (501) staff       (20)        1 2023-05-29 04:25:56.000000 predibase-2023.5.8/predibase.egg-info/not-zip-safe
--rw-r--r--   0 tgaddair   (501) staff       (20)      232 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase.egg-info/requires.txt
--rw-r--r--   0 tgaddair   (501) staff       (20)       29 2023-05-30 16:42:34.000000 predibase-2023.5.8/predibase.egg-info/top_level.txt
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.842900 predibase-2023.5.8/predibase_notebook/
--rw-r--r--   0 tgaddair   (501) staff       (20)     3427 2023-02-28 05:17:35.000000 predibase-2023.5.8/predibase_notebook/__init__.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      552 2023-02-28 05:17:35.000000 predibase-2023.5.8/predibase_notebook/env.py
-drwxr-xr-x   0 tgaddair   (501) staff       (20)        0 2023-05-30 16:42:34.843406 predibase-2023.5.8/predibase_notebook/nbextension/
--rw-r--r--   0 tgaddair   (501) staff       (20)        0 2021-03-28 16:41:01.000000 predibase-2023.5.8/predibase_notebook/nbextension/__init__.py
--rw-r--r--   0 tgaddair   (501) staff       (20)      169 2023-04-28 17:54:01.000000 predibase-2023.5.8/requirements.txt
--rw-r--r--   0 tgaddair   (501) staff       (20)       42 2023-02-28 05:17:35.000000 predibase-2023.5.8/requirements_predictor.txt
--rw-r--r--   0 tgaddair   (501) staff       (20)       38 2023-05-30 16:42:34.844867 predibase-2023.5.8/setup.cfg
--rw-r--r--   0 tgaddair   (501) staff       (20)      888 2023-05-30 16:35:38.000000 predibase-2023.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.083139 predibase-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 22:08:36.000000 predibase-2023.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 22:09:27.083139 predibase-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-06 22:08:36.000000 predibase-2023.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.079139 predibase-2023.7.1/predibase/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.079139 predibase-2023.7.1/predibase/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli_commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli_commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli_commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/connection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/deployment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/engine_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/llm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/permission_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.079139 predibase-2023.7.1/predibase/pql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/pql/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/pql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/pql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/query_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.083139 predibase-2023.7.1/predibase/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/connection_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/resource_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/triton_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 22:09:26.000000 predibase-2023.7.1/predibase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.079139 predibase-2023.7.1/predibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 22:09:27.000000 predibase-2023.7.1/predibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.083139 predibase-2023.7.1/predibase_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 22:09:27.083139 predibase-2023.7.1/predibase_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 22:08:36.000000 predibase-2023.7.1/predibase_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 22:09:26.000000 predibase-2023.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 22:08:36.000000 predibase-2023.7.1/requirements_predictor.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 22:09:27.083139 predibase-2023.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 22:08:36.000000 predibase-2023.7.1/setup.py
```

### Comparing `predibase-2023.5.8/predibase/cli.py` & `predibase-2023.7.1/predibase/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,30 +5,33 @@
 # from predibase.cli_commands import create
 # from predibase.cli_commands import list
 # from predibase.cli_commands import run
 from predibase.cli_commands import delete, deploy, prompt, settings
 from predibase.cli_commands.settings import load_settings, save_local_settings
 from predibase.cli_commands.utils import set_defaults_from_settings
 
-app = typer.Typer()
-# app.add_typer(run.app, name="run")
-# app.add_typer(create.app, name="create")
-# app.add_typer(list.app, name="list")
-app.add_typer(deploy.app, name="deploy")
-app.add_typer(delete.app, name="delete")
-app.add_typer(prompt.app, name="prompt")
-app.add_typer(settings.app, name="settings")
-
-
-@app.command()
-def init(repo: Optional[str] = None, engine: Optional[str] = None, quiet: bool = False):
-    if not quiet:
-        repo = repo or typer.prompt("Model repository name", default="")
-        engine = engine or typer.prompt("Engine name", default="")
-    save_local_settings({k: v for k, v in dict(repo=repo, engine=engine).items() if v})
+app = typer.Typer(help="Predibase CLI commands")
+
+app.add_typer(deploy.app, name="deploy", help="Deploy Predibase resources")
+app.add_typer(delete.app, name="delete", help="Delete Predibase resources")
+app.add_typer(prompt.app, name="prompt", help="Prompt Predibase models")
+app.add_typer(settings.app, name="settings", help="Configure Predibase settings")
+
+
+@app.command(help="Initialize default model repository and engine")
+def init(
+    repository_name: Optional[str] = typer.Option(
+        None,
+        "--repository-name",
+        "-r",
+        help="The optional model repository name",
+    ),
+    engine_name: Optional[str] = typer.Option(None, "--engine-name", "-e", help="The optional engine name"),
+):
+    save_local_settings({k: v for k, v in dict(repo=repository_name or "", engine=engine_name or "").items() if v})
 
 
 def main():
     set_defaults_from_settings(load_settings())
     app()
```

### Comparing `predibase-2023.5.8/predibase/cli_commands/deploy.py` & `predibase-2023.7.1/predibase/cli_commands/deploy.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,42 +8,52 @@
 app = typer.Typer()
 
 
 # TODO(travis): this should be dynamic based on model type and pushed to the backend
 DEFAULT_TEMPLATE = "llm-gpu-small"
 
 
-@app.command()
+@app.command(help="Create a Large Language Model (LLM) deployment")
 def llm(
-    name: str = typer.Argument(None, help="Name of the model"),
-    model_name: str = typer.Argument(None, help="Name of the model"),
+    deployment_name: str = typer.Option(
+        None,
+        "--deployment-name",
+        "-d",
+        prompt="Deployment name",
+        prompt_required=True,
+        help="Name of the deployment",
+    ),
+    model_name: str = typer.Option(
+        None,
+        "--model-name",
+        "-m",
+        prompt="Model to deploy",
+        prompt_required=True,
+        help="Name of the model",
+    ),
     engine_template: Optional[str] = typer.Option(
         DEFAULT_TEMPLATE,
         "--engine-template",
         "-e",
-        help="Engine template to provision for hosting the model",
+        prompt="Engine name",
+        prompt_required=False,
+        help="Optional engine template to provision for hosting the model",
     ),
     # auto_suspend_secs: Optional[int] = 3600,  # TODO: add ability to auto suspend
 ):
-    if name is None:
-        raise ValueError("name is required")
-
-    if model_name is None:
-        raise ValueError("model_name is required")
-
     # raise ValueError if name is not lower case alphanumeric characters or '-'
-    if re.match(r"^[a-z0-9-]+$", name) is None:
+    if re.match(r"^[a-z0-9-]+$", deployment_name) is None:
         raise ValueError("name must be lower case alphanumeric characters or '-'")
 
     client = get_client()
 
     get_console().print("Deploying an LLM with the following parameters:")
-    get_console().print("\tname:", name)
+    get_console().print("\tdeployment_name:", deployment_name)
     get_console().print("\tmodel_name:", model_name)
     get_console().print("\tengine_template:", engine_template)
 
-    client.session.post_json("/llms", json={"name": name, "modelName": model_name, "engineTemplate": engine_template})
+    client.deploy_llm(deployment_name, model_name, engine_template=engine_template)
     get_console().print("Deploy request sent.")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `predibase-2023.5.8/predibase/cli_commands/prompt.py` & `predibase-2023.7.1/predibase/cli_commands/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,78 @@
 from rich.table import Table
 
 from predibase.cli_commands.utils import get_client, get_console
 
 app = typer.Typer()
 
 
+@app.command(help="Query a Large Language Model (LLM)")
+def llm(
+    template: str = typer.Option(
+        None,
+        "--template",
+        "-t",
+        prompt="Template input",
+        prompt_required=True,
+        help="Prompt template input text",
+    ),
+    model_name: str = typer.Option(
+        None,
+        "--model-name",
+        "-m",
+        prompt="Model to query",
+        prompt_required=True,
+        help="Name of the model",
+    ),
+    index_name: Optional[str] = typer.Option(
+        None,
+        "--index-name",
+        "-i",
+        prompt_required=False,
+        help="Optional dataset to index",
+    ),
+    dataset_name: Optional[str] = typer.Option(
+        None,
+        "--dataset-name",
+        "-d",
+        prompt_required=False,
+        help="Optional dataset for batch inference",
+    ),
+    limit: Optional[int] = typer.Option(None, "--limit", "-l", prompt_required=False, help="Optional results limit"),
+):
+    client = get_client()
+
+    with Progress(
+        SpinnerColumn(),
+        TextColumn("[progress.description]{task.description}"),
+        transient=True,
+    ) as progress:
+        progress.add_task(description="Querying LLM...", total=None)
+
+        df = client.prompt(
+            template,
+            model_name,
+            index=index_name,
+            dataset=dataset_name,
+            limit=limit,
+            return_df=True,
+        )
+
+    table = Table(show_header=True, header_style="bold magenta")
+
+    # Modify the table instance to have the data from the DataFrame
+    table = df_to_table(df, table)
+
+    # Update the style of the table
+    table.row_styles = ["none", "dim"]
+    table.box = box.SIMPLE_HEAD
+
+    get_console().print(table)
+
+
 def df_to_table(
     pandas_dataframe: pd.DataFrame,
     rich_table: Table,
     show_index: bool = True,
     index_name: Optional[str] = None,
 ) -> Table:
     """Convert a pandas.DataFrame obj into a rich.Table obj.
@@ -39,47 +103,9 @@
         row = [str(index)] if show_index else []
         row += [str(x) for x in value_list]
         rich_table.add_row(*row)
 
     return rich_table
 
 
-@app.command()
-def llm(
-    template: str,
-    model_name: Optional[str] = typer.Option(None, "--model-name", "-m", prompt="Model to query"),
-    index: Optional[str] = typer.Option(None, "--index", "-i"),
-    dataset: Optional[str] = typer.Option(None, "--dataset", "-d"),
-    limit: Optional[int] = typer.Option(None, "--limit", "-l"),
-):
-    client = get_client()
-
-    with Progress(
-        SpinnerColumn(),
-        TextColumn("[progress.description]{task.description}"),
-        transient=True,
-    ) as progress:
-        progress.add_task(description="Querying LLM...", total=None)
-
-        df = client.prompt(
-            template,
-            model_name,
-            index=index,
-            dataset=dataset,
-            limit=limit,
-            return_df=True,
-        )
-
-    table = Table(show_header=True, header_style="bold magenta")
-
-    # Modify the table instance to have the data from the DataFrame
-    table = df_to_table(df, table)
-
-    # Update the style of the table
-    table.row_styles = ["none", "dim"]
-    table.box = box.SIMPLE_HEAD
-
-    get_console().print(table)
-
-
 if __name__ == "__main__":
     app()
```

### Comparing `predibase-2023.5.8/predibase/cli_commands/utils.py` & `predibase-2023.7.1/predibase/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/client.py` & `predibase-2023.7.1/predibase/client.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/connection.py` & `predibase-2023.7.1/predibase/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/connection_mixin.py` & `predibase-2023.7.1/predibase/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/dataset_mixin.py` & `predibase-2023.7.1/predibase/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/deployment_mixin.py` & `predibase-2023.7.1/predibase/deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/engine_mixin.py` & `predibase-2023.7.1/predibase/engine_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/llm_mixin.py` & `predibase-2023.7.1/predibase/llm_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 class LlmMixin:
     session: Session
 
     def prompt(
         self,
         templates: Union[str, List[str]],
         model_name: Union[str, List[str]],
-        index: Optional[Union[str, Dataset]] = None,
-        dataset: Optional[Union[str, Dataset]] = None,
+        index_name: Optional[Union[str, Dataset]] = None,
+        dataset_name: Optional[Union[str, Dataset]] = None,
         limit: Optional[int] = None,
         options: Optional[Dict[str, float]] = None,
         return_df: bool = False,
     ) -> Union[List[GeneratedResponse], pd.DataFrame]:
         options_str = ", ".join(f"{k}={v}" for k, v in options.items()) if options else ""
         options_clause = f"WITH OPTIONS ({options_str}) " if options_str else ""
 
         models = [model_name] if isinstance(model_name, str) else model_name
         models_str = ", ".join(f'"{m}"' for m in models)
         model_clause = f"USING {models_str} " if models_str else ""
 
-        index = self.get_dataset(index) if isinstance(index, str) else index
+        index = self.get_dataset(index_name) if isinstance(index_name, str) else index_name
         index_clause = f'OVER "{index.connection.name}"."{index.name}" ' if index else ""
 
-        dataset = self.get_dataset(dataset) if isinstance(dataset, str) else dataset
-        limit_clause = f" limit {limit}" if limit else ""
+        dataset = self.get_dataset(dataset_name) if isinstance(dataset_name, str) else dataset_name
+        limit_clause = f" LIMIT {limit}" if limit else ""
         given_clause = (
             f'GIVEN select * from "{dataset.connection.name}"."{dataset.name}"{limit_clause}' if dataset else ""
         )
 
         templates = [templates] if isinstance(templates, str) else templates
         templates_str = ", ".join(f"'{t}'" for t in templates)
         query_str = f"PROMPT {templates_str} {options_clause}{model_clause}{index_clause}{given_clause};"
@@ -52,14 +52,27 @@
 
         df = self.session.execute(
             query_str,
             connection_id=conn_id,
         )
         return GeneratedResponse.to_responses(df) if not return_df else df
 
+    def deploy_llm(self, deployment_name: str, model_name: str, engine_template: Optional[str] = None):
+        self.session.post_json(
+            "/llms",
+            json={
+                "name": deployment_name,
+                "modelName": model_name,
+                "engineTemplate": engine_template,
+            },
+        )
+
+    def delete_llm(self, deployment_name: str):
+        self.session.delete_json(f"/llms/{deployment_name}")
+
     @abstractmethod
     def get_dataset(self) -> Dataset:
         pass
 
     @abstractmethod
     def list_connections(self) -> List[Connection]:
         pass
```

### Comparing `predibase-2023.5.8/predibase/model_mixin.py` & `predibase-2023.7.1/predibase/model_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/permission_mixin.py` & `predibase-2023.7.1/predibase/permission_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/pql/__init__.py` & `predibase-2023.7.1/predibase/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/pql/adapter.py` & `predibase-2023.7.1/predibase/pql/adapter.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/pql/api.py` & `predibase-2023.7.1/predibase/pql/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,45 +3,27 @@
 
 import logging
 import sys
 import time
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
-import jinja2schema
 import pandas as pd
 import requests
 import requests.exceptions
-from jinja2 import Template
 from urllib3.util import Retry
 
 from predibase.pql.adapter import TimeoutHTTPAdapter
-from predibase.pql.utils import get_caller_global_local_vars, get_results_df, retry
+from predibase.pql.utils import get_results_df, retry
 from predibase.resource.user import User
 
-DEFAULT_API_ENDPOINT = "https://api.app.predibase.com"
+DEFAULT_API_ENDPOINT = "https://api.app.predibase.com/v1"
 DEFAULT_SERVING_ENDPOINT = "serving.app.predibase.com"
 
 
-def _render(s: str, params: Dict[str, Any]) -> Tuple[str, Dict[str, Any]]:
-    global_vars, local_vars = get_caller_global_local_vars()
-    variables = dict(global_vars, **local_vars, **params)
-    placeholders = jinja2schema.infer(s).keys()
-    placeholder_vars = {k: v for k, v in variables.items() if k in placeholders}
-
-    query_params = {}
-    for k, v in placeholder_vars.items():
-        if isinstance(v, pd.DataFrame):
-            query_params[k] = v.to_json()
-            placeholder_vars[k] = k
-
-    t = Template(s)
-    return t.render(**placeholder_vars), query_params
-
-
 class PQLException(RuntimeError):
     def __init__(self, message):
         super().__init__(message)
         self.message = message
 
 
 class ServerResponseError(RuntimeError):
@@ -73,15 +55,14 @@
         engine_id: Optional[int] = None,
     ) -> int:
         if not self.is_plan_expired():
             if not statement.endswith(";"):
                 statement += ";"
 
             params = params or {}
-            statement, params = _render(statement, params)
             if self.verbose:
                 logging.info("-- EXECUTE:")
                 logging.info(statement)
 
             conn = connection_id or self.connection_id
             resp = self._post(
                 "/queries",
@@ -294,27 +275,29 @@
     if t - last_t > 1:
         sys.stdout.write("")
         sys.stdout.flush()
         return t
     return last_t
 
 
-def _to_json(resp):
+def _to_json(resp: requests.Response) -> Dict:
     if resp.status_code != 200:
         if resp.status_code == 202:
             # Processing in progress
             return {}
 
         raise ServerResponseError(f"Error {resp.status_code}: {_get_error(resp)}", resp.status_code)
-    data = resp.json()
-    if data:
-        error_message = data.get("errorMessage")
-        if error_message:
-            raise PQLException(error_message)
-    return data
+    if resp.content:
+        data = resp.json()
+        if data:
+            error_message = data.get("errorMessage")
+            if error_message:
+                raise PQLException(error_message)
+        return data
+    return {}
 
 
 def _get_error(resp):
     data = resp.json()
     if data is None:
         return "Unknown server error"
     if "error" in data:
```

### Comparing `predibase-2023.5.8/predibase/pql/utils.py` & `predibase-2023.7.1/predibase/pql/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/predictor.py` & `predibase-2023.7.1/predibase/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,28 @@
 
         Set stream to true, to fetch results via secure grpc connection.
         """
         try:
             from predibase.triton_util import (
                 get_data_iterator,
                 get_grpc_creds,
+                InferenceServerException,
                 triton_predict_grpc_stream,
                 triton_predict_http,
             )
         except ModuleNotFoundError:
             print("Predict not supported, please ensure you have installed predictor requirements:")
             print('pip install "predibase[predictor]"')
             return
 
-        metadata = self.metadata()
+        try:
+            metadata = self.metadata()
+        except InferenceServerException as e:
+            print(f"Failed to get metadata: {e.message}")
+            return
 
         # Get model inputs and outputs from metadata
         model_inputs = [(md.name, md.shape, md.datatype) for md in metadata.inputs]
         model_outputs = [md.name for md in metadata.outputs]
 
         # Get the data iterator using model metadata
         data_iterator = get_data_iterator(metadata, input_df)
```

### Comparing `predibase-2023.5.8/predibase/query_mixin.py` & `predibase-2023.7.1/predibase/query_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/config.py` & `predibase-2023.7.1/predibase/resource/config.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/connection.py` & `predibase-2023.7.1/predibase/resource/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/connection_object.py` & `predibase-2023.7.1/predibase/resource/connection_object.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/connection_properties.py` & `predibase-2023.7.1/predibase/resource/connection_properties.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/dataset.py` & `predibase-2023.7.1/predibase/resource/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     _uuid: str = field(metadata=config(field_name="uuid"))
     _name: str = field(metadata=config(field_name="name"))
     _object_name: str = field(metadata=config(field_name="objectName"))
     _created: str = field(metadata=config(field_name="created"))
     _updated: str = field(metadata=config(field_name="updated"))
     _connection_id: int = field(metadata=config(field_name="connectionID"))
     _dataset_info: Optional[DatasetInfoWrapper] = field(metadata=config(field_name="datasetInfo"), default=None)
+    _dataset_profile: Dict = field(metadata=config(field_name="datasetProfile"), default=None)
     _connection: Optional[Connection] = field(metadata=config(field_name="connection"), default=None)
     _user: Optional[User] = field(metadata=config(field_name="user"), default=None)
 
     def __repr__(self):
         return (
             f"Dataset(id={self.id}, name={self.name}, object_name={self.object_name}, "
             f"connection_id={self.connection_id}, author={self.author}, "
@@ -142,14 +143,22 @@
         if self._dataset_info is None:
             resp = self._get(with_dataset_info=True)
             if "datasetInfo" in resp:
                 self._dataset_info = DatasetInfoWrapper.from_dict(resp["datasetInfo"])
         return self._dataset_info
 
     @property
+    def dataset_profile(self):
+        if self._dataset_profile is None:
+            resp = self._get(with_dataset_info=True)
+            if "datasetInfo" in resp and "datasetProfile" in resp["datasetInfo"]:
+                self._dataset_profile = resp["datasetInfo"]["datasetProfile"]["DatasetProfile"]
+        return self._dataset_profile
+
+    @property
     def created(self):
         return self._created
 
     @property
     def updated(self):
         return self._updated
```

### Comparing `predibase-2023.5.8/predibase/resource/dataset_info.py` & `predibase-2023.7.1/predibase/resource/dataset_info.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/deployment.py` & `predibase-2023.7.1/predibase/resource/deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,17 @@
         :param bool stream: Optional flag to stream results via gRPC protocol (default False).
         :return: pandas dataframe with predictions.
         """
         if not self.session.tenant:
             raise Exception("tenant must be set on session before calling predict")
         predictor = Predictor(self.session, deployment_name=self._name, deployment_version=self._deployment_version)
         results = predictor.predict(input_df, stream)
-        return results.to_pandas()
+        if results:
+            return results.to_pandas()
+        return pd.DataFrame()
 
     @spinner(name="Async Predict")
     async def async_predict(self, input_df: pd.DataFrame, stream=False) -> pd.DataFrame:
         """Make predictions for each row of the pandas dataframe.
 
         :param input_df pandas DataFrame: Required input dataframe.
         :param bool stream: Optional flag to stream results via gRPC protocol (default False).
@@ -50,15 +52,17 @@
             raise Exception("tenant must be set on session before calling predict")
         predictor = AsyncPredictor(
             self.session,
             deployment_name=self._name,
             deployment_version=self._deployment_version,
         )
         results = await predictor.predict(input_df, stream)
-        return results.to_pandas()
+        if results:
+            return results.to_pandas()
+        return pd.DataFrame()
 
     def __repr__(self):
         return (
             f"Deployment(name={self.name}, deployment_version={self.deployment_version}, "
             f"engine_name={self.engine_name}, model_name={self.model_name}, "
             f"model_version={self.model_version}, deployment_url={self.deployment_url}, "
             f"comment='{self.comment}', error_text='{self.error_text}')"
```

### Comparing `predibase-2023.5.8/predibase/resource/engine.py` & `predibase-2023.7.1/predibase/resource/engine.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/llm.py` & `predibase-2023.7.1/predibase/resource/llm.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/model.py` & `predibase-2023.7.1/predibase/resource/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import copy
 import datetime
 import os
+import tempfile
+import zipfile
 from collections import defaultdict
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import Any, Dict, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import pandas as pd
@@ -144,31 +146,67 @@
             name=self._name,
             config=config,
             dataset=dataset,
             description=description,
         )
 
     def upload_model(self, zip_fp: str, dataset: Optional[Dataset] = None) -> "Model":
-        with open(zip_fp, "rb") as f:
-            files = {"file": f}
+        required_metadata_files = ["model_hyperparameters.json", "training_progress.json", "training_set_metadata.json"]
 
-            file_name, _ = os.path.splitext(os.path.basename(zip_fp))
-            dataset_id = dataset.id if dataset is not None else self.latest_dataset_id
+        dataset_id = dataset.id if dataset is not None else self.latest_dataset_id
+        if dataset_id is None:
+            raise ValueError("must either provide a dataset or upload to a model repo with a dataset configured")
+
+        with tempfile.TemporaryDirectory() as tmpdir:
+            with zipfile.ZipFile(zip_fp, "r") as zf:
+                zf.extractall(path=tmpdir)
+
+            # Some model zips may save the files of interest in a model/ sub-directory.
+            model_artifacts_path = os.path.join(tmpdir, "model")
+            if not os.path.exists(model_artifacts_path):
+                # Since no model/ sub-directory exists, search at the root.
+                model_artifacts_path = tmpdir
+
+            for required_file in required_metadata_files + ["model_weights"]:
+                if not os.path.exists(os.path.join(model_artifacts_path, required_file)):
+                    raise FileNotFoundError(f"required file {required_file} not found in model zip archive")
+
+            metadata_zip_path = os.path.join(tmpdir, "model_metadata.zip")
+            with zipfile.ZipFile(metadata_zip_path, "w") as metadata_zip:
+                for f in required_metadata_files:
+                    metadata_zip.write(os.path.join(model_artifacts_path, f), arcname=f)
+
+            with open(metadata_zip_path, "rb") as zipped_metadata:
+                files = {"file": zipped_metadata}
+                file_name, _ = os.path.splitext(os.path.basename(metadata_zip_path))
+                data = {
+                    "fileName": file_name,
+                    "datasetID": dataset_id,
+                    "repoID": self.id,
+                }
+                register_model_resp = self.session.post("/models/register_uploaded_model", files=files, data=data)
+
+            model_dict = register_model_resp["model"]
+            upload_url = register_model_resp["modelWeightsPresignedUploadUrl"]
+            upload_required_headers = register_model_resp["modelWeightsUploadHeaders"]
+
+            # Get required headers for presigned url upload
+            headers = {"Content-Type": "binary/octet-stream"}
+            for k, v in upload_required_headers:
+                headers[k] = v
+
+            with open(os.path.join(model_artifacts_path, "model_weights"), "rb") as weights_file:
+                # Upload file to blob storage with pre-signed url
+                requests.put(upload_url, data=weights_file, headers=headers).raise_for_status()
 
-            if dataset_id is None:
-                raise ValueError("must either provide a dataset or upload to a model repo with a dataset configured")
+            # Signal successful upload of model weights.
+            self.session.post(f"/models/complete_upload_model/{model_dict['id']}")
 
-            data = {
-                "fileName": file_name,
-                "datasetID": dataset_id,
-                "repoID": self.id,
-            }
-
-            resp = self.session.post("/models/upload", files=files, data=data)
-            return self._build_model_with_backref(resp["model"])
+            model_dict["status"] = "ready"
+            return self._build_model_with_backref(model_dict)
 
     def list_models(self, df: bool = False):
         endpoint = f"/models/repo/{self._id}?withVersions=true"
         resp = self.session.get_json(endpoint)
         if df:
             return pd.DataFrame([m for m in resp["modelRepo"]["models"]])
         return [self._build_model_with_backref(m) for m in resp["modelRepo"]["models"]]
@@ -675,16 +713,16 @@
         connection_id = None
         if isinstance(source, Dataset):
             connection_id = source.connection_id
             source = f'SELECT * FROM "{source.connection.name}"."{source.name}"'
             if limit is not None:
                 source += f" LIMIT {limit}"
         elif isinstance(source, pd.DataFrame):
-            params = {"sdk_df_dataset": source}
-            source = "{{ sdk_df_dataset }}"
+            params = {"sdk_df_dataset": source.to_json()}
+            source = "sdk_df_dataset"
         elif not isinstance(source, str):
             raise Exception(f"unexpected source type {type(source)}")
         return source, params, connection_id
 
     def to_draft(self):
         return ModelDraft(
             session=self.session,
```

### Comparing `predibase-2023.5.8/predibase/resource/query.py` & `predibase-2023.7.1/predibase/resource/query.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource/user.py` & `predibase-2023.7.1/predibase/resource/user.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/resource_util.py` & `predibase-2023.7.1/predibase/resource_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/triton_util.py` & `predibase-2023.7.1/predibase/triton_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase/util.py` & `predibase-2023.7.1/predibase/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def get_url(session: Session, endpoint: str) -> str:
     if session.url == DEFAULT_API_ENDPOINT:
         root_url = "http://localhost:8000"
     else:
         url = session.url
         if "api." in url:
-            url = url.replace("api.", "")
+            url = url.replace("api.", "").replace("/v1", "")
         root_url = url
     return f"{root_url}/{endpoint}"
 
 
 class JSONFloat(float):
     def __repr__(self):
         return format(Decimal(self), "f")
```

### Comparing `predibase-2023.5.8/predibase.egg-info/SOURCES.txt` & `predibase-2023.7.1/predibase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase_notebook/__init__.py` & `predibase-2023.7.1/predibase_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/predibase_notebook/env.py` & `predibase-2023.7.1/predibase_notebook/env.py`

 * *Files identical despite different names*

### Comparing `predibase-2023.5.8/setup.py` & `predibase-2023.7.1/setup.py`

 * *Files identical despite different names*


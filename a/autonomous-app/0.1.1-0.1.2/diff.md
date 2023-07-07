# Comparing `tmp/autonomous-app-0.1.1.tar.gz` & `tmp/autonomous-app-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.1.1.tar", last modified: Wed Jul  5 17:12:59 2023, max compression
+gzip compressed data, was "autonomous-app-0.1.2.tar", last modified: Fri Jul  7 13:30:54 2023, max compression
```

## Comparing `autonomous-app-0.1.1.tar` & `autonomous-app-0.1.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.622607 autonomous-app-0.1.1/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.1/LICENSE
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-05 17:12:59.621607 autonomous-app-0.1.1/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.1/README.md
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1401 2023-06-28 15:16:05.000000 autonomous-app-0.1.1/pyproject.toml
--rw-r--r--   0 samoore   (1000) samoore   (1000)      510 2023-06-12 14:16:24.000000 autonomous-app-0.1.1/requirements.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-05 17:12:59.622607 autonomous-app-0.1.1/setup.cfg
--rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.1/setup.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.616607 autonomous-app-0.1.1/src/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.617607 autonomous-app-0.1.1/src/autonomous/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-05 17:08:40.000000 autonomous-app-0.1.1/src/autonomous/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.617607 autonomous-app-0.1.1/src/autonomous/apis/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.1/src/autonomous/apis/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1793 2023-06-28 16:27:02.000000 autonomous-app-0.1.1/src/autonomous/apis/openai.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.617607 autonomous-app-0.1.1/src/autonomous/apis/version_control/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.1/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.1/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.1/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.1/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.1/src/autonomous/apis/version_control/__init__.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.615607 autonomous-app-0.1.1/src/autonomous/app_template/
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.618607 autonomous-app-0.1.1/src/autonomous/app_template/app/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-04-04 14:32:12.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1495 2023-04-28 17:49:36.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      574 2023-04-28 17:51:04.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/config.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.618607 autonomous-app-0.1.1/src/autonomous/app_template/app/models/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/models/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/models/model.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.618607 autonomous-app-0.1.1/src/autonomous/app_template/app/views/
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/views/admin.py
--rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.1/src/autonomous/app_template/app/views/index.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.618607 autonomous-app-0.1.1/src/autonomous/app_template/tests/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.1/src/autonomous/app_template/tests/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.1/src/autonomous/app_template/tests/test_app.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-04-04 18:40:13.000000 autonomous-app-0.1.1/src/autonomous/app_template/tests/test_modules.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.619607 autonomous-app-0.1.1/src/autonomous/app_template/vendor/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.1/src/autonomous/app_template/vendor/gunicorn.conf.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.1/src/autonomous/assets.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.1/src/autonomous/cli.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.619607 autonomous-app-0.1.1/src/autonomous/db/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       95 2023-06-28 15:23:00.000000 autonomous-app-0.1.1/src/autonomous/db/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      840 2023-06-28 15:22:15.000000 autonomous-app-0.1.1/src/autonomous/db/autodb.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.1/src/autonomous/db/storage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.1/src/autonomous/db/table.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.1/src/autonomous/logger.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.619607 autonomous-app-0.1.1/src/autonomous/model/
--rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.1/src/autonomous/model/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3278 2023-06-15 19:12:58.000000 autonomous-app-0.1.1/src/autonomous/model/automodel.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.1/src/autonomous/model/orm.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.620607 autonomous-app-0.1.1/src/autonomous/storage/
--rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.1/src/autonomous/storage/__init__.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.1/src/autonomous/storage/basestorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1618 2023-06-08 12:35:19.000000 autonomous-app-0.1.1/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.1/src/autonomous/storage/localstorage.py
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.1/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-05 17:12:59.621607 autonomous-app-0.1.1/src/autonomous_app.egg-info/
--rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-05 17:12:59.000000 autonomous-app-0.1.1/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 samoore   (1000) samoore   (1000)     1641 2023-07-05 17:12:59.000000 autonomous-app-0.1.1/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-05 17:12:59.000000 autonomous-app-0.1.1/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-05 17:12:59.000000 autonomous-app-0.1.1/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-07-05 17:12:59.000000 autonomous-app-0.1.1/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-07-05 17:12:59.000000 autonomous-app-0.1.1/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.388411 autonomous-app-0.1.2/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1076 2023-03-07 12:36:40.000000 autonomous-app-0.1.2/LICENSE
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-07 13:30:54.387411 autonomous-app-0.1.2/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2011 2023-06-20 21:09:23.000000 autonomous-app-0.1.2/README.md
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1431 2023-07-07 12:26:43.000000 autonomous-app-0.1.2/pyproject.toml
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      510 2023-06-12 14:16:24.000000 autonomous-app-0.1.2/requirements.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-07-07 13:30:54.388411 autonomous-app-0.1.2/setup.cfg
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       38 2023-04-04 14:14:59.000000 autonomous-app-0.1.2/setup.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.376411 autonomous-app-0.1.2/src/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.378411 autonomous-app-0.1.2/src/autonomous/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       86 2023-07-07 13:14:12.000000 autonomous-app-0.1.2/src/autonomous/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.379411 autonomous-app-0.1.2/src/autonomous/apis/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       27 2023-06-20 19:34:19.000000 autonomous-app-0.1.2/src/autonomous/apis/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2149 2023-07-07 13:12:31.000000 autonomous-app-0.1.2/src/autonomous/apis/openai.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.380411 autonomous-app-0.1.2/src/autonomous/apis/version_control/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1069 2023-03-07 16:24:11.000000 autonomous-app-0.1.2/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1155 2023-03-07 21:09:26.000000 autonomous-app-0.1.2/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     4622 2023-03-07 16:24:11.000000 autonomous-app-0.1.2/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      196 2023-03-07 16:24:11.000000 autonomous-app-0.1.2/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      117 2023-03-07 16:24:11.000000 autonomous-app-0.1.2/src/autonomous/apis/version_control/__init__.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.376411 autonomous-app-0.1.2/src/autonomous/app_template/
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.380411 autonomous-app-0.1.2/src/autonomous/app_template/app/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       29 2023-04-04 14:32:12.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1495 2023-04-28 17:49:36.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      574 2023-04-28 17:51:04.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/config.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.381411 autonomous-app-0.1.2/src/autonomous/app_template/app/models/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-04-04 14:32:12.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/models/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      203 2023-04-04 15:41:08.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/models/model.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.381411 autonomous-app-0.1.2/src/autonomous/app_template/app/views/
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-04 14:32:12.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/views/admin.py
+-rwxr-xr-x   0 samoore   (1000) samoore   (1000)      589 2023-04-28 17:48:57.000000 autonomous-app-0.1.2/src/autonomous/app_template/app/views/index.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.382411 autonomous-app-0.1.2/src/autonomous/app_template/tests/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-04 14:32:12.000000 autonomous-app-0.1.2/src/autonomous/app_template/tests/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      204 2023-04-04 18:40:47.000000 autonomous-app-0.1.2/src/autonomous/app_template/tests/test_app.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      558 2023-04-04 18:40:13.000000 autonomous-app-0.1.2/src/autonomous/app_template/tests/test_modules.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.382411 autonomous-app-0.1.2/src/autonomous/app_template/vendor/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1124 2023-04-13 17:57:17.000000 autonomous-app-0.1.2/src/autonomous/app_template/vendor/gunicorn.conf.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2252 2023-06-08 19:19:57.000000 autonomous-app-0.1.2/src/autonomous/assets.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       42 2023-04-04 14:14:59.000000 autonomous-app-0.1.2/src/autonomous/cli.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.383411 autonomous-app-0.1.2/src/autonomous/db/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       94 2023-07-07 12:00:23.000000 autonomous-app-0.1.2/src/autonomous/db/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      812 2023-07-07 12:05:15.000000 autonomous-app-0.1.2/src/autonomous/db/autodb.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      531 2023-04-04 14:14:59.000000 autonomous-app-0.1.2/src/autonomous/db/storage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     2521 2023-06-20 21:17:55.000000 autonomous-app-0.1.2/src/autonomous/db/table.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1245 2023-06-01 20:06:24.000000 autonomous-app-0.1.2/src/autonomous/logger.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.384411 autonomous-app-0.1.2/src/autonomous/model/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        0 2023-04-02 18:01:05.000000 autonomous-app-0.1.2/src/autonomous/model/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3278 2023-06-15 19:12:58.000000 autonomous-app-0.1.2/src/autonomous/model/automodel.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      650 2023-06-13 18:03:23.000000 autonomous-app-0.1.2/src/autonomous/model/orm.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.385411 autonomous-app-0.1.2/src/autonomous/storage/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       88 2023-06-13 18:11:53.000000 autonomous-app-0.1.2/src/autonomous/storage/__init__.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      447 2023-06-05 17:49:27.000000 autonomous-app-0.1.2/src/autonomous/storage/basestorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1620 2023-07-07 13:13:20.000000 autonomous-app-0.1.2/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      156 2023-06-13 18:11:43.000000 autonomous-app-0.1.2/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1381 2023-06-13 18:12:16.000000 autonomous-app-0.1.2/src/autonomous/storage/s3storage.py
+drwxr-xr-x   0 samoore   (1000) samoore   (1000)        0 2023-07-07 13:30:54.387411 autonomous-app-0.1.2/src/autonomous_app.egg-info/
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     3809 2023-07-07 13:30:54.000000 autonomous-app-0.1.2/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 samoore   (1000) samoore   (1000)     1641 2023-07-07 13:30:54.000000 autonomous-app-0.1.2/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)        1 2023-07-07 13:30:54.000000 autonomous-app-0.1.2/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       53 2023-07-07 13:30:54.000000 autonomous-app-0.1.2/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)      148 2023-07-07 13:30:54.000000 autonomous-app-0.1.2/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 samoore   (1000) samoore   (1000)       11 2023-07-07 13:30:54.000000 autonomous-app-0.1.2/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.1.1/LICENSE` & `autonomous-app-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/PKG-INFO` & `autonomous-app-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.1
+Version: 0.1.2
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.1/README.md` & `autonomous-app-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/pyproject.toml` & `autonomous-app-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -35,11 +35,14 @@
 
 [tool.setuptools.packages.find]
 # All the following settings are optional:
 where = ["src"]
 include = ["autonomous*"]
 
 [tool.pytest.ini_options]
-addopts = "--cov=autonomous -rx -l -x -s --log-level=INFO --ignore=src --no-cov-on-fail --import-mode=importlib" #  -v  --cov-reset
+addopts = "--cov=autonomous -rx -l -x -s --log-level=INFO --ignore=src --no-cov-on-fail -v --import-mode=importlib" # --cov-reset
 testpaths = [
      "tests",
-]
+]
+
+[tool.isort]
+profile = "black"
```

### Comparing `autonomous-app-0.1.1/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.1.2/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.1.2/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.1.2/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/app_template/app/app.py` & `autonomous-app-0.1.2/src/autonomous/app_template/app/app.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/app_template/app/config.py` & `autonomous-app-0.1.2/src/autonomous/app_template/app/config.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/app_template/app/views/admin.py` & `autonomous-app-0.1.2/src/autonomous/app_template/app/views/admin.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/app_template/app/views/index.py` & `autonomous-app-0.1.2/src/autonomous/app_template/app/views/index.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/app_template/tests/test_modules.py` & `autonomous-app-0.1.2/src/autonomous/app_template/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/app_template/vendor/gunicorn.conf.py` & `autonomous-app-0.1.2/src/autonomous/app_template/vendor/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/assets.py` & `autonomous-app-0.1.2/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/db/autodb.py` & `autonomous-app-0.1.2/src/autonomous/db/autodb.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import pathlib
 
 # from autonomous import log
 from .table import Table
 
 
 class Database:
-    def __init__(self, path="."):
+    def __init__(self, path=""):
         """
         create an interface for your database
         """
         if not path.startswith("/"):
             path = f"{pathlib.Path().resolve()}{path}"
         if not path.endswith("/"):
             path = path + "/"
+
         self.db_path = f'{path}{os.environ.get("DB_NAME", "tables")}'
-        # log(self.db_path)
         os.path.isdir(self.db_path) or os.makedirs(self.db_path)
         self.tables = {}
 
     def get_table(self, table="default"):
         """
         opens the table from the file, which clears any changed data
         """
```

### Comparing `autonomous-app-0.1.1/src/autonomous/db/storage.py` & `autonomous-app-0.1.2/src/autonomous/db/storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/db/table.py` & `autonomous-app-0.1.2/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/logger.py` & `autonomous-app-0.1.2/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/model/automodel.py` & `autonomous-app-0.1.2/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/model/orm.py` & `autonomous-app-0.1.2/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.1.2/src/autonomous/storage/cloudinarystorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             api_key=self.api_key,
             api_secret=self.api_secret,
             secure=True,
         )
 
     @classmethod
     def get_metadata(cls, asset_id):
-        log(cls.api_secret, cls.api_key, cls.cloud_name)
+        # log(cls.api_secret, cls.api_key, cls.cloud_name)
         return cloudinary.api.resource_by_asset_id(asset_id)
 
     def geturl(self, key):
         response = self.get_metadata(key)
         return response.get("url")
 
     def save(self, file, **kwargs):
```

### Comparing `autonomous-app-0.1.1/src/autonomous/storage/s3storage.py` & `autonomous-app-0.1.2/src/autonomous/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.1.1/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.1.2/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.1.1
+Version: 0.1.2
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous-app-0.1.1/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous-app-0.1.2/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*


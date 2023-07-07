# Comparing `tmp/cosmotech-run-orchestrator-1.0.1.tar.gz` & `tmp/cosmotech-run-orchestrator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-run-orchestrator-1.0.1.tar", last modified: Thu Jul  6 15:46:42 2023, max compression
+gzip compressed data, was "cosmotech-run-orchestrator-1.0.2.tar", last modified: Fri Jul  7 08:35:42 2023, max compression
```

## Comparing `cosmotech-run-orchestrator-1.0.1.tar` & `cosmotech-run-orchestrator-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1260 2023-07-06 15:34:06.000000 cosmotech-run-orchestrator-1.0.1/LICENCE.md
--rw-r--r--   0 afossart  (1001) afossart  (1001)       58 2023-07-06 14:39:00.000000 cosmotech-run-orchestrator-1.0.1/MANIFEST.in
--rw-r--r--   0 afossart  (1001) afossart  (1001)      285 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/PKG-INFO
--rw-r--r--   0 afossart  (1001) afossart  (1001)      269 2023-06-26 12:51:15.000000 cosmotech-run-orchestrator-1.0.1/README.md
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/
--rw-r--r--   0 afossart  (1001) afossart  (1001)       18 2023-07-06 15:46:22.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/__init__.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/
--rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-06-15 09:01:23.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/__init__.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     9932 2023-07-06 15:34:44.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     5362 2023-07-06 15:34:41.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)    19950 2023-07-06 15:34:51.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1926 2023-07-06 15:34:57.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/main.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     3189 2023-07-06 15:35:13.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/orchestrator.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     7133 2023-07-06 15:35:18.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/parameters_generation.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     4881 2023-07-06 15:35:23.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/run_step.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     7993 2023-07-06 15:35:32.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/
--rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-07-06 12:57:57.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/__init__.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1303 2023-07-06 15:35:44.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/command_template.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1440 2023-07-06 15:35:53.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/environment.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     4719 2023-07-06 15:35:59.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/orchestrator.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      968 2023-07-06 15:36:04.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/runner.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     6101 2023-07-06 15:36:13.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/step.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/schema/
--rw-r--r--   0 afossart  (1001) afossart  (1001)     4094 2023-07-06 08:43:07.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/schema/run_template_json_schema.json
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/
--rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-06-15 13:17:05.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/__init__.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     2686 2023-07-06 15:36:22.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/api.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      848 2023-07-06 15:36:30.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/click.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      912 2023-07-06 15:36:34.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/decorators.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      879 2023-07-06 15:36:41.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/json.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      970 2023-07-06 15:36:53.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/logger.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      653 2023-07-06 15:37:00.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/singleton.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/
--rw-r--r--   0 afossart  (1001) afossart  (1001)      285 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1539 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)        1 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)       90 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/entry_points.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)        1 2023-07-06 13:40:56.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/not-zip-safe
--rw-r--r--   0 afossart  (1001) afossart  (1001)      229 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/requires.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)       10 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)       38 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/setup.cfg
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1185 2023-07-06 15:40:44.000000 cosmotech-run-orchestrator-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.271175 cosmotech-run-orchestrator-1.0.2/cosmotech/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.275175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.275175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/parameters_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.279175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/command_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.279175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/schema/run_template_json_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.279175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/setup.py
```

### Comparing `cosmotech-run-orchestrator-1.0.1/LICENCE.md` & `cosmotech-run-orchestrator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/download_cloud_steps.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/download_cloud_steps.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/legacy_json_generator.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/legacy_json_generator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/main.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/main.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/orchestrator.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/parameters_generation.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/parameters_generation.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/run_step.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/command_template.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/command_template.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/environment.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/environment.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/orchestrator.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/runner.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/runner.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/step.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/schema/run_template_json_schema.json` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/schema/run_template_json_schema.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/api.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/api.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/click.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/click.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/decorators.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/json.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/logger.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/singleton.py` & `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/SOURCES.txt` & `cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-LICENCE.md
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 cosmotech/orchestrator/__init__.py
 cosmotech/orchestrator/console_scripts/__init__.py
 cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
 cosmotech/orchestrator/console_scripts/download_cloud_steps.py
```

### Comparing `cosmotech-run-orchestrator-1.0.1/setup.py` & `cosmotech-run-orchestrator-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,27 +6,34 @@
 # specifically authorized by written means by Cosmo Tech.
 
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 from cosmotech.orchestrator import VERSION
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='cosmotech-run-orchestrator',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url="https://github.com/Cosmo-Tech/run_template_orchestrator",
     description='Orchestration suite for Cosmotech Run Templates',
     packages=find_namespace_packages(include=["cosmotech.*"]),
     include_package_data=True,
     zip_safe=False,
+    long_description=long_description,
+    long_description_type="text/markdown",
+    license_files=("LICENSE",),
     install_requires=required,
     entry_points={
         'console_scripts': [
             'csm-run-orchestrator=cosmotech.orchestrator.console_scripts.main:main',
         ]
     },
 )
```


# Comparing `tmp/cosmotech-run-orchestrator-1.0.2.tar.gz` & `tmp/cosmotech-run-orchestrator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-run-orchestrator-1.0.2.tar", last modified: Fri Jul  7 08:35:42 2023, max compression
+gzip compressed data, was "cosmotech-run-orchestrator-1.0.3.tar", last modified: Fri Jul  7 09:44:02 2023, max compression
```

## Comparing `cosmotech-run-orchestrator-1.0.2.tar` & `cosmotech-run-orchestrator-1.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.271175 cosmotech-run-orchestrator-1.0.2/cosmotech/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.275175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.275175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/parameters_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.279175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/command_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.279175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/schema/run_template_json_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.279175 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 08:35:42.000000 cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:35:42.283175 cosmotech-run-orchestrator-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 08:35:31.000000 cosmotech-run-orchestrator-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.065537 cosmotech-run-orchestrator-1.0.3/cosmotech/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.065537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/parameters_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/command_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/schema/run_template_json_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.069537 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:44:01.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 09:44:02.000000 cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 09:44:02.073537 cosmotech-run-orchestrator-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-07 09:43:49.000000 cosmotech-run-orchestrator-1.0.3/setup.py
```

### Comparing `cosmotech-run-orchestrator-1.0.2/LICENSE` & `cosmotech-run-orchestrator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/PKG-INFO` & `cosmotech-run-orchestrator-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cosmotech-run-orchestrator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Orchestration suite for Cosmotech Run Templates
-Home-page: https://github.com/Cosmo-Tech/run_template_orchestrator
+Home-page: https://github.com/Cosmo-Tech/run-orchestrator
 Author: Alexis Fossart
 Author-email: alexis.fossart@cosmotech.com
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cosmotech-run-orchestrator
 
 This library contains the `csm-run-orchestrator` cli developed by [Cosmo Tech](https://cosmotech.com/) for its Digital
 Twin platform.
 
 If you are interested in using it, please contact [Cosmo Tech](https://cosmotech.com/)
 
 ## Installation
 
 Documentation on the installation is available on
-our [GitHub Page](https://cosmo-tech.github.io/run_template_orchestrator/)
+our [GitHub Page](https://cosmo-tech.github.io/run-orchestrator/)
 
 Once installed you will have access to the `csm-run-orchestrator` CLI and all its commands.
```

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/download_cloud_steps.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/download_cloud_steps.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/legacy_json_generator.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/legacy_json_generator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/main.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/main.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/orchestrator.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/parameters_generation.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/parameters_generation.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/run_step.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/command_template.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/command_template.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/environment.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/environment.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/orchestrator.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/runner.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/runner.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/core/step.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/core/step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/schema/run_template_json_schema.json` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/schema/run_template_json_schema.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/api.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/api.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/click.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/click.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/decorators.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/json.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/logger.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech/orchestrator/utils/singleton.py` & `cosmotech-run-orchestrator-1.0.3/cosmotech/orchestrator/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/PKG-INFO` & `cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cosmotech-run-orchestrator
-Version: 1.0.2
+Version: 1.0.3
 Summary: Orchestration suite for Cosmotech Run Templates
-Home-page: https://github.com/Cosmo-Tech/run_template_orchestrator
+Home-page: https://github.com/Cosmo-Tech/run-orchestrator
 Author: Alexis Fossart
 Author-email: alexis.fossart@cosmotech.com
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cosmotech-run-orchestrator
 
 This library contains the `csm-run-orchestrator` cli developed by [Cosmo Tech](https://cosmotech.com/) for its Digital
 Twin platform.
 
 If you are interested in using it, please contact [Cosmo Tech](https://cosmotech.com/)
 
 ## Installation
 
 Documentation on the installation is available on
-our [GitHub Page](https://cosmo-tech.github.io/run_template_orchestrator/)
+our [GitHub Page](https://cosmo-tech.github.io/run-orchestrator/)
 
 Once installed you will have access to the `csm-run-orchestrator` CLI and all its commands.
```

### Comparing `cosmotech-run-orchestrator-1.0.2/cosmotech_run_orchestrator.egg-info/SOURCES.txt` & `cosmotech-run-orchestrator-1.0.3/cosmotech_run_orchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.2/setup.py` & `cosmotech-run-orchestrator-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     required = f.read().splitlines()
 
 setup(
     name='cosmotech-run-orchestrator',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
-    url="https://github.com/Cosmo-Tech/run_template_orchestrator",
+    url="https://github.com/Cosmo-Tech/run-orchestrator",
     description='Orchestration suite for Cosmotech Run Templates',
     packages=find_namespace_packages(include=["cosmotech.*"]),
     include_package_data=True,
     zip_safe=False,
     long_description=long_description,
-    long_description_type="text/markdown",
+    long_description_content_type="text/markdown",
     license_files=("LICENSE",),
     install_requires=required,
     entry_points={
         'console_scripts': [
             'csm-run-orchestrator=cosmotech.orchestrator.console_scripts.main:main',
         ]
     },
```


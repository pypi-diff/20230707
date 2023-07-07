# Comparing `tmp/auterion-cli-1.1.0.tar.gz` & `tmp/auterion-cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.1.0.tar", last modified: Wed Jun 21 12:06:06 2023, max compression
+gzip compressed data, was "auterion-cli-1.2.0.tar", last modified: Fri Jul  7 12:10:11 2023, max compression
```

## Comparing `auterion-cli-1.1.0.tar` & `auterion-cli-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 12:06:04.000000 auterion-cli-1.1.0/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.192475 auterion-cli-1.1.0/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-21 12:06:06.000000 auterion-cli-1.1.0/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 12:06:05.000000 auterion-cli-1.1.0/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.192475 auterion-cli-1.1.0/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.192475 auterion-cli-1.1.0/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 12:06:06.196475 auterion-cli-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-21 12:05:51.000000 auterion-cli-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 12:10:11.000000 auterion-cli-1.2.0/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-07 12:10:04.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-07 12:10:04.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8807 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3690 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:10:11.920605 auterion-cli-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 12:10:03.000000 auterion-cli-1.2.0/setup.py
```

### Comparing `auterion-cli-1.1.0/README.md` & `auterion-cli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.2.0/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_command.py` & `auterion-cli-1.2.0/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980218855218855%*

 * *Differences: {"'definitions'": "{'AuterionAppYml': {'properties': {'dependencies': OrderedDict([('type', "*

 * *                  "'object'), ('additionalProperties', False), ('patternProperties', "*

 * *                  "OrderedDict([('^[a-z]+(\\\\.[a-z][a-z0-9-_]*)*$', OrderedDict([('type', "*

 * *                  "'string')]))])), ('minProperties', 1)])}}, 'AuterionAppYmlTargetPlatform': "*

 * *                  "{'pattern': '^skynode|ainode|jetson|simulation$'}}"}*

```diff
@@ -22,14 +22,24 @@
                 "auterion-app-base": {
                     "pattern": "^v\\d+|none$",
                     "type": "string"
                 },
                 "compose-override": {
                     "$ref": "compose-spec.json"
                 },
+                "dependencies": {
+                    "additionalProperties": false,
+                    "minProperties": 1,
+                    "patternProperties": {
+                        "^[a-z]+(\\.[a-z][a-z0-9-_]*)*$": {
+                            "type": "string"
+                        }
+                    },
+                    "type": "object"
+                },
                 "services": {
                     "$ref": "#/definitions/AuterionAppYmlServices"
                 },
                 "target-platform": {
                     "anyOf": [
                         {
                             "$ref": "#/definitions/AuterionAppYmlTargetPlatform"
@@ -203,12 +213,12 @@
                     "$ref": "#/definitions/AuterionAppYmlService"
                 }
             },
             "title": "AuterionAppYmlServices",
             "type": "object"
         },
         "AuterionAppYmlTargetPlatform": {
-            "pattern": "^skynode|ainode|jetson$",
+            "pattern": "^skynode|ainode|jetson|simulation$",
             "type": "string"
         }
     }
 }
```

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import pathlib
 import yaml
 import json
 import tempfile
 import jsonschema
 from auterioncli.commands.command_base import CliCommand
 from auterioncli.commands.app_sdk.environment import \
-    ensure_docker, ensure_mender_artifact, check_not_running_in_docker, MENDER_CI_TOOLS_TAG
+    ensure_docker, ensure_mender_artifact, check_not_running_in_docker, check_not_running_on_skynode, \
+    MENDER_CI_TOOLS_TAG
 from auterioncli.commands.app_sdk.slimify import slimify
 import subprocess
 import collections.abc
 import re
 import copy
 import sys
 
 DEVICE_ALIAS = {
     'ainode': 'jetson'
 }
 
 PLATFORM_ALIAS = {
     'skynode': 'linux/arm64',
-    'jetson': 'linux/arm64'
+    'jetson': 'linux/arm64',
+    'simulation': 'linux/amd64'
 }
 
 
 def deep_dict_update(d, u):
     for k, v in u.items():
         if isinstance(v, collections.abc.Mapping):
             d[k] = deep_dict_update(d.get(k, {}), v)
@@ -60,14 +62,15 @@
 
     def setup_parser(self, parser):
         parser.add_argument('project_dir', help='Location of the project', nargs='?', default='.')
         parser.add_argument('--skip-docker-build', help='Do not execute docker build step. Just package.', action='store_true')
         parser.add_argument('--skip-packaging', help='Do not create an AuterionOS app, just build the docker images and leave them in local docker.', action='store_true')
 
     def run(self, args):
+        check_not_running_on_skynode(self._config.get('this_device_type', 'unknown'))
         compose_cmd = ensure_docker()
         ensure_mender_artifact()
         check_not_running_in_docker()
 
         self._temp_dir = tempfile.mkdtemp()
         meta = self._load_metadata(args)
         self._verify_metadata(meta)
```

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/slimify.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     print(f'.. Pulled {base_image}')
     print('> Inspecting image')
     try:
         ret = run_docker_command(['docker', 'inspect', base_image])
     except:
         error(f'Failed to inspect image {base_image}. Aborting..')
 
-    assert(ret[0]['Architecture'] == 'arm64')
     assert(ret[0]['Os'] == 'linux')
     layers = ret[0]['RootFS']['Layers']
     print(f'.. Base image has {len(layers)} layers')
 
     if cache_dir is not None:
         cache_file = os.path.join(cache_dir, cache_key)
         with open(cache_file, 'w') as f:
```

### Comparing `auterion-cli-1.1.0/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.2.0/auterioncli/commands/app_sdk/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import enum
 from datetime import datetime
 try:
     from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
     from tqdm import tqdm
 except ImportError as e:
     print("Modules tqdm and requests-toolbelt are missing")
-    print("Run 'pip3 install --user -r setup/requirements.txt'")
     exit(1)
 
 UPDATE_ENDPOINT_BASE="http://{}/api/local-updater"
 TIMEOUT = 1800  # 30 minutes
 
 class ExitCode(enum.Enum):
     SUCCESS = 0
```

### Comparing `auterion-cli-1.1.0/auterioncli/commands/container_command.py` & `auterion-cli-1.2.0/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/device_command.py` & `auterion-cli-1.2.0/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/info_command.py` & `auterion-cli-1.2.0/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/report_command.py` & `auterion-cli-1.2.0/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/commands/utils.py` & `auterion-cli-1.2.0/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.1.0/auterioncli/main.py` & `auterion-cli-1.2.0/auterioncli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 from auterioncli.commands import available_commands
 
 from auterioncli.meta_util import PersistentState, check_for_updates, get_version, eprint, \
     get_device_presence, get_host_device_type
 
 
 def main():
-    persistent = PersistentState()
+    this_device_type = get_host_device_type()
+
+    persistent = PersistentState(this_device_type)
     selected_serial = persistent["selected_serial"]
     selected_address = persistent["selected_address"]
     have_selected_device = selected_serial is not None and selected_address is not None
 
-    host_device = get_host_device_type()
-    env_address = os.getenv('AUTERION_DEVICE_ADDRESS', "127.0.0.1" if host_device == 'skynode' else "10.41.1.1")
+    env_address = os.getenv('AUTERION_DEVICE_ADDRESS', "127.0.0.1" if this_device_type == 'skynode' else "10.41.1.1")
 
     config = {
         "persistent": persistent,
         "persistent_dir": persistent.persistent_dir,
         "device_address": selected_address if have_selected_device else env_address,
         "device_serial": selected_serial if have_selected_device else None,
-        "have_selected_device": have_selected_device
+        "have_selected_device": have_selected_device,
+        "this_device_type": this_device_type
     }
     commands = available_commands(config)
 
     main_parser = argparse.ArgumentParser()
     main_parser.add_argument('--version', help='Print version of this tool', action='store_true')
     command_subparsers = main_parser.add_subparsers(title="command", metavar='<command>', dest="root_command")
 
@@ -51,17 +53,18 @@
         device_present, serial_at_address = get_device_presence(config['device_address'])
         if not device_present:
             eprint(f"Error: No device reachable at {config['device_address']}.\n"
                    f"       Use 'device discover' command to show available devices.\n"
                    f"Aborting.\n")
             exit(1)
         elif not config['have_selected_device']:
-            eprint(f'Warn: No device serial selected.\n'
-                  f'      Use \'device discover\' and \'device select\' commands to specify which device to use.\n'
-                  f'      Falling back to device with serial {serial_at_address} on {config["device_address"]}\n')
+            if config['this_device_type'] != 'skynode':
+                eprint(f'Warn: No device serial selected.\n'
+                      f'      Use \'device discover\' and \'device select\' commands to specify which device to use.\n'
+                      f'      Falling back to device with serial {serial_at_address} on {config["device_address"]}\n')
 
         elif serial_at_address != config['device_serial']:
             if serial_at_address == '':
                 eprint(f"Warn: Could not verify serial number of device at address {config['device_address']}.\n"
                        f"You may be connected to the wrong device, "
                        f"or your device may be experiencing networking problems.\n"
                        f"Continuing anyways..")
```

### Comparing `auterion-cli-1.1.0/auterioncli/meta_util.py` & `auterion-cli-1.2.0/auterioncli/meta_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,22 @@
 
 
 def get_version():
     return pkg_resources.require('auterion-cli')[0].version
 
 
 class PersistentState:
-    def __init__(self):
+    def __init__(self, device_type):
         user_home = Path.home()
         self.persistent_dir = user_home / ".auterion-cli"
 
+        # On skynode, we can't store in the users home directory, because it is read-only
+        if device_type == 'skynode':
+            self.persistent_dir = Path('/var/auterion-cli')
+
         # make sure the persistent dir exits
         # Older auterion-cli had .auterion-cli as a file. Remove that file if it exists
         if self.persistent_dir.exists() and self.persistent_dir.is_file():
             os.unlink(self.persistent_dir)
 
         if not self.persistent_dir.exists():
             os.mkdir(self.persistent_dir)
```

### Comparing `auterion-cli-1.1.0/setup.py` & `auterion-cli-1.2.0/setup.py`

 * *Files identical despite different names*


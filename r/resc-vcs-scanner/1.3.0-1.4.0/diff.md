# Comparing `tmp/resc_vcs_scanner-1.3.0.tar.gz` & `tmp/resc_vcs_scanner-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scanner-1.3.0.tar", last modified: Thu May 25 09:50:49 2023, max compression
+gzip compressed data, was "resc_vcs_scanner-1.4.0.tar", last modified: Fri Jul  7 10:59:36 2023, max compression
```

## Comparing `resc_vcs_scanner-1.3.0.tar` & `resc_vcs_scanner-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.850524 resc_vcs_scanner-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.850524 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 09:50:49.000000 resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/env_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/finding_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/output_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/resc_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/celery_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/git_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/secret_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/stdout_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:49.854524 resc_vcs_scanner-1.3.0/src/vcs_scanner/static/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 09:50:43.000000 resc_vcs_scanner-1.3.0/src/vcs_scanner/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.264092 resc_vcs_scanner-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-07 10:59:36.264092 resc_vcs_scanner-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-07 10:59:36.264092 resc_vcs_scanner-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.260092 resc_vcs_scanner-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.260092 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:59:36.000000 resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.260092 resc_vcs_scanner-1.4.0/src/vcs_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.260092 resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/env_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/finding_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/output_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/resc_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.264092 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/celery_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/git_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/rws_api_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/secret_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/stdout_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:36.264092 resc_vcs_scanner-1.4.0/src/vcs_scanner/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 10:59:30.000000 resc_vcs_scanner-1.4.0/src/vcs_scanner/static/logging.ini
```

### Comparing `resc_vcs_scanner-1.3.0/PKG-INFO` & `resc_vcs_scanner-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scanner
-Version: 1.3.0
+Version: 1.4.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-1.3.0/setup.cfg` & `resc_vcs_scanner-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scanner
 description = Repository Scanner - Version Control System - Scanner
-version = 1.3.0
+version = 1.4.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/PKG-INFO` & `resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-vcs-scanner
-Version: 1.3.0
+Version: 1.4.0
 Summary: Repository Scanner - Version Control System - Scanner
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scanner-1.3.0/src/resc_vcs_scanner.egg-info/SOURCES.txt` & `resc_vcs_scanner-1.4.0/src/resc_vcs_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/common.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/env_default.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/env_default.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/helpers/environment_wrapper.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/helpers/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/input_parser.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/input_parser.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/model.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # pylint: disable=no-name-in-module
 # Standard Library
 import os
 from typing import List, Optional
 
 # Third Party
 from pydantic import BaseModel, conint, constr, validator
-from resc_backend.resc_web_service.schema.branch import Branch
 from resc_backend.resc_web_service.schema.repository import Repository
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 
 class RepositoryRuntime(BaseModel):
     repository_name: str
     repository_id: str
     repository_url: str
     project_key: str
     vcs_instance_name: str
-    branches: List[Branch]
+    latest_commit: Optional[str] = None
 
     def convert_to_repository(self, vcs_instance_id: int) -> Repository:
         return Repository(
             project_key=self.project_key,
             repository_id=self.repository_id,
             repository_name=self.repository_name,
             repository_url=self.repository_url,
             vcs_instance=vcs_instance_id,
-            branches=self.branches
+            latest_commit=self.latest_commit
         )
 
 
 class VCSInstanceRuntime(BaseModel):
     id_: Optional[int]
     name: constr(max_length=200)
     provider_type: VCSProviders
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/output_module.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/output_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 # Standard Library
 import abc
 from typing import List
 
 # Third Party
-from resc_backend.resc_web_service.schema.branch import Branch
 from resc_backend.resc_web_service.schema.finding import FindingCreate
 from resc_backend.resc_web_service.schema.repository import Repository
-from resc_backend.resc_web_service.schema.scan import Scan
+from resc_backend.resc_web_service.schema.scan import Scan, ScanRead
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 # First Party
 from vcs_scanner.model import VCSInstanceRuntime
 
 
 class OutputModule(metaclass=abc.ABCMeta):
     def write_vcs_instance(self, vcs_instance_runtime: VCSInstanceRuntime):
         pass
 
     def write_repository(self, repository: Repository):
         pass
 
-    def write_branch(self, repository: Repository, branch: Branch):
-        pass
-
     def write_findings(
             self,
             scan_id: int,
-            branch_id: int,
+            repository_id: int,
             scan_findings: List[FindingCreate],):
         pass
 
     def write_scan(
             self,
             scan_type_to_run: ScanType,
             last_scanned_commit: str,
             scan_timestamp: str,
-            branch: Branch,
+            repository: Repository,
             rule_pack: str) -> Scan:
         pass
 
-    def get_last_scanned_commit(self, branch: Branch):
+    def get_last_scan_for_repository(self, repository: Repository) -> ScanRead:
         pass
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/celery_worker.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/celery_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,26 +63,26 @@
     try:
         vcs_instance = vcs_instances[repository_runtime.vcs_instance_name]
 
         repository = Repository(project_key=repository_runtime.project_key,
                                 repository_id=repository_runtime.repository_id,
                                 repository_name=repository_runtime.repository_name,
                                 repository_url=repository_runtime.repository_url,
-                                vcs_instance=vcs_instance.id_,
-                                branches=repository_runtime.branches,
+                                vcs_instance=vcs_instance.id_
                                 )
 
         secret_scanner = SecretScanner(
             gitleaks_binary_path=env_variables[GITLEAKS_PATH],
             gitleaks_rules_path=TEMP_RULE_FILE,
             rule_pack_version=active_rule_pack_version,
             output_plugin=RESTAPIWriter(rws_url=rws_url),
             repository=repository,
             username=vcs_instance.username,
             personal_access_token=vcs_instance.token,
-            force_base_scan=os.getenv('FORCE_BASE_SCAN', "false").lower() in "true"
+            force_base_scan=os.getenv('FORCE_BASE_SCAN', "false").lower() in "true",
+            latest_commit=repository_runtime.latest_commit
         )
 
         secret_scanner.run_repository_scan()
     except KeyError:
         logger.error(f"No configuration found for vcs instance {repository_runtime.vcs_instance_name}, "
                      f"unable to scan {repository_runtime.project_key}/{repository_runtime.repository_name}")
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/cli.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import logging.config
 import os
 import pathlib
 from argparse import ArgumentParser, Namespace
 from urllib.parse import urlparse
 
 # Third Party
-from resc_backend.resc_web_service.schema.branch import Branch
 from resc_backend.resc_web_service.schema.vcs_provider import VCSProviders
 
 # First Party
 from vcs_scanner.common import get_rule_pack_version_from_file, initialise_logs
 from vcs_scanner.constants import CLI_VCS_AZURE, CLI_VCS_BITBUCKET, CLI_VCS_LOCAL_SCAN, LOG_FILE_PATH_CLI
 from vcs_scanner.helpers.env_default import EnvDefault
 from vcs_scanner.model import RepositoryRuntime
@@ -63,16 +62,14 @@
     parser_common.add_argument("-v", "--verbose", required=False, action="store_true",
                                help="Enable more verbose logging")
 
     repository_common = ArgumentParser(add_help=False)
     repository_common.add_argument("--repo-name", type=str, required=False, action=EnvDefault, envvar="RESC_REPO_NAME",
                                    help="The name of the repository. "
                                         "Can also be set via the RESC_REPO_NAME environment variable")
-    repository_common.add_argument("--branches", default=["master", "main"], nargs="+", required=False,
-                                   help="The name of the branches to scan, default main and master")
     repository_common.add_argument("--force-base-scan", required=False, action="store_true")
 
     repository_common.add_argument("--rws-url", type=str, required=False, action=EnvDefault, envvar="RESC_RWS_URL",
                                    help="The URL to the secret tracking service to which the scan results should "
                                         "be written. "
                                         "Can also be set via the RESC_RWS_URL environment variable")
 
@@ -194,15 +191,15 @@
     """
     repository = RepositoryRuntime(
         repository_url=FAKE_URL,
         repository_name="local",
         repository_id="local",
         project_key="local",
         vcs_instance_name="vcs_instance_name",
-        branches=[]
+        latest_commit=FAKE_COMMIT
     )
 
     output_plugin = STDOUTWriter(toml_rule_file_path=args.gitleaks_rules_path,
                                  exit_code_warn=args.exit_code_warn, exit_code_block=args.exit_code_block,
                                  filter_tag=args.filter_tag)
     with open(args.gitleaks_rules_path, encoding="utf-8") as rule_pack:
         rule_pack_version = get_rule_pack_version_from_file(rule_pack.read())
@@ -225,32 +222,24 @@
 
 def scan_repository(args: Namespace):
     """
         Start the process of scanning a git repository (remote or local)
     :param args:
         Namespace object containing the CLI arguments
     """
-    branches = []
-    for i, branch in enumerate(args.branches):
-        logger.info(f"Adding branch {branch} to the list of branches to be scanned")
-        branches.append(
-            Branch(**{"branch_name": branch, "branch_id": i, "latest_commit": FAKE_COMMIT})
-        )
-
     vcs_type = guess_vcs_provider(args.repo_url)
     vcs_name = determine_vcs_name(args.repo_url, vcs_type)
 
     repository = RepositoryRuntime(
         repository_url=args.repo_url,
         repository_name=args.repo_name,
         repository_id=args.repo_name,
         project_key=args.repo_name,
         vcs_instance_name=vcs_name,
-        branches=branches
-
+        latest_commit=FAKE_COMMIT
     )
 
     if args.rws_url:
         output_plugin = RESTAPIWriter(rws_url=args.rws_url)
         rule_pack_version = output_plugin.download_rule_pack()
 
     else:
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/configuration.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/git_operation.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/git_operation.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 # Third Party
 from git import Repo  # noqa: E402
 
 logger = logging.getLogger(__name__)
 
 
 def clone_repository(repository_url: str,
-                     branch_name: str,
                      repo_clone_path: str,
                      username: str = "",
                      personal_access_token: str = "") -> None:
     """
         Clones the given repository
     :param repository_url:
         Repository url to clone
-    :param branch_name:
-        Branch name of the repository url to clone
     :param repo_clone_path:
         Path where to clone the repository
     :param username:
         Username to clone the repository, only needed if the repository is private
     :param personal_access_token:
         Personal access token|password to clone the repository, only needed if the repository is private
     """
     url = repository_url.replace("https://", "")
     repo_clone_url = f"https://{username}:{personal_access_token}@{url}"
-    Repo.clone_from(repo_clone_url, repo_clone_path, branch=branch_name)
-    logger.debug(f"Repository {repository_url}:{branch_name} cloned successfully")
+    Repo.clone_from(repo_clone_url, repo_clone_path)
+    logger.debug(f"Repository {repository_url} cloned successfully")
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/gitleaks_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/rws_api_writer.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/rws_api_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 import sys
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, List, Optional
 
 # Third Party
 from resc_backend.constants import TEMP_RULE_FILE
-from resc_backend.resc_web_service.schema.branch import BranchCreate, BranchRead
 from resc_backend.resc_web_service.schema.finding import FindingBase, FindingCreate
 from resc_backend.resc_web_service.schema.repository import RepositoryCreate, RepositoryRead
 from resc_backend.resc_web_service.schema.scan import Scan, ScanCreate, ScanRead
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_instance import VCSInstanceCreate, VCSInstanceRead
-from resc_backend.resc_web_service_interface.branches import create_branch, get_last_scan_for_branch
 from resc_backend.resc_web_service_interface.findings import create_findings_with_scan_id
-from resc_backend.resc_web_service_interface.repositories import create_repository
+from resc_backend.resc_web_service_interface.repositories import create_repository, get_last_scan_for_repository
 from resc_backend.resc_web_service_interface.rule_packs import download_rule_pack_toml_file, get_rule_packs
 from resc_backend.resc_web_service_interface.scans import create_scan
 from resc_backend.resc_web_service_interface.vcs_instances import create_vcs_instance
 from tenacity import retry, stop_after_attempt, wait_exponential
 
 # First Party
 from vcs_scanner.common import get_rule_pack_version_from_file
@@ -51,86 +49,70 @@
             created_vcs_instance = VCSInstanceRead(**json.loads(response.text))
         else:
             logger.warning(f"Creating vcs_instance failed with error: {response.status_code}->{response.text}")
         return created_vcs_instance
 
     def write_repository(self, repository: RepositoryCreate) -> Optional[RepositoryRead]:
         created_repository = None
-        response = create_repository(self.rws_url,
-                                     repository)
+        response = create_repository(self.rws_url, repository)
         if response.status_code == 201:
             created_repository = RepositoryRead(**json.loads(response.text))
         else:
             logger.warning(f"Creating repository failed with error: {response.status_code}->{response.text}")
         return created_repository
 
-    def write_branch(self, repository: RepositoryRead, branch: BranchCreate) \
-            -> Optional[BranchRead]:
-        created_branch = None
-        branch = BranchCreate.create_from_base_class(
-            base_object=branch, repository_id=repository.id_)
-
-        response = create_branch(self.rws_url, branch)
-        if response.status_code == 201:
-            created_branch = BranchRead(**json.loads(response.text))
-        else:
-            logger.warning(f"Creating branch failed with error: {response.status_code}->{response.text}")
-        return created_branch
-
     def write_findings(
             self,
             scan_id: int,
-            branch_id: int,
+            repository_id: int,
             scan_findings: List[FindingBase], ):
         findings_create = []
         for finding in scan_findings:
-            new_finding = FindingCreate.create_from_base_class(base_object=finding, branch_id=branch_id)
+            new_finding = FindingCreate.create_from_base_class(base_object=finding, repository_id=repository_id)
             findings_create.append(new_finding)
 
         response = create_findings_with_scan_id(self.rws_url,
                                                 findings_create,
                                                 scan_id)
 
         if response.status_code != 201:
             logger.warning(f"Creating findings for scan {scan_id} "
                            f"failed with error: {response.status_code}->{response.text}")
-        logger.info(f"Found {len(scan_findings)} issues during scan: {scan_id} ")
+        logger.info(f"Found {len(scan_findings)} issues during scan for scan_id: {scan_id} ")
 
     def write_scan(
             self,
             scan_type_to_run: ScanType,
             last_scanned_commit: str,
             scan_timestamp: datetime,
-            branch: BranchRead,
+            repository: RepositoryRead,
             rule_pack: str) -> ScanRead:
         created_scan = None
         scan_object = ScanCreate.create_from_base_class(
             base_object=Scan(scan_type=scan_type_to_run, last_scanned_commit=last_scanned_commit,
-                             timestamp=scan_timestamp, rule_pack=rule_pack), branch_id=branch.id_)
+                             timestamp=scan_timestamp, rule_pack=rule_pack), repository_id=repository.id_)
 
         response = create_scan(self.rws_url, scan_object)
         if response.status_code == 201:
             created_scan = ScanRead(**json.loads(response.text))
-            logger.info(f"Successfully created scan for branch {branch.branch_name} ")
+            logger.info(f"Successfully created scan for repository {repository.repository_url} ")
         else:
             logger.warning(
                 f"Creating {scan_type_to_run} scan failed with error: {response.status_code}->{response.text}")
 
         return created_scan
 
-    def get_last_scanned_commit(self, branch: BranchRead):
-        last_scanned_commit = None
-        response = get_last_scan_for_branch(self.rws_url,
-                                            branch.id_)
+    def get_last_scan_for_repository(self, repository: RepositoryRead) -> ScanRead:
+        response = get_last_scan_for_repository(self.rws_url, repository.id_)
         if response.status_code == 200:
-            json_body = json.loads(response.text)
-            last_scanned_commit = json_body['last_scanned_commit'] if json_body else None
-        else:
-            logger.warning(f"Retrieving last scan details failed with error: {response.status_code}->{response.text}")
-        return last_scanned_commit
+            if not response.text or response.text == 'null':
+                return None
+            return ScanRead(**json.loads(response.text))
+        logger.warning(f"Retrieving last scan details failed with error: {response.status_code}->{response.text}")
+        return None
 
     @retry(wait=wait_exponential(multiplier=1, min=2, max=10), stop=stop_after_attempt(100))
     def write_vcs_instances(self, vcs_instances_dict: Dict[str, VCSInstanceRuntime]) \
             -> Dict[str, VCSInstanceRuntime]:
         try:
             for key in vcs_instances_dict:
                 vcs_instance = vcs_instances_dict[key]
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/secret_scanner.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/secret_scanner.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import uuid
 from datetime import datetime
 from typing import List, Optional
 
 # Third Party
 from resc_backend.resc_web_service.schema.finding import FindingBase
 from resc_backend.resc_web_service.schema.repository import Repository
+from resc_backend.resc_web_service.schema.scan import Scan
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 
 # First Party
 from vcs_scanner.output_module import OutputModule
 from vcs_scanner.resc_worker import RESCWorker
 from vcs_scanner.secret_scanners.git_operation import clone_repository
 from vcs_scanner.secret_scanners.gitleaks_wrapper import GitLeaksWrapper
@@ -35,35 +36,37 @@
                  rule_pack_version: str,
                  output_plugin: OutputModule,
                  repository: Repository,
                  username: str,
                  personal_access_token: str,
                  scan_tmp_directory: str = ".",
                  local_path: str = None,
-                 force_base_scan: bool = False):
+                 force_base_scan: bool = False,
+                 latest_commit: str = None):
 
         self.gitleaks_rules_path: str = gitleaks_rules_path
         self.gitleaks_binary_path: str = gitleaks_binary_path
         self.rule_pack_version: str = rule_pack_version
         self._output_module: OutputModule = output_plugin
         self._scan_tmp_directory: str = scan_tmp_directory
         self.repository: Repository = repository
         self.username: str = username
         self.personal_access_token: str = personal_access_token
         self.local_path = local_path
         self.force_base_scan = force_base_scan
+        self.latest_commit = latest_commit
         if self.local_path:
             self.repo_display_name = self.local_path.replace(".", "_").replace("/", "_")
         else:
             self.repo_display_name = self.repository.repository_url
 
-    def clone_repo(self, branch_name: str) -> str:
-        repo_clone_path = f"{self._scan_tmp_directory}/{self.repository.repository_name}@{branch_name}"
-        clone_repository(self.repository.repository_url, branch_name, repo_clone_path,
-                         username=self.username, personal_access_token=self.personal_access_token)
+    def clone_repo(self) -> str:
+        repo_clone_path = f"{self._scan_tmp_directory}/{self.repository.repository_name}"
+        clone_repository(self.repository.repository_url, repo_clone_path, username=self.username,
+                         personal_access_token=self.personal_access_token)
         return repo_clone_path
 
     def run_repository_scan(self) -> None:
         logger.info(
             f"Started task for scanning {self.repository.repository_name} using "
             f"rule pack version: {self.rule_pack_version}")
 
@@ -71,113 +74,91 @@
         created_repository = self._output_module.write_repository(self.repository)
         if not created_repository:
             logger.error(f"Error processing "
                          f"{self.repository.repository_name}."
                          f" Error details: unable to create repository: {created_repository}")
             return
 
-        for branch in self.repository.branches:
-            logger.info(f"Scanning branch {branch.branch_name} of repository "
-                        f"{self.repository.project_key}/{self.repository.repository_name}")
-
-            # Insert in to branch table
-            created_branch = self._output_module.write_branch(created_repository, branch)
-            if not created_branch:
-                logger.error(f"Error processing "
-                             f"{self.repository.project_key}/{self.repository.repository_name}:"
-                             f"{branch.branch_name}. Error details: unable to create branch")
-                return
+        logger.info(f"Scanning repository {self.repository.project_key}/{self.repository.repository_name}")
 
-            # Get last scanned commit for the branch
-            last_scanned_commit = self._output_module.get_last_scanned_commit(branch=created_branch)
+        # Get last scanned commit for the repository
+        last_scan_for_repository = self._output_module.get_last_scan_for_repository(repository=created_repository)
+        last_scanned_commit = last_scan_for_repository.last_scanned_commit if last_scan_for_repository else None
+        scan_type_to_run = self.determine_scan_type(latest_commit=self.latest_commit,
+                                                    last_scan_for_repository=last_scan_for_repository)
+
+        if scan_type_to_run:
+            # Insert in to scan table
+            scan_timestamp_start = datetime.utcnow()
+            created_scan = self._output_module.write_scan(
+                scan_type_to_run, self.latest_commit,
+                scan_timestamp_start.isoformat(), created_repository,
+                rule_pack=self.rule_pack_version)
+            if not created_scan:
+                logger.error(f"Error processing {self.repository.project_key}/{self.repository.repository_name} "
+                             f"Error details: unable to create scan object")
+                return
 
-            # Decide which type of scan to run
-            if self.force_base_scan:
-                scan_type_to_run = ScanType.BASE
+            # Clone and run scan upon the repository
+            if not self.local_path:
+                repo_clone_path: str = self.clone_repo()
             else:
-                scan_type_to_run = ScanType.INCREMENTAL if last_scanned_commit else ScanType.BASE
+                repo_clone_path = self.local_path
 
-            # Only insert in to scan and finding table if its BASE Scan or there is new commit, else skip
-            if scan_type_to_run == ScanType.BASE or last_scanned_commit != branch.latest_commit:
-                # Insert in to scan table
-                scan_timestamp_start = datetime.utcnow()
-                created_scan = self._output_module.write_scan(
-                    scan_type_to_run, branch.latest_commit,
-                    scan_timestamp_start.isoformat(), created_branch,
-                    rule_pack=self.rule_pack_version)
-                if not created_scan:
-                    logger.error(f"Error processing "
-                                 f"{self.repository.project_key}/{self.repository.repository_name}:"
-                                 f"{branch.branch_name}. Error details: unable to create scan object")
-                    return
-
-                # Clone and run scan upon the repository
-                if not self.local_path:
-                    repo_clone_path: str = self.clone_repo(branch.branch_name)
-                else:
-                    repo_clone_path = self.local_path
-
-                findings = self.scan_repo(scan_type_to_run,
-                                          branch.branch_name,
-                                          last_scanned_commit,
-                                          repo_clone_path)
-                scan_timestamp_end = datetime.utcnow()
-                logger.info(f"Running {scan_type_to_run} scan on branch {branch.branch_name} of repository "
-                            f"{self.repository.project_key}/{self.repository.repository_name}"
-                            f" took {scan_timestamp_end - scan_timestamp_start} ms.")
-
-                if findings:
-                    logger.info(f"Scan completed: {len(findings)} findings were found.")
-                    self._output_module.write_findings(branch_id=created_branch.id_, scan_id=created_scan.id_,
-                                                       scan_findings=findings)
-                else:
-                    logger.info("No findings registered in "
-                                f"{self.repository.project_key}/{self.repository.repository_name}"
-                                f":{branch.branch_name}.")
+            findings = self.scan_repo(scan_type_to_run, last_scanned_commit, repo_clone_path)
+            scan_timestamp_end = datetime.utcnow()
+            logger.info(f"Running {scan_type_to_run} scan on repository "
+                        f"{self.repository.project_key}/{self.repository.repository_name}"
+                        f" took {scan_timestamp_end - scan_timestamp_start} ms.")
+
+            if findings:
+                logger.info(f"Scan completed: {len(findings)} findings were found.")
+                self._output_module.write_findings(repository_id=created_repository.id_, scan_id=created_scan.id_,
+                                                   scan_findings=findings)
             else:
-                logger.info(f"Skipped {scan_type_to_run} scanning on branch: {branch.branch_name} of repository: "
-                            f"{self.repository.project_key}/{self.repository.repository_name}"
-                            f" no new commits found.")
+                logger.info("No findings registered in "
+                            f"{self.repository.project_key}/{self.repository.repository_name}")
+        else:
+            logger.info(f"Skipped {scan_type_to_run} scanning on repository: "
+                        f"{self.repository.project_key}/{self.repository.repository_name} no new commits found.")
 
     def run_directory_scan(self) -> None:
         """
             Scan the given non-git directory, set in the self.local_path variable
         """
         logger.info(f"Started task for scanning {self.local_path} using rule pack version: {self.rule_pack_version}")
 
         scan_timestamp_start = datetime.utcnow()
         findings = self.scan_directory(self.local_path)
         scan_timestamp_end = datetime.utcnow()
         logger.info(f"Running local scan on {self.local_path} took {scan_timestamp_end - scan_timestamp_start} ms.")
 
         if findings:
             logger.info(f"Scan completed: {len(findings)} findings were found.")
-            self._output_module.write_findings(branch_id=0, scan_id=0, scan_findings=findings)
+            self._output_module.write_findings(repository_id=0, scan_id=0, scan_findings=findings)
         else:
             logger.info(f"No findings registered in {self.local_path}.")
 
-    def scan_repo(self, scan_type_to_run: str, branch_name: str, last_scanned_commit: str, repo_clone_path: str) \
+    def scan_repo(self, scan_type_to_run: str, last_scanned_commit: str, repo_clone_path: str) \
             -> Optional[List[FindingBase]]:
 
         """
             Clone and scan the given repository
         :param repo_clone_path:
             Directory path where the repository has already been cloned
         :param scan_type_to_run:
             Type of scan to run (Base or Incremental)
-        :param branch_name:
-            Branch name of the repository url to scan
         :param last_scanned_commit:
-            Last scanned commit of the branch to scan
+            Last scanned commit of the repository to scan
         :return: Success, output.
             If Success is False, the output will contain an error message.
             Otherwise, the output will contain a list of findings or an empty list if no issue was found
         """
 
-        logger.debug(f"Started scanning {self.repo_display_name}:{branch_name}")
+        logger.debug(f"Started scanning {self.repo_display_name}")
         if not self.local_path:
             report_filepath = f"{self._scan_tmp_directory}/{repo_clone_path}_{str(uuid.uuid4().hex)}.json"
         else:
             report_filepath = f"{self.local_path}/{self.repo_display_name}_{str(uuid.uuid4().hex)}.json"
         try:
 
             if scan_type_to_run == ScanType.BASE:
@@ -197,17 +178,16 @@
             before_scan = time.time()
             findings: Optional[List[FindingBase]] = gitleaks_command.start_scan()
             after_scan = time.time()
             scan_duration = int(after_scan - before_scan)
             logger.info(f"scan of repository {repo_clone_path} took {scan_duration} seconds")
             return findings
         except BaseException as error:
-            logger.error(f"An exception occurred while scanning repository "
-                         f"{self.repository.repository_url}:{branch_name}"
-                         f" error: {error}")
+            logger.error(f"An exception occurred while scanning repository {self.repository.repository_url} "
+                         f"error: {error}")
         finally:
             # Make sure the tempfile and repo cloned path removed
             logger.debug(f"Cleaning up the temporary report: {report_filepath}")
             if os.path.exists(report_filepath):
                 os.remove(report_filepath)
             if repo_clone_path and not self.local_path and os.path.exists(repo_clone_path):
                 logger.debug(f"Cleaning up the repository cloned directory: {repo_clone_path}")
@@ -247,7 +227,23 @@
             logger.error(f"An exception occurred while scanning directory {directory_path} error: {error}")
         finally:
             # Make sure the tempfile is removed
             logger.debug(f"Cleaning up the temporary report: {report_filepath}")
             if os.path.exists(report_filepath):
                 os.remove(report_filepath)
         return None
+
+    # Decide which type of scan to run
+    def determine_scan_type(self, last_scan_for_repository: Scan, latest_commit: str = None):
+        # Force base scan, or has no previous scan
+        if self.force_base_scan or last_scan_for_repository is None:
+            return ScanType.BASE
+        # Has previous scan
+        if last_scan_for_repository:
+            # Rule-pack is different from previous scan
+            if last_scan_for_repository.rule_pack != self.rule_pack_version:
+                return ScanType.BASE
+            # Last commit is different from previous scan
+            if latest_commit and latest_commit != last_scan_for_repository.last_scanned_commit:
+                return ScanType.INCREMENTAL
+        # Skip scanning, no conditions match
+        return None
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/secret_scanners/stdout_writer.py` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/secret_scanners/stdout_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import sys
 from datetime import datetime
 from typing import List, Optional
 
 # Third Party
 import tomlkit
 from prettytable import PrettyTable
-from resc_backend.resc_web_service.schema.branch import Branch
 from resc_backend.resc_web_service.schema.finding import FindingCreate
 from resc_backend.resc_web_service.schema.repository import Repository
 from resc_backend.resc_web_service.schema.scan import ScanRead
 from resc_backend.resc_web_service.schema.scan_type import ScanType
 from resc_backend.resc_web_service.schema.vcs_instance import VCSInstanceRead
 from termcolor import colored
 
@@ -45,18 +44,14 @@
         logger.info(f"Scanning vcs instance {vcs_instance.name}")
         return vcs_instance
 
     def write_repository(self, repository: Repository) -> Repository:
         logger.info(f"Scanning repository {repository.project_key}/{repository.repository_name}")
         return repository
 
-    def write_branch(self, repository: Repository, branch: Branch) -> Optional[Branch]:
-        logger.info(f"Scanning branch {branch.branch_name} of repository {repository.repository_name}")
-        return branch
-
     def _get_rule_tags(self) -> dict:
         """
             Get the tags per rule from the .toml rule file, from self.toml_rule_file_path
         :return: dict.
             The output will contain a dictionary with the rule id as the key and the tags as a list in the value
         """
         rule_tags = {}
@@ -100,21 +95,21 @@
         :return bool:
             The output will be boolean, based on the tag filter given
         """
         if filter_tag and filter_tag not in rule_tags.get(finding.rule_name, []):
             return False
         return True
 
-    def write_findings(self, scan_id: int, branch_id: int, scan_findings: List[FindingCreate]):
+    def write_findings(self, scan_id: int, repository_id: int, scan_findings: List[FindingCreate]):
         """
             Write the findings to the STDOUT in a nice table and set the exit code based on the FindingActions found
         :param scan_id:
             id of the scan in question
-        :param branch_id:
-            id of the branch in question
+        :param repository_id:
+            id of the repository in question
         :param scan_findings:
             List of FindingCreate of all the findings from the scan
         """
         # Initialize table
         output_table = PrettyTable()
         output_table.field_names = ['Level', 'Rule', 'Line', 'Position', 'File path']
         output_table.align = 'l'
@@ -167,17 +162,17 @@
         elif exit_code == self.exit_code_warn:
             logger.info(f"Findings threshold check results: {colored('PASS', 'light_green', attrs=['bold'])}")
             logger.info(colored(f"Warning for policy violations: [Warn:{warn_count}]", "light_red", attrs=["bold"]))
 
         sys.exit(exit_code)
 
     def write_scan(self, scan_type_to_run: ScanType, last_scanned_commit: str, scan_timestamp: datetime,
-                   branch: Branch, rule_pack: str) -> Optional[ScanRead]:
-        logger.info(f"Running {scan_type_to_run} scan on branch {branch.branch_name}")
+                   repository: Repository, rule_pack: str) -> Optional[ScanRead]:
+        logger.info(f"Running {scan_type_to_run} scan on repository {repository.repository_url}")
         return ScanRead(last_scanned_commit="NONE",
                         timestamp=datetime.now(),
-                        branch_id=1,
+                        repository_id=1,
                         id_=1,
                         rule_pack=rule_pack)
 
-    def get_last_scanned_commit(self, branch: Branch):
+    def get_last_scan_for_repository(self, repository: Repository) -> ScanRead:
         return None
```

### Comparing `resc_vcs_scanner-1.3.0/src/vcs_scanner/static/logging.ini` & `resc_vcs_scanner-1.4.0/src/vcs_scanner/static/logging.ini`

 * *Files identical despite different names*


# Comparing `tmp/resc_vcs_scraper-1.3.0.tar.gz` & `tmp/resc_vcs_scraper-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_vcs_scraper-1.3.0.tar", last modified: Thu May 25 09:50:43 2023, max compression
+gzip compressed data, was "resc_vcs_scraper-1.4.0.tar", last modified: Fri Jul  7 10:59:26 2023, max compression
```

## Comparing `resc_vcs_scraper-1.3.0.tar` & `resc_vcs_scraper-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.203304 resc_vcs_scraper-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.203304 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 09:50:43.000000 resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/dict_remapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/environment_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/static/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/static/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:43.207305 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-25 09:50:33.000000 resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_instances_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.133722 resc_vcs_scraper-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 10:59:26.000000 resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/src/vcs_scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/dict_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/environment_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/src/vcs_scraper/project_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/project_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/project_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/src/vcs_scraper/repository_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/repository_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/repository_collector/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/src/vcs_scraper/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/static/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:26.137723 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/azure_devops_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/bitbucket_data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/github_public_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/vcs_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-07 10:59:18.000000 resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_instances_parser.py
```

### Comparing `resc_vcs_scraper-1.3.0/PKG-INFO` & `resc_vcs_scraper-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_vcs_scraper
-Version: 1.3.0
+Version: 1.4.0
 Summary: Repository Scanner - Version Control System - Scraper
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scraper-1.3.0/setup.cfg` & `resc_vcs_scraper-1.4.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_vcs_scraper
 description = Repository Scanner - Version Control System - Scraper
-version = 1.3.0
+version = 1.4.0
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/PKG-INFO` & `resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-vcs-scraper
-Version: 1.3.0
+Version: 1.4.0
 Summary: Repository Scanner - Version Control System - Scraper
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_vcs_scraper-1.3.0/src/resc_vcs_scraper.egg-info/SOURCES.txt` & `resc_vcs_scraper-1.4.0/src/resc_vcs_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/common.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/configuration.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/configuration.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/dict_remapper.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/dict_remapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/environment_wrapper.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/environment_wrapper.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/model.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,34 +11,22 @@
 from pydantic.types import conint, constr
 
 # First Party
 from vcs_scraper.constants import AZURE_DEVOPS, BITBUCKET, GITHUB_PUBLIC
 
 
 @dataclasses.dataclass
-class Branch:
-    repository_id: int
-    branch_name: str
-    branch_id: str
-    latest_commit: str
-
-    def json(self):
-        json_branch = json.dumps(dataclasses.asdict(self))
-        return json_branch
-
-
-@dataclasses.dataclass
 class Repository:
 
     repository_name: str
     repository_id: str
     repository_url: str
     project_key: str
     vcs_instance_name: str
-    branches: List[Branch]
+    latest_commit: str
 
     def json(self):
         json_repo = json.dumps(dataclasses.asdict(self))
         return json_repo
 
 
 class VCSProviders(str, Enum):
```

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/project_collector/common.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/project_collector/common.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/repository_collector/common.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/repository_collector/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,38 +35,36 @@
     """
     logger.info(f"Fetching repositories for project: '{project_key}' in vcs instance '{vcs_instance_name}'")
     project_repositories = vcs_client.get_repos(project_key)
     logger.info(f"Fetched {len(project_repositories)} repositories for project: '{project_key}'")
     project_tasks = []
     for repository in project_repositories:
         try:
-            logger.info(f"Fetching branches for repository: '{project_key}/{repository['name']}'")
-            repository_branches = vcs_client.get_branches(project_key=project_key, repository_id=repository["name"])
-            task_parameters = vcs_client.export_repository(repository, repository_branches, vcs_instance_name)
+            logger.info(f"Fetching latest commit for repository: '{project_key}/{repository['name']}'")
+            latest_commit = vcs_client.get_latest_commit(project_key=project_key, repository_id=repository["name"])
+            task_parameters = vcs_client.export_repository(repository, latest_commit, vcs_instance_name)
             project_tasks.append(task_parameters)
 
-            logger.info(f"{len(task_parameters.branches)} branch(es) for repository: "
-                        f"'{project_key}/{repository['name']}' were fetched successfully")
+            logger.info(f"Information for repository: '{project_key}/{repository['name']}' was fetched successfully")
         except requests.exceptions.HTTPError as http_exception:
             logger.error(
                 f"Error while processing repository '{project_key}/{repository['name']}':"
-                f" Unable to obtain the repository's branches: {http_exception}")
+                f" Unable to obtain the repository's latest commit: {http_exception}")
     return project_tasks
 
 
 def send_tasks_to_celery_queue(task_name: str, queue_name: str, project_tasks: List[Repository]):
     for task in project_tasks:
         celery_client.send_task(task_name, kwargs={"repository": task.json()}, queue=queue_name)
 
 
 @celery_client.task(Queue=PROJECT_QUEUE)
 def collect_repositories(project_key, vcs_instance_name):
     """
-    Celery worker which takes as input a project ID and collects the required information about all of its repos and
-    their respective branches.
+    Celery worker which takes as input a project ID and collects the required information about all of its repos.
     """
     vcs_instances_map = load_vcs_instances_into_map(env_variables[VCS_INSTANCES_FILE_PATH])
 
     logger.info(f"Project processor received an azure project key: '{project_key}'")
 
     vcs_client = VCSConnectorFactory.create_client_from_vcs_instance(vcs_instances_map[vcs_instance_name])
     project_tasks = extract_project_information(project_key, vcs_client, vcs_instance_name)
```

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/static/logging.ini` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/static/logging.ini`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/azure_devops_connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Standard Library
 import logging
-import os
-from typing import Dict, List
+from typing import Dict
 
 # Third Party
 from azure.devops.connection import Connection
 from azure.devops.exceptions import AzureDevOpsServiceError
 from azure.devops.released.core.core_client import CoreClient
 from msrest.authentication import BasicAuthentication
 from msrest.exceptions import ClientRequestError
 
 # First Party
-from vcs_scraper.model import Branch, Repository
-from vcs_scraper.vcs_connectors.azure_devops_data_mapper import map_azure_devops_branch, map_azure_devops_repository
+from vcs_scraper.model import Repository
+from vcs_scraper.vcs_connectors.azure_devops_data_mapper import map_azure_devops_repository
 from vcs_scraper.vcs_connectors.vcs_connector import VCSConnector
 from vcs_scraper.vcs_instances_parser import VCSInstance
 
 logger = logging.getLogger(__name__)
 
 
 class AzureDevopsConnector(VCSConnector):
@@ -79,54 +78,41 @@
 
     def project_exists(self, project_key: str) -> bool:
         return bool(self.core_api_client.get_project(project_key))
 
     def get_repos(self, project_key):
         return list(repo.as_dict() for repo in self.git_api_client.get_repositories(project_key))
 
-    def get_branches(self, project_key, repository_id):
-        all_branches = []
+    def get_latest_commit(self, project_key, repository_id):
+        latest_commit = None
         try:
-            all_branches = list(self.git_api_client.get_branches(project=project_key, repository_id=repository_id))
-            all_branches = [branch.as_dict() for branch in all_branches]
+            latest_commits = list(self.git_api_client.get_commits(project=project_key, repository_id=repository_id,
+                                                                  top=1, search_criteria=None))
+            if latest_commits:
+                latest_commit = latest_commits[0].commit_id
         except AzureDevOpsServiceError as azure_exception:
-            logger.error(f"Failed to list branches for repository: {project_key}/{repository_id} --> {azure_exception}")
-        return all_branches
+            logger.error(f"Failed to get latest commit for repository: {project_key}/{repository_id} --> "
+                         f"{azure_exception}")
+        return latest_commit
 
     @staticmethod
     def get_clone_url(clone_urls, name):
         for url in clone_urls:
             if url["name"] == name:
                 return url["href"]
         return ""
 
     @staticmethod
-    def export_repository(repository_information: Dict, branches_information: List[Dict],
-                          vcs_instance_name: str) \
-            -> Repository:
+    def export_repository(repository_information: Dict, latest_commit: str, vcs_instance_name: str) -> Repository:
         """
         A method which generate a repositoryInfo object about a single bitbucket repository.
 
         :param vcs_instance_name: Name of the VCS instance to which the repository belongs
         :param repository_information: Azure Devops repository information as returned by the Azure API.
-        :param branches_information: Azure Devops branches information for a single repo as returned by the Azure API.
+        :param latest_commit: Azure Devops latest_commit for a single repo as returned by the Azure API.
         :return Repository object
         """
-
-        branches: List[Branch] = []
-        for branch_information in branches_information:
-            if os.getenv('SCAN_ONLY_MASTER_BRANCH', "true").lower() in "true":
-                if branch_information["name"].lower() in ["main", "master"]:
-                    branch = Branch(repository_id=repository_information["id"],
-                                    **map_azure_devops_branch(branch_information))
-                    branches.append(branch)
-                    break
-            else:
-                branch = Branch(repository_id=repository_information["id"],
-                                **map_azure_devops_branch(branch_information))
-                branches.append(branch)
-
-        repository = Repository(branches=branches,
+        repository = Repository(latest_commit=latest_commit,
                                 vcs_instance_name=vcs_instance_name,
                                 **map_azure_devops_repository(repository_information))
 
         return repository
```

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/bitbucket_connector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Standard Library
-import os
-from typing import Dict, List
+from typing import Dict
 
 # Third Party
 import requests
 from atlassian import Bitbucket
 
 # First Party
-from vcs_scraper.model import Branch, Repository
-from vcs_scraper.vcs_connectors.bitbucket_data_mapper import map_bitbucket_branch, map_bitbucket_repository
+from vcs_scraper.model import Repository
+from vcs_scraper.vcs_connectors.bitbucket_data_mapper import map_bitbucket_repository
 from vcs_scraper.vcs_connectors.vcs_connector import VCSConnector
 from vcs_scraper.vcs_instances_parser import VCSInstance
 
 
 class BitbucketConnector(VCSConnector):
     def __init__(self, scheme, host, port, access_token, proxy=None):
         self.url = f"{scheme}://{host}:{port}"
@@ -51,48 +50,38 @@
 
     def project_exists(self, project_key: str) -> bool:
         return bool(self.api_client.project(project_key))
 
     def get_repos(self, project_key):
         return list(self.api_client.repo_all_list(project_key))
 
-    def get_branches(self, project_key, repository_id):
-        return list(self.api_client.get_branches(project_key, repository_id))
+    def get_latest_commit(self, project_key, repository_id):
+        last_commit = None
+        latest_edited_branch = list(self.api_client.get_branches(project_key, repository_id,
+                                                                 order_by="MODIFICATION", limit=1))
+        if latest_edited_branch:
+            last_commit = latest_edited_branch[0]["latestCommit"]
+        return last_commit
 
     @staticmethod
     def get_clone_url(clone_urls, name):
         for url in clone_urls:
             if url["name"] == name:
                 return url["href"]
         return ""
 
     @staticmethod
-    def export_repository(repository_information: Dict, branches_information: List[Dict],
-                          vcs_instance_name: str) \
-            -> Repository:
+    def export_repository(repository_information: Dict, latest_commit: str, vcs_instance_name: str) -> Repository:
         """
         A method which generate a repositoryInfo object about a single bitbucket repository.
 
         :param vcs_instance_name: Name of the VCS instance to which the repository belongs
         :param repository_information: Bitbucket repository information as returned by the Bitbucket API.
-        :param branches_information: Bitbucket branches information for a single repo as returned by the Bitbucket API.
+        :param latest_commit: Bitbucket latest_commit for a single repo as returned by the Bitbucket API.
         :return RepositoryInfo object
         """
-
-        branches: List[Branch] = []
-        for branch_information in branches_information:
-            if os.getenv('SCAN_ONLY_MASTER_BRANCH', "true").lower() in "true":
-                if branch_information["displayId"].lower() in ["main", "master"]:
-                    branch = Branch(repository_id=repository_information["id"],
-                                    **map_bitbucket_branch(branch_information))
-                    branches.append(branch)
-                    break
-            else:
-                branch = Branch(repository_id=repository_information["id"],
-                                **map_bitbucket_branch(branch_information))
-                branches.append(branch)
         http_clone_url = BitbucketConnector.get_clone_url(repository_information["links"]["clone"], "http")
-        repository = Repository(branches=branches,
+        repository = Repository(latest_commit=latest_commit,
                                 repository_url=http_clone_url,
                                 vcs_instance_name=vcs_instance_name,
                                 **map_bitbucket_repository(repository_information))
         return repository
```

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/github_public_connector.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/github_public_connector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Standard Library
-import os
 from typing import List
 
 # Third Party
 import requests
 from github import Github
-from github.Branch import Branch as GithubBranch
 from github.Repository import Repository as GithubRepository
 
 # First Party
-from vcs_scraper.model import Branch, Repository, VCSInstance
+from vcs_scraper.model import Repository, VCSInstance
 from vcs_scraper.vcs_connectors.vcs_connector import VCSConnector
 
 
 class GithubPublicConnector(VCSConnector):
 
     def project_exists(self, project_key: str) -> bool:
         return bool(self.api_client.get_user(project_key))
@@ -51,56 +49,35 @@
             repository_list.append(repo_dict)
         return repository_list
 
     def get_repository_details(self, project_key: str, repository_name: str) -> GithubRepository:
         repo_details = self.api_client.get_repo(f"{project_key}/{repository_name}")
         return repo_details
 
-    def get_branches(self, project_key: str, repository_id: str) -> List[GithubBranch]:
-        branches = self.api_client.get_repo(f"{project_key}/{repository_id}").get_branches()
-        for branch in branches:
-            branch_details = self.get_branch_details(project_key=project_key, repository_name=repository_id,
-                                                     branch=branch.name)
-            branch.latest_commit = branch_details.commit.sha
-        return branches
-
-    def get_branch_details(self, project_key: str, repository_name: str, branch: str) -> GithubBranch:
-        branch = self.api_client.get_repo(f"{project_key}/{repository_name}").get_branch(branch)
-        return branch
+    def get_latest_commit(self, project_key: str, repository_id: str) -> str:
+        latest_commit = None
+        self.api_client.per_page = 1
+        commits = self.api_client.get_repo(f"{project_key}/{repository_id}").get_commits()
+        if commits:
+            latest_commit = commits[0].sha
+        self.api_client.per_page = None
+        return latest_commit
 
     @staticmethod
-    def export_repository(repository_information: GithubRepository, branches_information: List[GithubBranch],
-                          vcs_instance_name: str) \
+    def export_repository(repository_information: GithubRepository, latest_commit: str, vcs_instance_name: str) \
             -> Repository:
         """
         A method which generate a repository object about a single bitbucket repository.
 
         :param vcs_instance_name: Name of the VCS instance to which the repository belongs
         :param repository_information: Github repository information as returned by the Bitbucket API.
-        :param branches_information: Github branches information for a single repo as returned by the Bitbucket API.
+        :param latest_commit: Github latest_commit for this repo as returned by the Bitbucket API.
         :return Repository object
         """
-
-        branches: List[Branch] = []
-        for branch_information in branches_information:
-            if os.getenv('SCAN_ONLY_MASTER_BRANCH', "true").lower() in "true":
-                if branch_information.name.lower() in ["main", "master"]:
-                    branch = Branch(repository_id=repository_information["id"],
-                                    branch_name=branch_information.name,
-                                    latest_commit=branch_information.latest_commit,
-                                    branch_id=branch_information.name)
-                    branches.append(branch)
-                    break
-            else:
-                branch = Branch(repository_id=repository_information["id"],
-                                branch_name=branch_information.name,
-                                latest_commit=branch_information.latest_commit,
-                                branch_id=branch_information.name)
-                branches.append(branch)
-        repository = Repository(branches=branches,
+        repository = Repository(latest_commit=latest_commit,
                                 repository_url=repository_information["html_url"],
                                 vcs_instance_name=vcs_instance_name,
                                 repository_name=repository_information["name"],
                                 repository_id=str(repository_information["id"]),
                                 project_key=repository_information["project_key"])
         return repository
```

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/vcs_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Standard Library
 import abc
-from typing import Dict, List
+from typing import Dict
 
 # First Party
 from vcs_scraper.model import Repository, VCSInstance
 
 
 class VCSConnector(metaclass=abc.ABCMeta):
 
@@ -18,22 +18,20 @@
         pass
 
     @abc.abstractmethod
     def get_repos(self, project_key):
         pass
 
     @abc.abstractmethod
-    def get_branches(self, project_key, repository_id):
+    def get_latest_commit(self, project_key, repository_id):
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def export_repository(repository_information: Dict, branches_information: List[Dict],
-                          vcs_instance_name: str) \
-            -> Repository:
+    def export_repository(repository_information: Dict, latest_commit, vcs_instance_name: str) -> Repository:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def create_client_from_vcs_instance(vcs_instance: VCSInstance):
         pass
```

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_connectors/vcs_connector_factory.py`

 * *Files identical despite different names*

### Comparing `resc_vcs_scraper-1.3.0/src/vcs_scraper/vcs_instances_parser.py` & `resc_vcs_scraper-1.4.0/src/vcs_scraper/vcs_instances_parser.py`

 * *Files identical despite different names*


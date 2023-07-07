# Comparing `tmp/dbt-workflows-factory-0.0.3.tar.gz` & `tmp/dbt-workflows-factory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-workflows-factory-0.0.3.tar", last modified: Thu Jul  6 12:33:49 2023, max compression
+gzip compressed data, was "dbt-workflows-factory-0.0.4.tar", last modified: Fri Jul  7 11:43:20 2023, max compression
```

## Comparing `dbt-workflows-factory-0.0.3.tar` & `dbt-workflows-factory-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:49.215435 dbt-workflows-factory-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-07-06 12:33:49.211435 dbt-workflows-factory-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:33:49.215435 dbt-workflows-factory-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:49.211435 dbt-workflows-factory-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:49.211435 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/dbt_workflows_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-06 12:33:31.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/yaml_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:49.211435 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-07-06 12:33:49.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-06 12:33:49.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:33:49.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:33:49.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 12:33:49.000000 dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:43:20.554665 dbt-workflows-factory-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-07 11:43:20.554665 dbt-workflows-factory-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:43:20.554665 dbt-workflows-factory-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:43:20.550665 dbt-workflows-factory-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:43:20.554665 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/dbt_workflows_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-07 11:43:04.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/yaml_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:43:20.554665 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-07 11:43:20.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-07 11:43:20.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:43:20.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:43:20.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 11:43:20.000000 dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/top_level.txt
```

### Comparing `dbt-workflows-factory-0.0.3/LICENSE` & `dbt-workflows-factory-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-workflows-factory-0.0.3/PKG-INFO` & `dbt-workflows-factory-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-workflows-factory
-Version: 0.0.3
+Version: 0.0.4
 Summary: DBT workflows factory for Google Cloud Platform
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,85 +212,63 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# dbt-workflows-converter
+# dbt-workflows-factory
 
-[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-workflows-converter)
-[![PyPI Version](https://badge.fury.io/py/dbt-workflows-converter.svg)](https://pypi.org/project/dbt-workflows-converter/)
-[![Downloads](https://pepy.tech/badge/dbt-workflows-converter)](https://pepy.tech/project/dbt-workflows-converter)
-[![Maintainability](https://api.codeclimate.com/v1/badges/e44ed9383a42b59984f6/maintainability)](https://codeclimate.com/github/getindata/dbt-workflows-converter/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/e44ed9383a42b59984f6/test_coverage)](https://codeclimate.com/github/getindata/dbt-workflows-converter/test_coverage)
-[![Documentation Status](https://readthedocs.org/projects/dbt-workflows-converter/badge/?version=latest)](https://dbt-workflows-converter.readthedocs.io/en/latest/?badge=latest)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-workflows-factory)
+[![PyPI Version](https://badge.fury.io/py/dbt-workflows-factory.svg)](https://pypi.org/project/dbt-workflows-factory/)
+[![Downloads](https://pepy.tech/badge/dbt-workflows-factory)](https://pepy.tech/project/dbt-workflows-factory)
 
 Creates dbt based GCP workflows.
 
 [//]: # (## Documentation)
 
 [//]: # ()
-[//]: # (Read the full documentation at [https://dbt-workflows-converter.readthedocs.io/]&#40;https://dbt-workflows-converter.readthedocs.io/en/latest/index.html&#41;)
+[//]: # (Read the full documentation at [https://dbt-workflows-factory.readthedocs.io/]&#40;https://dbt-workflows-factory.readthedocs.io/en/latest/index.html&#41;)
 
 ## Installation
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [dbt-workflows-converter](https://pypi.org/project/dbt-workflows-converter/) for [dp (data-pipelines-cli)]:
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [dbt-workflows-factory](https://pypi.org/project/dbt-workflows-factory/) for [dp (data-pipelines-cli)]:
 
 ```bash
-pip install dbt-workflows-converter
+pip install dbt-workflows-factory
 ```
-
-## Usage
-
-In order to run the dbt-workflows-converter, you will need:
-- `manifest.json` file with dbt manifest
-- `params` for the special parameters.
-
 ### Params
 
 Parameters specified for the converters are:
 1. `image_uri`: url address for the image
 2. `region`: the location where tge workflow executes on GCP (example: `us-central1` or `europe-west1`)
 3. `full_command`: full command executed on image (example: `"dbt --no-write-json run --target env_execution --project-dir /dbt --profiles-dir /root/.dbt --select "`)
 4. `remote_path`: gcs mount path (example: ` "/mnt/disks/var"`)
 5. `key_volume_mount_path`: path for mounting the volume containg key (ex. `/mnt/disks/var/keyfile_name.json`)
 6. `key_volume_path`: path for mounting (ex. `["/mnt/disks/var/:/mnt/disks/var/:rw"]`)
 7. `key_path`:  is a remote path for bucket containing key to be mounted
 
 ### How to run
 
-While running, you can specify the location of manifest file and the yaml file, but they are set by default to: "manifest.json" and "workflow.yaml".
-
-```python
-import DbtWorkflowsConverter
-
-converter = DbtWorkflowsConverter(params)
-converter.convert() # writes to file workflow.yaml
-
-```
-
 To call from cli, you can
 
 ```
-python src/dbt_workflows_converter/compile.py tests/manifest.json --image-uri xxx --region xxx --full-command xxx --remote-path xxx --key-volume-mount-path xxx --key-volume-path xxx --key-path xxx
+python -m dbt_workflows_factory.cli path/to/manifest.json --image-uri xxx --region xxx --full-command xxx --remote-path xxx --key-volume-mount-path xxx --key-volume-path xxx --key-path xxx
 
 ```
 
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
-    - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
     - pull-request.yml - Build and Test pull requests before commiting to main.
     - template-sync.yml - Update GitHub Repo with enhancments to base template
 - docs - collect documents (default format .md)
 - src - place new source code here
   - python_package - sample package (this can be deleted when creating a new repository)
 - tests - contains Python based test cases to validation src code
 - .pre-commit-config.yaml - Contains various pre-check fixes for Python
 - pyproject.toml - Python Project Declaration
-- ws.code-workspace - Recommended configurations for [Visual Studio Code](https://code.visualstudio.com/)
 
 ## Publish to PyPi from GitHub
 In order to publish to PyPi, a repostirory secret must be created, "PYPI_PASSWORD". In order to publish to the Test PyPi, a second secret must be added, "TEST_PYPI_PASSWORD".
```

### Comparing `dbt-workflows-factory-0.0.3/pyproject.toml` & `dbt-workflows-factory-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "dbt-graph-builder>=0.4.1",
+    "dbt-graph-builder>=0.5.0",
     "click>=8.1.3",
 ]
 license = {file = "LICENSE"}
 dynamic = ["version"]
 
 [tool.bandit]
 exclude_dirs = ["build","dist","tests","scripts"]
```

### Comparing `dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/cli.py` & `dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import sys
+from datetime import datetime, timedelta, timezone
 
 import click
 
 from .dbt_workflows_converter import DbtWorkflowsConverter
 from .params import Params
 
 
@@ -14,58 +15,67 @@
     """CLI entrypoint."""
 
 
 @cli.command()
 @click.argument("manifest_file", type=click.Path(exists=True))
 @click.option("--image-uri", type=str, help="Docker image URI", required=True)
 @click.option("--region", type=str, help="GCP region", required=True)
+@click.option("--gcs-key-volume-remote-path", type=str, help="GCS Remote path for private key", required=True)
 @click.option(
-    "--full-command",
+    "--gcs-key-volume-mount-path",
     type=str,
-    help="Full command to run in container",
+    help="Volume mount path for private key",
     required=True,
 )
-@click.option("--remote-path", type=str, help="Path to remote file", required=True)
 @click.option(
-    "--key-volume-mount-path",
+    "--gcs-key-volume-container-mount-path",
     type=str,
-    help="Volume mount path for private key",
+    help="Volume mount path for private key in container",
     required=True,
 )
 @click.option(
-    "--key-volume-path",
+    "--container-gcp-key-path",
     type=str,
-    help="Path for the private key file on the host",
+    help="Path for the private key file in the container",
     required=True,
 )
 @click.option(
-    "--key-path",
+    "--container-gcp-project-id",
     type=str,
-    help="Path for the private key file in the container",
+    help="GCP project ID in the container",
     required=True,
 )
+@click.option(
+    "--job-id-suffix",
+    type=str,
+    help="Job ID suffix",
+    required=False,
+    default=f'"{int(datetime.now(tz=timezone(offset=timedelta(hours=0))).timestamp())}"',
+)
 def convert(
     manifest_file: str,
     image_uri: str,
     region: str,
-    full_command: str,
-    remote_path: str,
-    key_volume_mount_path: str,
-    key_volume_path: str,
-    key_path: str,
+    gcs_key_volume_remote_path: str,
+    gcs_key_volume_mount_path: str,
+    gcs_key_volume_container_mount_path: str,
+    container_gcp_key_path: str,
+    container_gcp_project_id: str,
+    job_id_suffix: str,
 ) -> None:
     """Convert dbt manifest.json to YAML for GCP Workflows."""  # noqa: DCO020
     params = Params(
         image_uri=image_uri,
         region=region,
-        full_command=full_command,
-        remote_path=remote_path,
-        key_volume_mount_path=key_volume_mount_path,
-        key_volume_path=key_volume_path,
-        key_path=key_path,
+        gcs_key_volume_remote_path=gcs_key_volume_remote_path,
+        gcs_key_volume_mount_path=gcs_key_volume_mount_path,
+        gcs_key_volume_container_mount_path=gcs_key_volume_container_mount_path,
+        container_gcp_key_path=container_gcp_key_path,
+        container_gcp_project_id=container_gcp_project_id,
+        job_id_suffix=job_id_suffix,
     )
     converter = DbtWorkflowsConverter(manifest_path=manifest_file, params=params)
     click.echo(json.dumps(converter.get_yaml()))
 
 
 @cli.command()
 @click.option("--name", type=str, help="Workflow name", required=True)
```

### Comparing `dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/dbt_workflows_converter.py` & `dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/dbt_workflows_converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     GraphConfiguration,
     create_tasks_graph,
     load_dbt_manifest,
 )
 from dbt_graph_builder.workflow import SequentialStepsGraphFactory
 
 from .params import Params
-from .tasks import WorkflowTaskFactory
+from .tasks import WorkflowStepFactory
 from .yaml_builder import TaskYamlBuilder
 
 
 class DbtWorkflowsConverter:
     """Convert dbt manifest to workflows python object representation."""
 
     def __init__(
@@ -27,19 +27,29 @@
         Args:
             params (Params): Parameters for workflows.
             manifest_path (str): Path to dbt manifest file.
         """
         self._manifest_path = manifest_path
         self._params = params
 
-    def get_yaml(self) -> dict[str, Any]:
+    def get_yaml(self, enable_dags_dependencies: bool = False, show_ephemeral_models: bool = False) -> dict[str, Any]:
         """Convert dbt manifest to workflows python object representation.
 
+        Args:
+            enable_dags_dependencies (bool): Enable DAGs dependencies.
+            show_ephemeral_models (bool): Show ephemeral models.
+
         Returns:
             dict[str, Any]: Workflows python object representation.
         """
-        dag = create_tasks_graph(load_dbt_manifest(self._manifest_path), GraphConfiguration())
-        task_list: list[str] = list(dag.graph.nodes)
-        tasks = SequentialStepsGraphFactory(dag, WorkflowTaskFactory()).get_workflow()
+        dag = create_tasks_graph(
+            load_dbt_manifest(self._manifest_path),
+            GraphConfiguration(
+                dbt_manifest_props={"alias": "alias"},
+                show_ephemeral_models=show_ephemeral_models,
+                enable_dags_dependencies=enable_dags_dependencies,
+            ),
+        )
+        tasks = SequentialStepsGraphFactory(dag, WorkflowStepFactory()).get_workflow()
         yaml_builder = TaskYamlBuilder(self._params)
-        result = yaml_builder.create_workflow(task_list, tasks)
+        result = yaml_builder.create_workflow(tasks)
         return result
```

### Comparing `dbt-workflows-factory-0.0.3/src/dbt_workflows_factory/yaml_builder.py` & `dbt-workflows-factory-0.0.4/src/dbt_workflows_factory/yaml_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,173 @@
 from __future__ import annotations
 
 from typing import Any
 
 from dbt_graph_builder.workflow import Step
 
 from .params import Params
-from .tasks import ChainTask
+from .tasks import CustomStep, WorkflowChainStep
 
 
-class MainChainTask(ChainTask):
+class MainChainTask(WorkflowChainStep):
     """Main chain task in workflow."""
 
-    def __init__(self, step: Step, next_step: ChainTask | None = None) -> None:
+    def __init__(self, step: Step, next_step: WorkflowChainStep | None = None) -> None:
         """Create a new main chain task.
 
         Args:
             step (Step): The step to add.
             next_step (ChainTask | None, optional): The next step. Defaults to None.
         """
         super().__init__(step, next_step)
         self._task_alias = "main"
 
 
-class SimpleSingleTask(Step):
-    """Simple single task in workflow."""
+class TaskYamlBuilder:
+    """Task yaml builder."""
 
-    def __init__(self, get_step_def: dict[str, Any]) -> None:
-        """Create a new simple single task.
+    def __init__(self, params: Params):
+        """Create a new task yaml builder.
 
         Args:
-            get_step_def (dict[str, Any]): The step definition.
+            params (Params): GCP workflow params.
         """
-        self._get_step_def = get_step_def
+        self._params = params
+
+    def create_workflow(
+        self,
+        additional_steps: Step,
+    ) -> dict[str, Any]:
+        """Create a workflow.
 
-    def get_step(self) -> dict[str, Any]:
-        """Return a step result.
+        Args:
+            additional_steps (Step): Additional steps to add to the workflow.
 
         Returns:
-            dict[str, Any]: Step result.
+            dict[str, Any]: Workflow.
         """
-        return self._get_step_def
+        maint_chain_task = MainChainTask(self._init_step())
+        maint_chain_task.add_step(additional_steps)
+        yaml_representation = maint_chain_task.get_step()
+        yaml_representation["subworkflowBatchJob"] = self._subworkflow
+        return yaml_representation
 
+    def _init_step(self) -> Step:
+        return CustomStep(
+            {
+                "init": {
+                    "assign": [
+                        {"projectId": '${sys.get_env("GOOGLE_CLOUD_PROJECT_ID")}'},
+                        {"region": self._params.region},
+                        {"batchApi": "batch.googleapis.com/v1"},
+                        {
+                            "batchApiUrl": (
+                                '${"https://" + batchApi + "/projects/" + projectId + "/locations/" + region + "/jobs"}'
+                            )
+                        },
+                        {"imageUri": self._params.image_uri},
+                    ]
+                }
+            }
+        )
 
-class TaskYamlBuilder:
-    """Task yaml builder."""
+    @property
+    def _subworkflow(self) -> dict[str, Any]:
+        return {
+            "params": self._subworkflow_job_params,
+            "steps": self._subworkflow_job_steps,
+        }
 
-    def __init__(self, params: Params):
-        """Create a new task yaml builder.
+    @property
+    def _subworkflow_job_params(self) -> list[str]:
+        return ["batchApiUrl", "command", "jobId", "imageUri", "select"]
 
-        Args:
-            params (Params): GCP workflow params.
-        """
-        self._params = params
+    @property
+    def _subworkflow_job_steps(self) -> list[dict[str, Any]]:
+        return [
+            self._subwork_init_job,
+            self._subwork_main_job,
+            self._subwork_get_job,
+        ]
 
     @property
-    def _subwork_batch_job_init(self) -> dict[str, Any]:
-        return {"init": {"assign": [{"fullcomand": self._params.full_command}]}}
+    def _subwork_init_job(self) -> dict[str, Any]:
+        return {
+            "init": {
+                "assign": [
+                    {"jobId": f'${{jobId + "-" + {self._params.job_id_suffix}}}'},
+                ]
+            }
+        }
 
     @property
-    def _subwork_batch_job_main(self) -> dict[str, Any]:
+    def _subwork_main_job(self) -> dict[str, Any]:
         return {
             "createAndRunBatchJob": {
                 "call": "http.post",
-                "args": self._subwork_batch_job_main_args,
+                "args": self._subwork_job_args,
                 "result": "createAndRunBatchJobResponse",
             }
         }
 
     @property
-    def _subwork_batch_job_main_args(self) -> dict[str, Any]:
+    def _subwork_job_args(self) -> dict[str, Any]:
         return {
             "url": "${batchApiUrl}",
-            "query": {"job_id": "${jobId}"},
+            "query": {"jobId": "${jobId}"},
             "headers": {"Content-Type": "application/json"},
             "auth": {"type": "OAuth2"},
             "body": {
                 "taskGroups": {
                     "taskSpec": {
-                        "volumes": self._subwork_batch_job_main_args_volumes,
-                        "runnables": self._subwork_batch_job_main_args_runnables,
+                        "volumes": self._subwork_job_volumes,
+                        "runnables": self._subwork_job_runnables,
                     }
                 },
                 "logsPolicy": {"destination": "CLOUD_LOGGING"},
             },
         }
 
     @property
-    def _subwork_batch_job_main_args_runnables(self) -> list[dict[str, Any]]:
+    def _subwork_job_volumes(self) -> list[dict[str, Any]]:
+        return [
+            {
+                "gcs": {"remotePath": self._params.gcs_key_volume_remote_path},
+                "mountPath": self._params.gcs_key_volume_mount_path,
+            }
+        ]
+
+    @property
+    def _subwork_job_runnables(self) -> list[dict[str, Any]]:
         return [
             {
                 "container": {
                     "imageUri": "imageUri",
-                    "entrypoint": "bash",
-                    "commands": ["-c", "full_command"],
-                    "volumes": [self._params.key_volume_path],
+                    "entrypoint": "/bin/bash",
+                    "commands": [
+                        "-c",
+                        '${"dbt --no-write-json " + command + " --target env_execution --project-dir /dbt '
+                        '--profiles-dir /root/.dbt --select " + select}',
+                    ],
+                    "volumes": [self._params.gcs_key_volume_container_mount_path],
                 },
                 "environment": {
                     "variables": {
-                        "GCP_KEY_PATH": self._params.key_path,
-                        "GCP_PROJECT": "dataops" "-test" "-project",
+                        "GCP_KEY_PATH": self._params.container_gcp_key_path,
+                        "GCP_PROJECT": self._params.container_gcp_project_id,
                     }
                 },
             }
         ]
 
     @property
-    def _subwork_batch_job_main_args_volumes(self) -> list[dict[str, Any]]:
-        return [
-            {
-                "gcs": {"remotePath": self._params.remote_path},
-                "mountPath": self._params.key_volume_mount_path,
-            }
-        ]
-
-    @property
-    def _subwork_batch_job_get(self) -> dict[str, Any]:
+    def _subwork_get_job(self) -> dict[str, Any]:
         return {
             "getJob": {
                 "call": "http.get",
                 "args": {
                     "url": '${batchApiUrl + "/" + jobId}',
                     "auth": {"type": "OAuth2"},
                 },
                 "result": "getJobResult",
             }
         }
-
-    @property
-    def _subworkflow(self) -> dict[str, Any]:
-        return {
-            "params": self._subworkflow_batch_job_params,
-            "steps": self._subworkflow_batch_job_steps,
-        }
-
-    @property
-    def _subworkflow_batch_job_steps(self) -> list[dict[str, Any]]:
-        return [
-            self._subwork_batch_job_init,
-            self._subwork_batch_job_main,
-            self._subwork_batch_job_get,
-        ]
-
-    @property
-    def _subworkflow_batch_job_params(self) -> list[str]:
-        return ["batchApiUrl", "command", "jobId", "imageUri"]
-
-    def _init_step(self, job_names: list[str]) -> Step:
-        return SimpleSingleTask(
-            {
-                "init": {
-                    "assign": [
-                        {"projectId": '${sys.get_env("GOOGLE_CLOUD_PROJECT_ID")}'},
-                        {"region": self._params.region},
-                        {"batchApi": "batch.googleapis.com/v1"},
-                        {
-                            "batchApiUrl": (
-                                '${"https://" + batchApi + "/projects/" + projectId + "/locations/" + region + "/jobs"}'
-                            )
-                        },
-                        {"containerEntrypoint": "bash"},
-                        {"imageUri": self._params.image_uri},
-                        *[{task_name: f"${{{task_name.lower()} + string(int(sys.now()))}}"} for task_name in job_names],
-                    ]
-                }
-            }
-        )
-
-    def create_workflow(
-        self,
-        job_list: list[str],
-        additional_steps: Step,
-    ) -> dict[str, Any]:
-        """Create a workflow.
-
-        Args:
-            job_list (list[str]): List of job names.
-            additional_steps (Step): Additional steps to add to the workflow.
-
-        Returns:
-            dict[str, Any]: Workflow.
-        """
-        maint_chain_task = MainChainTask(self._init_step(job_list))
-        maint_chain_task.add_step(additional_steps)
-        yaml_representation = maint_chain_task.get_step()
-        yaml_representation["subworkflowBatchJob"] = self._subworkflow
-        return yaml_representation
```

### Comparing `dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/PKG-INFO` & `dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-workflows-factory
-Version: 0.0.3
+Version: 0.0.4
 Summary: DBT workflows factory for Google Cloud Platform
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -212,85 +212,63 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# dbt-workflows-converter
+# dbt-workflows-factory
 
-[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-workflows-converter)
-[![PyPI Version](https://badge.fury.io/py/dbt-workflows-converter.svg)](https://pypi.org/project/dbt-workflows-converter/)
-[![Downloads](https://pepy.tech/badge/dbt-workflows-converter)](https://pepy.tech/project/dbt-workflows-converter)
-[![Maintainability](https://api.codeclimate.com/v1/badges/e44ed9383a42b59984f6/maintainability)](https://codeclimate.com/github/getindata/dbt-workflows-converter/maintainability)
-[![Test Coverage](https://api.codeclimate.com/v1/badges/e44ed9383a42b59984f6/test_coverage)](https://codeclimate.com/github/getindata/dbt-workflows-converter/test_coverage)
-[![Documentation Status](https://readthedocs.org/projects/dbt-workflows-converter/badge/?version=latest)](https://dbt-workflows-converter.readthedocs.io/en/latest/?badge=latest)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-workflows-factory)
+[![PyPI Version](https://badge.fury.io/py/dbt-workflows-factory.svg)](https://pypi.org/project/dbt-workflows-factory/)
+[![Downloads](https://pepy.tech/badge/dbt-workflows-factory)](https://pepy.tech/project/dbt-workflows-factory)
 
 Creates dbt based GCP workflows.
 
 [//]: # (## Documentation)
 
 [//]: # ()
-[//]: # (Read the full documentation at [https://dbt-workflows-converter.readthedocs.io/]&#40;https://dbt-workflows-converter.readthedocs.io/en/latest/index.html&#41;)
+[//]: # (Read the full documentation at [https://dbt-workflows-factory.readthedocs.io/]&#40;https://dbt-workflows-factory.readthedocs.io/en/latest/index.html&#41;)
 
 ## Installation
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [dbt-workflows-converter](https://pypi.org/project/dbt-workflows-converter/) for [dp (data-pipelines-cli)]:
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [dbt-workflows-factory](https://pypi.org/project/dbt-workflows-factory/) for [dp (data-pipelines-cli)]:
 
 ```bash
-pip install dbt-workflows-converter
+pip install dbt-workflows-factory
 ```
-
-## Usage
-
-In order to run the dbt-workflows-converter, you will need:
-- `manifest.json` file with dbt manifest
-- `params` for the special parameters.
-
 ### Params
 
 Parameters specified for the converters are:
 1. `image_uri`: url address for the image
 2. `region`: the location where tge workflow executes on GCP (example: `us-central1` or `europe-west1`)
 3. `full_command`: full command executed on image (example: `"dbt --no-write-json run --target env_execution --project-dir /dbt --profiles-dir /root/.dbt --select "`)
 4. `remote_path`: gcs mount path (example: ` "/mnt/disks/var"`)
 5. `key_volume_mount_path`: path for mounting the volume containg key (ex. `/mnt/disks/var/keyfile_name.json`)
 6. `key_volume_path`: path for mounting (ex. `["/mnt/disks/var/:/mnt/disks/var/:rw"]`)
 7. `key_path`:  is a remote path for bucket containing key to be mounted
 
 ### How to run
 
-While running, you can specify the location of manifest file and the yaml file, but they are set by default to: "manifest.json" and "workflow.yaml".
-
-```python
-import DbtWorkflowsConverter
-
-converter = DbtWorkflowsConverter(params)
-converter.convert() # writes to file workflow.yaml
-
-```
-
 To call from cli, you can
 
 ```
-python src/dbt_workflows_converter/compile.py tests/manifest.json --image-uri xxx --region xxx --full-command xxx --remote-path xxx --key-volume-mount-path xxx --key-volume-path xxx --key-path xxx
+python -m dbt_workflows_factory.cli path/to/manifest.json --image-uri xxx --region xxx --full-command xxx --remote-path xxx --key-volume-mount-path xxx --key-volume-path xxx --key-path xxx
 
 ```
 
 ## Project Organization
 
 - .devcontainer - This directory contains required files for creating a [Codespace](https://github.com/features/codespaces).
 - .github
   - workflows - Contains GitHub Actions used for building, testing and publishing.
-    - publish-test.yml - Publish wheels to [https://test.pypi.org/](https://test.pypi.org/)
     - publish.yml - Publish wheels to [https://pypi.org/](https://pypi.org/)
     - pull-request.yml - Build and Test pull requests before commiting to main.
     - template-sync.yml - Update GitHub Repo with enhancments to base template
 - docs - collect documents (default format .md)
 - src - place new source code here
   - python_package - sample package (this can be deleted when creating a new repository)
 - tests - contains Python based test cases to validation src code
 - .pre-commit-config.yaml - Contains various pre-check fixes for Python
 - pyproject.toml - Python Project Declaration
-- ws.code-workspace - Recommended configurations for [Visual Studio Code](https://code.visualstudio.com/)
 
 ## Publish to PyPi from GitHub
 In order to publish to PyPi, a repostirory secret must be created, "PYPI_PASSWORD". In order to publish to the Test PyPi, a second secret must be added, "TEST_PYPI_PASSWORD".
```

### Comparing `dbt-workflows-factory-0.0.3/src/dbt_workflows_factory.egg-info/SOURCES.txt` & `dbt-workflows-factory-0.0.4/src/dbt_workflows_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*


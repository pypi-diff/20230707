# Comparing `tmp/lusid-workflow-sdk-preview-0.1.333.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.342.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.333.tar", last modified: Wed Jul  5 13:14:49 2023, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.342.tar", last modified: Fri Jul  7 09:04:58 2023, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.333.tar` & `lusid-workflow-sdk-preview-0.1.342.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9644 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     4531 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56187 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    41163 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    36409 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27406 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     3451 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6094 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/action_definition.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/action_details.py
--rw-r--r--   0 root         (0) root         (0)     6004 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0 root         (0) root         (0)    13450 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6783 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/field_mapping.py
--rw-r--r--   0 root         (0) root         (0)     5878 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5984 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6165 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0 root         (0) root         (0)     9530 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7575 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0 root         (0) root         (0)     9076 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/parameter.py
--rw-r--r--   0 root         (0) root         (0)     5767 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/parameter_value.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/result_field.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)    10386 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6704 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0 root         (0) root         (0)    12968 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    14045 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     6387 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)    12376 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    12546 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     5389 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)    10977 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/version.py
--rw-r--r--   0 root         (0) root         (0)    11007 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     7614 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)     8967 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0 root         (0) root         (0)    13551 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2574 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 13:14:49.000000 lusid-workflow-sdk-preview-0.1.333/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2023-07-05 13:14:21.000000 lusid-workflow-sdk-preview-0.1.333/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9652 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56187 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    41163 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    36409 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27406 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6094 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/action_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/action_details.py
+-rw-r--r--   0 root         (0) root         (0)     6004 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6783 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/result_field.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10386 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0 root         (0) root         (0)    12984 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12376 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     5389 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)    11105 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/version_info.py
+-rw-r--r--   0 root         (0) root         (0)    11023 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     7614 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-07 09:04:57.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 09:04:57.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-07 09:04:57.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-07 09:04:57.000000 lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 09:04:58.000000 lusid-workflow-sdk-preview-0.1.342/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-07-07 09:00:30.000000 lusid-workflow-sdk-preview-0.1.342/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/README.md` & `lusid-workflow-sdk-preview-0.1.342/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.333
-- Package version: 0.1.333
+- API version: 0.1.342
+- Package version: 0.1.342
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -146,15 +146,15 @@
  - [TaskStateDefinition](docs/TaskStateDefinition.md)
  - [TaskTransitionDefinition](docs/TaskTransitionDefinition.md)
  - [TransitionTriggerDefinition](docs/TransitionTriggerDefinition.md)
  - [TriggerParentTaskAction](docs/TriggerParentTaskAction.md)
  - [TriggerSchema](docs/TriggerSchema.md)
  - [UpdateTaskDefinitionRequest](docs/UpdateTaskDefinitionRequest.md)
  - [UpdateTaskRequest](docs/UpdateTaskRequest.md)
- - [Version](docs/Version.md)
+ - [VersionInfo](docs/VersionInfo.md)
  - [Worker](docs/Worker.md)
  - [WorkerConfiguration](docs/WorkerConfiguration.md)
  - [WorkerStatusTriggers](docs/WorkerStatusTriggers.md)
 
 
 ## Documentation For Authorization
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.333"
+__version__ = "0.1.342"
 
 # import apis into sdk package
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
 
 # import ApiClient
@@ -66,15 +66,15 @@
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
 from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from lusid_workflow.models.trigger_schema import TriggerSchema
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 from lusid_workflow.models.update_task_request import UpdateTaskRequest
-from lusid_workflow.models.version import Version
+from lusid_workflow.models.version_info import VersionInfo
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
 
 # import utilities into sdk package
 from fbnsdkutilities.utilities.api_client_builder import ApiClientBuilder
 from fbnsdkutilities.utilities.api_configuration import ApiConfiguration
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/task_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -328,15 +328,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -505,15 +505,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -666,15 +666,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -843,15 +843,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -1027,15 +1027,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/tasks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -173,15 +173,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Task",
             400: "LusidValidationProblemDetails",
@@ -323,15 +323,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -481,15 +481,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
@@ -642,15 +642,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -818,15 +818,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api/workers_api.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api/workers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -338,15 +338,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -498,15 +498,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "PagedResourceListOfWorker",
             400: "LusidValidationProblemDetails",
@@ -688,15 +688,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.333'
+        header_params['X-LUSID-SDK-Version'] = '0.1.342'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RunWorkerResponse",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.333/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.342/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.333\n"\
-               "SDK Package Version: 0.1.333".\
+               "Version of the API: 0.1.342\n"\
+               "SDK Package Version: 0.1.342".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -50,11 +50,11 @@
 from lusid_workflow.models.task_state_definition import TaskStateDefinition
 from lusid_workflow.models.task_transition_definition import TaskTransitionDefinition
 from lusid_workflow.models.transition_trigger_definition import TransitionTriggerDefinition
 from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from lusid_workflow.models.trigger_schema import TriggerSchema
 from lusid_workflow.models.update_task_definition_request import UpdateTaskDefinitionRequest
 from lusid_workflow.models.update_task_request import UpdateTaskRequest
-from lusid_workflow.models.version import Version
+from lusid_workflow.models.version_info import VersionInfo
 from lusid_workflow.models.worker import Worker
 from lusid_workflow.models.worker_configuration import WorkerConfiguration
 from lusid_workflow.models.worker_status_triggers import WorkerStatusTriggers
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/action_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/action_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/action_details.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/action_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_child_tasks_action.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_child_tasks_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/create_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/deleted_entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/field_mapping.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/field_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/health_check.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/initial_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/luminesce_view.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/luminesce_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/parameter.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/parameter_value.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/parameter_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/result_field.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/result_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/result_matching_pattern.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/result_matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/run_worker_action.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/run_worker_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/run_worker_request.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/run_worker_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/run_worker_response.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/run_worker_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -39,15 +39,15 @@
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'str',
         'correlation_ids': 'list[str]',
         'task_definition_id': 'ResourceId',
         'task_definition_version': 'TaskDefinitionVersion',
-        'version': 'Version',
+        'version': 'VersionInfo',
         'state': 'str',
         'terminal_state': 'bool',
         'as_at_last_transition': 'datetime',
         'fields': 'list[TaskInstanceField]'
     }
 
     attribute_map = {
@@ -82,15 +82,15 @@
         :param correlation_ids:  User-provided ID used to link entities and tasks
         :type correlation_ids: list[str]
         :param task_definition_id:  (required)
         :type task_definition_id: lusid_workflow.ResourceId
         :param task_definition_version:  (required)
         :type task_definition_version: lusid_workflow.TaskDefinitionVersion
         :param version: 
-        :type version: lusid_workflow.Version
+        :type version: lusid_workflow.VersionInfo
         :param state:  Current State (required)
         :type state: str
         :param terminal_state:  True if no onward transitions are possible (required)
         :type terminal_state: bool
         :param as_at_last_transition:  Last Transition timestamp
         :type as_at_last_transition: datetime
         :param fields:  Fields and their latest values - should correspond with the Task Definition field schema
@@ -219,25 +219,25 @@
 
     @property
     def version(self):
         """Gets the version of this Task.  # noqa: E501
 
 
         :return: The version of this Task.  # noqa: E501
-        :rtype: lusid_workflow.Version
+        :rtype: lusid_workflow.VersionInfo
         """
         return self._version
 
     @version.setter
     def version(self, version):
         """Sets the version of this Task.
 
 
         :param version: The version of this Task.  # noqa: E501
-        :type version: lusid_workflow.Version
+        :type version: lusid_workflow.VersionInfo
         """
 
         self._version = version
 
     @property
     def state(self):
         """Gets the state of this Task.  # noqa: E501
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -36,15 +36,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'ResourceId',
-        'version': 'Version',
+        'version': 'VersionInfo',
         'display_name': 'str',
         'description': 'str',
         'states': 'list[TaskStateDefinition]',
         'field_schema': 'list[TaskFieldDefinition]',
         'initial_state': 'InitialState',
         'triggers': 'list[TransitionTriggerDefinition]',
         'actions': 'list[ActionDefinition]',
@@ -79,15 +79,15 @@
 
     def __init__(self, id=None, version=None, display_name=None, description=None, states=None, field_schema=None, initial_state=None, triggers=None, actions=None, transitions=None, local_vars_configuration=None):  # noqa: E501
         """TaskDefinition - a model defined in OpenAPI"
         
         :param id:  (required)
         :type id: lusid_workflow.ResourceId
         :param version: 
-        :type version: lusid_workflow.Version
+        :type version: lusid_workflow.VersionInfo
         :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
         :param states:  The states this Task Definition operates over (required)
         :type states: list[lusid_workflow.TaskStateDefinition]
         :param field_schema:  The Fields that this Task Definition operates on
@@ -155,25 +155,25 @@
 
     @property
     def version(self):
         """Gets the version of this TaskDefinition.  # noqa: E501
 
 
         :return: The version of this TaskDefinition.  # noqa: E501
-        :rtype: lusid_workflow.Version
+        :rtype: lusid_workflow.VersionInfo
         """
         return self._version
 
     @version.setter
     def version(self, version):
         """Sets the version of this TaskDefinition.
 
 
         :param version: The version of this TaskDefinition.  # noqa: E501
-        :type version: lusid_workflow.Version
+        :type version: lusid_workflow.VersionInfo
         """
 
         self._version = version
 
     @property
     def display_name(self):
         """Gets the display_name of this TaskDefinition.  # noqa: E501
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_definition_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_field_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_instance_field.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_instance_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_state_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_state_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/task_transition_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/task_transition_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/trigger_parent_task_action.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/trigger_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/update_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/update_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/update_task_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/version.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/version_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_workflow.configuration import Configuration
 
 
-class Version(object):
+class VersionInfo(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -65,15 +65,15 @@
         'as_at_modified': 'optional',
         'user_id_modified': 'optional',
         'request_id_modified': 'optional',
         'as_at_version_number': 'optional'
     }
 
     def __init__(self, as_at_created=None, user_id_created=None, request_id_created=None, as_at_modified=None, user_id_modified=None, request_id_modified=None, as_at_version_number=None, local_vars_configuration=None):  # noqa: E501
-        """Version - a model defined in OpenAPI"
+        """VersionInfo - a model defined in OpenAPI"
         
         :param as_at_created:  The asAt datetime at which this entity was first created.
         :type as_at_created: datetime
         :param user_id_created:  The unique id of the user who created this entity.
         :type user_id_created: str
         :param request_id_created:  The request id of the request that created this entity.
         :type request_id_created: str
@@ -106,168 +106,168 @@
         self.as_at_modified = as_at_modified
         self.user_id_modified = user_id_modified
         self.request_id_modified = request_id_modified
         self.as_at_version_number = as_at_version_number
 
     @property
     def as_at_created(self):
-        """Gets the as_at_created of this Version.  # noqa: E501
+        """Gets the as_at_created of this VersionInfo.  # noqa: E501
 
         The asAt datetime at which this entity was first created.  # noqa: E501
 
-        :return: The as_at_created of this Version.  # noqa: E501
+        :return: The as_at_created of this VersionInfo.  # noqa: E501
         :rtype: datetime
         """
         return self._as_at_created
 
     @as_at_created.setter
     def as_at_created(self, as_at_created):
-        """Sets the as_at_created of this Version.
+        """Sets the as_at_created of this VersionInfo.
 
         The asAt datetime at which this entity was first created.  # noqa: E501
 
-        :param as_at_created: The as_at_created of this Version.  # noqa: E501
+        :param as_at_created: The as_at_created of this VersionInfo.  # noqa: E501
         :type as_at_created: datetime
         """
 
         self._as_at_created = as_at_created
 
     @property
     def user_id_created(self):
-        """Gets the user_id_created of this Version.  # noqa: E501
+        """Gets the user_id_created of this VersionInfo.  # noqa: E501
 
         The unique id of the user who created this entity.  # noqa: E501
 
-        :return: The user_id_created of this Version.  # noqa: E501
+        :return: The user_id_created of this VersionInfo.  # noqa: E501
         :rtype: str
         """
         return self._user_id_created
 
     @user_id_created.setter
     def user_id_created(self, user_id_created):
-        """Sets the user_id_created of this Version.
+        """Sets the user_id_created of this VersionInfo.
 
         The unique id of the user who created this entity.  # noqa: E501
 
-        :param user_id_created: The user_id_created of this Version.  # noqa: E501
+        :param user_id_created: The user_id_created of this VersionInfo.  # noqa: E501
         :type user_id_created: str
         """
 
         self._user_id_created = user_id_created
 
     @property
     def request_id_created(self):
-        """Gets the request_id_created of this Version.  # noqa: E501
+        """Gets the request_id_created of this VersionInfo.  # noqa: E501
 
         The request id of the request that created this entity.  # noqa: E501
 
-        :return: The request_id_created of this Version.  # noqa: E501
+        :return: The request_id_created of this VersionInfo.  # noqa: E501
         :rtype: str
         """
         return self._request_id_created
 
     @request_id_created.setter
     def request_id_created(self, request_id_created):
-        """Sets the request_id_created of this Version.
+        """Sets the request_id_created of this VersionInfo.
 
         The request id of the request that created this entity.  # noqa: E501
 
-        :param request_id_created: The request_id_created of this Version.  # noqa: E501
+        :param request_id_created: The request_id_created of this VersionInfo.  # noqa: E501
         :type request_id_created: str
         """
 
         self._request_id_created = request_id_created
 
     @property
     def as_at_modified(self):
-        """Gets the as_at_modified of this Version.  # noqa: E501
+        """Gets the as_at_modified of this VersionInfo.  # noqa: E501
 
         The asAt datetime at which this entity was last updated.  # noqa: E501
 
-        :return: The as_at_modified of this Version.  # noqa: E501
+        :return: The as_at_modified of this VersionInfo.  # noqa: E501
         :rtype: datetime
         """
         return self._as_at_modified
 
     @as_at_modified.setter
     def as_at_modified(self, as_at_modified):
-        """Sets the as_at_modified of this Version.
+        """Sets the as_at_modified of this VersionInfo.
 
         The asAt datetime at which this entity was last updated.  # noqa: E501
 
-        :param as_at_modified: The as_at_modified of this Version.  # noqa: E501
+        :param as_at_modified: The as_at_modified of this VersionInfo.  # noqa: E501
         :type as_at_modified: datetime
         """
 
         self._as_at_modified = as_at_modified
 
     @property
     def user_id_modified(self):
-        """Gets the user_id_modified of this Version.  # noqa: E501
+        """Gets the user_id_modified of this VersionInfo.  # noqa: E501
 
         The unique id of the user who last updated this entity.  # noqa: E501
 
-        :return: The user_id_modified of this Version.  # noqa: E501
+        :return: The user_id_modified of this VersionInfo.  # noqa: E501
         :rtype: str
         """
         return self._user_id_modified
 
     @user_id_modified.setter
     def user_id_modified(self, user_id_modified):
-        """Sets the user_id_modified of this Version.
+        """Sets the user_id_modified of this VersionInfo.
 
         The unique id of the user who last updated this entity.  # noqa: E501
 
-        :param user_id_modified: The user_id_modified of this Version.  # noqa: E501
+        :param user_id_modified: The user_id_modified of this VersionInfo.  # noqa: E501
         :type user_id_modified: str
         """
 
         self._user_id_modified = user_id_modified
 
     @property
     def request_id_modified(self):
-        """Gets the request_id_modified of this Version.  # noqa: E501
+        """Gets the request_id_modified of this VersionInfo.  # noqa: E501
 
         The request id of the request that last updated this entity.  # noqa: E501
 
-        :return: The request_id_modified of this Version.  # noqa: E501
+        :return: The request_id_modified of this VersionInfo.  # noqa: E501
         :rtype: str
         """
         return self._request_id_modified
 
     @request_id_modified.setter
     def request_id_modified(self, request_id_modified):
-        """Sets the request_id_modified of this Version.
+        """Sets the request_id_modified of this VersionInfo.
 
         The request id of the request that last updated this entity.  # noqa: E501
 
-        :param request_id_modified: The request_id_modified of this Version.  # noqa: E501
+        :param request_id_modified: The request_id_modified of this VersionInfo.  # noqa: E501
         :type request_id_modified: str
         """
 
         self._request_id_modified = request_id_modified
 
     @property
     def as_at_version_number(self):
-        """Gets the as_at_version_number of this Version.  # noqa: E501
+        """Gets the as_at_version_number of this VersionInfo.  # noqa: E501
 
         The integer version number for this entity (the entity was created at version 1).  # noqa: E501
 
-        :return: The as_at_version_number of this Version.  # noqa: E501
+        :return: The as_at_version_number of this VersionInfo.  # noqa: E501
         :rtype: int
         """
         return self._as_at_version_number
 
     @as_at_version_number.setter
     def as_at_version_number(self, as_at_version_number):
-        """Sets the as_at_version_number of this Version.
+        """Sets the as_at_version_number of this VersionInfo.
 
         The integer version number for this entity (the entity was created at version 1).  # noqa: E501
 
-        :param as_at_version_number: The as_at_version_number of this Version.  # noqa: E501
+        :param as_at_version_number: The as_at_version_number of this VersionInfo.  # noqa: E501
         :type as_at_version_number: int
         """
 
         self._as_at_version_number = as_at_version_number
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -307,18 +307,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Version):
+        if not isinstance(other, VersionInfo):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Version):
+        if not isinstance(other, VersionInfo):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/worker.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -39,15 +39,15 @@
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'ResourceId',
         'display_name': 'str',
         'description': 'str',
         'worker_configuration': 'object',
-        'version': 'Version',
+        'version': 'VersionInfo',
         'parameters': 'list[Parameter]',
         'result_fields': 'list[ResultField]',
         'links': 'list[Link]'
     }
 
     attribute_map = {
         'id': 'id',
@@ -79,15 +79,15 @@
         :param display_name:  Human readable name (required)
         :type display_name: str
         :param description:  Human readable description
         :type description: str
         :param worker_configuration:  Information about how the worker should be executed (required)
         :type worker_configuration: object
         :param version: 
-        :type version: lusid_workflow.Version
+        :type version: lusid_workflow.VersionInfo
         :param parameters:  The Parameters this Worker accepts or requires.
         :type parameters: list[lusid_workflow.Parameter]
         :param result_fields:  The Fields that the Worker results will come back with.
         :type result_fields: list[lusid_workflow.ResultField]
         :param links: 
         :type links: list[lusid_workflow.Link]
 
@@ -215,25 +215,25 @@
 
     @property
     def version(self):
         """Gets the version of this Worker.  # noqa: E501
 
 
         :return: The version of this Worker.  # noqa: E501
-        :rtype: lusid_workflow.Version
+        :rtype: lusid_workflow.VersionInfo
         """
         return self._version
 
     @version.setter
     def version(self, version):
         """Sets the version of this Worker.
 
 
         :param version: The version of this Worker.  # noqa: E501
-        :type version: lusid_workflow.Version
+        :type version: lusid_workflow.VersionInfo
         """
 
         self._version = version
 
     @property
     def parameters(self):
         """Gets the parameters of this Worker.  # noqa: E501
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/worker_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/models/worker_status_triggers.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/models/worker_status_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.333
+    The version of the OpenAPI document: 0.1.342
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.342/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 lusid_workflow/models/task_state_definition.py
 lusid_workflow/models/task_transition_definition.py
 lusid_workflow/models/transition_trigger_definition.py
 lusid_workflow/models/trigger_parent_task_action.py
 lusid_workflow/models/trigger_schema.py
 lusid_workflow/models/update_task_definition_request.py
 lusid_workflow/models/update_task_request.py
-lusid_workflow/models/version.py
+lusid_workflow/models/version_info.py
 lusid_workflow/models/worker.py
 lusid_workflow/models/worker_configuration.py
 lusid_workflow/models/worker_status_triggers.py
 lusid_workflow_sdk_preview.egg-info/PKG-INFO
 lusid_workflow_sdk_preview.egg-info/SOURCES.txt
 lusid_workflow_sdk_preview.egg-info/dependency_links.txt
 lusid_workflow_sdk_preview.egg-info/requires.txt
```

### Comparing `lusid-workflow-sdk-preview-0.1.333/setup.py` & `lusid-workflow-sdk-preview-0.1.342/setup.py`

 * *Files identical despite different names*


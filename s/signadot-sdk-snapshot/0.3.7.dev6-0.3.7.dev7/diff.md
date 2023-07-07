# Comparing `tmp/signadot-sdk-snapshot-0.3.7.dev6.tar.gz` & `tmp/signadot-sdk-snapshot-0.3.7.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signadot-sdk-snapshot-0.3.7.dev6.tar", last modified: Tue Mar 21 22:49:39 2023, max compression
+gzip compressed data, was "signadot-sdk-snapshot-0.3.7.dev7.tar", last modified: Fri Jul  7 18:05:05 2023, max compression
```

## Comparing `signadot-sdk-snapshot-0.3.7.dev6.tar` & `signadot-sdk-snapshot-0.3.7.dev7.tar`

### file list

```diff
@@ -1,276 +1,282 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.431308 signadot-sdk-snapshot-0.3.7.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-21 22:49:39.431308 signadot-sdk-snapshot-0.3.7.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 22:49:39.431308 signadot-sdk-snapshot-0.3.7.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-21 22:49:37.000000 signadot-sdk-snapshot-0.3.7.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.383306 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.383306 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/cluster_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/route_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19371 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.391306 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster_token_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_match_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_spec_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_custom_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_default_route_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_value_from_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_value_from_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_fork_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_fork_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_host_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.391306 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.395306 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/cluster_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/resource_plugins_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/route_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25392 2023-03-21 22:49:37.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-03-21 22:49:37.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.407307 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/apierrs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_token_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/connect_cluster_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/connect_cluster_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_cluster_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_preview_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_sandbox_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_sandbox_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/custom_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_value_from_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_value_from_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/fork_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/fork_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/get_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/get_sandbox_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/get_sandboxes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/handler_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/preview_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resource_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resource_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-03-21 22:49:37.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-03-21 22:49:37.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step_input_to.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-21 22:49:37.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_value_from_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_match_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_spec_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroups_endpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_custom_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_default_route_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_value_from_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_value_from_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_host_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_preview_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_ready_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_route_group_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandboxes_sandbox_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/upsert_pr_workspaces_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/upsert_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/v1_image_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.391306 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-21 22:49:39.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-03-21 22:49:39.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 22:49:39.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-21 22:49:39.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-21 22:49:39.000000 signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.407307 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.411307 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api/cluster_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35653 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api/sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25359 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.419307 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/connect_cluster_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/connect_cluster_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_cluster_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_preview_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_sandbox_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_sandbox_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/env_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/fork_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/fork_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/get_sandbox_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/get_sandboxes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/handler_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/preview_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_ready_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/upsert_pr_workspaces_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/upsert_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/v1_image_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:39.431308 signadot-sdk-snapshot-0.3.7.dev6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 22:49:36.000000 signadot-sdk-snapshot-0.3.7.dev6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_apierrs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_token_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_connect_cluster_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_connect_cluster_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_create_cluster_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_create_preview_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_create_sandbox_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_create_sandbox_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_custom_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_env_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_env_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_env_value_from_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_env_value_from_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_fork_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_fork_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_get_clusters_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_get_sandbox_by_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_get_sandboxes_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_handler_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_preview_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resource_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resource_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resource_plugins_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step_input_to.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_value_from_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_match_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_spec_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_route_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroups_endpoint_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_custom_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_default_route_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_value_from.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_value_from_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_value_from_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_host_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_preview_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_ready_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_route_group_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandboxes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_sandboxes_sandbox_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_upsert_pr_workspaces_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_upsert_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-21 22:49:18.000000 signadot-sdk-snapshot-0.3.7.dev6/test/test_v1_image_replacement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.199577 signadot-sdk-snapshot-0.3.7.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-07 18:05:05.195577 signadot-sdk-snapshot-0.3.7.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:05:05.199577 signadot-sdk-snapshot-0.3.7.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.171576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.171576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/cluster_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/route_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19371 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.175576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster_token_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_match_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_spec_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_custom_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_default_route_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_value_from_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_value_from_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_fork_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_fork_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_host_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.175576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.175576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38652 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/cluster_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/resource_plugins_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/route_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25392 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.183576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/apierrs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_token_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/connect_cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/connect_cluster_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_cluster_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_preview_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_sandbox_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_sandbox_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/custom_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_value_from_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_value_from_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/fork_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/fork_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/get_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/get_sandbox_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/get_sandboxes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/handler_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/preview_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resource_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resource_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step_input_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_value_from_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_match_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_spec_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-07 18:05:00.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroups_endpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_custom_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_default_route_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_value_from_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_value_from_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_host_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_local_workload_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_local_workload_status_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_local_workload_status_tunnel_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_preview_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_ready_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_route_group_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandboxes_sandbox_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/upsert_pr_workspaces_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/upsert_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/v1_image_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.175576 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-07 18:05:05.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-07 18:05:05.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:05:05.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-07 18:05:05.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-07 18:05:05.000000 signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.187577 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.187577 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15510 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api/cluster_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35653 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api/sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25359 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.187577 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/connect_cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/connect_cluster_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_cluster_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_preview_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_sandbox_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_sandbox_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/env_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/fork_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/fork_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/get_sandbox_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/get_sandboxes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/handler_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/preview_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_ready_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/upsert_pr_workspaces_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/upsert_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/v1_image_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:05.195577 signadot-sdk-snapshot-0.3.7.dev7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_apierrs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_token_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_connect_cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_connect_cluster_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_create_cluster_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_create_preview_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_create_sandbox_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_create_sandbox_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_custom_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_env_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_env_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_env_value_from_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_env_value_from_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_fork_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_fork_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_get_clusters_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_get_sandbox_by_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_get_sandboxes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_handler_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_preview_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resource_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resource_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resource_plugins_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step_input_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_value_from_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_match_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_spec_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_route_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroups_endpoint_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_custom_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_default_route_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_value_from_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_value_from_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_host_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_local_workload_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_local_workload_status_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-07 18:05:01.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_local_workload_status_tunnel_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_preview_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_ready_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_route_group_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandboxes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_sandboxes_sandbox_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_upsert_pr_workspaces_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_upsert_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-07 18:04:44.000000 signadot-sdk-snapshot-0.3.7.dev7/test/test_v1_image_replacement.py
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/README.md` & `signadot-sdk-snapshot-0.3.7.dev7/README.md`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/setup.py` & `signadot-sdk-snapshot-0.3.7.dev7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "signadot-sdk-snapshot"
-VERSION = "0.3.7.dev6"
+VERSION = "0.3.7.dev7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/__init__.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/cluster_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/route_groups_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/route_groups_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api/sandboxes_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api/sandboxes_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/api_client.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/configuration.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/__init__.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster_operator.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster_operator.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster_token.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster_token.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/cluster_token_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/cluster_token_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/empty_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/empty_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/error_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/error_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_match.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_match.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_match_label.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_match_label.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_spec_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_spec_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/route_group_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/route_group_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_custom_patch.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_custom_patch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_customizations.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_customizations.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_default_route_group.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_default_route_group.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_value_from.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_value_from.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_value_from_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_value_from_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_value_from_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_value_from_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_env_var.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_env_var.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_fork_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_fork_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_fork_of.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_fork_of.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_host_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_host_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_image.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_image.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_readiness.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_readiness.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/models/sandbox_ttl.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/models/sandbox_ttl.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk/rest.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/__init__.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Signadot API
 
     API for Signadot Sandboxes  # noqa: E501
 
     OpenAPI spec version: 2.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from signadot_sdk_snapshot.api.cluster_api import ClusterApi
-from signadot_sdk_snapshot.api.resource_plugins_api import ResourcePluginsApi
-from signadot_sdk_snapshot.api.route_groups_api import RouteGroupsApi
-from signadot_sdk_snapshot.api.sandboxes_api import SandboxesApi
-
-# import ApiClient
-from signadot_sdk_snapshot.api_client import ApiClient
-from signadot_sdk_snapshot.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from signadot_sdk_snapshot.models.cluster import Cluster
 from signadot_sdk_snapshot.models.cluster_operator import ClusterOperator
 from signadot_sdk_snapshot.models.cluster_token import ClusterToken
 from signadot_sdk_snapshot.models.cluster_token_status import ClusterTokenStatus
 from signadot_sdk_snapshot.models.empty_response import EmptyResponse
 from signadot_sdk_snapshot.models.error_response import ErrorResponse
 from signadot_sdk_snapshot.models.resource_info import ResourceInfo
@@ -58,11 +48,14 @@
 from signadot_sdk_snapshot.models.sandbox_env_value_from_resource import SandboxEnvValueFromResource
 from signadot_sdk_snapshot.models.sandbox_env_var import SandboxEnvVar
 from signadot_sdk_snapshot.models.sandbox_fork import SandboxFork
 from signadot_sdk_snapshot.models.sandbox_fork_endpoint import SandboxForkEndpoint
 from signadot_sdk_snapshot.models.sandbox_fork_of import SandboxForkOf
 from signadot_sdk_snapshot.models.sandbox_host_endpoint import SandboxHostEndpoint
 from signadot_sdk_snapshot.models.sandbox_image import SandboxImage
+from signadot_sdk_snapshot.models.sandbox_local_workload_status import SandboxLocalWorkloadStatus
+from signadot_sdk_snapshot.models.sandbox_local_workload_status_tunnel import SandboxLocalWorkloadStatusTunnel
+from signadot_sdk_snapshot.models.sandbox_local_workload_status_tunnel_health import SandboxLocalWorkloadStatusTunnelHealth
 from signadot_sdk_snapshot.models.sandbox_readiness import SandboxReadiness
 from signadot_sdk_snapshot.models.sandbox_resource import SandboxResource
 from signadot_sdk_snapshot.models.sandbox_spec import SandboxSpec
 from signadot_sdk_snapshot.models.sandbox_ttl import SandboxTTL
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/cluster_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/resource_plugins_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/resource_plugins_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/route_groups_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/route_groups_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api/sandboxes_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api/sandboxes_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/api_client.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/0.3.7.dev6/python'
+        self.user_agent = 'Swagger-Codegen/0.3.7.dev7/python'
         self.accept_version = '20211220'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/configuration.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,9 +247,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0\n"\
-               "SDK Package Version: 0.3.7.dev6".\
+               "SDK Package Version: 0.3.7.dev7".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/__init__.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Signadot API
 
     API for Signadot Sandboxes  # noqa: E501
 
     OpenAPI spec version: 2.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from signadot_sdk_snapshot.api.cluster_api import ClusterApi
+from signadot_sdk_snapshot.api.resource_plugins_api import ResourcePluginsApi
+from signadot_sdk_snapshot.api.route_groups_api import RouteGroupsApi
+from signadot_sdk_snapshot.api.sandboxes_api import SandboxesApi
+
+# import ApiClient
+from signadot_sdk_snapshot.api_client import ApiClient
+from signadot_sdk_snapshot.configuration import Configuration
+# import models into sdk package
 from signadot_sdk_snapshot.models.cluster import Cluster
 from signadot_sdk_snapshot.models.cluster_operator import ClusterOperator
 from signadot_sdk_snapshot.models.cluster_token import ClusterToken
 from signadot_sdk_snapshot.models.cluster_token_status import ClusterTokenStatus
 from signadot_sdk_snapshot.models.empty_response import EmptyResponse
 from signadot_sdk_snapshot.models.error_response import ErrorResponse
 from signadot_sdk_snapshot.models.resource_info import ResourceInfo
@@ -48,11 +58,14 @@
 from signadot_sdk_snapshot.models.sandbox_env_value_from_resource import SandboxEnvValueFromResource
 from signadot_sdk_snapshot.models.sandbox_env_var import SandboxEnvVar
 from signadot_sdk_snapshot.models.sandbox_fork import SandboxFork
 from signadot_sdk_snapshot.models.sandbox_fork_endpoint import SandboxForkEndpoint
 from signadot_sdk_snapshot.models.sandbox_fork_of import SandboxForkOf
 from signadot_sdk_snapshot.models.sandbox_host_endpoint import SandboxHostEndpoint
 from signadot_sdk_snapshot.models.sandbox_image import SandboxImage
+from signadot_sdk_snapshot.models.sandbox_local_workload_status import SandboxLocalWorkloadStatus
+from signadot_sdk_snapshot.models.sandbox_local_workload_status_tunnel import SandboxLocalWorkloadStatusTunnel
+from signadot_sdk_snapshot.models.sandbox_local_workload_status_tunnel_health import SandboxLocalWorkloadStatusTunnelHealth
 from signadot_sdk_snapshot.models.sandbox_readiness import SandboxReadiness
 from signadot_sdk_snapshot.models.sandbox_resource import SandboxResource
 from signadot_sdk_snapshot.models.sandbox_spec import SandboxSpec
 from signadot_sdk_snapshot.models.sandbox_ttl import SandboxTTL
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/apierrs_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/apierrs_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/branch.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/branch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_operator.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_operator.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_registration.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_registration.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_token.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_token.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/cluster_token_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/cluster_token_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/connect_cluster_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/connect_cluster_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/connect_cluster_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/connect_cluster_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_cluster_token_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_cluster_token_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_preview_endpoint_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_preview_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_sandbox_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_sandbox_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/create_sandbox_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/create_sandbox_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/custom_patch.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/custom_patch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/empty_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/empty_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_op.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_op.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_value_from.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_value_from.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_value_from_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_value_from_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/env_value_from_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/env_value_from_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/error_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/error_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/fork_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/fork_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/fork_of.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/fork_of.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/get_clusters_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/get_clusters_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/get_sandbox_by_id_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/get_sandbox_by_id_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/get_sandboxes_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/get_sandboxes_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/handler_empty_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/handler_empty_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/image.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/image.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/preview_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/preview_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resource_info.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resource_info.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resource_plugin.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resource_plugin.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_runner.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_runner.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step_input.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step_input.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step_input_to.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step_input_to.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_step_out.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_step_out.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/resourceplugin_value_from_step.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/resourceplugin_value_from_step.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_match.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_match.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_match_label.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_match_label.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_spec_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_spec_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/route_group_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/route_group_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_label.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_label.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_match.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_match.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroup_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroup_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/routegroups_endpoint_url.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/routegroups_endpoint_url.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_custom_patch.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_custom_patch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_customizations.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_customizations.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_default_route_group.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_default_route_group.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_details.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_details.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_op.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_op.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_value_from.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_value_from.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_value_from_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_value_from_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_value_from_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_value_from_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_env_var.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_env_var.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork_of.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork_of.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_fork_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_fork_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_host_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_host_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_image.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_image.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_info.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_info.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_preview_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_preview_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_readiness.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_readiness.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,44 +29,70 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'local': 'list[SandboxLocalWorkloadStatus]',
         'message': 'str',
         'ready': 'bool',
         'reason': 'str'
     }
 
     attribute_map = {
+        'local': 'local',
         'message': 'message',
         'ready': 'ready',
         'reason': 'reason'
     }
 
-    def __init__(self, message=None, ready=None, reason=None, _configuration=None):  # noqa: E501
+    def __init__(self, local=None, message=None, ready=None, reason=None, _configuration=None):  # noqa: E501
         """SandboxReadiness - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
+        self._local = None
         self._message = None
         self._ready = None
         self._reason = None
         self.discriminator = None
 
+        if local is not None:
+            self.local = local
         if message is not None:
             self.message = message
         if ready is not None:
             self.ready = ready
         if reason is not None:
             self.reason = reason
 
     @property
+    def local(self):
+        """Gets the local of this SandboxReadiness.  # noqa: E501
+
+
+        :return: The local of this SandboxReadiness.  # noqa: E501
+        :rtype: list[SandboxLocalWorkloadStatus]
+        """
+        return self._local
+
+    @local.setter
+    def local(self, local):
+        """Sets the local of this SandboxReadiness.
+
+
+        :param local: The local of this SandboxReadiness.  # noqa: E501
+        :type: list[SandboxLocalWorkloadStatus]
+        """
+
+        self._local = local
+
+    @property
     def message(self):
         """Gets the message of this SandboxReadiness.  # noqa: E501
 
         Message is a human readable explanation of why the sandbox is healthy or not.  # noqa: E501
 
         :return: The message of this SandboxReadiness.  # noqa: E501
         :rtype: str
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_ready_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_ready_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_route_group_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_route_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_status_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_status_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_tags.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_tags.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandbox_ttl.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandbox_ttl.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/sandboxes_sandbox_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/sandboxes_sandbox_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/tag.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/tag.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/upsert_pr_workspaces_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/upsert_pr_workspaces_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/upsert_workspace_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/upsert_workspace_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/models/v1_image_replacement.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/models/v1_image_replacement.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot/rest.py` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot/rest.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/signadot_sdk_snapshot.egg-info/SOURCES.txt` & `signadot-sdk-snapshot-0.3.7.dev7/signadot_sdk_snapshot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,17 @@
 signadot_sdk_snapshot/models/sandbox_fork.py
 signadot_sdk_snapshot/models/sandbox_fork_endpoint.py
 signadot_sdk_snapshot/models/sandbox_fork_of.py
 signadot_sdk_snapshot/models/sandbox_fork_spec.py
 signadot_sdk_snapshot/models/sandbox_host_endpoint.py
 signadot_sdk_snapshot/models/sandbox_image.py
 signadot_sdk_snapshot/models/sandbox_info.py
+signadot_sdk_snapshot/models/sandbox_local_workload_status.py
+signadot_sdk_snapshot/models/sandbox_local_workload_status_tunnel.py
+signadot_sdk_snapshot/models/sandbox_local_workload_status_tunnel_health.py
 signadot_sdk_snapshot/models/sandbox_preview_endpoint.py
 signadot_sdk_snapshot/models/sandbox_readiness.py
 signadot_sdk_snapshot/models/sandbox_ready_response.py
 signadot_sdk_snapshot/models/sandbox_resource.py
 signadot_sdk_snapshot/models/sandbox_route_group_endpoint.py
 signadot_sdk_snapshot/models/sandbox_spec.py
 signadot_sdk_snapshot/models/sandbox_status.py
@@ -240,14 +243,17 @@
 test/test_sandbox_fork.py
 test/test_sandbox_fork_endpoint.py
 test/test_sandbox_fork_of.py
 test/test_sandbox_fork_spec.py
 test/test_sandbox_host_endpoint.py
 test/test_sandbox_image.py
 test/test_sandbox_info.py
+test/test_sandbox_local_workload_status.py
+test/test_sandbox_local_workload_status_tunnel.py
+test/test_sandbox_local_workload_status_tunnel_health.py
 test/test_sandbox_preview_endpoint.py
 test/test_sandbox_readiness.py
 test/test_sandbox_ready_response.py
 test/test_sandbox_resource.py
 test/test_sandbox_route_group_endpoint.py
 test/test_sandbox_spec.py
 test/test_sandbox_status.py
```

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/__init__.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api/cluster_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api/sandboxes_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api/sandboxes_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/api_client.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/configuration.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/__init__.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/branch.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/branch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/connect_cluster_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/connect_cluster_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/connect_cluster_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/connect_cluster_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_cluster_token_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_cluster_token_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_preview_endpoint_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_preview_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_sandbox_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_sandbox_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/create_sandbox_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/create_sandbox_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/env_op.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/env_op.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/fork_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/fork_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/fork_of.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/fork_of.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/get_sandbox_by_id_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/get_sandbox_by_id_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/get_sandboxes_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/get_sandboxes_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/handler_empty_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/handler_empty_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/image.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/image.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/preview_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/preview_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_customizations.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_customizations.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_details.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_details.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_info.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_info.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/sandbox_ready_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/sandbox_ready_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/upsert_pr_workspaces_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/upsert_pr_workspaces_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/upsert_workspace_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/upsert_workspace_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/models/v1_image_replacement.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/models/v1_image_replacement.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/swagger_client/rest.py` & `signadot-sdk-snapshot-0.3.7.dev7/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_apierrs_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_apierrs_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_branch.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_branch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_operator.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_operator.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_registration.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_registration.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_token.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_token.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_cluster_token_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_cluster_token_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_connect_cluster_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_connect_cluster_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_connect_cluster_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_connect_cluster_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_create_cluster_token_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_create_cluster_token_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_create_preview_endpoint_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_create_preview_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_create_sandbox_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_create_sandbox_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_create_sandbox_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_create_sandbox_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_custom_patch.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_custom_patch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_empty_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_empty_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_env_op.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_env_op.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_env_value_from.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_env_value_from.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_env_value_from_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_env_value_from_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_env_value_from_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_env_value_from_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_error_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_fork_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_fork_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_fork_of.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_fork_of.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_get_clusters_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_get_clusters_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_get_sandbox_by_id_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_get_sandbox_by_id_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_get_sandboxes_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_get_sandboxes_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_handler_empty_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_handler_empty_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_image.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_image.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_preview_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_preview_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resource_info.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resource_info.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resource_plugin.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resource_plugin.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resource_plugins_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resource_plugins_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_runner.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_runner.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step_input.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step_input.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step_input_to.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step_input_to.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_step_out.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_step_out.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_resourceplugin_value_from_step.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_resourceplugin_value_from_step.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_match.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_match.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_match_label.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_match_label.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_spec_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_spec_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_group_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_group_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_route_groups_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_route_groups_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_label.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_label.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_match.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_match.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroup_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroup_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_routegroups_endpoint_url.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_routegroups_endpoint_url.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_custom_patch.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_custom_patch.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_customizations.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_customizations.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_default_route_group.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_default_route_group.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_details.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_details.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_op.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_op.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_value_from.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_value_from.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_value_from_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_value_from_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_value_from_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_value_from_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_env_var.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_env_var.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork_of.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork_of.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_fork_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_fork_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_host_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_host_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_image.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_image.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_info.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_info.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_preview_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_preview_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_readiness.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_readiness.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_ready_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_ready_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_resource.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_resource.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_route_group_endpoint.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_route_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_spec.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_spec.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_status_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_status_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_tags.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_tags.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandbox_ttl.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandbox_ttl.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandboxes_api.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandboxes_api.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_sandboxes_sandbox_status.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_sandboxes_sandbox_status.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_tag.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_upsert_pr_workspaces_request.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_upsert_pr_workspaces_request.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_upsert_workspace_response.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_upsert_workspace_response.py`

 * *Files identical despite different names*

### Comparing `signadot-sdk-snapshot-0.3.7.dev6/test/test_v1_image_replacement.py` & `signadot-sdk-snapshot-0.3.7.dev7/test/test_v1_image_replacement.py`

 * *Files identical despite different names*


# Comparing `tmp/syft-0.8.2b2.tar.gz` & `tmp/syft-0.8.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.2b2.tar", last modified: Thu Jun 29 07:04:21 2023, max compression
+gzip compressed data, was "syft-0.8.2b3.tar", last modified: Fri Jul  7 10:25:30 2023, max compression
```

## Comparing `syft-0.8.2b2.tar` & `syft-0.8.2b3.tar`

### file list

```diff
@@ -1,203 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.289957 syft-0.8.2b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-29 06:59:22.000000 syft-0.8.2b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 06:59:22.000000 syft-0.8.2b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-06-29 07:04:21.289957 syft-0.8.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16170 2023-06-29 06:59:22.000000 syft-0.8.2b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-29 06:59:22.000000 syft-0.8.2b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-29 07:04:21.289957 syft-0.8.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-29 06:59:22.000000 syft-0.8.2b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.241956 syft-0.8.2b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.249956 syft-0.8.2b2/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-29 06:59:41.000000 syft-0.8.2b2/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-29 06:59:41.000000 syft-0.8.2b2/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.249956 syft-0.8.2b2/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.253956 syft-0.8.2b2/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.253956 syft-0.8.2b2/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.253956 syft-0.8.2b2/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.257956 syft-0.8.2b2/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)    25535 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    41764 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.257956 syft-0.8.2b2/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.261956 syft-0.8.2b2/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11639 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.261956 syft-0.8.2b2/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.265956 syft-0.8.2b2/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    48704 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.265956 syft-0.8.2b2/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24725 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.269956 syft-0.8.2b2/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.269956 syft-0.8.2b2/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23173 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.269956 syft-0.8.2b2/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.269956 syft-0.8.2b2/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.273957 syft-0.8.2b2/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.273957 syft-0.8.2b2/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.273957 syft-0.8.2b2/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48081 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15336 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.273957 syft-0.8.2b2/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.277957 syft-0.8.2b2/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26287 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.277957 syft-0.8.2b2/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.277957 syft-0.8.2b2/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.277957 syft-0.8.2b2/src/syft/service/vpn/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/vpn/headscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/vpn/tailscale_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/service/vpn/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.281957 syft-0.8.2b2/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22993 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.281957 syft-0.8.2b2/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    25848 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.285957 syft-0.8.2b2/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.289957 syft-0.8.2b2/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    27090 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22738 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-29 06:59:22.000000 syft-0.8.2b2/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:04:21.249956 syft-0.8.2b2/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-06-29 07:04:21.000000 syft-0.8.2b2/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-29 07:04:21.000000 syft-0.8.2b2/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:04:21.000000 syft-0.8.2b2/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 07:04:21.000000 syft-0.8.2b2/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:04:20.000000 syft-0.8.2b2/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-29 07:04:21.000000 syft-0.8.2b2/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 07:04:21.000000 syft-0.8.2b2/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.959880 syft-0.8.2b3/
+-rw-r--r--   0 om        (1001) users      (100)    11843 2023-07-07 10:23:23.000000 syft-0.8.2b3/LICENSE
+-rw-r--r--   0 om        (1001) users      (100)       98 2023-07-07 10:23:23.000000 syft-0.8.2b3/MANIFEST.in
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-07 10:25:30.959880 syft-0.8.2b3/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)    16170 2023-07-07 10:23:22.000000 syft-0.8.2b3/README.md
+-rw-r--r--   0 om        (1001) users      (100)      272 2023-07-07 10:23:23.000000 syft-0.8.2b3/pyproject.toml
+-rw-r--r--   0 om        (1001) users      (100)     3210 2023-07-07 10:25:30.959880 syft-0.8.2b3/setup.cfg
+-rw-r--r--   0 om        (1001) users      (100)      107 2023-07-07 10:23:23.000000 syft-0.8.2b3/setup.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.939880 syft-0.8.2b3/src/
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/
+-rw-r--r--   0 om        (1001) users      (100)      580 2023-07-07 10:23:29.000000 syft-0.8.2b3/src/syft/VERSION
+-rw-r--r--   0 om        (1001) users      (100)     5576 2023-07-07 10:23:29.000000 syft-0.8.2b3/src/syft/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       93 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/__main__.py
+-rw-r--r--   0 om        (1001) users      (100)      542 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/abstract_node.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/capnp/
+-rw-r--r--   0 om        (1001) users      (100)      270 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)       75 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 om        (1001) users      (100)      186 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/client/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    25448 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/api.py
+-rw-r--r--   0 om        (1001) users      (100)    27509 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/client.py
+-rw-r--r--   0 om        (1001) users      (100)      568 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/connection.py
+-rw-r--r--   0 om        (1001) users      (100)      650 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/deploy.py
+-rw-r--r--   0 om        (1001) users      (100)     7468 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/domain_client.py
+-rw-r--r--   0 om        (1001) users      (100)     2598 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/enclave_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1116 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/gateway_client.py
+-rw-r--r--   0 om        (1001) users      (100)    15257 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/registry.py
+-rw-r--r--   0 om        (1001) users      (100)     2623 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/search.py
+-rw-r--r--   0 om        (1001) users      (100)      549 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/client/user_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft/external/
+-rw-r--r--   0 om        (1001) users      (100)     1735 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/external/oblv/
+-rw-r--r--   0 om        (1001) users      (100)      860 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      284 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/auth.py
+-rw-r--r--   0 om        (1001) users      (100)      212 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     4835 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 om        (1001) users      (100)    12233 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 om        (1001) users      (100)     1800 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 om        (1001) users      (100)      489 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 om        (1001) users      (100)     2280 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7462 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 om        (1001) users      (100)    13948 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1146 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/gevent_patch.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/img/
+-rw-r--r--   0 om        (1001) users      (100)      297 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/img/base64.py
+-rw-r--r--   0 om        (1001) users      (100)    25535 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/img/logo.png
+-rw-r--r--   0 om        (1001) users      (100)    41764 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/node/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     2631 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/credentials.py
+-rw-r--r--   0 om        (1001) users      (100)      152 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/domain.py
+-rw-r--r--   0 om        (1001) users      (100)      259 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/enclave.py
+-rw-r--r--   0 om        (1001) users      (100)      728 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/gateway.py
+-rw-r--r--   0 om        (1001) users      (100)    31549 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/node.py
+-rw-r--r--   0 om        (1001) users      (100)     6979 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/routes.py
+-rw-r--r--   0 om        (1001) users      (100)     2064 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/run.py
+-rw-r--r--   0 om        (1001) users      (100)     6992 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/server.py
+-rw-r--r--   0 om        (1001) users      (100)      127 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/worker.py
+-rw-r--r--   0 om        (1001) users      (100)     1100 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/node/worker_settings.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/serde/
+-rw-r--r--   0 om        (1001) users      (100)      159 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3597 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/array.py
+-rw-r--r--   0 om        (1001) users      (100)     4099 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/arrow.py
+-rw-r--r--   0 om        (1001) users      (100)      298 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/capnp.py
+-rw-r--r--   0 om        (1001) users      (100)      722 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/deserialize.py
+-rw-r--r--   0 om        (1001) users      (100)     1230 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    11663 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 om        (1001) users      (100)      875 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/mock.py
+-rw-r--r--   0 om        (1001) users      (100)    11639 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/recursive.py
+-rw-r--r--   0 om        (1001) users      (100)    10253 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 om        (1001) users      (100)     1822 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/serializable.py
+-rw-r--r--   0 om        (1001) users      (100)      369 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/serialize.py
+-rw-r--r--   0 om        (1001) users      (100)     4959 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/signature.py
+-rw-r--r--   0 om        (1001) users      (100)     4885 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/serde/third_party.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.947880 syft-0.8.2b3/src/syft/service/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/__init__.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/action/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      703 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 om        (1001) users      (100)    16706 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_graph.py
+-rw-r--r--   0 om        (1001) users      (100)     6874 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 om        (1001) users      (100)    48723 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_object.py
+-rw-r--r--   0 om        (1001) users      (100)     2416 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 om        (1001) users      (100)    26998 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_service.py
+-rw-r--r--   0 om        (1001) users      (100)    10264 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_store.py
+-rw-r--r--   0 om        (1001) users      (100)     1165 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/action_types.py
+-rw-r--r--   0 om        (1001) users      (100)     3889 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/numpy.py
+-rw-r--r--   0 om        (1001) users      (100)     2233 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/pandas.py
+-rw-r--r--   0 om        (1001) users      (100)     2920 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/plan.py
+-rw-r--r--   0 om        (1001) users      (100)     4951 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/action/verification.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/code/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      236 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)      102 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/unparse.py
+-rw-r--r--   0 om        (1001) users      (100)    24908 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code.py
+-rw-r--r--   0 om        (1001) users      (100)     1756 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 om        (1001) users      (100)    10109 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1446 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     1782 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/context.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/data_subject/
+-rw-r--r--   0 om        (1001) users      (100)       69 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     4076 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 om        (1001) users      (100)      870 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 om        (1001) users      (100)     3215 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 om        (1001) users      (100)     5006 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/dataset/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    23367 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 om        (1001) users      (100)     6382 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1911 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/enclave/
+-rw-r--r--   0 om        (1001) users      (100)     6038 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/metadata/
+-rw-r--r--   0 om        (1001) users      (100)     3481 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/network/
+-rw-r--r--   0 om        (1001) users      (100)    16636 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/network/network_service.py
+-rw-r--r--   0 om        (1001) users      (100)     2976 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/network/node_peer.py
+-rw-r--r--   0 om        (1001) users      (100)     4593 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/network/routes.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/notification/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     7961 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4566 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     3259 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/policy/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    22437 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/policy.py
+-rw-r--r--   0 om        (1001) users      (100)     2081 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1077 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/project/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    48080 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/project.py
+-rw-r--r--   0 om        (1001) users      (100)    15374 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/project_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1908 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.951880 syft-0.8.2b3/src/syft/service/queue/
+-rw-r--r--   0 om        (1001) users      (100)     2044 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 om        (1001) users      (100)     3008 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/queue.py
+-rw-r--r--   0 om        (1001) users      (100)     4845 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     7929 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/request/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)    26514 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/request.py
+-rw-r--r--   0 om        (1001) users      (100)    10112 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/request_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1410 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/request/request_stash.py
+-rw-r--r--   0 om        (1001) users      (100)     2850 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/response.py
+-rw-r--r--   0 om        (1001) users      (100)    13653 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/service.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/settings/
+-rw-r--r--   0 om        (1001) users      (100)      882 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/settings/settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3486 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 om        (1001) users      (100)     1711 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/user/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      201 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/roles.py
+-rw-r--r--   0 om        (1001) users      (100)     6115 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user.py
+-rw-r--r--   0 om        (1001) users      (100)     3427 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user_roles.py
+-rw-r--r--   0 om        (1001) users      (100)    14978 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user_service.py
+-rw-r--r--   0 om        (1001) users      (100)     4363 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/service/vpn/
+-rw-r--r--   0 om        (1001) users      (100)     1809 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     6789 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 om        (1001) users      (100)     5414 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/store/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)     3235 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/dict_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    22993 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    21837 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/kv_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)     4326 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/linked_obj.py
+-rw-r--r--   0 om        (1001) users      (100)    11840 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/locks.py
+-rw-r--r--   0 om        (1001) users      (100)     8768 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/mongo_client.py
+-rw-r--r--   0 om        (1001) users      (100)      846 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 om        (1001) users      (100)    13836 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 om        (1001) users      (100)    13136 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.955880 syft-0.8.2b3/src/syft/types/
+-rw-r--r--   0 om        (1001) users      (100)        0 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      136 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/base.py
+-rw-r--r--   0 om        (1001) users      (100)     1091 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/datetime.py
+-rw-r--r--   0 om        (1001) users      (100)     5167 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/grid_url.py
+-rw-r--r--   0 om        (1001) users      (100)     4807 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 om        (1001) users      (100)    25848 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/syft_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8113 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/transforms.py
+-rw-r--r--   0 om        (1001) users      (100)     2098 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/twin_object.py
+-rw-r--r--   0 om        (1001) users      (100)     8038 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/types/uid.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.959880 syft-0.8.2b3/src/syft/util/
+-rw-r--r--   0 om        (1001) users      (100)       67 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/__init__.py
+-rw-r--r--   0 om        (1001) users      (100)      852 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/autoreload.py
+-rw-r--r--   0 om        (1001) users      (100)      271 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/colors.py
+-rw-r--r--   0 om        (1001) users      (100)       34 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/constants.py
+-rw-r--r--   0 om        (1001) users      (100)     1514 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/decorators.py
+-rw-r--r--   0 om        (1001) users      (100)     1607 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/experimental_flags.py
+-rw-r--r--   0 om        (1001) users      (100)     1327 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/filterwarnings.py
+-rw-r--r--   0 om        (1001) users      (100)     2940 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/fonts.py
+-rw-r--r--   0 om        (1001) users      (100)      153 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/jax_settings.py
+-rw-r--r--   0 om        (1001) users      (100)     3779 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/logger.py
+-rw-r--r--   0 om        (1001) users      (100)      752 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/markdown.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.959880 syft-0.8.2b3/src/syft/util/notebook_ui/
+-rw-r--r--   0 om        (1001) users      (100)    27090 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 om        (1001) users      (100)       42 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/options.py
+-rw-r--r--   0 om        (1001) users      (100)     5297 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/schema.py
+-rw-r--r--   0 om        (1001) users      (100)     2771 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/telemetry.py
+-rw-r--r--   0 om        (1001) users      (100)     6728 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/trace_decorator.py
+-rw-r--r--   0 om        (1001) users      (100)    22738 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/util.py
+-rw-r--r--   0 om        (1001) users      (100)     3123 2023-07-07 10:23:23.000000 syft-0.8.2b3/src/syft/util/version_compare.py
+drwxr-xr-x   0 om        (1001) users      (100)        0 2023-07-07 10:25:30.943880 syft-0.8.2b3/src/syft.egg-info/
+-rw-r--r--   0 om        (1001) users      (100)    16852 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 om        (1001) users      (100)     5879 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 om        (1001) users      (100)       43 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 om        (1001) users      (100)        1 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 om        (1001) users      (100)     1555 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/requires.txt
+-rw-r--r--   0 om        (1001) users      (100)        5 2023-07-07 10:25:30.000000 syft-0.8.2b3/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.2b2/LICENSE` & `syft-0.8.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/PKG-INFO` & `syft-0.8.2b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b2
+Version: 0.8.2b3
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b2 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b3 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b2/README.md` & `syft-0.8.2b3/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/setup.cfg` & `syft-0.8.2b3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.2-beta.2"
+version = attr: "0.8.2-beta.3"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -54,14 +54,15 @@
 	hagrid>=0.3
 	matplotlib==3.7.1
 	dm-haiku==0.0.9
 	itables==1.5.3
 	transformers==4.30.2
 	evaluate==0.4.0
 	torch==2.0.1
+	recordlinkage==0.15
 install_requires = 
 	%(syft)s
 python_requires = >=3.9
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `syft-0.8.2b2/src/syft/VERSION` & `syft-0.8.2b3/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.2-beta.2"
+__version__ = "0.8.2-beta.3"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.2b2/src/syft/__init__.py` & `syft-0.8.2b3/src/syft/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.2-beta.2"
+__version__ = "0.8.2-beta.3"
 
 # stdlib
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
@@ -10,23 +10,25 @@
 # relative
 from . import gevent_patch  # noqa: F401
 from .client.client import connect  # noqa: F401
 from .client.client import login  # noqa: F401
 from .client.client import register  # noqa: F401
 from .client.deploy import Orchestra  # noqa: F401
 from .client.registry import DomainRegistry  # noqa: F401
+from .client.registry import EnclaveRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
 from .client.search import Search  # noqa: F401
 from .client.search import SearchResults  # noqa: F401
 from .client.user_settings import UserSettings  # noqa: F401
 from .client.user_settings import settings  # noqa: F401
 from .external import OBLV  # noqa: F401
 from .external import enable_external_lib  # noqa: F401
 from .node.credentials import SyftSigningKey  # noqa: F401
 from .node.domain import Domain  # noqa: F401
+from .node.enclave import Enclave  # noqa: F401
 from .node.gateway import Gateway  # noqa: F401
 from .node.server import serve_node  # noqa: F401
 from .node.server import serve_node as bind_worker  # noqa: F401
 from .node.worker import Worker  # noqa: F401
 from .serde import NOTHING  # noqa: F401
 from .serde.deserialize import _deserialize as deserialize  # noqa: F401
 from .serde.serializable import serializable  # noqa: F401
@@ -38,15 +40,15 @@
 from .service.code.user_code import UserCodeStatus  # noqa: F401; noqa: F401
 from .service.code.user_code import syft_function  # noqa: F401; noqa: F401
 from .service.code.user_code import syft_function_single_use  # noqa: F401; noqa: F401
 from .service.data_subject import DataSubjectCreate as DataSubject  # noqa: F401
 from .service.dataset.dataset import Contributor  # noqa: F401
 from .service.dataset.dataset import CreateAsset as Asset  # noqa: F401
 from .service.dataset.dataset import CreateDataset as Dataset  # noqa: F401
-from .service.message.messages import MessageStatus  # noqa: F401
+from .service.notification.notifications import NotificationStatus  # noqa: F401
 from .service.policy.policy import CustomInputPolicy  # noqa: F401
 from .service.policy.policy import CustomOutputPolicy  # noqa: F401
 from .service.policy.policy import ExactMatch  # noqa: F401
 from .service.policy.policy import SingleExecutionExactOutput  # noqa: F401
 from .service.policy.policy import UserInputPolicy  # noqa: F401
 from .service.policy.policy import UserOutputPolicy  # noqa: F401
 from .service.project.project import ProjectSubmit as Project  # noqa: F401
@@ -119,14 +121,19 @@
 
 @module_property
 def _gateways() -> NetworkRegistry:
     return NetworkRegistry()
 
 
 @module_property
+def _enclaves() -> EnclaveRegistry:
+    return EnclaveRegistry()
+
+
+@module_property
 def _domains() -> DomainRegistry:
     return DomainRegistry()
 
 
 @module_property
 def _settings() -> UserSettings:
     return settings
```

### Comparing `syft-0.8.2b2/src/syft/abstract_node.py` & `syft-0.8.2b3/src/syft/abstract_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 @serializable()
 class NodeType(Enum):
     DOMAIN = "domain"
     NETWORK = "network"
     ENCLAVE = "enclave"
+    GATEWAY = "gateway"
 
 
 class AbstractNode:
     id: Optional[UID]
     name: Optional[str]
     node_type: Optional[NodeType]
```

### Comparing `syft-0.8.2b2/src/syft/client/api.py` & `syft-0.8.2b3/src/syft/client/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ..serde.recursive import index_syft_by_module_name
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..serde.signature import Signature
 from ..serde.signature import signature_remove_context
 from ..serde.signature import signature_remove_self
 from ..service.context import AuthedServiceContext
+from ..service.context import ChangeContext
 from ..service.response import SyftAttributeError
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftBaseObject
@@ -338,14 +339,26 @@
         if hasattr(self, "get_all_unread"):
             results = self.get_all_unread()
         else:
             results = self.get_all()
         return results._repr_html_()
 
 
+def debox_signed_syftapicall_response(
+    signed_result: SignedSyftAPICall,
+) -> Union[Any, SyftError]:
+    if not isinstance(signed_result, SignedSyftAPICall):
+        return SyftError(message="The result is not signed")  # type: ignore
+
+    if not signed_result.is_valid:
+        return SyftError(message="The result signature is invalid")  # type: ignore
+
+    return signed_result.message.data
+
+
 @instrument
 @serializable(attrs=["endpoints", "node_uid", "node_name", "lib_endpoints"])
 class SyftAPI(SyftObject):
     # version
     __canonical_name__ = "SyftAPI"
     __version__ = SYFT_OBJECT_VERSION_1
 
@@ -438,21 +451,15 @@
             lib_endpoints=lib_endpoints,
         )
 
     def make_call(self, api_call: SyftAPICall) -> Result:
         signed_call = api_call.sign(credentials=self.signing_key)
         signed_result = self.connection.make_call(signed_call)
 
-        if not isinstance(signed_result, SignedSyftAPICall):
-            return SyftError(message="The result is not signed")  # type: ignore
-
-        if not signed_result.is_valid:
-            return SyftError(message="The result signature is invalid")  # type: ignore
-
-        result = signed_result.message.data
+        result = debox_signed_syftapicall_response(signed_result=signed_result)
 
         if isinstance(result, OkErr):
             if result.is_ok():
                 res = result.ok()
                 # we update the api when we create objects that change it
                 self.update_api(res)
                 return res
@@ -636,29 +643,43 @@
 
 @serializable()
 class NodeView(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     node_name: str
+    node_id: UID
     verify_key: SyftVerifyKey
 
     @staticmethod
     def from_api(api: SyftAPI):
         # stores the name root verify key of the domain node
         node_metadata = api.connection.get_node_metadata(api.signing_key)
         return NodeView(
             node_name=node_metadata.name,
+            node_id=api.node_uid,
             verify_key=SyftVerifyKey.from_string(node_metadata.verify_key),
         )
 
+    @classmethod
+    def from_change_context(cls, context: ChangeContext):
+        return cls(
+            node_name=context.node.name,
+            node_id=context.node.id,
+            verify_key=context.node.signing_key.verify_key,
+        )
+
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, NodeView):
             return False
-        return self.node_name == other.node_name and self.verify_key == other.verify_key
+        return (
+            self.node_name == other.node_name
+            and self.verify_key == other.verify_key
+            and self.node_id == other.node_id
+        )
 
     def __hash__(self) -> int:
         return hash((self.node_name, self.verify_key))
 
 
 def validate_callable_args_and_kwargs(args, kwargs, signature: Signature):
     _valid_kwargs = {}
```

### Comparing `syft-0.8.2b2/src/syft/client/client.py` & `syft-0.8.2b3/src/syft/client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,88 +2,109 @@
 from __future__ import annotations
 
 # stdlib
 from enum import Enum
 import hashlib
 import json
 from typing import Any
+from typing import Callable
 from typing import Dict
 from typing import Optional
-from typing import TYPE_CHECKING
+from typing import Tuple
 from typing import Type
 from typing import Union
 from typing import cast
 
 # third party
 import pydantic
 import requests
 from requests import Response
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
-from tqdm import tqdm
 from typing_extensions import Self
 
 # relative
 from .. import __version__
 from ..abstract_node import AbstractNode
-from ..img.base64 import base64read
 from ..node.credentials import SyftSigningKey
 from ..node.credentials import SyftVerifyKey
 from ..node.credentials import UserLoginCredentials
 from ..serde.deserialize import _deserialize
 from ..serde.serializable import serializable
 from ..serde.serialize import _serialize
 from ..service.context import NodeServiceContext
-from ..service.dataset.dataset import CreateDataset
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..types.grid_url import GridURL
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.uid import UID
-from ..util.fonts import fonts_css
 from ..util.logger import debug
 from ..util.telemetry import instrument
-from ..util.util import get_mb_size
 from ..util.util import thread_ident
 from ..util.util import verify_tls
 from .api import APIModule
 from .api import APIRegistry
 from .api import SignedSyftAPICall
 from .api import SyftAPI
 from .api import SyftAPICall
+from .api import debox_signed_syftapicall_response
 from .connection import NodeConnection
 
 # use to enable mitm proxy
 # from syft.grid.connections.http_connection import HTTPConnection
 # HTTPConnection.proxies = {"http": "http://127.0.0.1:8080"}
 
-if TYPE_CHECKING:
-    # relative
-    from ..service.project.project import Project
-
 
 def upgrade_tls(url: GridURL, response: Response) -> GridURL:
     try:
         if response.url.startswith("https://") and url.protocol == "http":
             # we got redirected to https
             https_url = GridURL.from_url(response.url).with_path("")
             debug(f"GridURL Upgraded to HTTPS. {https_url}")
             return https_url
     except Exception as e:
         print(f"Failed to upgrade to HTTPS. {e}")
     return url
 
 
+def forward_message_to_proxy(
+    make_call: Callable,
+    proxy_target_uid: UID,
+    path: str,
+    credentials: Optional[SyftSigningKey] = None,
+    args: Optional[Tuple] = None,
+    kwargs: Optional[Dict] = None,
+):
+    kwargs = {} if kwargs is None else kwargs
+    args = [] if args is None else args
+    call = SyftAPICall(
+        node_uid=proxy_target_uid,
+        path=path,
+        args=args,
+        kwargs=kwargs,
+        blocking=True,
+    )
+
+    if credentials is None:
+        # generate a random signing key
+        credentials = SyftSigningKey.generate()
+
+    signed_message = call.sign(credentials=credentials)
+    signed_result = make_call(signed_message)
+    response = debox_signed_syftapicall_response(signed_result)
+    return response
+
+
 API_PATH = "/api/v2"
 DEFAULT_PYGRID_PORT = 80
 DEFAULT_PYGRID_ADDRESS = f"http://localhost:{DEFAULT_PYGRID_PORT}"
 
 
 class Routes(Enum):
     ROUTE_METADATA = f"{API_PATH}/metadata"
@@ -161,53 +182,77 @@
         # upgrade to tls if available
         self.url = upgrade_tls(self.url, response)
 
         return response.content
 
     def get_node_metadata(self, credentials: SyftSigningKey) -> NodeMetadataJSON:
         if self.proxy_target_uid:
-            call = SyftAPICall(
-                node_uid=self.proxy_target_uid,
+            response = forward_message_to_proxy(
+                make_call=self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
                 path="metadata",
-                args=[],
-                kwargs={},
-                blocking=True,
-            )
-            signed_call = call.sign(credentials=credentials)
-            response = self.make_call(signed_call)
-            if isinstance(response, SyftError):
-                return response
-            return response.to(NodeMetadataJSON)
+                credentials=credentials,
+            )
+            return response
         else:
             response = self._make_get(self.routes.ROUTE_METADATA.value)
             metadata_json = json.loads(response)
             return NodeMetadataJSON(**metadata_json)
 
     def get_api(self, credentials: SyftSigningKey) -> SyftAPI:
         params = {"verify_key": str(credentials.verify_key)}
-        content = self._make_get(self.routes.ROUTE_API.value, params=params)
-        obj = _deserialize(content, from_bytes=True)
+        if self.proxy_target_uid:
+            obj = forward_message_to_proxy(
+                self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
+                path="api",
+                kwargs={"credentials": credentials},
+                credentials=credentials,
+            )
+        else:
+            content = self._make_get(self.routes.ROUTE_API.value, params=params)
+            obj = _deserialize(content, from_bytes=True)
         obj.connection = self
         obj.signing_key = credentials
         if self.proxy_target_uid:
             obj.node_uid = self.proxy_target_uid
         return cast(SyftAPI, obj)
 
-    def login(self, email: str, password: str) -> Optional[SyftSigningKey]:
+    def login(
+        self,
+        email: str,
+        password: str,
+    ) -> Optional[SyftSigningKey]:
         credentials = {"email": email, "password": password}
-        response = self._make_post(self.routes.ROUTE_LOGIN.value, credentials)
-        obj = _deserialize(response, from_bytes=True)
+        if self.proxy_target_uid:
+            obj = forward_message_to_proxy(
+                self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
+                path="login",
+                kwargs=credentials,
+            )
+        else:
+            response = self._make_post(self.routes.ROUTE_LOGIN.value, credentials)
+            obj = _deserialize(response, from_bytes=True)
         if isinstance(obj, UserPrivateKey):
             return obj
         return None
 
     def register(self, new_user: UserCreate) -> SyftSigningKey:
         data = _serialize(new_user, to_bytes=True)
-        response = self._make_post(self.routes.ROUTE_REGISTER.value, data=data)
-        response = _deserialize(response, from_bytes=True)
+        if self.proxy_target_uid:
+            response = forward_message_to_proxy(
+                self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
+                path="register",
+                kwargs={"new_user": new_user},
+            )
+        else:
+            response = self._make_post(self.routes.ROUTE_REGISTER.value, data=data)
+            response = _deserialize(response, from_bytes=True)
         return response
 
     def make_call(self, signed_call: SignedSyftAPICall) -> Union[Any, SyftError]:
         msg_bytes: bytes = _serialize(obj=signed_call, to_bytes=True)
         response = requests.post(  # nosec
             url=str(self.api_url),
             data=msg_bytes,
@@ -226,46 +271,69 @@
 
     def __str__(self) -> str:
         return f"{type(self).__name__}: {self.url}"
 
     def __hash__(self) -> int:
         return hash(self.proxy_target_uid) + hash(self.url)
 
+    def get_client_type(self) -> Type[SyftClient]:
+        # TODO: Rasswanth, should remove passing in credentials
+        # when metadata are proxy forwarded in the grid routes
+        # in the gateway fixes PR
+        # relative
+        from .domain_client import DomainClient
+        from .enclave_client import EnclaveClient
+        from .gateway_client import GatewayClient
+
+        metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
+        if metadata.node_type == "domain":
+            return DomainClient
+        elif metadata.node_type == "gateway":
+            return GatewayClient
+        elif metadata.node_type == "enclave":
+            return EnclaveClient
+        else:
+            return SyftError(message=f"Unknown node type {metadata.node_type}")
+
 
 @serializable()
 class PythonConnection(NodeConnection):
     __canonical_name__ = "PythonConnection"
     __version__ = SYFT_OBJECT_VERSION_1
 
     node: AbstractNode
     proxy_target_uid: Optional[UID]
 
     def with_proxy(self, proxy_target_uid: UID) -> Self:
         return PythonConnection(node=self.node, proxy_target_uid=proxy_target_uid)
 
     def get_node_metadata(self, credentials: SyftSigningKey) -> NodeMetadataJSON:
         if self.proxy_target_uid:
-            call = SyftAPICall(
-                node_uid=self.proxy_target_uid,
+            response = forward_message_to_proxy(
+                make_call=self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
                 path="metadata",
-                args=[],
-                kwargs={},
-                blocking=True,
-            )
-            signed_call = call.sign(credentials=credentials)
-            response = self.make_call(signed_call)
-            if isinstance(response, SyftError):
-                return response
-            return response.to(NodeMetadataJSON)
+                credentials=credentials,
+            )
+            return response
         else:
             return self.node.metadata.to(NodeMetadataJSON)
 
     def get_api(self, credentials: SyftSigningKey) -> SyftAPI:
         # todo: its a bit odd to identify a user by its verify key maybe?
-        obj = self.node.get_api(for_user=credentials.verify_key)
+        if self.proxy_target_uid:
+            obj = forward_message_to_proxy(
+                self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
+                path="api",
+                kwargs={"credentials": credentials},
+                credentials=credentials,
+            )
+        else:
+            obj = self.node.get_api(for_user=credentials.verify_key)
         obj.connection = self
         obj.signing_key = credentials
         if self.proxy_target_uid:
             obj.node_uid = self.proxy_target_uid
         return obj
 
     def get_cache_key(self) -> str:
@@ -279,35 +347,75 @@
         )
         method = self.node.get_method_with_context(
             UserService.exchange_credentials, context
         )
         result = method()
         return result
 
-    def login(self, email: str, password: str) -> Optional[SyftSigningKey]:
-        obj = self.exchange_credentials(email=email, password=password)
+    def login(
+        self,
+        email: str,
+        password: str,
+    ) -> Optional[SyftSigningKey]:
+        if self.proxy_target_uid:
+            obj = forward_message_to_proxy(
+                self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
+                path="login",
+                kwargs={"email": email, "password": password},
+            )
+
+        else:
+            obj = self.exchange_credentials(email=email, password=password)
         if isinstance(obj, UserPrivateKey):
             return obj
         return None
 
     def register(self, new_user: UserCreate) -> Optional[SyftSigningKey]:
-        service_context = NodeServiceContext(node=self.node)
-        method = self.node.get_service_method(UserService.register)
-        response = method(context=service_context, new_user=new_user)
+        if self.proxy_target_uid:
+            response = forward_message_to_proxy(
+                self.make_call,
+                proxy_target_uid=self.proxy_target_uid,
+                path="register",
+                kwargs={"new_user": new_user},
+            )
+        else:
+            service_context = NodeServiceContext(node=self.node)
+            method = self.node.get_service_method(UserService.register)
+            response = method(context=service_context, new_user=new_user)
         return response
 
     def make_call(self, signed_call: SignedSyftAPICall) -> Union[Any, SyftError]:
         return self.node.handle_api_call(signed_call)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}"
 
     def __str__(self) -> str:
         return f"{type(self).__name__}"
 
+    def get_client_type(self) -> Type[SyftClient]:
+        # TODO: Rasswanth, should remove passing in credentials
+        # when metadata are proxy forwarded in the grid routes
+        # in the gateway fixes PR
+        # relative
+        from .domain_client import DomainClient
+        from .enclave_client import EnclaveClient
+        from .gateway_client import GatewayClient
+
+        metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
+        if metadata.node_type == "domain":
+            return DomainClient
+        elif metadata.node_type == "gateway":
+            return GatewayClient
+        elif metadata.node_type == "enclave":
+            return EnclaveClient
+        else:
+            return SyftError(message=f"Unknown node type {metadata.node_type}")
+
 
 @instrument
 @serializable()
 class SyftClient:
     connection: NodeConnection
     metadata: Optional[NodeMetadataJSON]
     credentials: Optional[SyftSigningKey]
@@ -346,78 +454,60 @@
 
     @property
     def verify_key(self) -> SyftVerifyKey:
         if self.credentials is None:
             raise ValueError("SigningKey not set on client")
         return self.credentials.verify_key
 
-    @staticmethod
-    def from_url(url: Union[str, GridURL]) -> Self:
-        return SyftClient(connection=HTTPConnection(GridURL.from_url(url)))
-
-    @staticmethod
-    def from_node(node: AbstractNode) -> Self:
-        return SyftClient(connection=PythonConnection(node=node))
+    @classmethod
+    def from_url(cls, url: Union[str, GridURL]) -> Self:
+        return cls(connection=HTTPConnection(GridURL.from_url(url)))
+
+    @classmethod
+    def from_node(cls, node: AbstractNode) -> Self:
+        return cls(connection=PythonConnection(node=node))
 
     @property
     def name(self) -> Optional[str]:
         return self.metadata.name if self.metadata else None
 
     @property
     def id(self) -> Optional[UID]:
         return UID.from_string(self.metadata.id) if self.metadata else None
 
     @property
     def icon(self) -> str:
         return "📡"
 
     @property
+    def peer(self) -> Any:
+        # relative
+        from ..service.network.network_service import NodePeer
+
+        return NodePeer.from_client(self)
+
+    @property
+    def route(self) -> Any:
+        return self.connection.route
+
+    @property
     def api(self) -> SyftAPI:
         # invalidate API
         if self._api is None or (self._api.signing_key != self.credentials):
             self._fetch_api(self.credentials)
 
         return self._api
 
     def guest(self) -> Self:
-        return SyftClient(
+        return self.__class__(
             connection=self.connection,
             credentials=SyftSigningKey.generate(),
             metadata=self.metadata,
         )
 
-    def upload_dataset(self, dataset: CreateDataset) -> Union[SyftSuccess, SyftError]:
-        # relative
-        from ..types.twin_object import TwinObject
-
-        dataset._check_asset_must_contain_mock()
-        dataset_size = 0
-
-        for asset in tqdm(dataset.asset_list):
-            print(f"Uploading: {asset.name}")
-            try:
-                twin = TwinObject(private_obj=asset.data, mock_obj=asset.mock)
-            except Exception as e:
-                return SyftError(message=f"Failed to create twin. {e}")
-            response = self.api.services.action.set(twin)
-            if isinstance(response, SyftError):
-                print(f"Failed to upload asset\n: {asset}")
-                return response
-            asset.action_id = twin.id
-            asset.node_uid = self.id
-            dataset_size += get_mb_size(asset.data)
-        dataset.mb_size = dataset_size
-        valid = dataset.check()
-        if valid.ok():
-            return self.api.services.dataset.add(dataset=dataset)
-        else:
-            if len(valid.err()) > 0:
-                return tuple(valid.err())
-            return valid.err()
-
     def exchange_route(self, client: Self) -> Union[SyftSuccess, SyftError]:
         # relative
         from ..service.network.routes import connection_to_route
 
         self_node_route = connection_to_route(self.connection)
         remote_node_route = connection_to_route(client.connection)
 
@@ -425,93 +515,51 @@
             self_node_route=self_node_route,
             remote_node_route=remote_node_route,
             remote_node_verify_key=client.metadata.to(NodeMetadata).verify_key,
         )
 
         return result
 
-    def apply_to_gateway(self, client: Self) -> None:
-        return self.exchange_route(client)
-
-    @property
-    def data_subject_registry(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("data_subject"):
-            return self.api.services.data_subject
-        return None
-
     @property
     def users(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("user"):
             return self.api.services.user
         return None
 
     @property
     def settings(self) -> Optional[APIModule]:
         if self.api is not None and self.api.has_service("user"):
             return self.api.services.settings
         return None
 
     @property
-    def code(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("code"):
-            return self.api.services.code
-
-    @property
-    def requests(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("request"):
-            return self.api.services.request
-        return None
-
-    @property
-    def datasets(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("dataset"):
-            return self.api.services.dataset
-        return None
-
-    @property
     def notifications(self) -> Optional[APIModule]:
         print(
             "WARNING: Notifications is currently is in a beta state, so use carefully!"
         )
         print("If possible try using client.requests/client.projects")
-        if self.api is not None and self.api.has_service("messages"):
-            return self.api.services.messages
+        if self.api is not None and self.api.has_service("notifications"):
+            return self.api.services.notifications
         return None
 
     @property
     def domains(self) -> Optional[APIModule]:
-        if self.api is not None and self.api.has_service("network"):
-            return self.api.services.network.get_all_peers()
-        return None
+        return self.peers
 
     @property
-    def projects(self) -> Optional[APIModule]:
-        if self.api.has_service("project"):
-            return self.api.services.project
+    def peers(self) -> Optional[APIModule]:
+        if self.api is not None and self.api.has_service("network"):
+            return self.api.services.network.get_all_peers()
         return None
 
-    def get_project(
-        self,
-        name: str = None,
-        uid: UID = None,
-    ) -> Optional[Project]:
-        """Get project by name or UID"""
-
-        if not self.api.has_service("project"):
-            return None
-
-        if name:
-            return self.api.services.project.get_by_name(name)
-
-        elif uid:
-            return self.api.services.project.get_by_uid(uid)
-
-        return self.api.services.project.get_all()
-
-    def login(self, email: str, password: str, cache: bool = True) -> Self:
+    def login(
+        self, email: str, password: str, cache: bool = True, register=False, **kwargs
+    ) -> Self:
+        if register:
+            self.register(email=email, password=password, **kwargs)
         user_private_key = self.connection.login(email=email, password=password)
         signing_key = None
         if user_private_key is not None:
             signing_key = user_private_key.signing_key
             self.__user_role = user_private_key.role
         if signing_key is not None:
             self.credentials = signing_key
@@ -575,33 +623,14 @@
         except Exception as e:
             return SyftError(message=str(e))
         response = self.connection.register(new_user=new_user)
         if isinstance(response, tuple):
             response = response[0]
         return response
 
-    @property
-    def peer(self) -> Any:
-        # relative
-        from ..service.network.network_service import NodePeer
-
-        return NodePeer.from_client(self)
-
-    @property
-    def route(self) -> Any:
-        return self.connection.route
-
-    def proxy_to(self, peer: Any) -> Self:
-        connection = self.connection.with_proxy(peer.id)
-        client = SyftClient(
-            connection=connection,
-            credentials=self.credentials,
-        )
-        return client
-
     def __getattr__(self, name):
         if (
             hasattr(self, "api")
             and hasattr(self.api, "lib")
             and hasattr(self.api.lib, name)
         ):
             return getattr(self.api.lib, name)
@@ -627,111 +656,17 @@
         if self.connection and self.connection.proxy_target_uid:
             proxy_target_uid = self.connection.proxy_target_uid
         client_type = type(self).__name__
         uid = self.id
         if proxy_target_uid:
             client_type = "ProxyClient"
             uid = proxy_target_uid
-            return f"<{client_type} - <{uid}>: via {self.id} {self.connection}>"
+            return f"<{client_type} - <{uid}>: via {self.connection}>"
         return f"<{client_type} - {self.name} <{uid}>: {self.connection}>"
 
-    def _repr_html_(self) -> str:
-        guest_commands = """
-        <li><span class='syft-code-block'>&lt;your_client&gt;.datasets</span> - list datasets</li>
-        <li><span class='syft-code-block'>&lt;your_client&gt;.code</span> - list code</li>
-        <li><span class='syft-code-block'>&lt;your_client&gt;.login</span> - list projects</li>
-        <li>
-            <span class='syft-code-block'>&lt;your_client&gt;.code.submit?</span> - display function signature
-        </li>"""
-        ds_commands = """
-        <li><span class='syft-code-block'>&lt;your_client&gt;.datasets</span> - list datasets</li>
-        <li><span class='syft-code-block'>&lt;your_client&gt;.code</span> - list code</li>
-        <li><span class='syft-code-block'>&lt;your_client&gt;.projects</span> - list projects</li>
-        <li>
-            <span class='syft-code-block'>&lt;your_client&gt;.code.submit?</span> - display function signature
-        </li>"""
-
-        do_commands = """
-        <li><span class='syft-code-block'>&lt;your_client&gt;.projects</span> - list projects</li>
-        <li><span class='syft-code-block'>&lt;your_client&gt;.requests</span> - list requests</li>
-        <li><span class='syft-code-block'>&lt;your_client&gt;.users</span> - list users</li>
-        <li>
-            <span class='syft-code-block'>&lt;your_client&gt;.requests.submit?</span> - display function signature
-        </li>"""
-
-        # TODO: how to select ds/do commands based on self.__user_role
-
-        if (
-            self.user_role.value == ServiceRole.NONE.value
-            or self.user_role.value == ServiceRole.GUEST.value
-        ):
-            commands = guest_commands
-        elif (
-            self.user_role is not None
-            and self.user_role.value == ServiceRole.DATA_SCIENTIST.value
-        ):
-            commands = ds_commands
-        elif (
-            self.user_role is not None
-            and self.user_role.value >= ServiceRole.DATA_OWNER.value
-        ):
-            commands = do_commands
-
-        command_list = f"""
-        <ul style='padding-left: 1em;'>
-            {commands}
-        </ul>
-        """
-
-        small_grid_symbol_logo = base64read("small-grid-symbol-logo.png")
-
-        return f"""
-        <style>
-            {fonts_css}
-
-            .syft-container {{
-                padding: 5px;
-                font-family: 'Open Sans';
-            }}
-            .syft-alert-info {{
-                color: #1F567A;
-                background-color: #C2DEF0;
-                border-radius: 4px;
-                padding: 5px;
-                padding: 13px 10px
-            }}
-            .syft-code-block {{
-                background-color: #f7f7f7;
-                border: 1px solid #cfcfcf;
-                padding: 0px 2px;
-            }}
-            .syft-space {{
-                margin-top: 1em;
-            }}
-        </style>
-        <div class="syft-client syft-container">
-            <img src="{small_grid_symbol_logo}" alt="Logo"
-            style="width:48px;height:48px;padding:3px;">
-            <h2>Welcome to {self.name}</h2>
-            <div class="syft-space">
-                <!-- <strong>Institution:</strong> TODO<br /> -->
-                <!-- <strong>Owner:</strong> TODO<br /> -->
-                <strong>URL:</strong> {getattr(self.connection, 'url', '')}<br />
-                <!-- <strong>PyGrid Admin:</strong> TODO<br /> -->
-            </div>
-            <div class='syft-alert-info syft-space'>
-                &#9432;&nbsp;
-                This domain is run by the library PySyft to learn more about how it works visit
-                <a href="https://github.com/OpenMined/PySyft">github.com/OpenMined/PySyft</a>.
-            </div>
-            <h4>Commands to Get Started</h4>
-            {command_list}
-        </div><br />
-        """
-
     def _fetch_node_metadata(self, credentials: SyftSigningKey) -> None:
         metadata = self.connection.get_node_metadata(credentials=credentials)
         if isinstance(metadata, NodeMetadataJSON):
             metadata.check_version(__version__)
             self.metadata = metadata
 
     def _fetch_api(self, credentials: SyftSigningKey):
@@ -758,16 +693,21 @@
     if node:
         connection = PythonConnection(node=node)
     else:
         url = GridURL.from_url(url)
         if isinstance(port, (int, str)):
             url.set_port(int(port))
         connection = HTTPConnection(url=url)
-    _client = SyftClient(connection=connection)
-    return _client
+
+    client_type = connection.get_client_type()
+
+    if isinstance(client_type, SyftError):
+        return client_type
+
+    return client_type(connection=connection)
 
 
 @instrument
 def register(
     url: Union[str, GridURL],
     port: int,
     name: str,
@@ -793,14 +733,16 @@
     port: Optional[int] = None,
     email: Optional[str] = None,
     password: Optional[str] = None,
     cache: bool = True,
     verbose: bool = True,
 ) -> SyftClient:
     _client = connect(url=url, node=node, port=port)
+    if isinstance(_client, SyftError):
+        return _client
     connection = _client.connection
 
     login_credentials = None
     if email and password:
         login_credentials = UserLoginCredentials(email=email, password=password)
 
     if login_credentials is None:
```

### Comparing `syft-0.8.2b2/src/syft/client/connection.py` & `syft-0.8.2b3/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/client/deploy.py` & `syft-0.8.2b3/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/client/registry.py` & `syft-0.8.2b3/src/syft/client/registry.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 # third party
 import pandas as pd
 import requests
 
 # relative
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.network.network_service import NodePeer
+from ..service.response import SyftException
 from ..types.grid_url import GridURL
+from ..util.constants import DEFAULT_TIMEOUT
 from ..util.logger import error
 from ..util.logger import warning
+from .enclave_client import EnclaveClient
 
 if TYPE_CHECKING:
     # relative
     from .client import Client
 
 NETWORK_REGISTRY_URL = (
     "https://raw.githubusercontent.com/OpenMined/NetworkRegistry/main/gateways.json"
@@ -47,37 +50,39 @@
     @property
     def online_networks(self) -> List[Dict]:
         networks = self.all_networks
 
         def check_network(network: Dict) -> Optional[Dict[Any, Any]]:
             url = "http://" + network["host_or_ip"] + ":" + str(network["port"]) + "/"
             try:
-                res = requests.get(url, timeout=0.5)  # nosec
+                res = requests.get(url, timeout=DEFAULT_TIMEOUT)  # nosec
                 online = "This is a PyGrid Network node." in res.text
             except Exception:
                 online = False
 
             # networks without frontend have a /ping route in 0.7.0
             if not online:
                 try:
                     ping_url = url + "ping"
-                    res = requests.get(ping_url, timeout=0.5)  # nosec
+                    res = requests.get(ping_url, timeout=DEFAULT_TIMEOUT)  # nosec
                     online = res.status_code == 200
                 except Exception:
                     online = False
 
             if online:
                 version = network.get("version", None)
                 # Check if syft version was described in NetworkRegistry
                 # If it's unknown, try to update it to an available version.
                 if not version or version == "unknown":
                     # If not defined, try to ask in /syft/version endpoint (supported by 0.7.0)
                     try:
                         version_url = url + "api/v2/metadata"
-                        res = requests.get(version_url, timeout=0.5)  # nosec
+                        res = requests.get(
+                            version_url, timeout=DEFAULT_TIMEOUT
+                        )  # nosec
                         if res.status_code == 200:
                             network["version"] = res.json()["syft_version"]
                         else:
                             network["version"] = "unknown"
                     except Exception:
                         network["version"] = "unknown"
                 return network
@@ -118,15 +123,15 @@
             protocol = network["protocol"]
             host_or_ip = network["host_or_ip"]
             grid_url = GridURL(port=port, protocol=protocol, host_or_ip=host_or_ip)
             client = connect(url=str(grid_url))
             return client.guest()
         except Exception as e:
             error(f"Failed to login with: {network}. {e}")
-            raise e
+            raise SyftException(f"Failed to login with: {network}. {e}")
 
     def __getitem__(self, key: Union[str, int]) -> Client:  # type: ignore
         if isinstance(key, int):
             return self.create_client(network=self.online_networks[key])
         else:
             on = self.online_networks
             for network in on:
@@ -151,37 +156,37 @@
     @property
     def online_networks(self) -> List[Dict]:
         networks = self.all_networks
 
         def check_network(network: Dict) -> Optional[Dict[Any, Any]]:
             url = "http://" + network["host_or_ip"] + ":" + str(network["port"]) + "/"
             try:
-                res = requests.get(url, timeout=0.5)
+                res = requests.get(url, timeout=DEFAULT_TIMEOUT)
                 online = "This is a PyGrid Network node." in res.text
             except Exception:
                 online = False
 
             # networks without frontend have a /ping route in 0.7.0
             if not online:
                 try:
                     ping_url = url + "ping"
-                    res = requests.get(ping_url, timeout=0.5)
+                    res = requests.get(ping_url, timeout=DEFAULT_TIMEOUT)
                     online = res.status_code == 200
                 except Exception:
                     online = False
 
             if online:
                 version = network.get("version", None)
                 # Check if syft version was described in NetworkRegistry
                 # If it's unknown, try to update it to an available version.
                 if not version or version == "unknown":
                     # If not defined, try to ask in /syft/version endpoint (supported by 0.7.0)
                     try:
                         version_url = url + "api/v2/metadata"
-                        res = requests.get(version_url, timeout=0.5)
+                        res = requests.get(version_url, timeout=DEFAULT_TIMEOUT)
                         if res.status_code == 200:
                             network["version"] = res.json()["syft_version"]
                         else:
                             network["version"] = "unknown"
                     except Exception:
                         network["version"] = "unknown"
                 return network
@@ -264,20 +269,122 @@
         return pd.DataFrame(on).to_string()
 
     def create_client(self, peer: NodePeer) -> Client:  # type: ignore
         try:
             return peer.guest_client
         except Exception as e:
             error(f"Failed to login to: {peer}. {e}")
-            raise e
+            raise SyftException(f"Failed to login to: {peer}. {e}")
 
     def __getitem__(self, key: Union[str, int]) -> Client:  # type: ignore
         if isinstance(key, int):
             return self.create_client(self.online_domains[key][0])
         else:
             on = self.online_domains
             count = 0
             for domain, _ in on:
                 if domain.name == key:
                     return self.create_client(self.online_domains[count][0])
                 count += 1
         raise KeyError(f"Invalid key: {key} for {on}")
+
+
+ENCLAVE_REGISTRY_URL = (
+    "https://raw.githubusercontent.com/OpenMined/NetworkRegistry/main/enclaves.json"
+)
+ENCLAVE_REGISTRY_REPO = "https://github.com/OpenMined/NetworkRegistry"
+
+
+class EnclaveRegistry:
+    def __init__(self) -> None:
+        self.all_enclaves: List[Dict] = []
+        try:
+            response = requests.get(ENCLAVE_REGISTRY_URL)  # nosec
+            enclaves_json = response.json()
+            self.all_enclaves = enclaves_json["2.0.0"]["enclaves"]
+        except Exception as e:
+            warning(
+                f"Failed to get Enclave Registry, go checkout: {ENCLAVE_REGISTRY_REPO}. {e}"
+            )
+
+    @property
+    def online_enclaves(self) -> List[Dict]:
+        enclaves = self.all_enclaves
+
+        def check_enclave(enclave: Dict) -> Optional[Dict[Any, Any]]:
+            url = "http://" + enclave["host_or_ip"] + ":" + str(enclave["port"]) + "/"
+            try:
+                res = requests.get(url, timeout=DEFAULT_TIMEOUT)  # nosec
+                online = "OpenMined Enclave Node Running" in res.text
+            except Exception:
+                online = False
+
+            if online:
+                version = enclave.get("version", None)
+                # Check if syft version was described in EnclaveRegistry
+                # If it's unknown, try to update it to an available version.
+                if not version or version == "unknown":
+                    # If not defined, try to ask in /syft/version endpoint (supported by 0.7.0)
+                    try:
+                        version_url = url + "api/v2/metadata"
+                        res = requests.get(
+                            version_url, timeout=DEFAULT_TIMEOUT
+                        )  # nosec
+                        if res.status_code == 200:
+                            enclave["version"] = res.json()["syft_version"]
+                        else:
+                            enclave["version"] = "unknown"
+                    except Exception:
+                        enclave["version"] = "unknown"
+                return enclave
+            return None
+
+        # We can use a with statement to ensure threads are cleaned up promptly
+        with futures.ThreadPoolExecutor(max_workers=20) as executor:
+            # map
+            _online_enclaves = list(
+                executor.map(lambda enclave: check_enclave(enclave), enclaves)
+            )
+
+        online_enclaves = list()
+        for each in _online_enclaves:
+            if each is not None:
+                online_enclaves.append(each)
+        return online_enclaves
+
+    def _repr_html_(self) -> str:
+        on = self.online_enclaves
+        if len(on) == 0:
+            return "(no enclaves online - try syft.enclaves.all_enclaves to see offline enclaves)"
+        return pd.DataFrame(on)._repr_html_()
+
+    def __repr__(self) -> str:
+        on = self.online_enclaves
+        if len(on) == 0:
+            return "(no enclaves online - try syft.enclaves.all_enclaves to see offline enclaves)"
+        return pd.DataFrame(on).to_string()
+
+    @staticmethod
+    def create_client(enclave: Dict[str, Any]) -> Client:  # type: ignore
+        # relative
+        from ..client.client import connect
+
+        try:
+            port = int(enclave["port"])
+            protocol = enclave["protocol"]
+            host_or_ip = enclave["host_or_ip"]
+            grid_url = GridURL(port=port, protocol=protocol, host_or_ip=host_or_ip)
+            client = connect(url=str(grid_url))
+            return client.guest()
+        except Exception as e:
+            error(f"Failed to login with: {enclave}. {e}")
+            raise SyftException(f"Failed to login with: {enclave}. {e}")
+
+    def __getitem__(self, key: Union[str, int]) -> EnclaveClient:  # type: ignore
+        if isinstance(key, int):
+            return self.create_client(enclave=self.online_enclaves[key])
+        else:
+            on = self.online_enclaves
+            for enclave in on:
+                if enclave["name"] == key:
+                    return self.create_client(enclave=enclave)
+        raise KeyError(f"Invalid key: {key} for {on}")
```

### Comparing `syft-0.8.2b2/src/syft/client/search.py` & `syft-0.8.2b3/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/client/user_settings.py` & `syft-0.8.2b3/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/__init__.py` & `syft-0.8.2b3/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/oblv/__init__.py` & `syft-0.8.2b3/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/oblv/deployment.py` & `syft-0.8.2b3/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/oblv/deployment_client.py` & `syft-0.8.2b3/src/syft/external/oblv/deployment_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,43 +13,39 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 
 # third party
 from oblv_ctl import OblvClient
-from pydantic import BaseModel
 from pydantic import validator
 import requests
 
 # relative
 from ...client.api import SyftAPI
 from ...client.client import SyftClient
 from ...client.client import login
+from ...enclave.metadata import EnclaveMetadata
 from ...serde.serializable import serializable
-from ...service.metadata.node_metadata import EnclaveMetadata
 from ...types.uid import UID
 from ...util.util import bcolors
 from .constants import LOCAL_MODE
 from .exceptions import OblvEnclaveError
 from .exceptions import OblvUnAuthorizedError
 from .oblv_proxy import check_oblv_proxy_installation_status
 
 if TYPE_CHECKING:
     # relative
     from ...service.code.user_code import SubmitUserCode
 
 
 @serializable()
-class OblvMetadata(EnclaveMetadata, BaseModel):
+class OblvMetadata(EnclaveMetadata):
     """Contains Metadata to connect to Oblivious Enclave"""
 
-    class Config:
-        arbitrary_types_allowed = True
-
     deployment_id: Optional[str]
     oblv_client: Optional[OblvClient]
 
     @validator("deployment_id")
     def check_valid_deployment_id(cls, deployment_id: str) -> str:
         if not deployment_id and not LOCAL_MODE:
             raise ValueError(
```

### Comparing `syft-0.8.2b2/src/syft/external/oblv/exceptions.py` & `syft-0.8.2b3/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.2b3/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.2b3/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/external/oblv/oblv_service.py` & `syft-0.8.2b3/src/syft/external/oblv/oblv_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,76 +5,53 @@
 import subprocess  # nosec
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
-from typing import Union
 from typing import cast
 
 # third party
 from oblv_ctl import OblvClient
 import requests
 from result import Err
 from result import Ok
 from result import Result
 
 # relative
-from ...client.api import NodeView
 from ...client.api import SyftAPI
 from ...client.client import HTTPConnection
 from ...client.client import Routes
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.deserialize import _deserialize as deserialize
 from ...serde.serializable import serializable
-from ...service.code.user_code import UserCode
+from ...service.action.action_object import ActionObject
 from ...service.code.user_code import UserCodeStatus
 from ...service.context import AuthedServiceContext
-from ...service.context import ChangeContext
 from ...service.response import SyftError
 from ...service.service import AbstractService
 from ...service.service import service_method
 from ...service.user.user_roles import GUEST_ROLE_LEVEL
 from ...store.document_store import DocumentStore
-from ...types.syft_object import SYFT_OBJECT_VERSION_1
-from ...types.syft_object import SyftObject
 from ...types.uid import UID
 from ...util.util import find_available_port
 from .constants import DOMAIN_CONNECTION_PORT
 from .constants import LOCAL_MODE
 from .deployment_client import OblvMetadata
 from .exceptions import OblvEnclaveError
 from .exceptions import OblvProxyConnectPCRError
 from .oblv_keys import OblvKeys
 from .oblv_keys_stash import OblvKeysStash
 
 # caches the connection to Enclave using the deployment ID
 OBLV_PROCESS_CACHE: Dict[str, List] = {}
 
 
-# TODO: 🟡 Duplication of PyPrimitive Dict
-# This is emulated since the action store curently accepts  only SyftObject types
-@serializable()
-class DictObject(SyftObject):
-    # version
-    __canonical_name__ = "Dict"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    base_dict: Dict[Any, Any] = {}
-
-    # serde / storage rules
-    __attr_searchable__ = []
-    __attr_unique__ = ["id"]
-
-    def __repr__(self) -> str:
-        return self.base_dict.__repr__()
-
-
 def connect_to_enclave(
     oblv_keys_stash: OblvKeysStash,
     verify_key: SyftVerifyKey,
     oblv_client: OblvClient,
     deployment_id: str,
     connection_port: int,
     oblv_key_name: str,
@@ -303,15 +280,17 @@
     def get_public_key(
         self,
         context: AuthedServiceContext,
     ) -> Result[Ok, Err]:
         "Retrieves the public key present on the Domain Node."
 
         if len(self.oblv_keys_stash):
-            oblv_keys = self.oblv_keys_stash.get_all(context.credentials)
+            # retrieve the public key from the stash using the node's verify key
+            # as the public should be accessible to all the users
+            oblv_keys = self.oblv_keys_stash.get_all(context.node.verify_key)
             if oblv_keys.is_ok():
                 oblv_keys = oblv_keys.ok()[0]
             else:
                 return oblv_keys.err()
 
             public_key_str = (
                 encodebytes(oblv_keys.public_key).decode("UTF-8").replace("\n", "")
@@ -405,72 +384,33 @@
         )
         if res.is_err():
             return res
         user_code.status = res.ok()
         user_code_service.update_code_state(context=context, code_item=user_code)
 
         if not action_service.exists(context=context, obj_id=user_code_id):
-            dict_object = DictObject(id=user_code_id)
-            dict_object.base_dict[str(context.credentials)] = inputs
+            dict_object = ActionObject.from_obj({})
+            dict_object.id = user_code_id
+            dict_object[str(context.credentials)] = inputs
             action_service.store.set(
                 uid=user_code_id,
                 credentials=context.node.verify_key,
                 syft_object=dict_object,
                 has_result_read_permission=True,
             )
 
         else:
             res = action_service.store.get(
                 uid=user_code_id, credentials=context.node.verify_key
             )
             if res.is_ok():
                 dict_object = res.ok()
-                dict_object.base_dict[str(context.credentials)] = inputs
+                dict_object[str(context.credentials)] = inputs
                 action_service.store.set(
                     uid=user_code_id,
                     credentials=context.node.verify_key,
                     syft_object=dict_object,
                 )
             else:
                 return res
 
         return Ok(Ok(True))
-
-
-# Checks if the given user code would  propogate value to enclave on acceptance
-def check_enclave_transfer(
-    user_code: UserCode, value: UserCodeStatus, context: ChangeContext
-) -> Union[Any, Ok]:
-    if not context.node or not context.node.signing_key:
-        return Err(f"{type(context)} has no node")
-    signing_key = context.node.signing_key
-    if (
-        isinstance(user_code.enclave_metadata, OblvMetadata)
-        and value == UserCodeStatus.EXECUTE
-    ):
-        method = context.node.get_service_method(OblvService.get_api_for)
-
-        api = method(
-            user_code.enclave_metadata,
-            context.node.signing_key,
-            worker_name=context.node.name,
-        )
-        # send data of the current node to enclave
-        node_view = NodeView(
-            node_name=context.node.name, verify_key=signing_key.verify_key
-        )
-        inputs = user_code.input_policy.inputs[node_view]
-        action_service = context.node.get_service("actionservice")
-        for var_name, uid in inputs.items():
-            action_object = action_service.store.get(
-                uid=uid, credentials=signing_key.verify_key
-            )
-            if action_object.is_err():
-                return action_object
-            inputs[var_name] = action_object.ok()
-
-        res = api.services.oblv.send_user_code_inputs_to_enclave(
-            user_code_id=user_code.id, inputs=inputs, node_name=context.node.name
-        )
-        return res
-    else:
-        return Ok()
```

### Comparing `syft-0.8.2b2/src/syft/gevent_patch.py` & `syft-0.8.2b3/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/img/logo.png` & `syft-0.8.2b3/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.2b3/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/node/credentials.py` & `syft-0.8.2b3/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/node/node.py` & `syft-0.8.2b3/src/syft/node/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,31 +32,33 @@
 from .. import __version__
 from ..abstract_node import AbstractNode
 from ..abstract_node import NodeType
 from ..client.api import SignedSyftAPICall
 from ..client.api import SyftAPI
 from ..client.api import SyftAPICall
 from ..client.api import SyftAPIData
+from ..client.api import debox_signed_syftapicall_response
 from ..external import OBLV
 from ..serde.deserialize import _deserialize
 from ..serde.serialize import _serialize
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import DictActionStore
 from ..service.action.action_store import SQLiteActionStore
 from ..service.code.user_code_service import UserCodeService
 from ..service.context import AuthedServiceContext
 from ..service.context import NodeServiceContext
 from ..service.context import UnauthedServiceContext
 from ..service.context import UserLoginCredentials
 from ..service.data_subject.data_subject_member_service import DataSubjectMemberService
 from ..service.data_subject.data_subject_service import DataSubjectService
 from ..service.dataset.dataset_service import DatasetService
-from ..service.message.message_service import MessageService
+from ..service.enclave.enclave_service import EnclaveService
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.network.network_service import NetworkService
+from ..service.notification.notification_service import NotificationService
 from ..service.policy.policy_service import PolicyService
 from ..service.project.project_service import ProjectService
 from ..service.queue.queue import APICallMessageHandler
 from ..service.queue.queue import QueueManager
 from ..service.queue.queue_stash import QueueItem
 from ..service.queue.queue_stash import QueueStash
 from ..service.queue.zmq_queue import QueueConfig
@@ -163,15 +165,15 @@
         signing_key: Optional[Union[SyftSigningKey, SigningKey]] = None,
         action_store_config: Optional[StoreConfig] = None,
         document_store_config: Optional[StoreConfig] = None,
         root_email: str = default_root_email,
         root_password: str = default_root_password,
         processes: int = 0,
         is_subprocess: bool = False,
-        node_type: NodeType = NodeType.DOMAIN,
+        node_type: Union[str, NodeType] = NodeType.DOMAIN,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
         queue_config: QueueConfig = ZMQQueueConfig,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         if node_uid_env is not None:
@@ -202,17 +204,18 @@
                 ActionService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
-                MessageService,
+                NotificationService,
                 DataSubjectMemberService,
                 ProjectService,
+                EnclaveService,
             ]
             if services is None
             else services
         )
 
         self.service_config = ServiceConfigRegistry.get_registered_configs()
         self.local_db = local_db
@@ -236,21 +239,25 @@
             name="Jane Doe",
             email=root_email,
             password=root_password,
             node=self,
         )
 
         self.client_cache = {}
+        if isinstance(node_type, str):
+            node_type = NodeType(node_type)
         self.node_type = node_type
 
         self.post_init()
         self.create_initial_settings()
         if not (self.is_subprocess or self.processes == 0):
             self.init_queue_manager(queue_config=queue_config)
 
+        NodeRegistry.set_node_for(self.id, self)
+
     def init_queue_manager(self, queue_config: QueueConfig):
         MessageHandlers = [APICallMessageHandler]
 
         self.queue_manager = QueueManager(queue_config)
         for message_handler in MessageHandlers:
             queue_name = message_handler.queue_name
             producer = self.queue_manager.create_producer(
@@ -260,19 +267,21 @@
                 message_handler, producer.address
             )
             consumer.run()
 
     @classmethod
     def named(
         cls,
+        *,  # Trasterisk
         name: str,
         processes: int = 0,
         reset: bool = False,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
+        node_type: Union[str, NodeType] = NodeType.DOMAIN,
     ) -> Self:
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
         name_hash_uuid = name_hash[0:16]
         name_hash_uuid = bytearray(name_hash_uuid)
         name_hash_uuid[6] = (
             name_hash_uuid[6] & 0x0F
         ) | 0x40  # Set version to 4 (uuid4)
@@ -308,41 +317,48 @@
         return cls(
             name=name,
             id=uid,
             signing_key=key,
             processes=processes,
             local_db=local_db,
             sqlite_path=sqlite_path,
+            node_type=node_type,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.verify_key
 
     @property
     def root_client(self):
         # relative
         from ..client.client import PythonConnection
-        from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
-        return SyftClient(connection=connection, credentials=self.signing_key)
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
+        return client_type(connection=connection, credentials=self.signing_key)
 
     @property
     def guest_client(self):
         return self.get_guest_client()
 
     def get_guest_client(self, verbose: bool = True):
         # relative
         from ..client.client import PythonConnection
-        from ..client.client import SyftClient
 
         connection = PythonConnection(node=self)
         if verbose:
             print(f"Logged into {self.name} as GUEST")
-        return SyftClient(connection=connection, credentials=SyftSigningKey.generate())
+
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
+
+        return client_type(connection=connection, credentials=SyftSigningKey.generate())
 
     def __repr__(self) -> str:
         service_string = ""
         if not self.is_subprocess:
             services = []
             for service in self.services:
                 services.append(service.__name__)
@@ -433,17 +449,18 @@
                 SettingsService,
                 DatasetService,
                 UserCodeService,
                 RequestService,
                 DataSubjectService,
                 NetworkService,
                 PolicyService,
-                MessageService,
+                NotificationService,
                 DataSubjectMemberService,
                 ProjectService,
+                EnclaveService,
             ]
 
             if OBLV:
                 # relative
                 from ..external.oblv.oblv_service import OblvService
 
                 store_services += [OblvService]
@@ -505,14 +522,15 @@
             highest_object_version=HIGHEST_SYFT_OBJECT_VERSION,
             lowest_object_version=LOWEST_SYFT_OBJECT_VERSION,
             syft_version=__version__,
             deployed_on=deployed_on,
             description=description,
             organization=organization,
             on_board=on_board,
+            node_type=self.node_type.value,
             signup_enabled=signup_enabled,
         )
 
     @property
     def icon(self) -> str:
         return "🦾"
 
@@ -558,20 +576,34 @@
             client = self.client_cache[node_uid]
         else:
             network_service = self.get_service(NetworkService)
             peer = network_service.stash.get_by_uid(self.verify_key, node_uid)
 
             if peer.is_ok() and peer.ok():
                 peer = peer.ok()
-                context = NodeServiceContext(node=self)
+                context = AuthedServiceContext(
+                    node=self, credentials=api_call.credentials
+                )
                 client = peer.client_with_context(context=context)
                 self.client_cache[node_uid] = client
-
         if client:
-            return client.connection.make_call(api_call)
+            message: SyftAPICall = api_call.message
+            if message.path == "metadata":
+                result = client.metadata
+            elif message.path == "login":
+                result = client.connection.login(**message.kwargs)
+            elif message.path == "register":
+                result = client.connection.register(**message.kwargs)
+            elif message.path == "api":
+                result = client.connection.get_api(**message.kwargs)
+            else:
+                signed_result = client.connection.make_call(api_call)
+                result = debox_signed_syftapicall_response(signed_result=signed_result)
+
+            return result
 
         return SyftError(message=(f"Node has no route to {node_uid}"))
 
     def get_role_for_credentials(self, credentials: SyftVerifyKey) -> ServiceRole:
         role = self.get_service("userservice").get_role_for_credentials(
             credentials=credentials
         )
@@ -676,14 +708,18 @@
         try:
             settings_stash = SettingsStash(store=self.document_store)
             settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
             if settings_exists:
                 self.name = settings_exists[0].name
                 return None
             else:
+                # Currently we allow automatic user registration on enclaves,
+                # as enclaves do not have superusers
+                if self.node_type == NodeType.ENCLAVE:
+                    flags.CAN_REGISTER = True
                 new_settings = NodeSettings(
                     name=self.name,
                     deployed_on=datetime.now().date().strftime("%m/%d/%Y"),
                     signup_enabled=flags.CAN_REGISTER,
                 )
                 result = settings_stash.set(
                     credentials=self.signing_key.verify_key, settings=new_settings
@@ -829,7 +865,30 @@
             if res.is_ok():
                 print("Successfully generated Oblv Key pair at startup")
             return res.err()
         else:
             print(f"Using Existing Public/Private Key pair: {len(oblv_keys_stash)}")
     except Exception as e:
         print("Unable to create Oblv Keys.", e)
+
+
+class NodeRegistry:
+    __node_registry__: Dict[UID, Node] = {}
+
+    @classmethod
+    def set_node_for(
+        cls,
+        node_uid: Union[UID, str],
+        node: Node,
+    ) -> None:
+        if isinstance(node_uid, str):
+            node_uid = UID.from_string(node_uid)
+
+        cls.__node_registry__[node_uid] = node
+
+    @classmethod
+    def node_for(cls, node_uid: UID) -> Node:
+        return cls.__node_registry__.get(node_uid, None)
+
+    @classmethod
+    def get_all_nodes(cls) -> List[Node]:
+        return list(cls.__node_registry__.values())
```

### Comparing `syft-0.8.2b2/src/syft/node/routes.py` & `syft-0.8.2b3/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/node/run.py` & `syft-0.8.2b3/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/node/server.py` & `syft-0.8.2b3/src/syft/node/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # stdlib
 import asyncio
+from enum import Enum
 import logging
 import multiprocessing
 import os
 import platform
 import signal
 import subprocess  # nosec
 import time
@@ -16,16 +17,20 @@
 from fastapi import FastAPI
 import requests
 from starlette.middleware.cors import CORSMiddleware
 import uvicorn
 
 # relative
 from ..client.client import API_PATH
+from ..util.constants import DEFAULT_TIMEOUT
 from ..util.util import os_name
 from .domain import Domain
+from .enclave import Enclave
+from .gateway import Gateway
+from .node import NodeType
 from .routes import make_routes
 
 if os_name() == "macOS":
     # needed on MacOS to prevent [__NSCFConstantString initialize] may have been in
     # progress in another thread when fork() was called.
     multiprocessing.set_start_method("spawn", True)
 
@@ -49,26 +54,50 @@
         allow_methods=["*"],
         allow_headers=["*"],
     )
 
     return app
 
 
-def run_uvicorn(name: str, host: str, port: int, reset: bool, dev_mode: bool):
+worker_classes = {
+    NodeType.DOMAIN: Domain,
+    NodeType.GATEWAY: Gateway,
+    NodeType.ENCLAVE: Enclave,
+}
+
+
+def run_uvicorn(
+    name: str, node_type: Enum, host: str, port: int, reset: bool, dev_mode: bool
+):
     async def _run_uvicorn(
-        name: str, host: str, port: int, reset: bool, dev_mode: bool
+        name: str, node_type: Enum, host: str, port: int, reset: bool, dev_mode: bool
     ):
+        if node_type not in worker_classes:
+            raise NotImplementedError(f"node_type: {node_type} is not supported")
+        worker_class = worker_classes[node_type]
         if dev_mode:
             print(
                 f"\nWARNING: private key is based on node name: {name} in dev_mode. "
                 "Don't run this in production."
             )
-            worker = Domain.named(name=name, processes=0, local_db=True, reset=reset)
+
+            worker = worker_class.named(
+                name=name,
+                processes=0,
+                reset=reset,
+                local_db=True,
+                node_type=node_type,
+            )
         else:
-            worker = Domain(name=name, processes=0, local_db=True)
+            worker = worker_class(
+                name=name,
+                processes=0,
+                local_db=True,
+                node_type=node_type,
+            )
         router = make_routes(worker=worker)
         app = make_app(worker.name, router=router)
 
         if reset:
             try:
                 python_pids = find_python_processes_on_port(port)
                 for pid in python_pids:
@@ -89,28 +118,29 @@
         server = uvicorn.Server(config)
 
         await server.serve()
         asyncio.get_running_loop().stop()
 
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
-    loop.run_until_complete(_run_uvicorn(name, host, port, reset, dev_mode))
+    loop.run_until_complete(_run_uvicorn(name, node_type, host, port, reset, dev_mode))
     loop.close()
 
 
 def serve_node(
     name: str,
+    node_type: NodeType = NodeType.DOMAIN,
     host: str = "0.0.0.0",  # nosec
     port: int = 8080,
     reset: bool = False,
     dev_mode: bool = False,
     tail: bool = False,
 ) -> Tuple[Callable, Callable]:
     server_process = multiprocessing.Process(
-        target=run_uvicorn, args=(name, host, port, reset, dev_mode)
+        target=run_uvicorn, args=(name, node_type, host, port, reset, dev_mode)
     )
 
     def stop():
         print(f"Stopping {name}")
         server_process.terminate()
         server_process.join()
 
@@ -127,15 +157,16 @@
                     stop()
                 except SystemExit:
                     os._exit(130)
         else:
             for i in range(WAIT_TIME_SECONDS):
                 try:
                     req = requests.get(
-                        f"http://{host}:{port}{API_PATH}/metadata", timeout=0.5
+                        f"http://{host}:{port}{API_PATH}/metadata",
+                        timeout=DEFAULT_TIMEOUT,
                     )
                     if req.status_code == 200:
                         print(" Done.")
                         break
                 except Exception:
                     time.sleep(1)
                     if i == 0:
```

### Comparing `syft-0.8.2b2/src/syft/node/worker_settings.py` & `syft-0.8.2b3/src/syft/node/worker_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ..abstract_node import AbstractNode
+from ..abstract_node import NodeType
 from ..node.credentials import SyftSigningKey
 from ..serde.serializable import serializable
 from ..store.document_store import StoreConfig
 from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 
@@ -17,20 +18,22 @@
 @serializable()
 class WorkerSettings(SyftObject):
     __canonical_name__ = "WorkerSettings"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
     name: str
+    node_type: NodeType
     signing_key: SyftSigningKey
     document_store_config: StoreConfig
     action_store_config: StoreConfig
 
     @staticmethod
     def from_node(node: AbstractNode) -> Self:
         return WorkerSettings(
             id=node.id,
             name=node.name,
+            node_type=node.node_type,
             signing_key=node.signing_key,
             document_store_config=node.document_store_config,
             action_store_config=node.action_store_config,
         )
```

### Comparing `syft-0.8.2b2/src/syft/serde/array.py` & `syft-0.8.2b3/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/arrow.py` & `syft-0.8.2b3/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/deserialize.py` & `syft-0.8.2b3/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/lib_permissions.py` & `syft-0.8.2b3/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/lib_service_registry.py` & `syft-0.8.2b3/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/mock.py` & `syft-0.8.2b3/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/recursive.py` & `syft-0.8.2b3/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/recursive_primitives.py` & `syft-0.8.2b3/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/serializable.py` & `syft-0.8.2b3/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/signature.py` & `syft-0.8.2b3/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/serde/third_party.py` & `syft-0.8.2b3/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_data_empty.py` & `syft-0.8.2b3/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_graph.py` & `syft-0.8.2b3/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_graph_service.py` & `syft-0.8.2b3/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_object.py` & `syft-0.8.2b3/src/syft/service/action/action_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     "__version__",  # syft
     "__args__",  # pydantic
     "to_pointer",  # syft
     "to",  # syft
     "send",  # syft
     "_copy_and_set_values",  # pydantic
     "get_from",  # syft
+    "get",  # syft
     "delete_data",  # syft
 ]
 dont_wrap_output_attrs = [
     "__repr__",
     "__str__",
     "_repr_html_",
     "_repr_markdown_",
```

### Comparing `syft-0.8.2b2/src/syft/service/action/action_permissions.py` & `syft-0.8.2b3/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_service.py` & `syft-0.8.2b3/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_store.py` & `syft-0.8.2b3/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/action_types.py` & `syft-0.8.2b3/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/numpy.py` & `syft-0.8.2b3/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/pandas.py` & `syft-0.8.2b3/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/action/plan.py` & `syft-0.8.2b3/src/syft/service/action/plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         else:
             return self.outputs
 
 
 def planify(func):
     TraceResult.reset()
     ActionObject.add_trace_hook()
-    worker = Worker.named("plan_building", reset=True, processes=0)
+    worker = Worker.named(name="plan_building", reset=True, processes=0)
     client = worker.root_client
     TraceResult._client = client
     plan_kwargs = build_plan_inputs(func, client)
     outputs = func(**plan_kwargs)
     if not (isinstance(outputs, list) or isinstance(outputs, tuple)):
         outputs = [outputs]
     ActionObject.remove_trace_hook()
```

### Comparing `syft-0.8.2b2/src/syft/service/action/verification.py` & `syft-0.8.2b3/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/code/user_code.py` & `syft-0.8.2b3/src/syft/service/code/user_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,20 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 # third party
-from result import Err
-from result import Ok
-from result import Result
+from typing_extensions import Self
 
 # relative
 from ...abstract_node import NodeType
 from ...client.api import NodeView
+from ...client.enclave_client import EnclaveMetadata
 from ...node.credentials import SyftVerifyKey
 from ...serde.deserialize import _deserialize
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.document_store import PartitionKey
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftHashableObject
@@ -38,15 +37,14 @@
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
 from ...util.markdown import CodeMarkdown
 from ...util.markdown import as_markdown_code
 from ..context import AuthedServiceContext
 from ..dataset.dataset import Asset
-from ..metadata.node_metadata import EnclaveMetadata
 from ..policy.policy import CustomInputPolicy
 from ..policy.policy import CustomOutputPolicy
 from ..policy.policy import ExactMatch
 from ..policy.policy import InputPolicy
 from ..policy.policy import OutputPolicy
 from ..policy.policy import Policy
 from ..policy.policy import SingleExecutionExactOutput
@@ -133,39 +131,42 @@
                 return UserCodeStatus.DENIED
             else:
                 return Exception(f"Invalid types in {keys} for Code Submission")
 
         elif context.node.node_type == NodeType.DOMAIN:
             node_view = NodeView(
                 node_name=context.node.name,
+                node_id=context.node.id,
                 verify_key=context.node.signing_key.verify_key,
             )
             if node_view in self.base_dict:
                 return self.base_dict[node_view]
             else:
                 raise Exception(
                     f"Code Object does not contain {context.node.name} Domain's data"
                 )
         else:
             raise Exception(
                 f"Invalid Node Type for Code Submission:{context.node.node_type}"
             )
 
     def mutate(
-        self, value: UserCodeStatus, node_name: str, verify_key: SyftVerifyKey
-    ) -> Result[Ok, Err]:
-        node_view = NodeView(node_name=node_name, verify_key=verify_key)
+        self, value: UserCodeStatus, node_name: str, node_id, verify_key: SyftVerifyKey
+    ) -> Union[SyftError, Self]:
+        node_view = NodeView(
+            node_name=node_name, node_id=node_id, verify_key=verify_key
+        )
         base_dict = self.base_dict
         if node_view in base_dict:
             base_dict[node_view] = value
             self.base_dict = base_dict
-            return Ok(self)
+            return self
         else:
-            return Err(
-                "Cannot Modify Status as the Domain's data is not included in the request"
+            return SyftError(
+                message="Cannot Modify Status as the Domain's data is not included in the request"
             )
 
 
 @serializable()
 class UserCode(SyftObject):
     # version
     __canonical_name__ = "UserCode"
@@ -634,28 +635,31 @@
     return context
 
 
 def add_custom_status(context: TransformContext) -> TransformContext:
     input_keys = list(context.output["input_policy_init_kwargs"].keys())
     if context.node.node_type == NodeType.DOMAIN:
         node_view = NodeView(
-            node_name=context.node.name, verify_key=context.node.signing_key.verify_key
+            node_name=context.node.name,
+            node_id=context.node.id,
+            verify_key=context.node.signing_key.verify_key,
         )
         if node_view in input_keys or len(input_keys) == 0:
             context.output["status"] = UserCodeStatusContext(
                 base_dict={node_view: UserCodeStatus.SUBMITTED}
             )
         else:
-            raise NotImplementedError
+            raise ValueError(f"Invalid input keys: {input_keys} for {node_view}")
     elif context.node.node_type == NodeType.ENCLAVE:
         base_dict = {key: UserCodeStatus.SUBMITTED for key in input_keys}
         context.output["status"] = UserCodeStatusContext(base_dict=base_dict)
     else:
-        # Consult with Madhava, on propogating errors from transforms
-        raise NotImplementedError
+        raise NotImplementedError(
+            f"Invalid node type:{context.node.node_type} for code submission"
+        )
     return context
 
 
 @transform(SubmitUserCode, UserCode)
 def submit_user_code_to_user_code() -> List[Callable]:
     return [
         generate_id,
```

### Comparing `syft-0.8.2b2/src/syft/service/code/user_code_parse.py` & `syft-0.8.2b3/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/code/user_code_service.py` & `syft-0.8.2b3/src/syft/service/code/user_code_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     ) -> Union[UserCode, SyftError]:
         """Add User Code"""
         result = self.stash.set(context.credentials, code.to(UserCode, context=context))
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="User Code Submitted")
 
-    def _code_execution(
+    def _request_code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
         reason: Optional[str] = "",
     ):
         user_code = code.to(UserCode, context=context)
         result = self.stash.set(context.credentials, user_code)
@@ -90,15 +90,15 @@
     def request_code_execution(
         self,
         context: AuthedServiceContext,
         code: SubmitUserCode,
         reason: Optional[str] = "",
     ) -> Union[SyftSuccess, SyftError]:
         """Request Code execution on user code"""
-        return self._code_execution(context=context, code=code, reason=reason)
+        return self._request_code_execution(context=context, code=code, reason=reason)
 
     @service_method(path="code.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(
         self, context: AuthedServiceContext
     ) -> Union[List[UserCode], SyftError]:
         """Get a Dataset"""
         result = self.stash.get_all(context.credentials)
```

### Comparing `syft-0.8.2b2/src/syft/service/code/user_code_stash.py` & `syft-0.8.2b3/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/context.py` & `syft-0.8.2b3/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/data_subject/data_subject.py` & `syft-0.8.2b3/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.2b3/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.2b3/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.2b3/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/dataset/dataset.py` & `syft-0.8.2b3/src/syft/service/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,14 +505,24 @@
                     _ASSET_WITH_NONE_MOCK_ERROR_MESSAGE,
                 ]
             )
         )
 
 
 @serializable()
+class DatasetPageView(SyftObject):
+    # version
+    __canonical_name__ = "DatasetPageView"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    datasets: List[Dataset]
+    total: int
+
+
+@serializable()
 class CreateDataset(Dataset):
     # version
     __canonical_name__ = "CreateDataset"
     __version__ = SYFT_OBJECT_VERSION_1
     asset_list: List[CreateAsset] = []
 
     __repr_attrs__ = ["name", "url"]
```

### Comparing `syft-0.8.2b2/src/syft/service/dataset/dataset_service.py` & `syft-0.8.2b3/src/syft/service/dataset/dataset_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ..service import service_method
 from ..user.user_roles import DATA_OWNER_ROLE_LEVEL
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .dataset import Asset
 from .dataset import CreateDataset
 from .dataset import Dataset
+from .dataset import DatasetPageView
 from .dataset_stash import DatasetStash
 
 
 @instrument
 @serializable()
 class DatasetService(AbstractService):
     store: DocumentStore
@@ -60,32 +61,34 @@
 
     @service_method(path="dataset.get_all", name="get_all", roles=GUEST_ROLE_LEVEL)
     def get_all(
         self,
         context: AuthedServiceContext,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
-    ) -> Union[List[Dataset], SyftError]:
+    ) -> Union[DatasetPageView, List[Dataset], SyftError]:
         """Get a Dataset"""
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             datasets = result.ok()
             results = []
             for dataset in datasets:
                 dataset.node_uid = context.node.id
                 results.append(dataset)
 
             # If chunk size is defined, then split list into evenly sized chunks
             if page_size:
+                total = len(results)
                 results = [
                     results[i : i + page_size]
                     for i in range(0, len(results), page_size)
                 ]
                 # Return the proper slice using chunk_index
                 results = results[page_index]
+                results = DatasetPageView(datasets=results, total=total)
 
             return results
         return SyftError(message=result.err())
 
     @service_method(path="dataset.search", name="search")
     def search(
         self,
@@ -99,20 +102,22 @@
 
         if not isinstance(results, SyftError):
             results = [dataset for dataset in results if name in dataset.name]
 
             # If chunk size is defined, then split list into evenly sized chunks
 
             if page_size:
+                total = len(results)
                 results = [
                     results[i : i + page_size]
                     for i in range(0, len(results), page_size)
                 ]
                 # Return the proper slice using chunk_index
                 results = results[page_index]
+                results = DatasetPageView(datasets=results, total=total)
 
         return results
 
     @service_method(path="dataset.get_by_id", name="get_by_id")
     def get_by_id(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
```

### Comparing `syft-0.8.2b2/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.2b3/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/message/message_service.py` & `syft-0.8.2b3/src/syft/service/notification/notification_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,202 +13,213 @@
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
-from .message_stash import MessageStash
-from .messages import CreateMessage
-from .messages import LinkedObject
-from .messages import Message
-from .messages import MessageStatus
-from .messages import ReplyMessage
+from .notification_stash import NotificationStash
+from .notifications import CreateNotification
+from .notifications import LinkedObject
+from .notifications import Notification
+from .notifications import NotificationStatus
+from .notifications import ReplyNotification
 
 
 @instrument
 @serializable()
-class MessageService(AbstractService):
+class NotificationService(AbstractService):
     store: DocumentStore
-    stash: MessageStash
+    stash: NotificationStash
 
     def __init__(self, store: DocumentStore) -> None:
         self.store = store
-        self.stash = MessageStash(store=store)
+        self.stash = NotificationStash(store=store)
 
-    @service_method(path="messages.send", name="send")
+    @service_method(path="notifications.send", name="send")
     def send(
-        self, context: AuthedServiceContext, message: CreateMessage
-    ) -> Union[Message, SyftError]:
-        """Send a new message"""
+        self, context: AuthedServiceContext, notification: CreateNotification
+    ) -> Union[Notification, SyftError]:
+        """Send a new notification"""
 
-        new_message = message.to(Message, context=context)
+        new_notification = notification.to(Notification, context=context)
 
         # Add read permissions to person receiving this message
         permissions = [
             ActionObjectREAD(
-                uid=new_message.id, credentials=new_message.to_user_verify_key
+                uid=new_notification.id, credentials=new_notification.to_user_verify_key
             )
         ]
 
         result = self.stash.set(
-            context.credentials, new_message, add_permissions=permissions
+            context.credentials, new_notification, add_permissions=permissions
         )
+
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
-    @service_method(path="messages.reply", name="reply", roles=GUEST_ROLE_LEVEL)
+    @service_method(path="notifications.reply", name="reply", roles=GUEST_ROLE_LEVEL)
     def reply(
         self,
         context: AuthedServiceContext,
-        reply: ReplyMessage,
-    ) -> Union[ReplyMessage, SyftError]:
+        reply: ReplyNotification,
+    ) -> Union[ReplyNotification, SyftError]:
         msg = self.stash.get_by_uid(
             credentials=context.credentials, uid=reply.target_msg
         )
         if msg.is_ok():
             msg = msg.ok()
             reply.from_user_verify_key = context.credentials
             msg.replies.append(reply)
             result = self.stash.update(credentials=context.credentials, obj=msg)
             if result.is_ok():
                 return result.ok()
             else:
                 SyftError(
-                    message="Couldn't add a new message reply in the target message."
+                    message="Couldn't add a new notification reply in the target notification."
                 )
         else:
-            SyftError(message="The target message id {reply.target_msg} was not found!")
+            SyftError(
+                message="The target notification id {reply.target_msg} was not found!"
+            )
 
     @service_method(
-        path="messages.get_all",
+        path="notifications.get_all",
         name="get_all",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
-    def get_all(self, context: AuthedServiceContext) -> Union[List[Message], SyftError]:
+    def get_all(
+        self,
+        context: AuthedServiceContext,
+    ) -> Union[List[Notification], SyftError]:
         result = self.stash.get_all_inbox_for_verify_key(
-            credentials=context.credentials,
+            context.credentials,
             verify_key=context.credentials,
         )
         if result.err():
             return SyftError(message=str(result.err()))
-        messages = result.ok()
-        return messages
+        notifications = result.ok()
+        return notifications
 
     @service_method(
-        path="messages.get_all_sent", name="outbox", roles=DATA_SCIENTIST_ROLE_LEVEL
+        path="notifications.get_all_sent",
+        name="outbox",
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def get_all_sent(
         self, context: AuthedServiceContext
-    ) -> Union[List[Message], SyftError]:
+    ) -> Union[List[Notification], SyftError]:
         result = self.stash.get_all_sent_for_verify_key(
             context.credentials, context.credentials
         )
         if result.err():
             return SyftError(message=str(result.err()))
-        messages = result.ok()
-        return messages
+        notifications = result.ok()
+        return notifications
 
     # get_all_read and unread cover the same functionality currently as
     # get_all_for_status. However, there may be more statuses added in the future,
     # so we are keeping the more generic get_all_for_status method.
     def get_all_for_status(
         self,
         context: AuthedServiceContext,
-        status: MessageStatus,
-    ) -> Union[List[Message], SyftError]:
+        status: NotificationStatus,
+    ) -> Union[List[Notification], SyftError]:
         result = self.stash.get_all_by_verify_key_for_status(
             context.credentials, verify_key=context.credentials, status=status
         )
         if result.err():
             return SyftError(message=str(result.err()))
-        messages = result.ok()
-        return messages
+        notifications = result.ok()
+        return notifications
 
     @service_method(
-        path="messages.get_all_read",
+        path="notifications.get_all_read",
         name="get_all_read",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def get_all_read(
         self,
         context: AuthedServiceContext,
-    ) -> Union[List[Message], SyftError]:
+    ) -> Union[List[Notification], SyftError]:
         return self.get_all_for_status(
             context=context,
-            status=MessageStatus.READ,
+            status=NotificationStatus.READ,
         )
 
     @service_method(
-        path="messages.get_all_unread",
+        path="notifications.get_all_unread",
         name="get_all_unread",
         roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def get_all_unread(
         self,
         context: AuthedServiceContext,
-    ) -> Union[List[Message], SyftError]:
+    ) -> Union[List[Notification], SyftError]:
         return self.get_all_for_status(
             context=context,
-            status=MessageStatus.UNREAD,
+            status=NotificationStatus.UNREAD,
         )
 
-    @service_method(path="messages.mark_as_read", name="mark_as_read")
+    @service_method(path="notifications.mark_as_read", name="mark_as_read")
     def mark_as_read(
         self, context: AuthedServiceContext, uid: UID
-    ) -> Union[Message, SyftError]:
-        result = self.stash.update_message_status(
-            context.credentials, uid=uid, status=MessageStatus.READ
+    ) -> Union[Notification, SyftError]:
+        result = self.stash.update_notification_status(
+            context.credentials, uid=uid, status=NotificationStatus.READ
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
-    @service_method(path="messages.mark_as_unread", name="mark_as_unread")
+    @service_method(path="notifications.mark_as_unread", name="mark_as_unread")
     def mark_as_unread(
         self, context: AuthedServiceContext, uid: UID
-    ) -> Union[Message, SyftError]:
-        result = self.stash.update_message_status(
-            context.credentials, uid=uid, status=MessageStatus.UNREAD
+    ) -> Union[Notification, SyftError]:
+        result = self.stash.update_notification_status(
+            context.credentials, uid=uid, status=NotificationStatus.UNREAD
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(
-        path="messages.resolve_object",
+        path="notifications.resolve_object",
         name="resolve_object",
-        roles=GUEST_ROLE_LEVEL,
+        roles=DATA_SCIENTIST_ROLE_LEVEL,
     )
     def resolve_object(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
-    ) -> Union[Message, SyftError]:
+    ) -> Union[Notification, SyftError]:
         service = context.node.get_service(linked_obj.service_type)
         result = service.resolve_link(context=context, linked_obj=linked_obj)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
-    @service_method(path="messages.clear", name="clear")
+    @service_method(path="notifications.clear", name="clear")
     def clear(self, context: AuthedServiceContext) -> Union[SyftError, SyftSuccess]:
         result = self.stash.delete_all_for_verify_key(
             credentials=context.credentials, verify_key=context.credentials
         )
         if result.is_ok():
-            return SyftSuccess(message="All messages cleared !!")
+            return SyftSuccess(message="All notifications cleared !!")
         return SyftError(message=str(result.err()))
 
     def filter_by_obj(
         self, context: AuthedServiceContext, obj_uid: UID
-    ) -> Union[Message, SyftError]:
-        messages = self.stash.get_all(context.credentials)
-        if messages.is_ok():
-            for message in messages.ok():
-                if message.linked_obj and message.linked_obj.object_uid == obj_uid:
-                    return message
+    ) -> Union[Notification, SyftError]:
+        notifications = self.stash.get_all(context.credentials)
+        if notifications.is_ok():
+            for notification in notifications.ok():
+                if (
+                    notification.linked_obj
+                    and notification.linked_obj.object_uid == obj_uid
+                ):
+                    return notification
         else:
-            return SyftError(message="Could not get messages!!")
+            return SyftError(message="Could not get notifications!!")
 
 
-TYPE_TO_SERVICE[Message] = MessageService
-SERVICE_TO_TYPES[MessageService].update({Message})
+TYPE_TO_SERVICE[Notification] = NotificationService
+SERVICE_TO_TYPES[NotificationService].update({Notification})
```

### Comparing `syft-0.8.2b2/src/syft/service/message/messages.py` & `syft-0.8.2b3/src/syft/service/notification/notifications.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,48 +16,48 @@
 from ...types.transforms import add_node_uid_for_key
 from ...types.transforms import generate_id
 from ...types.transforms import transform
 from ...types.uid import UID
 
 
 @serializable()
-class MessageStatus(Enum):
+class NotificationStatus(Enum):
     UNREAD = 0
     READ = 1
 
 
-class MessageExpiryStatus(Enum):
+class NotificationExpiryStatus(Enum):
     AUTO = 0
     NEVER = 1
 
 
 @serializable()
-class ReplyMessage(SyftObject):
-    __canonical_name__ = "ReplyMessage"
+class ReplyNotification(SyftObject):
+    __canonical_name__ = "ReplyNotification"
     __version__ = SYFT_OBJECT_VERSION_1
 
     text: str
     target_msg: UID
     id: Optional[UID]
     from_user_verify_key: Optional[SyftVerifyKey]
 
 
 @serializable()
-class Message(SyftObject):
-    __canonical_name__ = "Message"
+class Notification(SyftObject):
+    __canonical_name__ = "Notification"
     __version__ = SYFT_OBJECT_VERSION_1
 
     subject: str
     node_uid: UID
     from_user_verify_key: SyftVerifyKey
     to_user_verify_key: SyftVerifyKey
     created_at: DateTime
-    status: MessageStatus = MessageStatus.UNREAD
+    status: NotificationStatus = NotificationStatus.UNREAD
     linked_obj: Optional[LinkedObject]
-    replies: Optional[List[ReplyMessage]] = []
+    replies: Optional[List[ReplyNotification]] = []
 
     __attr_searchable__ = [
         "from_user_verify_key",
         "to_user_verify_key",
         "status",
     ]
     __repr_attrs__ = ["subject", "status", "created_at", "linked_obj"]
@@ -73,42 +73,43 @@
             "Subject": self.subject,
             "Status": self.status.name.capitalize(),
             "Created At": str(self.created_at),
             "Linked object": f"{self.linked_obj.object_type.__canonical_name__} ({self.linked_obj.object_uid})",
         }
 
     def mark_read(self) -> None:
-        api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
-        return api.services.messages.mark_as_read(uid=self.id)
+        api = APIRegistry.api_for(
+            self.node_uid, user_verify_key=self.syft_client_verify_key
+        )
+        return api.services.notifications.mark_as_read(uid=self.id)
 
     def mark_unread(self) -> None:
         api = APIRegistry.api_for(
-            self.node_uid,
-            self.syft_client_verify_key,
+            self.node_uid, user_verify_key=self.syft_client_verify_key
         )
-        return api.services.messages.mark_as_unread(uid=self.id)
+        return api.services.notifications.mark_as_unread(uid=self.id)
 
 
 @serializable()
-class CreateMessage(Message):
-    __canonical_name__ = "CreateMessage"
+class CreateNotification(Notification):
+    __canonical_name__ = "CreateNotification"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
     node_uid: Optional[UID]
     from_user_verify_key: Optional[SyftVerifyKey]
     created_at: Optional[DateTime]
 
 
 def add_msg_creation_time(context: TransformContext) -> TransformContext:
     context.output["created_at"] = DateTime.now()
     return context
 
 
-@transform(CreateMessage, Message)
-def createmessage_to_message():
+@transform(CreateNotification, Notification)
+def createnotification_to_notification():
     return [
         generate_id,
         add_msg_creation_time,
         add_credentials_for_key("from_user_verify_key"),
         add_node_uid_for_key("node_uid"),
     ]
```

### Comparing `syft-0.8.2b2/src/syft/service/metadata/node_metadata.py` & `syft-0.8.2b3/src/syft/service/metadata/node_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     name: str
     id: UID
     verify_key: SyftVerifyKey
     highest_object_version: int
     lowest_object_version: int
     syft_version: str
-    node_type: str = "Domain"
+    node_type: str = "domain"
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "Text"
     signup_enabled: bool
 
     def check_version(self, client_version: str) -> None:
@@ -88,15 +88,15 @@
     metadata_version: int
     name: str
     id: str
     verify_key: str
     highest_object_version: int
     lowest_object_version: int
     syft_version: str
-    node_type: str = "Domain"
+    node_type: str = "domain"
     deployed_on: str = "Date"
     organization: str = "OpenMined"
     on_board: bool = False
     description: str = "My cool domain"
     signup_enabled: bool
 
     def check_version(self, client_version: str) -> bool:
@@ -118,13 +118,7 @@
 
 @transform(NodeMetadataJSON, NodeMetadata)
 def json_to_metadata() -> List[Callable]:
     return [
         drop(["metadata_version"]),
         convert_types(["id", "verify_key"], [UID, SyftVerifyKey]),
     ]
-
-
-class EnclaveMetadata:
-    """Contains metadata to connect to a specific Enclave"""
-
-    pass
```

### Comparing `syft-0.8.2b2/src/syft/service/network/network_service.py` & `syft-0.8.2b3/src/syft/service/network/network_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,20 +263,22 @@
             )
         peer.update_routes([route])
         result = self.stash.update_peer(context.node.verify_key, peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Network Route Verified")
 
-    @service_method(path="network.get_all_peers", name="get_all_peers")
+    @service_method(
+        path="network.get_all_peers", name="get_all_peers", roles=GUEST_ROLE_LEVEL
+    )
     def get_all_peers(
         self, context: AuthedServiceContext
     ) -> Union[List[NodePeer], SyftError]:
         """Get all Peers"""
-        result = self.stash.get_all(context.credentials)
+        result = self.stash.get_all(credentials=context.node.verify_key)
         if result.is_ok():
             peers = result.ok()
             return peers
         return SyftError(message=result.err())
 
     @service_method(path="network.join_vpn", name="join_vpn")
     def join_vpn(
@@ -441,48 +443,50 @@
 
 def from_grid_url(context: TransformContext) -> TransformContext:
     url = context.obj.url.as_container_host()
     context.output["host_or_ip"] = url.host_or_ip
     context.output["protocol"] = url.protocol
     context.output["port"] = url.port
     context.output["private"] = False
+    context.output["proxy_target_uid"] = context.obj.proxy_target_uid
     return context
 
 
 @transform(HTTPConnection, HTTPNodeRoute)
 def http_connection_to_node_route() -> List[Callable]:
     return [from_grid_url]
 
 
 def get_python_node_route(context: TransformContext) -> TransformContext:
     context.output["id"] = context.obj.node.id
     context.output["worker_settings"] = WorkerSettings.from_node(context.obj.node)
+    context.output["proxy_target_uid"] = context.obj.proxy_target_uid
     return context
 
 
 @transform(PythonConnection, PythonNodeRoute)
 def python_connection_to_node_route() -> List[Callable]:
     return [get_python_node_route]
 
 
 @transform_method(PythonNodeRoute, PythonConnection)
 def node_route_to_python_connection(
     obj: Any, context: Optional[TransformContext] = None
 ) -> List[Callable]:
-    return PythonConnection(node=obj.node)
+    return PythonConnection(node=obj.node, proxy_target_uid=obj.proxy_target_uid)
 
 
 @transform_method(HTTPNodeRoute, HTTPConnection)
 def node_route_to_http_connection(
     obj: Any, context: Optional[TransformContext] = None
 ) -> List[Callable]:
     url = GridURL(
         protocol=obj.protocol, host_or_ip=obj.host_or_ip, port=obj.port
     ).as_container_host()
-    return HTTPConnection(url=url)
+    return HTTPConnection(url=url, proxy_target_uid=obj.proxy_target_uid)
 
 
 @transform(NodeMetadata, NodePeer)
 def metadata_to_peer() -> List[Callable]:
     return [
         keep(["id", "name", "verify_key"]),
     ]
```

### Comparing `syft-0.8.2b2/src/syft/service/network/node_peer.py` & `syft-0.8.2b3/src/syft/service/network/node_peer.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 from typing_extensions import Self
 
 # relative
 from ...client.client import SyftClient
 from ...node.credentials import SyftSigningKey
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
+from ...service.response import SyftError
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.uid import UID
 from ..context import NodeServiceContext
 from ..metadata.node_metadata import NodeMetadata
 from .routes import NodeRoute
+from .routes import NodeRouteType
 from .routes import connection_to_route
 from .routes import route_to_connection
 
 
 @serializable()
 class NodePeer(SyftObject):
     # version
@@ -27,15 +29,15 @@
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
     name: str
     verify_key: SyftVerifyKey
     is_vpn: bool = False
     vpn_auth_key: Optional[str] = None
-    node_routes: List[NodeRoute] = []
+    node_routes: List[NodeRouteType] = []
 
     __attr_searchable__ = ["name"]
     __attr_unique__ = ["verify_key"]
     __repr_attrs__ = ["name"]
 
     def update_routes(self, new_routes: List[NodeRoute]) -> None:
         add_routes = []
@@ -56,22 +58,30 @@
         return peer
 
     def client_with_context(self, context: NodeServiceContext) -> SyftClient:
         if len(self.node_routes) < 1:
             raise Exception(f"No routes to peer: {self}")
         route = self.node_routes[0]
         connection = route_to_connection(route=route)
-        return SyftClient(connection=connection, credentials=context.node.signing_key)
+
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
+        return client_type(connection=connection, credentials=context.node.signing_key)
 
     def client_with_key(self, credentials: SyftSigningKey) -> SyftClient:
         if len(self.node_routes) < 1:
             raise Exception(f"No routes to peer: {self}")
         route = self.node_routes[0]
         connection = route_to_connection(route=route)
-        return SyftClient(connection=connection, credentials=credentials)
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
+
+        return client_type(connection=connection, credentials=credentials)
 
     @property
     def guest_client(self) -> SyftClient:
         guest_key = SyftSigningKey.generate()
         return self.client_with_key(credentials=guest_key)
 
     def proxy_from(self, client: SyftClient) -> SyftClient:
```

### Comparing `syft-0.8.2b2/src/syft/service/network/routes.py` & `syft-0.8.2b3/src/syft/service/network/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 # stdlib
 import secrets
 from typing import Any
 from typing import Optional
 from typing import TYPE_CHECKING
+from typing import Union
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ...abstract_node import AbstractNode
 from ...client.client import HTTPConnection
@@ -17,27 +18,31 @@
 from ...client.client import PythonConnection
 from ...client.client import SyftClient
 from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
 from ...types.transforms import TransformContext
+from ...types.uid import UID
 from ..context import AuthedServiceContext
 from ..context import NodeServiceContext
 from ..response import SyftError
 
 if TYPE_CHECKING:
     # relative
     from .node_peer import NodePeer
 
 
 class NodeRoute:
     def client_with_context(self, context: NodeServiceContext) -> SyftClient:
         connection = route_to_connection(route=self, context=context)
-        return SyftClient(connection=connection, credentials=context.node.signing_key)
+        client_type = connection.get_client_type()
+        if isinstance(client_type, SyftError):
+            return client_type
+        return client_type(connection=connection, credentials=context.node.signing_key)
 
     def validate_with_context(self, context: AuthedServiceContext) -> NodePeer:
         # relative
         from .node_peer import NodePeer
 
         # Step 1: Check if the given route is able to reach the given node
         # As we allow the user to give custom routes, we need to check the reachability of the route
@@ -70,36 +75,39 @@
     __canonical_name__ = "HTTPNodeRoute"
     __version__ = SYFT_OBJECT_VERSION_1
 
     host_or_ip: str
     private: bool = False
     protocol: str = "http"
     port: int = 80
+    proxy_target_uid: Optional[UID] = None
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, HTTPNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
 
 @serializable()
 class PythonNodeRoute(SyftObject, NodeRoute):
     __canonical_name__ = "PythonNodeRoute"
     __version__ = SYFT_OBJECT_VERSION_1
 
     worker_settings: WorkerSettings
+    proxy_target_uid: Optional[UID] = None
 
     @property
     def node(self) -> Optional[AbstractNode]:
         # relative
         from ...node.worker import Worker
 
         node = Worker(
             id=self.worker_settings.id,
             name=self.worker_settings.name,
+            node_type=self.worker_settings.node_type,
             signing_key=self.worker_settings.signing_key,
             document_store_config=self.worker_settings.document_store_config,
             action_store_config=self.worker_settings.action_store_config,
             processes=1,
         )
         return node
 
@@ -110,14 +118,17 @@
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, PythonNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
 
+NodeRouteType = Union[HTTPNodeRoute, PythonNodeRoute]
+
+
 def route_to_connection(
     route: NodeRoute, context: Optional[TransformContext] = None
 ) -> NodeConnection:
     if isinstance(route, HTTPNodeRoute):
         return route.to(HTTPConnection, context=context)
     else:
         return route.to(PythonConnection, context=context)
```

### Comparing `syft-0.8.2b2/src/syft/service/policy/policy.py` & `syft-0.8.2b3/src/syft/service/policy/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from ...types.twin_object import TwinObject
 from ...types.uid import UID
 from ...util.util import is_interpreter_jupyter
 from ..action.action_object import ActionObject
 from ..code.code_parse import GlobalsVisitor
 from ..code.unparse import unparse
 from ..context import AuthedServiceContext
+from ..context import ChangeContext
 from ..context import NodeServiceContext
 from ..dataset.dataset import Asset
 from ..response import SyftError
 from ..response import SyftSuccess
 
 PolicyUserVerifyKeyPartitionKey = PartitionKey(
     key="user_verify_key", type_=SyftVerifyKey
@@ -185,14 +186,28 @@
     ) -> Dict[Any, Any]:
         raise NotImplementedError
 
     @property
     def inputs(self) -> Dict[NodeView, Any]:
         return self.init_kwargs
 
+    def _inputs_for_context(self, context: ChangeContext):
+        user_node_view = NodeView.from_change_context(context)
+        inputs = self.inputs[user_node_view]
+
+        action_service = context.node.get_service("actionservice")
+        for var_name, uid in inputs.items():
+            action_object = action_service.store.get(
+                uid=uid, credentials=user_node_view.verify_key
+            )
+            if action_object.is_err():
+                return SyftError(message=action_object.err())
+            inputs[var_name] = action_object.ok()
+        return inputs
+
 
 def retrieve_from_db(
     code_item_id: UID, allowed_inputs: Dict[str, UID], context: AuthedServiceContext
 ) -> Dict:
     # relative
     from ...service.action.action_object import TwinMode
 
@@ -209,22 +224,22 @@
     )
     if context.node.node_type == NodeType.DOMAIN:
         for var_name, arg_id in allowed_inputs.items():
             kwarg_value = action_service.get(
                 context=root_context, uid=arg_id, twin_mode=TwinMode.NONE
             )
             if kwarg_value.is_err():
-                return kwarg_value
+                return SyftError(message=kwarg_value.err())
             code_inputs[var_name] = kwarg_value.ok()
 
     elif context.node.node_type == NodeType.ENCLAVE:
         dict_object = action_service.get(context=root_context, uid=code_item_id)
         if dict_object.is_err():
-            return dict_object
-        for value in dict_object.ok().base_dict.values():
+            return SyftError(message=dict_object.err())
+        for value in dict_object.ok().syft_action_data.values():
             code_inputs.update(value)
 
     else:
         raise Exception(
             f"Invalid Node Type for Code Submission:{context.node.node_type}"
         )
     return Ok(code_inputs)
@@ -233,15 +248,17 @@
 def allowed_ids_only(
     allowed_inputs: Dict[str, UID],
     kwargs: Dict[str, Any],
     context: AuthedServiceContext,
 ) -> Dict[str, UID]:
     if context.node.node_type == NodeType.DOMAIN:
         node_view = NodeView(
-            node_name=context.node.name, verify_key=context.node.signing_key.verify_key
+            node_name=context.node.name,
+            node_id=context.node.id,
+            verify_key=context.node.signing_key.verify_key,
         )
         allowed_inputs = allowed_inputs[node_view]
     elif context.node.node_type == NodeType.ENCLAVE:
         base_dict = {}
         for key in allowed_inputs.values():
             base_dict.update(key)
         allowed_inputs = base_dict
```

### Comparing `syft-0.8.2b2/src/syft/service/policy/policy_service.py` & `syft-0.8.2b3/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.2b3/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/project/project.py` & `syft-0.8.2b3/src/syft/service/project/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1398,15 +1398,15 @@
         ]
     )
 
 
 def create_project_event_hash(project_event: ProjectEvent) -> Tuple[bytes, str]:
     # Creating a custom hash for the project
     # as the recursive hash is yet to be revamped
-    # for primitives python types.
+    # for primitives python types
 
     # hashing is calculated based on the following attributes,
     # attrs = ["id", "project_id", "seq no",
     # "prev_event_uid", "prev_event_hash", "creator_verify_key"]
 
     return hash_object(
         [
```

### Comparing `syft-0.8.2b2/src/syft/service/project/project_service.py` & `syft-0.8.2b3/src/syft/service/project/project_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # relative
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
-from ..message.message_service import CreateMessage
-from ..message.message_service import MessageService
+from ..notification.notification_service import NotificationService
+from ..notification.notifications import CreateNotification
 from ..response import SyftError
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
@@ -376,22 +376,22 @@
             Union[SyftSuccess, SyftError]: SyftSuccess if message is created else SyftError
         """
         if (
             isinstance(project_event, ProjectRequest)
             and project_event.linked_request.node_uid == context.node.id
         ):
             link = LinkedObject.with_context(project, context=context)
-            message = CreateMessage(
+            message = CreateNotification(
                 subject=f"A new request has been added to the Project: {project.name}.",
                 from_user_verify_key=context.credentials,
                 to_user_verify_key=context.node.verify_key,
                 linked_obj=link,
             )
-            method = context.node.get_service_method(MessageService.send)
-            result = method(context=context, message=message)
+            method = context.node.get_service_method(NotificationService.send)
+            result = method(context=context, notification=message)
             if isinstance(result, SyftError):
                 return result
         return SyftSuccess(message="Successfully Validated Project Request")
 
 
 TYPE_TO_SERVICE[Project] = ProjectService
 SERVICE_TO_TYPES[ProjectService].update({Project})
```

### Comparing `syft-0.8.2b2/src/syft/service/project/project_stash.py` & `syft-0.8.2b3/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/queue/base_queue.py` & `syft-0.8.2b3/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/queue/queue.py` & `syft-0.8.2b3/src/syft/service/queue/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .base_queue import AbstractMessageHandler
 from .base_queue import BaseQueueManager
 from .base_queue import QueueConfig
 from .queue_stash import QueueItem
 from .queue_stash import Status
 
 
+@serializable()
 class QueueManager(BaseQueueManager):
     config: QueueConfig
 
     def post_init(self):
         self.client_config = self.config.client_config()
         self._client = self.config.client_type(self.client_config)
```

### Comparing `syft-0.8.2b2/src/syft/service/queue/queue_stash.py` & `syft-0.8.2b3/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/queue/zmq_queue.py` & `syft-0.8.2b3/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/request/request.py` & `syft-0.8.2b3/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
 # relative
 from ...client.api import APIRegistry
-from ...external import OBLV
 from ...node.credentials import SyftVerifyKey
 from ...serde.serializable import serializable
 from ...serde.serialize import _serialize
 from ...store.linked_obj import LinkedObject
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
@@ -40,15 +39,15 @@
 from ..action.action_service import ActionService
 from ..action.action_store import ActionObjectPermission
 from ..action.action_store import ActionPermission
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatus
 from ..context import AuthedServiceContext
 from ..context import ChangeContext
-from ..message.messages import Message
+from ..notification.notifications import Notification
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..user.user import UserView
 
 
 @serializable()
 class RequestStatus(Enum):
@@ -143,15 +142,15 @@
 
 @serializable()
 class Request(SyftObject):
     __canonical_name__ = "Request"
     __version__ = SYFT_OBJECT_VERSION_1
 
     requesting_user_verify_key: SyftVerifyKey
-    requesting_user_name: str
+    requesting_user_name: str = ""
     approving_user_verify_key: Optional[SyftVerifyKey]
     request_time: DateTime
     updated_at: Optional[DateTime]
     node_uid: UID
     request_hash: str
     changes: List[Change]
     history: List[ChangeStatus] = []
@@ -295,14 +294,15 @@
 
             # If no error, then change successfully applied.
             change_status.applied = True
             self.history.append(change_status)
 
         self.updated_at = DateTime.now()
         self.save(context=context)
+
         return Ok(SyftSuccess(message=f"Request {self.id} changes applied"))
 
     def undo(self, context: AuthedServiceContext) -> Result[SyftSuccess, SyftError]:
         change_context = ChangeContext.from_service(context)
         change_context.requesting_user_credentials = self.requesting_user_verify_key
 
         current_change_state = self.current_change_state
@@ -339,14 +339,15 @@
 
         save_method = context.node.get_service_method(RequestService.save)
         return save_method(context=context, request=self)
 
     def accept_by_depositing_result(self, result: Any, force: bool = False):
         # this code is extremely brittle because its a work around that relies on
         # the type of request being very specifically tied to code which needs approving
+
         change = self.changes[0]
         if not change.is_type(UserCode):
             raise Exception(
                 f"accept_by_depositing_result can only be run on {UserCode} not "
                 f"{change.linked_obj.object_type}"
             )
         if not type(change) == UserCodeStatusChange:
@@ -417,15 +418,15 @@
 class RequestInfo(SyftObject):
     # version
     __canonical_name__ = "RequestInfo"
     __version__ = SYFT_OBJECT_VERSION_1
 
     user: UserView
     request: Request
-    message: Message
+    message: Notification
 
 
 @serializable()
 class RequestInfoFilter(SyftObject):
     # version
     __canonical_name__ = "RequestInfoFilter"
     __version__ = SYFT_OBJECT_VERSION_1
@@ -688,64 +689,65 @@
         return SyftSuccess(message=f"{type(self)} valid")
 
     def mutate(self, obj: UserCode, context: ChangeContext, undo: bool) -> Any:
         if not undo:
             res = obj.status.mutate(
                 value=self.value,
                 node_name=context.node.name,
+                node_id=context.node.id,
                 verify_key=context.node.signing_key.verify_key,
             )
         else:
             res = obj.status.mutate(
                 value=UserCodeStatus.DENIED,
                 node_name=context.node.name,
+                node_id=context.node.id,
                 verify_key=context.node.signing_key.verify_key,
             )
-        if res.is_ok():
-            obj.status = res.ok()
-            return Ok(obj)
+        if not isinstance(res, SyftError):
+            obj.status = res
+            return obj
         return res
 
+    def is_enclave_request(self, req_enclave_metadata):
+        return req_enclave_metadata is not None and self.value == UserCodeStatus.EXECUTE
+
     def _run(
         self, context: ChangeContext, apply: bool
     ) -> Result[SyftSuccess, SyftError]:
         try:
             valid = self.valid
             if not valid:
                 return Err(valid)
             obj = self.linked_obj.resolve_with_context(context)
             if obj.is_err():
                 return SyftError(message=obj.err())
             obj = obj.ok()
             if apply:
                 res = self.mutate(obj, context, undo=False)
 
-                if res.is_err():
+                if isinstance(res, SyftError):
                     return res
-                res = res.ok()
-                if OBLV:
-                    # relative
-                    from ...external.oblv.oblv_service import check_enclave_transfer
 
-                    enclave_res = check_enclave_transfer(
-                        user_code=res, value=self.value, context=context
-                    )
-                else:
-                    enclave_res = Ok()
+                # relative
+                from ..enclave.enclave_service import propagate_inputs_to_enclave
 
-                if enclave_res.is_err():
-                    return enclave_res
-                self.linked_obj.update_with_context(context, res)
+                user_code = res
+                if self.is_enclave_request(user_code.enclave_metadata):
+                    enclave_res = propagate_inputs_to_enclave(
+                        user_code=res, context=context
+                    )
+                    if isinstance(enclave_res, SyftError):
+                        return enclave_res
+                self.linked_obj.update_with_context(context, user_code)
             else:
                 res = self.mutate(obj, context, undo=True)
-                if res.is_err():
+                if isinstance(res, SyftError):
                     return res
 
-                res = res.ok()
-
                 # TODO: Handle Enclave approval.
                 self.linked_obj.update_with_context(context, res)
             return Ok(SyftSuccess(message=f"{type(self)} Success"))
         except Exception as e:
             print(f"failed to apply {type(self)}. {e}")
             return Err(SyftError(message=str(e)))
```

### Comparing `syft-0.8.2b2/src/syft/service/request/request_service.py` & `syft-0.8.2b3/src/syft/service/request/request_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
 from ..context import AuthedServiceContext
-from ..message.message_service import CreateMessage
-from ..message.message_service import Message
-from ..message.message_service import MessageService
+from ..notification.notification_service import CreateNotification
+from ..notification.notification_service import NotificationService
+from ..notification.notifications import Notification
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user import UserView
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..user.user_service import UserService
 from .request import Change
 from .request import Request
 from .request import RequestInfo
 from .request import RequestInfoFilter
+from .request import RequestStatus
 from .request import SubmitRequest
 from .request_stash import RequestStash
 
 
 @instrument
 @serializable()
 class RequestService(AbstractService):
@@ -73,23 +74,23 @@
                     UserService.admin_verify_key
                 )
 
                 root_verify_key = admin_verify_key()
                 if send_message:
                     subject_msg = f"Result to request {str(request.id)[:4]}...{str(request.id)[-3:]}\
                         has been successfully deposited."
-                    message = CreateMessage(
+                    message = CreateNotification(
                         subject=subject_msg if not reason else reason,
                         from_user_verify_key=context.credentials,
                         to_user_verify_key=root_verify_key,
                         linked_obj=link,
                     )
-                    method = context.node.get_service_method(MessageService.send)
-                    result = method(context=context, message=message)
-                    if isinstance(result, Message):
+                    method = context.node.get_service_method(NotificationService.send)
+                    result = method(context=context, notification=message)
+                    if isinstance(result, Notification):
                         return Ok(request)
                     else:
                         return Err(result)
 
                 return Ok(request)
 
             if result.is_err():
@@ -113,22 +114,24 @@
         context: AuthedServiceContext,
         page_index: Optional[int] = 0,
         page_size: Optional[int] = 0,
     ) -> Union[List[RequestInfo], SyftError]:
         """Get a Dataset"""
         result = self.stash.get_all(context.credentials)
         method = context.node.get_service_method(UserService.get_by_verify_key)
-        get_message = context.node.get_service_method(MessageService.filter_by_obj)
+        get_message = context.node.get_service_method(NotificationService.filter_by_obj)
 
         requests = []
         if result.is_ok():
             for req in result.ok():
                 user = method(req.requesting_user_verify_key).to(UserView)
                 message = get_message(context=context, obj_uid=req.id)
-                requests.append(RequestInfo(user=user, request=req, message=message))
+                requests.append(
+                    RequestInfo(user=user, request=req, notification=message)
+                )
 
             # If chunk size is defined, then split list into evenly sized chunks
             if page_size:
                 requests = [
                     requests[i : i + page_size]
                     for i in range(0, len(requests), page_size)
                 ]
@@ -182,14 +185,37 @@
     def apply(
         self, context: AuthedServiceContext, uid: UID
     ) -> Union[SyftSuccess, SyftError]:
         request = self.stash.get_by_uid(context.credentials, uid)
         if request.is_ok():
             request = request.ok()
             result = request.apply(context=context)
+
+            filter_by_obj = context.node.get_service_method(
+                NotificationService.filter_by_obj
+            )
+            request_notification = filter_by_obj(context=context, obj_uid=uid)
+
+            link = LinkedObject.with_context(request, context=context)
+            if not request.status == RequestStatus.PENDING:
+                mark_as_read = context.node.get_service_method(
+                    NotificationService.mark_as_read
+                )
+                mark_as_read(context=context, uid=request_notification.id)
+
+                notification = CreateNotification(
+                    subject=f"{request.changes} for Request id: {uid} has status updated to {request.status}",
+                    to_user_verify_key=request.requesting_user_verify_key,
+                    linked_obj=link,
+                )
+                send_notification = context.node.get_service_method(
+                    NotificationService.send
+                )
+                send_notification(context=context, notification=notification)
+
             return result.value
         return request.value
 
     @service_method(path="request.undo", name="undo")
     def undo(
         self, context: AuthedServiceContext, uid: UID, reason: str
     ) -> Union[SyftSuccess, SyftError]:
@@ -212,22 +238,22 @@
 
         link = LinkedObject.with_context(request, context=context)
         message_subject = (
             f"Your request for uid: {uid} has been denied. "
             f"Reason specified by Data Owner: {reason}."
         )
 
-        notification = CreateMessage(
+        notification = CreateNotification(
             subject=message_subject,
             to_user_verify_key=request.requesting_user_verify_key,
             linked_obj=link,
         )
-        send_notification = context.node.get_service_method(MessageService.send)
+        send_notification = context.node.get_service_method(NotificationService.send)
 
-        result = send_notification(context=context, message=notification)
+        result = send_notification(context=context, notification=notification)
         return SyftSuccess(message=f"Request {uid} successfully denied !")
 
     def save(
         self, context: AuthedServiceContext, request: Request
     ) -> Union[Request, SyftError]:
         result = self.stash.update(context.credentials, request)
         if result.is_ok():
```

### Comparing `syft-0.8.2b2/src/syft/service/request/request_stash.py` & `syft-0.8.2b3/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/response.py` & `syft-0.8.2b3/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/service.py` & `syft-0.8.2b3/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/settings/settings.py` & `syft-0.8.2b3/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/settings/settings_service.py` & `syft-0.8.2b3/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/settings/settings_stash.py` & `syft-0.8.2b3/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/user/user.py` & `syft-0.8.2b3/src/syft/service/user/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,23 @@
             "Email": self.email,
             "Institute": self.institution,
             "Website": self.website,
             "Role": self.role.name.capitalize(),
         }
 
 
+@serializable()
+class UserViewPage(SyftObject):
+    __canonical_name__ = "UserViewPage"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    users: List[UserView]
+    total: int
+
+
 @transform(UserUpdate, User)
 def user_update_to_user() -> List[Callable]:
     return [
         validate_email,
         hash_password,
         drop(["password", "password_verify"]),
     ]
```

### Comparing `syft-0.8.2b2/src/syft/service/user/user_roles.py` & `syft-0.8.2b3/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/user/user_service.py` & `syft-0.8.2b3/src/syft/service/user/user_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from ..service import service_method
 from .user import User
 from .user import UserCreate
 from .user import UserPrivateKey
 from .user import UserSearch
 from .user import UserUpdate
 from .user import UserView
+from .user import UserViewPage
 from .user import check_pwd
 from .user import salt_and_hash_password
 from .user_roles import DATA_OWNER_ROLE_LEVEL
 from .user_roles import GUEST_ROLE_LEVEL
 from .user_roles import ServiceRole
 from .user_roles import ServiceRoleCapability
 from .user_stash import UserStash
@@ -94,27 +95,29 @@
 
     @service_method(path="user.get_all", name="get_all", roles=DATA_OWNER_ROLE_LEVEL)
     def get_all(
         self,
         context: AuthedServiceContext,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
-    ) -> Union[Optional[UserView], SyftError]:
+    ) -> Union[Optional[UserViewPage], Optional[UserView], SyftError]:
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             results = [user.to(UserView) for user in result.ok()]
 
             # If chunk size is defined, then split list into evenly sized chunks
             if page_size:
+                total = len(results)
                 results = [
                     results[i : i + page_size]
                     for i in range(0, len(results), page_size)
                 ]
                 # Return the proper slice using chunk_index
                 results = results[page_index]
+                results = UserViewPage(users=results, total=total)
 
             return results
 
         # 🟡 TODO: No user exists will happen when result.ok() is empty list
         return SyftError(message="No users exists")
 
     def get_role_for_credentials(
@@ -140,15 +143,15 @@
     @service_method(path="user.search", name="search", autosplat=["user_search"])
     def search(
         self,
         context: AuthedServiceContext,
         user_search: UserSearch,
         page_size: Optional[int] = 0,
         page_index: Optional[int] = 0,
-    ) -> Union[List[UserView], SyftError]:
+    ) -> Union[Optional[UserViewPage], List[UserView], SyftError]:
         kwargs = user_search.to_dict(exclude_empty=True)
 
         if len(kwargs) == 0:
             valid_search_params = list(UserSearch.__fields__.keys())
             return SyftError(
                 message=f"Invalid Search parameters. \
                 Allowed params: {valid_search_params}"
@@ -158,19 +161,21 @@
         if result.is_err():
             return SyftError(message=str(result.err()))
         users = result.ok()
         results = [user.to(UserView) for user in users] if users is not None else []
 
         # If page size is defined, then split list into evenly sized chunks
         if page_size:
+            total = len(results)
             results = [
                 results[i : i + page_size] for i in range(0, len(results), page_size)
             ]
             # Return the proper slice using page_index
             results = results[page_index]
+            results = UserViewPage(users=results, total=total)
 
         return results
 
     @service_method(path="user.update", name="update", roles=GUEST_ROLE_LEVEL)
     def update(
         self, context: AuthedServiceContext, uid: UID, user_update: UserUpdate
     ) -> Union[UserView, SyftError]:
@@ -338,16 +343,17 @@
         """Register new user"""
 
         request_user_role = (
             ServiceRole.GUEST
             if new_user.created_by is None
             else self.get_role_for_credentials(new_user.created_by)
         )
-        can_user_register = context.node.metadata.signup_enabled or (
-            request_user_role in DATA_OWNER_ROLE_LEVEL
+        can_user_register = (
+            context.node.metadata.signup_enabled
+            or request_user_role in DATA_OWNER_ROLE_LEVEL
         )
 
         if not can_user_register:
             return SyftError(
                 message=f"You don't have permission to create an account "
                 f"on the domain: {context.node.name}. Please contact the Domain Owner."
             )
```

### Comparing `syft-0.8.2b2/src/syft/service/user/user_stash.py` & `syft-0.8.2b3/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/vpn/headscale_client.py` & `syft-0.8.2b3/src/syft/service/vpn/headscale_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/service/vpn/tailscale_client.py` & `syft-0.8.2b3/src/syft/service/vpn/tailscale_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
         if result.is_err():
             return SyftError(message=result.err())
 
         command_result = result.ok()
 
         if command_result.error:
-            return SyftError(message=result.error)
+            return SyftError(message=command_result.error)
 
         return SyftSuccess(message="Disconnected Successfully !")
 
 
 def get_vpn_client(
     client_type: Type[BaseVPNClient],
 ) -> Result[BaseVPNClient, str]:
@@ -242,8 +242,8 @@
     if api_key is not None and url is not None:
         client = client_type(
             connection=VPNClientConnection(url=url, routes=routes),
             api_key=api_key,
         )
         return Ok(client)
 
-    return Err(f"Failed to create client for: {client_type.__name__}")
+    return Err(f"Cannot create client for: {client_type.__name__}")
```

### Comparing `syft-0.8.2b2/src/syft/service/vpn/vpn.py` & `syft-0.8.2b3/src/syft/service/vpn/vpn.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 from ...client.client import upgrade_tls
 from ...client.connection import NodeConnection
 from ...serde.serializable import serializable
 from ...types.grid_url import GridURL
 from ...types.syft_object import PartialSyftObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
+from ...util.constants import DEFAULT_TIMEOUT
 from ...util.util import verify_tls
 
-DEFAULT_TIMEOUT = 5  # in seconds
-
 
 @serializable()
 class VPNRoutes(Enum):
     pass
 
 
 @serializable()
```

### Comparing `syft-0.8.2b2/src/syft/store/dict_document_store.py` & `syft-0.8.2b3/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/document_store.py` & `syft-0.8.2b3/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/kv_document_store.py` & `syft-0.8.2b3/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/linked_obj.py` & `syft-0.8.2b3/src/syft/store/linked_obj.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         # relative
         from ..client.api import APIRegistry
 
         api = APIRegistry.api_for(
             node_uid=self.node_uid,
             user_verify_key=self.syft_client_verify_key,
         )
-        return api.services.messages.resolve_object(self)
+        return api.services.notifications.resolve_object(self)
 
     def resolve_with_context(self, context: NodeServiceContext) -> Any:
         return context.node.get_service(self.service_type).resolve_link(
             context=context, linked_obj=self
         )
 
     def update_with_context(
```

### Comparing `syft-0.8.2b2/src/syft/store/locks.py` & `syft-0.8.2b3/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/mongo_client.py` & `syft-0.8.2b3/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/mongo_codecs.py` & `syft-0.8.2b3/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/mongo_document_store.py` & `syft-0.8.2b3/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/store/sqlite_document_store.py` & `syft-0.8.2b3/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/types/datetime.py` & `syft-0.8.2b3/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/types/grid_url.py` & `syft-0.8.2b3/src/syft/types/grid_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             parts = urlparse(url)
             host_or_ip_parts = parts.netloc.split(":")
             # netloc is host:port
             port = 80
             if len(host_or_ip_parts) > 1:
                 port = int(host_or_ip_parts[1])
             host_or_ip = host_or_ip_parts[0]
+            if parts.scheme == "https":
+                port = 443
             return GridURL(
                 host_or_ip=host_or_ip,
                 path=parts.path,
                 port=port,
                 protocol=parts.scheme,
                 query=getattr(parts, "query", ""),
             )
```

### Comparing `syft-0.8.2b2/src/syft/types/syft_metaclass.py` & `syft-0.8.2b3/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/types/syft_object.py` & `syft-0.8.2b3/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/types/transforms.py` & `syft-0.8.2b3/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/types/twin_object.py` & `syft-0.8.2b3/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/types/uid.py` & `syft-0.8.2b3/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/autoreload.py` & `syft-0.8.2b3/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/decorators.py` & `syft-0.8.2b3/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/experimental_flags.py` & `syft-0.8.2b3/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/filterwarnings.py` & `syft-0.8.2b3/src/syft/util/filterwarnings.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,7 +22,17 @@
 # UserWarning: libuv only supports millisecond timer resolution; all times less will be
 # # set to 1 ms
 warnings.filterwarnings(
     "ignore",
     ".*libuv only supports millisecond timer resolution*",
     category=UserWarning,
 )
+
+# site-packages/IPython/core/formatters.py:367: FormatterWarning:
+#  text/html formatter returned invalid type <class 'type'> (expected <class 'str'>)
+#  for object: <EnclaveClient - cranky_norvig <a2fa3fe86007429189dcd88081185bd5>: HTTPConnection: http://localhost:8082>
+# during printing of client object
+warnings.filterwarnings(
+    "ignore",
+    ".*text/html formatter returned invalid type <class 'type'>*",
+    category=UserWarning,
+)
```

### Comparing `syft-0.8.2b2/src/syft/util/fonts.py` & `syft-0.8.2b3/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/logger.py` & `syft-0.8.2b3/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/markdown.py` & `syft-0.8.2b3/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.2b3/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/schema.py` & `syft-0.8.2b3/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/telemetry.py` & `syft-0.8.2b3/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/trace_decorator.py` & `syft-0.8.2b3/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/util.py` & `syft-0.8.2b3/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft/util/version_compare.py` & `syft-0.8.2b3/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.2b2/src/syft.egg-info/PKG-INFO` & `syft-0.8.2b3/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.2b2
+Version: 0.8.2b3
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.2b2 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.2b3 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: telemetry
```

### Comparing `syft-0.8.2b2/src/syft.egg-info/SOURCES.txt` & `syft-0.8.2b3/src/syft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/syft/VERSION
 src/syft/__init__.py
+src/syft/__main__.py
 src/syft/abstract_node.py
 src/syft/gevent_patch.py
 src/syft.egg-info/PKG-INFO
 src/syft.egg-info/SOURCES.txt
 src/syft.egg-info/dependency_links.txt
 src/syft.egg-info/entry_points.txt
 src/syft.egg-info/not-zip-safe
@@ -20,14 +21,17 @@
 src/syft/capnp/kv_iterable.capnp
 src/syft/capnp/recursive_serde.capnp
 src/syft/client/__init__.py
 src/syft/client/api.py
 src/syft/client/client.py
 src/syft/client/connection.py
 src/syft/client/deploy.py
+src/syft/client/domain_client.py
+src/syft/client/enclave_client.py
+src/syft/client/gateway_client.py
 src/syft/client/registry.py
 src/syft/client/search.py
 src/syft/client/user_settings.py
 src/syft/external/__init__.py
 src/syft/external/oblv/__init__.py
 src/syft/external/oblv/auth.py
 src/syft/external/oblv/constants.py
@@ -40,14 +44,15 @@
 src/syft/external/oblv/oblv_service.py
 src/syft/img/base64.py
 src/syft/img/logo.png
 src/syft/img/small-grid-symbol-logo.png
 src/syft/node/__init__.py
 src/syft/node/credentials.py
 src/syft/node/domain.py
+src/syft/node/enclave.py
 src/syft/node/gateway.py
 src/syft/node/node.py
 src/syft/node/routes.py
 src/syft/node/run.py
 src/syft/node/server.py
 src/syft/node/worker.py
 src/syft/node/worker_settings.py
@@ -94,22 +99,23 @@
 src/syft/service/data_subject/data_subject_member.py
 src/syft/service/data_subject/data_subject_member_service.py
 src/syft/service/data_subject/data_subject_service.py
 src/syft/service/dataset/__init__.py
 src/syft/service/dataset/dataset.py
 src/syft/service/dataset/dataset_service.py
 src/syft/service/dataset/dataset_stash.py
-src/syft/service/message/__init__.py
-src/syft/service/message/message_service.py
-src/syft/service/message/message_stash.py
-src/syft/service/message/messages.py
+src/syft/service/enclave/enclave_service.py
 src/syft/service/metadata/node_metadata.py
 src/syft/service/network/network_service.py
 src/syft/service/network/node_peer.py
 src/syft/service/network/routes.py
+src/syft/service/notification/__init__.py
+src/syft/service/notification/notification_service.py
+src/syft/service/notification/notification_stash.py
+src/syft/service/notification/notifications.py
 src/syft/service/policy/__init__.py
 src/syft/service/policy/policy.py
 src/syft/service/policy/policy_service.py
 src/syft/service/policy/user_policy_stash.py
 src/syft/service/project/__init__.py
 src/syft/service/project/project.py
 src/syft/service/project/project_service.py
@@ -152,14 +158,15 @@
 src/syft/types/syft_object.py
 src/syft/types/transforms.py
 src/syft/types/twin_object.py
 src/syft/types/uid.py
 src/syft/util/__init__.py
 src/syft/util/autoreload.py
 src/syft/util/colors.py
+src/syft/util/constants.py
 src/syft/util/decorators.py
 src/syft/util/experimental_flags.py
 src/syft/util/filterwarnings.py
 src/syft/util/fonts.py
 src/syft/util/jax_settings.py
 src/syft/util/logger.py
 src/syft/util/markdown.py
```

### Comparing `syft-0.8.2b2/src/syft.egg-info/requires.txt` & `syft-0.8.2b3/src/syft.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 hagrid>=0.3
 matplotlib==3.7.1
 dm-haiku==0.0.9
 itables==1.5.3
 transformers==4.30.2
 evaluate==0.4.0
 torch==2.0.1
+recordlinkage==0.15
 
 [dev]
 pytest
 pytest-cov
 pytest-xdist[psutil]
 pytest-parallel
 pytest-asyncio
```


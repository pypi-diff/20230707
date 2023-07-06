# Comparing `tmp/flwr_nightly-1.5.0.dev20230704.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230704.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230705.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230704.tar` & `flwr_nightly-1.5.0.dev20230705.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    11358 2023-07-04 23:02:26.282966 flwr_nightly-1.5.0.dev20230704/LICENSE
--rw-r--r--   0        0        0    10363 2023-07-04 23:02:26.282966 flwr_nightly-1.5.0.dev20230704/README.md
--rw-r--r--   0        0        0     5158 2023-07-04 23:02:56.467373 flwr_nightly-1.5.0.dev20230704/pyproject.toml
--rw-r--r--   0        0        0      952 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    13835 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4295 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     5474 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1685 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8333 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-07-04 23:02:26.590970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3459 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16315 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26333 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-07-04 23:02:26.594970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1858 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2024 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3686 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19294 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4654 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6995 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5893 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7014 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11522 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9991 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8286 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2708 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5428 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7126 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     6026 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3519 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7079 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6343 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10154 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5478 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4940 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-07-04 23:02:26.598970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7762 2023-07-04 23:02:26.602970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-07-04 23:02:26.602970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5471 2023-07-04 23:02:26.602970 flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12531 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230704/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-05 23:02:37.285993 flwr_nightly-1.5.0.dev20230705/LICENSE
+-rw-r--r--   0        0        0    10721 2023-07-05 23:02:37.285993 flwr_nightly-1.5.0.dev20230705/README.md
+-rw-r--r--   0        0        0     5221 2023-07-05 23:03:06.877939 flwr_nightly-1.5.0.dev20230705/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    14126 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4446 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     6823 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1685 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8448 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3459 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16315 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-07-05 23:02:37.598013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7295 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     6182 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     7505 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2183 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26333 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     2546 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2876 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3686 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19294 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-07-05 23:02:37.602013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5478 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4940 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7762 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5471 2023-07-05 23:02:37.606013 flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12946 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230705/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230704/LICENSE` & `flwr_nightly-1.5.0.dev20230705/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/README.md` & `flwr_nightly-1.5.0.dev20230705/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,19 @@
    
 4. **Custom Clients for Federated Learning**
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))
 
 Stay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.
 
+## 30 Minute Federated Learning Tutorial
+
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb))
+
+
 ## Documentation
 
 [Flower Docs](https://flower.dev/docs):
 * [Installation](https://flower.dev/docs/installation.html)
 * [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
 * [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)
 * [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)
```

#### html2text {}

```diff
@@ -52,54 +52,59 @@
 Building-a-Strategy-PyTorch.ipynb)) 4. **Custom Clients for Federated
 Learning** [![Open in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/
 source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the
 [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
 tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb)) Stay tuned, more
 tutorials are coming soon. Topics include **Privacy and Security in Federated
-Learning**, and **Scaling Federated Learning**. ## Documentation [Flower Docs]
-(https://flower.dev/docs): * [Installation](https://flower.dev/docs/
-installation.html) * [Quickstart (TensorFlow)](https://flower.dev/docs/
-quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/docs/
-quickstart-pytorch.html) * [Quickstart (Hugging Face [code example])](https://
-flower.dev/docs/quickstart-huggingface.html) * [Quickstart (PyTorch Lightning
-[code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html) *
-[Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html) *
-[Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html) *
-[Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html) *
-[Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
-quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
-tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
-example])](https://github.com/adap/flower/tree/main/examples/android) *
-[Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html) ## Flower
-Baselines Flower Baselines is a collection of community-contributed experiments
-that reproduce the experiments performed in popular federated learning
-publications. Researchers can build on Flower Baselines to quickly evaluate new
-ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST](https://
-github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
-fedavg_mnist) * [FedProx](https://arxiv.org/abs/1812.06127): * [MNIST](https://
-github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
-fedprox_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
-Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
-github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/
-convergence_rate) * [Adaptive Federated Optimization](https://arxiv.org/abs/
-2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/adaptive_federated_optimization) Check
-the Flower documentation to learn more: [Using Baselines](https://flower.dev/
-docs/using-baselines.html) The Flower community loves contributions! Make your
-work more visible and enable others to build on it by contributing it as a
-baseline: [Contributing Baselines](https://flower.dev/docs/contributing-
-baselines.html) ## Flower Usage Examples Several code examples show different
-usage scenarios of Flower (in combination with popular machine learning
-frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
-(TensorFlow)](https://github.com/adap/flower/tree/main/examples/
-quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/
-tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging Face)](https://
-github.com/adap/flower/tree/main/examples/quickstart_huggingface) * [Quickstart
-(PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/
+Learning**, and **Scaling Federated Learning**. ## 30 Minute Federated Learning
+Tutorial [![Open in Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/
+examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter
+Notebook](https://github.com/adap/flower/blob/main/examples/
+simulation_pytorch_colab/tutorial.ipynb)) ## Documentation [Flower Docs](https:
+//flower.dev/docs): * [Installation](https://flower.dev/docs/installation.html)
+* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
+* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html) *
+[Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-
+huggingface.html) * [Quickstart (PyTorch Lightning [code example])](https://
+flower.dev/docs/quickstart-pytorch-lightning.html) * [Quickstart (MXNet)]
+(https://flower.dev/docs/example-mxnet-walk-through.html) * [Quickstart
+(Pandas)](https://flower.dev/docs/quickstart-pandas.html) * [Quickstart
+(fastai)](https://flower.dev/docs/quickstart-fastai.html) * [Quickstart (JAX)]
+(https://github.com/adap/flower/tree/main/examples/quickstart_jax) *
+[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
+sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code example])](https:/
+/github.com/adap/flower/tree/main/examples/android) * [Quickstart (iOS)](https:
+//flower.dev/docs/quickstart-ios.html) ## Flower Baselines Flower Baselines is
+a collection of community-contributed experiments that reproduce the
+experiments performed in popular federated learning publications. Researchers
+can build on Flower Baselines to quickly evaluate new ideas: * [FedAvg](https:/
+/arxiv.org/abs/1602.05629): * [MNIST](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedavg_mnist) * [FedProx](https://
+arxiv.org/abs/1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedprox_mnist) * [FedBN: Federated
+Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/
+abs/2102.07623): * [Convergence Rate](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedbn/convergence_rate) * [Adaptive
+Federated Optimization](https://arxiv.org/abs/2003.00295): * [CIFAR-10/100]
+(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
+publications/adaptive_federated_optimization) Check the Flower documentation to
+learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html) The
+Flower community loves contributions! Make your work more visible and enable
+others to build on it by contributing it as a baseline: [Contributing
+Baselines](https://flower.dev/docs/contributing-baselines.html) ## Flower Usage
+Examples Several code examples show different usage scenarios of Flower (in
+combination with popular machine learning frameworks such as PyTorch or
+TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
+github.com/adap/flower/tree/main/examples/quickstart_tensorflow) * [Quickstart
+(PyTorch)](https://github.com/adap/flower/tree/main/examples/
+quickstart_pytorch) * [Quickstart (Hugging Face)](https://github.com/adap/
+flower/tree/main/examples/quickstart_huggingface) * [Quickstart (PyTorch
+Lightning)](https://github.com/adap/flower/tree/main/examples/
 quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
 flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
 github.com/adap/flower/tree/main/examples/quickstart_pandas) * [Quickstart
 (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet) *
 [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
 quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
 tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android)]
```

### Comparing `flwr_nightly-1.5.0.dev20230704/pyproject.toml` & `flwr_nightly-1.5.0.dev20230705/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230704"
+version = "1.5.0-dev20230705"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -55,22 +55,23 @@
 numpy = "^1.21.0"
 grpcio = "^1.48.2,!=1.52.0"
 protobuf = "^3.19.0"
 importlib-metadata = { version = "^4.0.0", markers = "python_version < '3.8'" }
 iterators = "^0.0.2"
 # Optional dependencies (VCE)
 ray = { version = "==2.5.1", extras = ["default"], optional = true }
+pydantic = { version = "<2.0.0", optional = true }
 # Optional dependencies (REST transport layer)
 requests = { version = "^2.28.2", optional = true }
 fastapi = { version = "^0.95.0", optional = true }
 starlette = { version = "^0.27.0", optional = true }
 uvicorn = { version = "^0.21.1", extras = ["standard"], optional = true }
 
 [tool.poetry.extras]
-simulation = ["ray"]
+simulation = ["ray", "pydantic"]
 rest = ["fastapi", "requests", "starlette", "uvicorn"]
 
 [tool.poetry.group.dev.dependencies]
 types-dataclasses = "==0.6.6"
 types-protobuf = "==3.19.18"
 types-requests = "==2.28.11.17"
 types-setuptools = "==67.7.0.1"
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,27 +187,36 @@
     while True:
         sleep_duration: int = 0
         with connection(
             address,
             max_message_length=grpc_max_message_length,
             root_certificates=root_certificates,
         ) as conn:
-            receive, send = conn
+            receive, send, create_node, delete_node = conn
+
+            # Register node
+            if create_node is not None:
+                create_node()  # pylint: disable=not-callable
 
             while True:
                 server_message = receive()
                 if server_message is None:
                     time.sleep(3)  # Wait for 3s before asking again
                     continue
                 client_message, sleep_duration, keep_going = handle(
                     client, server_message
                 )
                 send(client_message)
                 if not keep_going:
                     break
+
+            # Unregister node
+            if delete_node is not None:
+                delete_node()  # pylint: disable=not-callable
+
         if sleep_duration == 0:
             log(INFO, "Disconnect and shut down")
             break
         # Sleep and reconnect afterwards
         log(
             INFO,
             "Disconnect, then re-establish connection after %s second(s)",
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_client/connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,15 +40,22 @@
 
 
 @contextmanager
 def grpc_connection(
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
-) -> Iterator[Tuple[Callable[[], ServerMessage], Callable[[ClientMessage], None]]]:
+) -> Iterator[
+    Tuple[
+        Callable[[], Optional[ServerMessage]],
+        Callable[[ClientMessage], None],
+        Optional[Callable[[], None]],
+        Optional[Callable[[], None]],
+    ]
+]:
     """Establish a gRPC connection to a gRPC server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower server runs on the same
         machine on port 8080, then `server_address` would be `"0.0.0.0:8080"` or
@@ -105,12 +112,13 @@
     def receive() -> ServerMessage:
         return next(server_message_iterator)
 
     def send(msg: ClientMessage) -> None:
         return queue.put(msg, block=False)
 
     try:
-        yield (receive, send)
+        # Yield methods
+        yield (receive, send, None, None)
     finally:
         # Make sure to have a final
         channel.close()
         log(DEBUG, "gRPC channel closed")
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/client/rest_client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,20 @@
 def http_request_response(
     server_address: str,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
     root_certificates: Optional[
         Union[bytes, str]
     ] = None,  # pylint: disable=unused-argument
 ) -> Iterator[
-    Tuple[Callable[[], Optional[ServerMessage]], Callable[[ClientMessage], None]]
+    Tuple[
+        Callable[[], Optional[ServerMessage]],
+        Callable[[ClientMessage], None],
+        Optional[Callable[[], None]],
+        Optional[Callable[[], None]],
+    ]
 ]:
     """Primitives for request/response-based interaction with a server.
 
     One notable difference to the grpc_connection context manager is that
     `receive` can return `None`.
 
     Parameters
@@ -230,12 +235,12 @@
         log(
             INFO,
             "[Node] POST /%s: success, created result %s",
             PATH_PUSH_TASK_RES,
             push_task_res_response_proto.results,  # pylint: disable=no-member
         )
 
-    # yield methods
     try:
-        yield (receive, send)
+        # Yield methods
+        yield (receive, send, None, None)
     except Exception as exc:  # pylint: disable=broad-except
         log(ERROR, exc)
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,54 @@
 import google.protobuf.internal.containers
 import google.protobuf.message
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+class CreateNodeRequest(google.protobuf.message.Message):
+    """CreateNode messages"""
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    def __init__(self,
+        ) -> None: ...
+global___CreateNodeRequest = CreateNodeRequest
+
+class CreateNodeResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    NODE_FIELD_NUMBER: builtins.int
+    @property
+    def node(self) -> flwr.proto.node_pb2.Node: ...
+    def __init__(self,
+        *,
+        node: typing.Optional[flwr.proto.node_pb2.Node] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["node",b"node"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["node",b"node"]) -> None: ...
+global___CreateNodeResponse = CreateNodeResponse
+
+class DeleteNodeRequest(google.protobuf.message.Message):
+    """DeleteNode messages"""
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    NODE_FIELD_NUMBER: builtins.int
+    @property
+    def node(self) -> flwr.proto.node_pb2.Node: ...
+    def __init__(self,
+        *,
+        node: typing.Optional[flwr.proto.node_pb2.Node] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["node",b"node"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["node",b"node"]) -> None: ...
+global___DeleteNodeRequest = DeleteNodeRequest
+
+class DeleteNodeResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    def __init__(self,
+        ) -> None: ...
+global___DeleteNodeResponse = DeleteNodeResponse
+
 class PullTaskInsRequest(google.protobuf.message.Message):
     """PullTaskIns messages"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     NODE_FIELD_NUMBER: builtins.int
     TASK_IDS_FIELD_NUMBER: builtins.int
     @property
     def node(self) -> flwr.proto.node_pb2.Node: ...
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 """
 import abc
 import flwr.proto.fleet_pb2
 import grpc
 
 class FleetStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
+    CreateNode: grpc.UnaryUnaryMultiCallable[
+        flwr.proto.fleet_pb2.CreateNodeRequest,
+        flwr.proto.fleet_pb2.CreateNodeResponse]
+
+    DeleteNode: grpc.UnaryUnaryMultiCallable[
+        flwr.proto.fleet_pb2.DeleteNodeRequest,
+        flwr.proto.fleet_pb2.DeleteNodeResponse]
+
     PullTaskIns: grpc.UnaryUnaryMultiCallable[
         flwr.proto.fleet_pb2.PullTaskInsRequest,
         flwr.proto.fleet_pb2.PullTaskInsResponse]
     """Retrieve one or more tasks, if possible
 
     HTTP API path: /api/v1/fleet/pull-task-ins
     """
@@ -23,14 +31,26 @@
 
     HTTP API path: /api/v1/fleet/push-task-res
     """
 
 
 class FleetServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
+    def CreateNode(self,
+        request: flwr.proto.fleet_pb2.CreateNodeRequest,
+        context: grpc.ServicerContext,
+    ) -> flwr.proto.fleet_pb2.CreateNodeResponse: ...
+
+    @abc.abstractmethod
+    def DeleteNode(self,
+        request: flwr.proto.fleet_pb2.DeleteNodeRequest,
+        context: grpc.ServicerContext,
+    ) -> flwr.proto.fleet_pb2.DeleteNodeResponse: ...
+
+    @abc.abstractmethod
     def PullTaskIns(self,
         request: flwr.proto.fleet_pb2.PullTaskInsRequest,
         context: grpc.ServicerContext,
     ) -> flwr.proto.fleet_pb2.PullTaskInsResponse:
         """Retrieve one or more tasks, if possible
 
         HTTP API path: /api/v1/fleet/pull-task-ins
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,28 +11,58 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Fleet API message handlers."""
 
 
+import random
 from typing import List, Optional
 from uuid import UUID
 
 from flwr.proto.fleet_pb2 import (
+    CreateNodeRequest,
+    CreateNodeResponse,
+    DeleteNodeRequest,
+    DeleteNodeResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
     Reconnect,
 )
+from flwr.proto.node_pb2 import Node
 from flwr.proto.task_pb2 import TaskIns, TaskRes
 from flwr.server.state import State
 
 
+def create_node(
+    request: CreateNodeRequest,  # pylint: disable=unused-argument
+    state: State,
+) -> CreateNodeResponse:
+    """."""
+    # Generate random node_id
+    random_node_id: int = random.randrange(9223372036854775808)
+
+    # Update state
+    state.register_node(node_id=random_node_id)
+    return CreateNodeResponse(node=Node(node_id=random_node_id, anonymous=False))
+
+
+def delete_node(request: DeleteNodeRequest, state: State) -> DeleteNodeResponse:
+    """."""
+    # Validate node_id
+    if request.node.anonymous or request.node.node_id <= 0:
+        return DeleteNodeResponse()
+
+    # Update state
+    state.unregister_node(node_id=request.node.node_id)
+    return DeleteNodeResponse()
+
+
 def pull_task_ins(request: PullTaskInsRequest, state: State) -> PullTaskInsResponse:
     """Pull TaskIns handler."""
     # Get node_id if client node is not anonymous
     node = request.node  # pylint: disable=no-member
     node_id: Optional[int] = None if node.anonymous else node.node_id
 
     # Retrieve TaskIns from State
```

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230705/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230704/PKG-INFO` & `flwr_nightly-1.5.0.dev20230705/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230704
+Version: 1.5.0.dev20230705
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,14 +33,15 @@
 Provides-Extra: simulation
 Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra == "rest"
 Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0)
 Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: protobuf (>=3.19.0,<4.0.0)
+Requires-Dist: pydantic (<2.0.0) ; extra == "simulation"
 Requires-Dist: ray[default] (==2.5.1) ; extra == "simulation"
 Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest"
 Requires-Dist: starlette (>=0.27.0,<0.28.0) ; extra == "rest"
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest"
 Project-URL: Documentation, https://flower.dev
 Project-URL: Repository, https://github.com/adap/flower
 Description-Content-Type: text/markdown
@@ -112,14 +113,19 @@
    
 4. **Custom Clients for Federated Learning**
 
    [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))
 
 Stay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.
 
+## 30 Minute Federated Learning Tutorial
+
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/simulation_pytorch_colab/tutorial.ipynb))
+
+
 ## Documentation
 
 [Flower Docs](https://flower.dev/docs):
 * [Installation](https://flower.dev/docs/installation.html)
 * [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
 * [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)
 * [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230704 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230705 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
@@ -17,21 +17,21 @@
 Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Libraries Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Typing :: Typed Provides-Extra: rest
 Provides-Extra: simulation Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra ==
 "rest" Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist:
 importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8" Requires-Dist:
 iterators (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
-Dist: protobuf (>=3.19.0,<4.0.0) Requires-Dist: ray[default] (==2.5.1) ; extra
-== "simulation" Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest"
-Requires-Dist: starlette (>=0.27.0,<0.28.0) ; extra == "rest" Requires-Dist:
-uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest" Project-URL:
-Documentation, https://flower.dev Project-URL: Repository, https://github.com/
-adap/flower Description-Content-Type: text/markdown # Flower: A Friendly
-Federated Learning Framework
+Dist: protobuf (>=3.19.0,<4.0.0) Requires-Dist: pydantic (<2.0.0) ; extra ==
+"simulation" Requires-Dist: ray[default] (==2.5.1) ; extra == "simulation"
+Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest" Requires-Dist:
+starlette (>=0.27.0,<0.28.0) ; extra == "rest" Requires-Dist: uvicorn[standard]
+(>=0.21.1,<0.22.0) ; extra == "rest" Project-URL: Documentation, https://
+flower.dev Project-URL: Repository, https://github.com/adap/flower Description-
+Content-Type: text/markdown # Flower: A Friendly Federated Learning Framework
                                [Flower_Website]
                   Website | Blog | Docs | Conference | Slack
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
@@ -81,54 +81,59 @@
 Building-a-Strategy-PyTorch.ipynb)) 4. **Custom Clients for Federated
 Learning** [![Open in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/
 source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the
 [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
 tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb)) Stay tuned, more
 tutorials are coming soon. Topics include **Privacy and Security in Federated
-Learning**, and **Scaling Federated Learning**. ## Documentation [Flower Docs]
-(https://flower.dev/docs): * [Installation](https://flower.dev/docs/
-installation.html) * [Quickstart (TensorFlow)](https://flower.dev/docs/
-quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/docs/
-quickstart-pytorch.html) * [Quickstart (Hugging Face [code example])](https://
-flower.dev/docs/quickstart-huggingface.html) * [Quickstart (PyTorch Lightning
-[code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html) *
-[Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html) *
-[Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html) *
-[Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html) *
-[Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
-quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
-tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
-example])](https://github.com/adap/flower/tree/main/examples/android) *
-[Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html) ## Flower
-Baselines Flower Baselines is a collection of community-contributed experiments
-that reproduce the experiments performed in popular federated learning
-publications. Researchers can build on Flower Baselines to quickly evaluate new
-ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST](https://
-github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
-fedavg_mnist) * [FedProx](https://arxiv.org/abs/1812.06127): * [MNIST](https://
-github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
-fedprox_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
-Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
-github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/
-convergence_rate) * [Adaptive Federated Optimization](https://arxiv.org/abs/
-2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/adaptive_federated_optimization) Check
-the Flower documentation to learn more: [Using Baselines](https://flower.dev/
-docs/using-baselines.html) The Flower community loves contributions! Make your
-work more visible and enable others to build on it by contributing it as a
-baseline: [Contributing Baselines](https://flower.dev/docs/contributing-
-baselines.html) ## Flower Usage Examples Several code examples show different
-usage scenarios of Flower (in combination with popular machine learning
-frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
-(TensorFlow)](https://github.com/adap/flower/tree/main/examples/
-quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/
-tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging Face)](https://
-github.com/adap/flower/tree/main/examples/quickstart_huggingface) * [Quickstart
-(PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/
+Learning**, and **Scaling Federated Learning**. ## 30 Minute Federated Learning
+Tutorial [![Open in Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/
+examples/simulation_pytorch_colab/tutorial.ipynb) (or open the [Jupyter
+Notebook](https://github.com/adap/flower/blob/main/examples/
+simulation_pytorch_colab/tutorial.ipynb)) ## Documentation [Flower Docs](https:
+//flower.dev/docs): * [Installation](https://flower.dev/docs/installation.html)
+* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
+* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html) *
+[Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-
+huggingface.html) * [Quickstart (PyTorch Lightning [code example])](https://
+flower.dev/docs/quickstart-pytorch-lightning.html) * [Quickstart (MXNet)]
+(https://flower.dev/docs/example-mxnet-walk-through.html) * [Quickstart
+(Pandas)](https://flower.dev/docs/quickstart-pandas.html) * [Quickstart
+(fastai)](https://flower.dev/docs/quickstart-fastai.html) * [Quickstart (JAX)]
+(https://github.com/adap/flower/tree/main/examples/quickstart_jax) *
+[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
+sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code example])](https:/
+/github.com/adap/flower/tree/main/examples/android) * [Quickstart (iOS)](https:
+//flower.dev/docs/quickstart-ios.html) ## Flower Baselines Flower Baselines is
+a collection of community-contributed experiments that reproduce the
+experiments performed in popular federated learning publications. Researchers
+can build on Flower Baselines to quickly evaluate new ideas: * [FedAvg](https:/
+/arxiv.org/abs/1602.05629): * [MNIST](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedavg_mnist) * [FedProx](https://
+arxiv.org/abs/1812.06127): * [MNIST](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedprox_mnist) * [FedBN: Federated
+Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/
+abs/2102.07623): * [Convergence Rate](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/fedbn/convergence_rate) * [Adaptive
+Federated Optimization](https://arxiv.org/abs/2003.00295): * [CIFAR-10/100]
+(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
+publications/adaptive_federated_optimization) Check the Flower documentation to
+learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html) The
+Flower community loves contributions! Make your work more visible and enable
+others to build on it by contributing it as a baseline: [Contributing
+Baselines](https://flower.dev/docs/contributing-baselines.html) ## Flower Usage
+Examples Several code examples show different usage scenarios of Flower (in
+combination with popular machine learning frameworks such as PyTorch or
+TensorFlow). Quickstart examples: * [Quickstart (TensorFlow)](https://
+github.com/adap/flower/tree/main/examples/quickstart_tensorflow) * [Quickstart
+(PyTorch)](https://github.com/adap/flower/tree/main/examples/
+quickstart_pytorch) * [Quickstart (Hugging Face)](https://github.com/adap/
+flower/tree/main/examples/quickstart_huggingface) * [Quickstart (PyTorch
+Lightning)](https://github.com/adap/flower/tree/main/examples/
 quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
 flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
 github.com/adap/flower/tree/main/examples/quickstart_pandas) * [Quickstart
 (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet) *
 [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
 quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
 tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android)]
```


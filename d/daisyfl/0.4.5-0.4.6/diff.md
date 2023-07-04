# Comparing `tmp/daisyfl-0.4.5.tar.gz` & `tmp/daisyfl-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.4.5.tar", max compression
+gzip compressed data, was "daisyfl-0.4.6.tar", max compression
```

## Comparing `daisyfl-0.4.5.tar` & `daisyfl-0.4.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11358 2023-06-13 11:19:33.755489 daisyfl-0.4.5/LICENSE
--rw-r--r--   0        0        0     1158 2023-06-13 11:19:33.755489 daisyfl-0.4.5/README.md
--rw-r--r--   0        0        0     3661 2023-06-21 00:25:20.622196 daisyfl-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1093 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0     9951 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0     1363 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/client_api_handler.py
--rw-r--r--   0        0        0     3780 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/client_operator_manager.py
--rw-r--r--   0        0        0     3367 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0    10038 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     6704 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     4998 2023-06-17 09:18:06.051724 daisyfl-0.4.5/src/py/daisyfl/client/trainer.py
--rw-r--r--   0        0        0     1663 2023-06-17 09:18:15.943647 daisyfl-0.4.5/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     5644 2023-06-19 11:07:59.531140 daisyfl-0.4.5/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3482 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     1421 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/metadata.py
--rw-r--r--   0        0        0     3938 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    16903 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     4044 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0        0 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base/__init__.py
--rw-r--r--   0        0        0     1162 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base/client_logic.py
--rw-r--r--   0        0        0     5700 2023-06-19 13:00:12.324689 daisyfl-0.4.5/src/py/daisyfl/operator/base/server_logic.py
--rw-r--r--   0        0        0        0 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base_async/__init__.py
--rw-r--r--   0        0        0     1162 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base_async/client_logic.py
--rw-r--r--   0        0        0     5383 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/base_async/server_logic.py
--rw-r--r--   0        0        0     1987 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/client_logic.py
--rw-r--r--   0        0        0      381 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/msg.py
--rw-r--r--   0        0        0     5483 2023-06-17 11:11:34.557702 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/server_logic.py
--rw-r--r--   0        0        0      961 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     5848 2023-06-17 11:17:34.761761 daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0    12137 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/client_logic.py
--rw-r--r--   0        0        0     1755 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/common.py
--rw-r--r--   0        0        0    10070 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/primitives.py
--rw-r--r--   0        0        0    22268 2023-06-19 13:47:16.702565 daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/server_logic.py
--rw-r--r--   0        0        0     1456 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/__init__.py
--rw-r--r--   0        0        0     3016 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/aggregate.py
--rw-r--r--   0        0        0     4538 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     5095 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     6134 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6993 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7245 2023-06-13 11:19:33.759489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadam.py
--rw-r--r--   0        0        0    13054 2023-06-19 06:30:37.042075 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedasync.py
--rw-r--r--   0        0        0    12396 2023-06-19 06:31:01.209923 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg.py
--rw-r--r--   0        0        0    10915 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg_android.py
--rw-r--r--   0        0        0     9115 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavgm.py
--rw-r--r--   0        0        0     5513 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedopt.py
--rw-r--r--   0        0        0     7263 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedyogi.py
--rw-r--r--   0        0        0    10952 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/qfedavg.py
--rw-r--r--   0        0        0     7867 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/strategy/strategy.py
--rw-r--r--   0        0        0      826 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/operator/utils/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-19 13:28:40.804096 daisyfl-0.4.5/src/py/daisyfl/operator/utils/op_tools.py
--rw-r--r--   0        0        0      676 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0    70900 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    25816 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2631 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0     1064 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0     5085 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0     7809 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2371 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0      714 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0    12768 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6827 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4459 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11290 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    11835 2023-06-16 07:31:46.690912 daisyfl-0.4.5/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0     6432 2023-06-19 12:57:16.218211 daisyfl-0.4.5/src/py/daisyfl/server/server_api_handler.py
--rw-r--r--   0        0        0     4560 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/server/server_operator_manager.py
--rw-r--r--   0        0        0    13571 2023-06-19 13:21:30.207305 daisyfl-0.4.5/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      859 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-13 11:19:33.763489 daisyfl-0.4.5/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     2765 2023-06-21 00:25:31.476601 daisyfl-0.4.5/setup.py
--rw-r--r--   0        0        0     3286 2023-06-21 00:25:31.476952 daisyfl-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-29 08:05:35.674456 daisyfl-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1158 2023-06-29 08:05:35.676455 daisyfl-0.4.6/README.md
+-rw-r--r--   0        0        0     3661 2023-07-04 08:37:53.611708 daisyfl-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1093 2023-06-29 08:05:35.860456 daisyfl-0.4.6/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1171 2023-06-29 08:05:35.866456 daisyfl-0.4.6/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9951 2023-06-29 08:05:35.868456 daisyfl-0.4.6/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-06-29 08:05:35.872456 daisyfl-0.4.6/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     1363 2023-06-29 08:05:35.874456 daisyfl-0.4.6/src/py/daisyfl/client/client_api_handler.py
+-rw-r--r--   0        0        0     3780 2023-06-29 08:05:35.876456 daisyfl-0.4.6/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-06-29 08:05:35.880456 daisyfl-0.4.6/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-06-29 08:05:35.882456 daisyfl-0.4.6/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0    10038 2023-06-29 08:05:35.885456 daisyfl-0.4.6/src/py/daisyfl/client/grpc_client/connection.py
+-rw-r--r--   0        0        0     6704 2023-06-29 08:05:35.889456 daisyfl-0.4.6/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     5084 2023-06-29 08:05:35.893456 daisyfl-0.4.6/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     4998 2023-06-29 08:05:35.897456 daisyfl-0.4.6/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     1663 2023-06-29 08:05:35.898456 daisyfl-0.4.6/src/py/daisyfl/client/zone_client.py
+-rw-r--r--   0        0        0     5644 2023-06-29 08:05:35.901456 daisyfl-0.4.6/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-06-29 08:05:35.904456 daisyfl-0.4.6/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-06-29 08:05:35.906456 daisyfl-0.4.6/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1421 2023-06-29 08:05:35.908456 daisyfl-0.4.6/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-06-29 08:05:35.909456 daisyfl-0.4.6/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    16903 2023-06-29 08:05:35.913456 daisyfl-0.4.6/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4044 2023-06-29 08:05:35.918456 daisyfl-0.4.6/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:05:35.920456 daisyfl-0.4.6/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:05:35.922456 daisyfl-0.4.6/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1162 2023-06-29 08:05:35.924456 daisyfl-0.4.6/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5700 2023-06-29 08:05:35.927456 daisyfl-0.4.6/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:05:35.929456 daisyfl-0.4.6/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1162 2023-06-29 08:05:35.931456 daisyfl-0.4.6/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5383 2023-06-29 08:05:35.932456 daisyfl-0.4.6/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     1987 2023-06-29 08:05:35.935456 daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-06-29 08:05:35.937456 daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5483 2023-06-29 08:05:35.938456 daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0      961 2023-06-29 08:05:35.940456 daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
+-rw-r--r--   0        0        0     5848 2023-06-29 08:05:35.941456 daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12137 2023-06-29 08:05:35.944456 daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-06-29 08:05:35.946456 daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-06-29 08:05:35.948456 daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    22268 2023-06-29 08:05:35.951456 daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-06-29 08:05:35.953456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3016 2023-06-29 08:05:35.955456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4538 2023-06-29 08:05:35.958456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5095 2023-06-29 08:05:35.960456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6134 2023-06-29 08:05:35.962456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6993 2023-06-29 08:05:35.966456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7245 2023-06-29 08:05:35.970456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13054 2023-06-29 08:05:35.972456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12396 2023-06-29 08:05:35.976456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    10915 2023-06-29 08:05:35.978456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9115 2023-06-29 08:05:35.982456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-06-29 08:05:35.986456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7263 2023-06-29 08:05:35.987456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    10952 2023-06-29 08:05:35.989456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7867 2023-06-29 08:05:35.991456 daisyfl-0.4.6/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      826 2023-06-29 08:05:35.993456 daisyfl-0.4.6/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-29 08:05:35.995456 daisyfl-0.4.6/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-06-29 08:05:35.997456 daisyfl-0.4.6/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    70900 2023-06-29 08:05:36.000456 daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    25816 2023-06-29 08:05:36.003456 daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-06-29 08:05:36.005456 daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-06-29 08:05:36.007456 daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1064 2023-06-29 08:05:36.010456 daisyfl-0.4.6/src/py/daisyfl/server/__init__.py
+-rw-r--r--   0        0        0     5085 2023-06-29 08:05:36.013456 daisyfl-0.4.6/src/py/daisyfl/server/app.py
+-rw-r--r--   0        0        0     7809 2023-06-29 08:05:36.015456 daisyfl-0.4.6/src/py/daisyfl/server/client_manager.py
+-rw-r--r--   0        0        0     2371 2023-06-29 08:05:36.020456 daisyfl-0.4.6/src/py/daisyfl/server/client_proxy.py
+-rw-r--r--   0        0        0      714 2023-06-29 08:05:36.025456 daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0    12768 2023-06-29 08:05:36.028456 daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6827 2023-06-29 08:05:36.031456 daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4459 2023-06-29 08:05:36.035456 daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11290 2023-06-29 08:05:36.039456 daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     3626 2023-06-29 08:05:36.042456 daisyfl-0.4.6/src/py/daisyfl/server/history.py
+-rw-r--r--   0        0        0    11865 2023-07-04 07:45:52.155496 daisyfl-0.4.6/src/py/daisyfl/server/server.py
+-rw-r--r--   0        0        0     6432 2023-06-29 08:05:36.047456 daisyfl-0.4.6/src/py/daisyfl/server/server_api_handler.py
+-rw-r--r--   0        0        0     4560 2023-06-29 08:05:36.049456 daisyfl-0.4.6/src/py/daisyfl/server/server_operator_manager.py
+-rw-r--r--   0        0        0    13571 2023-06-29 08:05:36.053456 daisyfl-0.4.6/src/py/daisyfl/server/task_manager.py
+-rw-r--r--   0        0        0     1273 2023-06-29 08:05:36.055456 daisyfl-0.4.6/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-29 08:05:36.058456 daisyfl-0.4.6/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-29 08:05:36.060456 daisyfl-0.4.6/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4661 2023-06-29 08:05:36.062456 daisyfl-0.4.6/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-06-29 08:05:36.064456 daisyfl-0.4.6/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:05:36.066456 daisyfl-0.4.6/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     2765 2023-07-04 08:55:47.446332 daisyfl-0.4.6/setup.py
+-rw-r--r--   0        0        0     3286 2023-07-04 08:55:47.446552 daisyfl-0.4.6/PKG-INFO
```

### Comparing `daisyfl-0.4.5/LICENSE` & `daisyfl-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/README.md` & `daisyfl-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/pyproject.toml` & `daisyfl-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.4.5"
+version = "0.4.6"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
```

### Comparing `daisyfl-0.4.5/src/py/daisyfl/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/app.py` & `daisyfl-0.4.6/src/py/daisyfl/client/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/client.py` & `daisyfl-0.4.6/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/client_api_handler.py` & `daisyfl-0.4.6/src/py/daisyfl/client/client_api_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/client_operator_manager.py` & `daisyfl-0.4.6/src/py/daisyfl/client/client_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.4.6/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/connection.py` & `daisyfl-0.4.6/src/py/daisyfl/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.4.6/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.4.6/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/trainer.py` & `daisyfl-0.4.6/src/py/daisyfl/client/trainer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/client/zone_client.py` & `daisyfl-0.4.6/src/py/daisyfl/client/zone_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/common/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/dp.py` & `daisyfl-0.4.6/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/logger.py` & `daisyfl-0.4.6/src/py/daisyfl/common/logger.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/metadata.py` & `daisyfl-0.4.6/src/py/daisyfl/common/metadata.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/parameter.py` & `daisyfl-0.4.6/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/serde.py` & `daisyfl-0.4.6/src/py/daisyfl/common/serde.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/common/typing.py` & `daisyfl-0.4.6/src/py/daisyfl/common/typing.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/base/client_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/base/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/base/server_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/base/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/base_async/client_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/base_async/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/base_async/server_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/client_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/server_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_client_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/zone_client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/msg_demo/zone_server_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/msg_demo/zone_server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/client_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/common.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/primitives.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/sec_agg/server_logic.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/aggregate.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadagrad.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedadam.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedasync.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavg_android.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedavgm.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedopt.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/fedyogi.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/qfedavg.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/strategy/strategy.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/utils/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/operator/utils/op_tools.py` & `daisyfl-0.4.6/src/py/daisyfl/operator/utils/op_tools.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.4.6/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/app.py` & `daisyfl-0.4.6/src/py/daisyfl/server/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/client_manager.py` & `daisyfl-0.4.6/src/py/daisyfl/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/client_proxy.py` & `daisyfl-0.4.6/src/py/daisyfl/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/flower_service_servicer.py` & `daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.4.6/src/py/daisyfl/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/history.py` & `daisyfl-0.4.6/src/py/daisyfl/server/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/server.py` & `daisyfl-0.4.6/src/py/daisyfl/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import concurrent.futures
 import timeit
 from threading import Event, Condition, Lock, Timer
 from queue import Queue
 from logging import DEBUG, INFO
 from typing import Dict, List, Optional, Tuple, Union, Callable
-
+import gc
 from daisyfl.common import (
     Task,
     Report,
     CURRENT_ROUND,
     EVALUATE,
     TIMEOUT,
     FIT_SAMPLES,
@@ -109,14 +109,15 @@
     def unregister_subtask(self, subtask_id: int) -> None:
         del self.subtasks[subtask_id]
         del self.queues[subtask_id]
         cid_list = self.client_previous_subtask.keys()
         for cid in cid_list:
             if self.client_previous_subtask[cid] == subtask_id:
                 del self.client_previous_subtask[cid]
+        gc.collect()
         return
 
     def submit_subtask(
         self, result: Tuple[ClientProxy, Union[FitRes, EvaluateRes]],
     ) -> None:
         client_proxy, res = result
         if (not self.client_previous_subtask.__contains__(client_proxy.cid)):
```

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/server_api_handler.py` & `daisyfl-0.4.6/src/py/daisyfl/server/server_api_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/server_operator_manager.py` & `daisyfl-0.4.6/src/py/daisyfl/server/server_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/server/task_manager.py` & `daisyfl-0.4.6/src/py/daisyfl/server/task_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/simulation/app.py` & `daisyfl-0.4.6/src/py/daisyfl/simulation/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py` & `daisyfl-0.4.6/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/src/py/daisyfl/utils/__init__.py` & `daisyfl-0.4.6/src/py/daisyfl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.5/setup.py` & `daisyfl-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
  'simulation': ['ray[default]>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'daisyfl',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': 'Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing',
     'long_description': "# Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing\n\n\n## dev mode (virtual environment)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\nprepare and activate your virtual environment (python=3.8^)\n```\ncd daisy\n./dev/bootstrap.sh\n```\n### develop<br>\n### setup examples\ndon't overwrite daisyfl dependency in this step.<br>\n```\ncd <example_path>\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## dev mode (docker)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\n```\ndocker run -it -v <daisy_source_code>:/root/daisy tcfwbper/daisyfl-dev:<version_tag> /bin/bash\n```\n### 3. develop<br>\n### 4. setup examples<br>\ndon't overwrite daisyfl dependency in this step.<br>\n```\ndocker attach <container_id>\n```\n```\ncd <example_path> && conda activate daisy\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## user mode\n### 1. install daisyfl\n```\npip install <daisyfl_version>\n```\n### 2. setup examples\n```\npip install <pkgs_for_your_example>\n```\n### 3. run examples",
     'author': 'tcfwbper',
     'author_email': 'b05208031@ntu.edu.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Intelligent-Systems-Lab/daisy',
```

### Comparing `daisyfl-0.4.5/PKG-INFO` & `daisyfl-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisyfl
-Version: 0.4.5
+Version: 0.4.6
 Summary: Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
 Home-page: https://github.com/Intelligent-Systems-Lab/daisy
 License: Apache-2.0
 Author: tcfwbper
 Author-email: b05208031@ntu.edu.tw
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


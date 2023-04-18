# Comparing `tmp/flwr_nightly-1.4.0.dev20230416.tar.gz` & `tmp/flwr_nightly-1.4.0.dev20230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.4.0.dev20230416.tar", max compression
+gzip compressed data, was "flwr_nightly-1.4.0.dev20230417.tar", max compression
```

## Comparing `flwr_nightly-1.4.0.dev20230416.tar` & `flwr_nightly-1.4.0.dev20230417.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0    11358 2023-04-16 23:02:13.655753 flwr_nightly-1.4.0.dev20230416/LICENSE
--rw-r--r--   0        0        0    10297 2023-04-16 23:02:13.655753 flwr_nightly-1.4.0.dev20230416/README.md
--rw-r--r--   0        0        0     4373 2023-04-16 23:02:37.559789 flwr_nightly-1.4.0.dev20230416/pyproject.toml
--rw-r--r--   0        0        0      929 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    11880 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     6503 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3351 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4117 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      712 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1686 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5100 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     7455 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2816 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0      884 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1827 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1894 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3481 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7683 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      846 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      769 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     3909 2023-04-16 23:02:13.907776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0      676 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     3217 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1331 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    17328 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0     1638 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/fleet/fleet_servicer.py
--rw-r--r--   0        0        0      728 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/__init__.py
--rw-r--r--   0        0        0     4450 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/driver_client_manager.py
--rw-r--r--   0        0        0     5594 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4623 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11509 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     6314 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/ins_scheduler.py
--rw-r--r--   0        0        0     4456 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/history.py
--rw-r--r--   0        0        0      728 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/rest_server/__init__.py
--rw-r--r--   0        0        0     4640 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/rest_server/rest_api.py
--rw-r--r--   0        0        0    15855 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      995 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6521 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19296 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4805 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1648 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1588 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     4994 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4519 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4874 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5978 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6730 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7012 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11495 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9985 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8953 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     6469 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5393 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7708 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     7772 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7044 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     7011 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10744 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5112 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4939 2023-04-16 23:02:13.911776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1270 2023-04-16 23:02:13.915776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7773 2023-04-16 23:02:13.915776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-04-16 23:02:13.915776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5472 2023-04-16 23:02:13.915776 flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12355 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230416/setup.py
--rw-r--r--   0        0        0    12857 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230416/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-17 23:02:20.049011 flwr_nightly-1.4.0.dev20230417/LICENSE
+-rw-r--r--   0        0        0    10297 2023-04-17 23:02:20.049011 flwr_nightly-1.4.0.dev20230417/README.md
+-rw-r--r--   0        0        0     4373 2023-04-17 23:02:49.169434 flwr_nightly-1.4.0.dev20230417/pyproject.toml
+-rw-r--r--   0        0        0      929 2023-04-17 23:02:20.377016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-04-17 23:02:20.377016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    12224 2023-04-17 23:02:20.377016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     6503 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4117 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      712 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1686 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5100 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     7455 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2816 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     2258 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0      884 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1827 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1894 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3481 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16316 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7683 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      846 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      769 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     3909 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0      676 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3217 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4286 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    19238 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     5941 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2228 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1058 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0     1638 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/fleet/fleet_servicer.py
+-rw-r--r--   0        0        0      728 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0     4450 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/driver_client_manager.py
+-rw-r--r--   0        0        0     5594 2023-04-17 23:02:20.381016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6416 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4623 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11509 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     6314 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/ins_scheduler.py
+-rw-r--r--   0        0        0     4456 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0      728 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/rest_server/__init__.py
+-rw-r--r--   0        0        0     4640 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/rest_server/rest_api.py
+-rw-r--r--   0        0        0    15855 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      995 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6521 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4805 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1648 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1588 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     4994 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4519 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4874 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5978 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6730 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7012 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11495 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9985 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8953 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     6469 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5393 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7708 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     7772 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7044 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     7011 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10744 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5112 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4939 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1270 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7773 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5472 2023-04-17 23:02:20.385016 flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12355 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230417/setup.py
+-rw-r--r--   0        0        0    12857 1970-01-01 00:00:00.000000 flwr_nightly-1.4.0.dev20230417/PKG-INFO
```

### Comparing `flwr_nightly-1.4.0.dev20230416/LICENSE` & `flwr_nightly-1.4.0.dev20230417/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/README.md` & `flwr_nightly-1.4.0.dev20230417/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/pyproject.toml` & `flwr_nightly-1.4.0.dev20230417/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.4.0-dev20230416"
+version = "1.4.0-dev20230417"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
```

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/app.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client app."""
 
 
+import sys
 import time
 from logging import INFO
 from typing import Callable, Dict, Optional, Union
 
 from flwr.common import (
     GRPC_MAX_MESSAGE_LENGTH,
     EventType,
     event,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
+from flwr.common.address import parse_address
 from flwr.common.logger import log
 from flwr.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
@@ -76,15 +78,15 @@
 
 """
 
 
 ClientLike = Union[Client, NumPyClient]
 
 
-# pylint: disable=import-outside-toplevel
+# pylint: disable=import-outside-toplevel,too-many-locals
 def start_client(
     *,
     server_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
     rest: bool = False,
@@ -133,14 +135,21 @@
     >>>     client=FlowerClient(),
     >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
     >>> )
     """
 
     event(EventType.START_CLIENT_ENTER)
 
+    # Parse IP address
+    parsed_address = parse_address(server_address)
+    if not parsed_address:
+        sys.exit(f"Server address ({server_address}) cannot be parsed.")
+    host, port, is_v6 = parsed_address
+    address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+
     # Use either gRPC bidirectional streaming or REST request/response
     if rest:
         try:
             from .rest_client.connection import http_request_response
         except ImportError as missing_dep:
             raise ImportError(
                 "To use the REST API you must install the "
@@ -148,15 +157,15 @@
             ) from missing_dep
         connection = http_request_response
     else:
         connection = grpc_connection
     while True:
         sleep_duration: int = 0
         with connection(
-            server_address,
+            address,
             max_message_length=grpc_max_message_length,
             root_certificates=root_certificates,
         ) as conn:
             receive, send = conn
 
             while True:
                 server_message = receive()
```

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/client.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/date.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/dp.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/grpc.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/logger.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/parameter.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/serde.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/typing.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/common/version.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/driver/driver.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server."""
 
 
+from . import strategy
 from .app import ServerConfig as ServerConfig
 from .app import run_driver_api as run_driver_api
 from .app import run_fleet_api as run_fleet_api
 from .app import run_server as run_server
 from .app import start_server as start_server
 from .client_manager import ClientManager as ClientManager
 from .client_manager import SimpleClientManager as SimpleClientManager
@@ -31,8 +32,9 @@
     "run_driver_api",
     "run_fleet_api",
     "run_server",
     "Server",
     "ServerConfig",
     "SimpleClientManager",
     "start_server",
+    "strategy",
 ]
```

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/app.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from signal import SIGINT, SIGTERM, signal
 from types import FrameType
 from typing import List, Optional, Tuple
 
 import grpc
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
+from flwr.common.address import parse_address
 from flwr.common.logger import log
 from flwr.proto.driver_pb2_grpc import add_DriverServicer_to_server
 from flwr.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
 from flwr.server.client_manager import ClientManager, SimpleClientManager
 from flwr.server.driver.driver_servicer import DriverServicer
 from flwr.server.grpc_server.driver_client_manager import DriverClientManager
 from flwr.server.grpc_server.flower_service_servicer import FlowerServiceServicer
@@ -59,15 +60,15 @@
     just the ones they care about.
     """
 
     num_rounds: int = 1
     round_timeout: Optional[float] = None
 
 
-def start_server(  # pylint: disable=too-many-arguments
+def start_server(  # pylint: disable=too-many-arguments,too-many-locals
     *,
     server_address: str = ADDRESS_FLEET_API_GRPC_BIDI,
     server: Optional[Server] = None,
     config: Optional[ServerConfig] = None,
     strategy: Optional[Strategy] = None,
     client_manager: Optional[ClientManager] = None,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
@@ -143,18 +144,25 @@
     )
     log(
         INFO,
         "Starting Flower server, config: %s",
         initialized_config,
     )
 
+    # Parse IP address
+    parsed_address = parse_address(server_address)
+    if not parsed_address:
+        sys.exit(f"Server IP address ({server_address}) cannot be parsed.")
+    host, port, is_v6 = parsed_address
+    address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+
     # Start gRPC server
     grpc_server = start_grpc_server(
         client_manager=initialized_server.client_manager(),
-        server_address=server_address,
+        server_address=address,
         max_message_length=grpc_max_message_length,
         certificates=certificates,
     )
     log(
         INFO,
         "Flower ECE: gRPC server running (%s rounds), SSL is %s",
         initialized_config.num_rounds,
@@ -219,20 +227,27 @@
 def run_driver_api() -> None:
     """Run Flower server (Driver API)."""
 
     log(INFO, "Starting Flower server (Driver API)")
     event(EventType.RUN_DRIVER_API_ENTER)
     args = _parse_args_driver().parse_args()
 
+    # Parse IP address
+    parsed_address = parse_address(args.driver_api_address)
+    if not parsed_address:
+        sys.exit(f"Driver IP address ({args.driver_api_address}) cannot be parsed.")
+    host, port, is_v6 = parsed_address
+    address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
     # Start server
     grpc_server: grpc.Server = _run_driver_api_grpc(
-        address=args.driver_api_address,
+        address=address,
         state_factory=state_factory,
     )
 
     # Graceful shutdown
     _register_exit_handlers(
         grpc_servers=[grpc_server],
         bckg_threads=[],
@@ -254,23 +269,34 @@
     state_factory = StateFactory(args.database)
 
     grpc_servers = []
     bckg_threads = []
 
     # Start Fleet API
     if args.fleet_api_type == "rest":
+        address_arg = args.rest_fleet_api_address
+        parsed_address = parse_address(address_arg)
+        if not parsed_address:
+            sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
+        host, port, _ = parsed_address
         fleet_thread = threading.Thread(
             target=_run_fleet_api_rest,
-            args=(args.rest_fleet_api_address, state_factory),
+            args=(host, port, state_factory),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
     elif args.fleet_api_type == "grpc":
+        address_arg = args.grpc_fleet_api_address
+        parsed_address = parse_address(address_arg)
+        if not parsed_address:
+            sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
+        host, port, is_v6 = parsed_address
+        address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_bidi(
-            address=args.grpc_fleet_api_address,
+            address=address,
             state_factory=state_factory,
         )
         grpc_servers.append(fleet_server)
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
@@ -290,37 +316,55 @@
 def run_server() -> None:
     """Run Flower server (Driver API and Fleet API)."""
 
     log(INFO, "Starting Flower server")
     event(EventType.RUN_SERVER_ENTER)
     args = _parse_args_server().parse_args()
 
+    # Parse IP address
+    parsed_address = parse_address(args.driver_api_address)
+    if not parsed_address:
+        sys.exit(f"Driver IP address ({args.driver_api_address}) cannot be parsed.")
+    host, port, is_v6 = parsed_address
+    address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
+
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
     # Start Driver API
     driver_server: grpc.Server = _run_driver_api_grpc(
-        address=args.driver_api_address,
+        address=address,
         state_factory=state_factory,
     )
 
     grpc_servers = [driver_server]
     bckg_threads = []
 
     # Start Fleet API
     if args.fleet_api_type == "rest":
+        address_arg = args.rest_fleet_api_address
+        parsed_address = parse_address(address_arg)
+        if not parsed_address:
+            sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
+        host, port, _ = parsed_address
         fleet_thread = threading.Thread(
             target=_run_fleet_api_rest,
-            args=(args.rest_fleet_api_address, state_factory),
+            args=(host, port, state_factory),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
     elif args.fleet_api_type == "grpc":
+        address_arg = args.grpc_fleet_api_address
+        parsed_address = parse_address(address_arg)
+        if not parsed_address:
+            sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
+        host, port, is_v6 = parsed_address
+        address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_bidi(
-            address=args.grpc_fleet_api_address,
+            address=address,
             state_factory=state_factory,
         )
         grpc_servers.append(fleet_server)
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
@@ -432,15 +476,16 @@
     fleet_grpc_server.start()
 
     return fleet_grpc_server
 
 
 # pylint: disable=import-outside-toplevel
 def _run_fleet_api_rest(
-    address: str,
+    host: str,
+    port: int,
     state_factory: StateFactory,
 ) -> None:
     """Run Driver API (REST-based)."""
     try:
         import uvicorn
 
         from flwr.server.rest_server.rest_api import app as fast_api_app
@@ -451,17 +496,14 @@
             "`pip install flwr['rest']`."
         ) from missing_dep
     log(INFO, "Starting Flower REST server")
 
     # See: https://www.starlette.io/applications/#accessing-the-app-instance
     fast_api_app.state.STATE_FACTORY = state_factory
 
-    host, port_str = address.split(":")
-    port = int(port_str)
-
     uvicorn.run(
         # "flwr.server.rest_server.rest_api:app",
         app=fast_api_app,
         port=port,
         host=host,
         reload=False,
         access_log=True,
```

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/criterion.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/fleet/fleet_servicer.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/fleet/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/driver_client_manager.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/flower_service_servicer.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/grpc_bridge.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/grpc_client_proxy.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/grpc_server.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/grpc_server/ins_scheduler.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/grpc_server/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/history.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/rest_server/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/rest_server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/rest_server/rest_api.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/rest_server/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/server.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/state.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/app.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.4.0.dev20230417/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.4.0.dev20230416/setup.py` & `flwr_nightly-1.4.0.dev20230417/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.4.0.dev20230416',
+    'version': '1.4.0.dev20230417',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
 'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
 [standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.3.0,<3.0.0'],
 'xgboost': ['xgboost>=1.6.2,<2.0.0']} entry_points = \ {'console_scripts':
 ['flower-client = flwr.client:run_client', 'flower-driver-api = flwr.server:
 run_driver_api', 'flower-fleet-api = flwr.server:run_fleet_api', 'flower-server
 = flwr.server:run_server']} setup_kwargs = { 'name': 'flwr-nightly', 'version':
-'1.4.0.dev20230416', 'description': 'Flower: A Friendly Federated Learning
+'1.4.0.dev20230417', 'description': 'Flower: A Friendly Federated Learning
 Framework', 'long_description': '# Flower: A Friendly Federated Learning
 Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
```

### Comparing `flwr_nightly-1.4.0.dev20230416/PKG-INFO` & `flwr_nightly-1.4.0.dev20230417/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.4.0.dev20230416
+Version: 1.4.0.dev20230417
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.4.0.dev20230416 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.4.0.dev20230417 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```


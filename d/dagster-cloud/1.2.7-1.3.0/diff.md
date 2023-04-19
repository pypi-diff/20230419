# Comparing `tmp/dagster_cloud-1.2.7.tar.gz` & `tmp/dagster_cloud-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.2.7.tar", last modified: Thu Apr 13 15:16:38 2023, max compression
+gzip compressed data, was "dagster_cloud-1.3.0.tar", last modified: Wed Apr 19 19:14:14 2023, max compression
```

## Comparing `dagster_cloud-1.2.7.tar` & `dagster_cloud-1.3.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.177919 dagster_cloud-1.2.7/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-04-13 15:16:38.177919 dagster_cloud-1.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.085919 dagster_cloud-1.2.7/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.089918 dagster_cloud-1.2.7/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.089918 dagster_cloud-1.2.7/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42939 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.093919 dagster_cloud-1.2.7/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16985 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.093919 dagster_cloud-1.2.7/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.097919 dagster_cloud-1.2.7/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.097919 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.097919 dagster_cloud-1.2.7/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14189 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.101919 dagster_cloud-1.2.7/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.101919 dagster_cloud-1.2.7/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18148 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.101919 dagster_cloud-1.2.7/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.105919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.105919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.109919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.109919 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.113919 dagster_cloud-1.2.7/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.113919 dagster_cloud-1.2.7/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.117919 dagster_cloud-1.2.7/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.117919 dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.121919 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26776 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.125919 dagster_cloud-1.2.7/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19167 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.129919 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     6552 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.129919 dagster_cloud-1.2.7/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.133919 dagster_cloud-1.2.7/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.133919 dagster_cloud-1.2.7/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.137919 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.137919 dagster_cloud-1.2.7/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.161919 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22459 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    19970 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.165919 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11403 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.173919 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    70432 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:16:38.089918 dagster_cloud-1.2.7/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-13 15:16:38.000000 dagster_cloud-1.2.7/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 15:16:38.177919 dagster_cloud-1.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-04-13 15:03:43.000000 dagster_cloud-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.799949 dagster_cloud-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-04-19 19:14:14.799949 dagster_cloud-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.683947 dagster_cloud-1.3.0/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.687948 dagster_cloud-1.3.0/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.703948 dagster_cloud-1.3.0/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43090 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.703948 dagster_cloud-1.3.0/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16985 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.711948 dagster_cloud-1.3.0/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.715948 dagster_cloud-1.3.0/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.723948 dagster_cloud-1.3.0/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.723948 dagster_cloud-1.3.0/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14189 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.723948 dagster_cloud-1.3.0/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.723948 dagster_cloud-1.3.0/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18148 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.723948 dagster_cloud-1.3.0/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.727948 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.731948 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.739948 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.743948 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.747948 dagster_cloud-1.3.0/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.747948 dagster_cloud-1.3.0/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.751948 dagster_cloud-1.3.0/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.751948 dagster_cloud-1.3.0/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.759948 dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    26776 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.763948 dagster_cloud-1.3.0/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19137 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.763948 dagster_cloud-1.3.0/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.767948 dagster_cloud-1.3.0/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.767948 dagster_cloud-1.3.0/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.767948 dagster_cloud-1.3.0/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.771948 dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.771948 dagster_cloud-1.3.0/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12011 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.783949 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22459 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    20446 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.787949 dagster_cloud-1.3.0/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.799949 dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74043 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:14:14.683947 dagster_cloud-1.3.0/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-04-19 19:14:14.000000 dagster_cloud-1.3.0/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-04-19 19:14:14.000000 dagster_cloud-1.3.0/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:14:14.000000 dagster_cloud-1.3.0/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:14:14.000000 dagster_cloud-1.3.0/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-19 19:14:14.000000 dagster_cloud-1.3.0/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 19:14:14.799949 dagster_cloud-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-04-19 19:01:49.000000 dagster_cloud-1.3.0/setup.py
```

### Comparing `dagster_cloud-1.2.7/PKG-INFO` & `dagster_cloud-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.2.7
+Version: 1.3.0
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.2.7/README.md` & `dagster_cloud-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.3.0/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,18 @@
 
         self._check_initial_deployment_names(instance)
 
         self._check_update_workspace(
             instance, user_code_launcher, upload_all=user_code_launcher.upload_snapshots_on_startup
         )
 
-        self._logger.info(f"Started polling for requests from {instance.dagster_cloud_url}")
+        self._logger.info(
+            f"Will start polling for requests from {instance.dagster_cloud_url} once user code has"
+            " been loaded."
+        )
 
         while True:
             try:
                 for error in self.run_iteration(instance, user_code_launcher):
                     if error:
                         self._logger.error(str(error))
                         self._errors.appendleft((error, pendulum.now("UTC")))
@@ -869,14 +872,17 @@
             return None
 
         return location_origin.location_name
 
     def run_iteration(
         self, instance: DagsterCloudAgentInstance, user_code_launcher: DagsterCloudUserCodeLauncher
     ) -> Iterator[Optional[SerializableErrorInfo]]:
+        if not user_code_launcher.ready_to_serve_requests:
+            return
+
         num_pending_requests = len(self._pending_requests)
 
         if num_pending_requests < self._pending_requests_limit:
             if instance.includes_branch_deployments:
                 result = instance.organization_scoped_graphql_client().execute(
                     GET_USER_CLOUD_REQUESTS_QUERY,
                     {"forBranchDeployments": True},
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud/agent/queries.py` & `dagster_cloud-1.3.0/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.3.0/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/auth/constants.py` & `dagster_cloud-1.3.0/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.3.0/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.3.0/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.3.0/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.3.0/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.3.0/dagster_cloud/serverless/io_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,96 @@
+import datetime
 import io
 import os
 import pickle
-from typing import Sequence, Union
+from typing import Sequence, Tuple, Union
 
 import boto3
 import dagster._check as check
 import requests
 from dagster import InputContext, MemoizableIOManager, OutputContext, io_manager
 from dagster._utils import PICKLE_PROTOCOL
+from dateutil import parser
+
+ECS_AGENT_IP = "169.254.170.2"
 
 
 class PickledObjectServerlessIOManager(MemoizableIOManager):
     def __init__(
         self,
         s3_bucket,
-        s3_session,
-        s3_prefix=None,
+        s3_prefix,
     ):
-        self.bucket = check.str_param(s3_bucket, "s3_bucket")
-        self.s3_prefix = check.opt_str_param(s3_prefix, "s3_prefix")
-        self.s3 = s3_session
+        self._bucket = check.str_param(s3_bucket, "s3_bucket")
+        self._s3_prefix = check.str_param(s3_prefix, "s3_prefix")
+        self._boto_session, self._boto_session_expiration = self._refresh_boto_session()
+
+    def _refresh_boto_session(self) -> Tuple[boto3.Session, datetime.datetime]:
+        # We have to do this whacky way to get credentials to ensure that we get iam role
+        # we assigned to the task. If we used the default boto behavior, it could get overriden
+        # when users set AWS env vars.
+        relative_uri = os.environ["AWS_CONTAINER_CREDENTIALS_RELATIVE_URI"]
+        aws_creds = requests.get(f"http://{ECS_AGENT_IP}{relative_uri}").json()
+        session = boto3.Session(
+            aws_access_key_id=aws_creds["AccessKeyId"],
+            aws_secret_access_key=aws_creds["SecretAccessKey"],
+            aws_session_token=aws_creds["Token"],
+        )
+        expiration = parser.parse(aws_creds["Expiration"])
+        return session, expiration
+
+    @property
+    def _s3(self):
+        if self._boto_session_expiration <= datetime.datetime.now(
+            self._boto_session_expiration.tzinfo
+        ) + datetime.timedelta(minutes=5):
+            self._boto_session, self._boto_session_expiration = self._refresh_boto_session()
+        return self._boto_session.client("s3")
 
     def _get_path(self, context: Union[InputContext, OutputContext]) -> str:
         path: Sequence[str]
         if context.has_asset_key:
             path = context.get_asset_identifier()
         else:
             path = ["storage", *context.get_identifier()]
 
-        return "/".join([self.s3_prefix, *path])
+        return "/".join([self._s3_prefix, *path])
 
     def has_output(self, context):
         key = self._get_path(context)
         return self._has_object(key)
 
     def _rm_object(self, key):
         check.str_param(key, "key")
         check.param_invariant(len(key) > 0, "key")
 
         # delete_object wont fail even if the item has been deleted.
-        self.s3.delete_object(Bucket=self.bucket, Key=key)
+        self._s3.delete_object(Bucket=self._bucket, Key=key)
 
     def _has_object(self, key):
         check.str_param(key, "key")
         check.param_invariant(len(key) > 0, "key")
 
         found_object = False
 
         try:
-            self.s3.get_object(Bucket=self.bucket, Key=key)
+            self._s3.get_object(Bucket=self._bucket, Key=key)
             found_object = True
-        except self.s3.exceptions.NoSuchKey:
+        except self._s3.exceptions.NoSuchKey:
             found_object = False
 
         return found_object
 
     def load_input(self, context):
         if context.dagster_type.typing_type == type(None):
             return None
 
         key = self._get_path(context)
-        obj = pickle.loads(self.s3.get_object(Bucket=self.bucket, Key=key)["Body"].read())
+        check.invariant(self._has_object(key), "Input not found. It may have expired.")
+        obj = pickle.loads(self._s3.get_object(Bucket=self._bucket, Key=key)["Body"].read())
 
         return obj
 
     def handle_output(self, context, obj):
         if context.dagster_type.typing_type == type(None):
             check.invariant(
                 obj is None,
@@ -78,29 +104,19 @@
         key = self._get_path(context)
 
         if self._has_object(key):
             self._rm_object(key)
 
         pickled_obj = pickle.dumps(obj, PICKLE_PROTOCOL)
         pickled_obj_bytes = io.BytesIO(pickled_obj)
-        self.s3.upload_fileobj(pickled_obj_bytes, self.bucket, key)
-
-
-ECS_AGENT_IP = "169.254.170.2"
-
-
-def _get_s3_client():
-    relative_uri = os.environ["AWS_CONTAINER_CREDENTIALS_RELATIVE_URI"]
-    aws_creds = requests.get(f"http://{ECS_AGENT_IP}{relative_uri}").json()
-    session = boto3.Session(
-        aws_access_key_id=aws_creds["AccessKeyId"],
-        aws_secret_access_key=aws_creds["SecretAccessKey"],
-        aws_session_token=aws_creds["Token"],
-    )
-    return session.client("s3")
+        self._s3.upload_fileobj(
+            pickled_obj_bytes,
+            self._bucket,
+            key,
+        )
 
 
 @io_manager
 def serverless_io_manager(init_context):
     bucket = os.getenv("DAGSTER_CLOUD_SERVERLESS_STORAGE_S3_BUCKET")
     prefix = os.getenv("DAGSTER_CLOUD_SERVERLESS_STORAGE_S3_PREFIX")
     check.invariant(
@@ -111,9 +127,9 @@
             " DAGSTER_CLOUD_SERVERLESS_STORAGE_S3_PREFIX not found."
         ),
     )
 
     deployment_name = init_context.instance.deployment_name
 
     return PickledObjectServerlessIOManager(
-        bucket, _get_s3_client(), s3_prefix=f"{prefix}/io_storage/{deployment_name}"
+        bucket, s3_prefix=f"{prefix}/io_storage/{deployment_name}"
     )
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/client.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/runs/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,21 +504,18 @@
     def update_backfill(self, partition_backfill: PartitionBackfill):
         """Update a partition backfill in run storage."""
         self._execute_query(
             UPDATE_BACKFILL_MUTATION,
             variables={"serializedPartitionBackfill": serialize_value(partition_backfill)},
         )
 
-    def supports_kvs(self):
-        return False
-
-    def kvs_get(self, keys: Set[str]):
+    def get_cursor_values(self, keys: Set[str]):
         return NotImplementedError("KVS is not supported from the user cloud")
 
-    def kvs_set(self, pairs: Mapping[str, str]):
+    def set_cursor_values(self, pairs: Mapping[str, str]):
         return NotImplementedError("KVS is not supported from the user cloud")
 
     # Migrating run history
     def replace_job_origin(self, run: DagsterRun, job_origin: ExternalPipelineOrigin):
         self._execute_query(
             MUTATE_JOB_ORIGIN,
             variables={
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.3.0/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/util/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Any, Collection, Dict, List, Mapping, Optional, Sequence
 
 import boto3
 from dagster import (
     Array,
     Enum,
     EnumValue,
@@ -217,14 +218,23 @@
     def from_config_value(cls, inst_data: ConfigurableClassData, config_value: Dict[str, Any]):
         return EcsUserCodeLauncher(inst_data=inst_data, **config_value)
 
     @property
     def inst_data(self) -> Optional[ConfigurableClassData]:
         return self._inst_data
 
+    def _write_liveness_sentinel(self) -> None:
+        # Write to a sentinel file to indicate that we've finished our initial
+        # reconciliation - this is used in serverless to indicate that we're ready to
+        # serve requests
+        Path("/opt/finished_initial_reconciliation_sentinel.txt").touch(exist_ok=True)
+        self._logger.info(
+            "Wrote liveness sentinel: indicating that agent is ready to serve requests"
+        )
+
     def _get_grpc_server_sidecars(self) -> Optional[List[Dict[str, Any]]]:
         return None
 
     def _get_service_cpu_override(self, container_context: EcsContainerContext) -> Optional[str]:
         return container_context.server_resources.get("cpu")
 
     def _get_service_memory_override(self, container_context: EcsContainerContext) -> Optional[str]:
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
     except Exception:
         logger.exception(
             "Error trying to get debug information for failed k8s pod {pod_name}".format(
                 pod_name=pod_name
             )
         )
 
-    return f"{pod_debug_info}\n{kubectl_prompt}" if pod_debug_info else kubectl_prompt
+    return f"{pod_debug_info}\n\n{kubectl_prompt}" if pod_debug_info else kubectl_prompt
 
 
 def wait_for_deployment_complete(
     k8s_deployment_name,
     namespace,
     logger,
     location_name,
@@ -259,15 +259,15 @@
 
         if time_elapsed >= timeout:
             timeout_message: str = f"Timed out waiting for deployment {k8s_deployment_name}."
             debug_info = get_deployment_failure_debug_info(
                 k8s_deployment_name, namespace, core_api, pod_list, logger
             )
             if debug_info:
-                timeout_message = timeout_message + "\n" + debug_info
+                timeout_message = timeout_message + "\n\n" + debug_info
 
             raise Exception(timeout_message)
 
         deployment = api.read_namespaced_deployment(k8s_deployment_name, namespace)
         status = deployment.status
         spec = deployment.spec
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,17 @@
 
 
 USER_CODE_LAUNCHER_RECONCILE_SLEEP_SECONDS = 1
 
 # Check on pending delete servers every 30th reconcile
 PENDING_DELETE_SERVER_CHECK_INTERVAL = 30
 
+# How often to sync actual_entries with pex server liveness
+MULTIPEX_ACTUAL_ENTRIES_REFRESH_INTERVAL = 30
+
 ServerHandle = TypeVar("ServerHandle")
 
 DEPLOYMENT_INFO_QUERY = """
     query DeploymentInfo {
          deploymentInfo {
              deploymentType
          }
@@ -209,14 +212,24 @@
         is_required=False,
         default_value=True,
         description=(
             "Upload information about code locations to Dagster Cloud whenever the "
             "agent starts up, even if the code location has not changed since the last upload."
         ),
     ),
+    "requires_healthcheck": Field(
+        BoolSource,
+        is_required=False,
+        default_value=False,
+        description=(
+            "Whether the agent update process expects a liveness sentinel to be written before an"
+            " agent is considered healthy. If using zero-downtime agent updates, this should be set"
+            " to True."
+        ),
+    ),
 }
 
 DeploymentAndLocation = Tuple[str, str]
 
 
 class ServerEndpoint(
     NamedTuple(
@@ -281,32 +294,35 @@
 ):
     def __init__(
         self,
         server_ttl: Optional[dict] = None,
         defer_job_snapshots: bool = True,
         server_process_startup_timeout=None,
         upload_snapshots_on_startup: bool = True,
+        requires_healthcheck: bool = False,
     ):
         self._grpc_servers: Dict[
             DeploymentAndLocation, Union[DagsterCloudGrpcServer, SerializableErrorInfo]
         ] = {}
         self._pending_delete_grpc_server_handles: Set[ServerHandle] = set()
         self._grpc_servers_lock = threading.Lock()
 
         self._multipex_servers: Dict[DeploymentAndLocation, DagsterCloudGrpcServer] = {}
 
         self._server_ttl_config = check.opt_dict_param(server_ttl, "server_ttl")
         self._defer_job_snapshots = defer_job_snapshots
         self.upload_snapshots_on_startup = check.bool_param(
             upload_snapshots_on_startup, "upload_snapshots_on_startup"
         )
+        self._requires_healthcheck = check.bool_param(requires_healthcheck, "requires_healthcheck")
 
         # periodically reconciles to make desired = actual
         self._desired_entries: Dict[DeploymentAndLocation, UserCodeLauncherEntry] = {}
         self._actual_entries: Dict[DeploymentAndLocation, UserCodeLauncherEntry] = {}
+        self._last_refreshed_actual_entries = 0
         self._metadata_lock = threading.Lock()
 
         self._upload_locations: Set[DeploymentAndLocation] = set()
 
         self._logger = logging.getLogger("dagster_cloud.user_code_launcher")
         self._event_logger = logging.getLogger("cloud-events")
         self._started: bool = False
@@ -833,24 +849,30 @@
                 self._logger.info(f"No runs, shutting down server {server_handle}")
             self._remove_server_handle(server_handle)
             with self._grpc_servers_lock:
                 self._pending_delete_grpc_server_handles.discard(server_handle)
 
     def _cleanup_servers(self, active_agent_ids: Set[str]) -> None:
         """Remove all servers, across all deployments and locations."""
-        for handle in self._list_server_handles():
-            self._logger.info(f"Attempting to cleanup server {handle}")
-            if self._can_cleanup_server(handle, active_agent_ids):
-                try:
+        with ThreadPoolExecutor() as executor:
+            futures = []
+            for handle in self._list_server_handles():
+                self._logger.info(f"Attempting to cleanup server {handle}")
+                if self._can_cleanup_server(handle, active_agent_ids):
                     self._logger.info(f"Can remove server {handle}. Cleaning up.")
-                    self._remove_server_handle(handle)
+                    futures.append(executor.submit(self._remove_server_handle, handle))
+                else:
+                    self._logger.info(f"Cannot remove server {handle}. Not cleaning up.")
+
+            wait(futures)
+            for future in futures:
+                try:
+                    future.result()
                 except:
                     self._logger.exception("Error cleaning up server")
-            else:
-                self._logger.info(f"Cannot remove server {handle}. Not cleaning up.")
 
     @abstractmethod
     def _list_server_handles(self) -> List[ServerHandle]:
         """Return a list of all server handles across all deployments and locations."""
 
     @abstractmethod
     def get_agent_id_for_server(self, handle: ServerHandle) -> Optional[str]:
@@ -954,33 +976,93 @@
             except Exception:
                 self._logger.error(
                     "Failure updating user code servers: {exc_info}".format(
                         exc_info=serializable_error_info_from_exc_info(sys.exc_info()),
                     )
                 )
 
-    def reconcile(self):
+    def reconcile(self) -> None:
         with self._metadata_lock:
             desired_entries = (
                 self._desired_entries.copy() if self._desired_entries is not None else None
             )
             upload_locations = self._upload_locations.copy()
             self._upload_locations = set()
 
         if desired_entries is None:
             # Wait for the first time the desired metadata is set before reconciling
             return
 
+        if (
+            time.time() - self._last_refreshed_actual_entries
+            > MULTIPEX_ACTUAL_ENTRIES_REFRESH_INTERVAL
+        ):
+            try:
+                self._refresh_actual_entries()
+            except:
+                self._logger.exception("Failed to refresh actual entries.")
+            self._last_refreshed_actual_entries = time.time()
+
         self._reconcile(
             desired_entries,
             upload_locations,
             check_on_pending_delete_servers=self._reconcile_count % self._reconcile_interval == 0,
         )
+        if self._reconcile_count == 0 and self._requires_healthcheck:
+            try:
+                self._write_liveness_sentinel()
+            except:
+                self._logger.exception("Failed to write liveness sentinel file.")
+
+        if self._reconcile_count == 0:
+            self._logger.info(
+                f"Started polling for requests from {self._instance.dagster_cloud_url}"
+            )
+
         self._reconcile_count += 1
 
+    @property
+    def ready_to_serve_requests(self) -> bool:
+        # thread-safe since reconcile_count is an integer
+        return self._reconcile_count > 0
+
+    def _refresh_actual_entries(self) -> None:
+        for deployment_location, server in self._multipex_servers.items():
+            if deployment_location in self._actual_entries:
+                # If a multipex server exists, we query it to make sure the pex server is still
+                # available
+                try:
+                    self._check_running_multipex_server(server)
+                except:
+                    # This is expected if ECS is currently spinning up this service after it crashed.
+                    # In this case, we want to wait for it to fully come up before we remove actual
+                    # entries. This ensures the recon loop uses the ECS replacement multiplex server
+                    # and not try to spin up a new multipex server.
+                    self._logger.info(
+                        "Multipex server entry exists but server is not running. "
+                        "Will wait for server to come up."
+                    )
+                    return
+                deployment_name, location_name = deployment_location
+                if not self._get_existing_pex_servers(deployment_name, location_name):
+                    self._logger.warning(
+                        (
+                            "Pex servers disappeared for %s, %s. Removing actual entries to"
+                            " activate reconciliation logic."
+                        ),
+                        deployment_name,
+                        location_name,
+                    )
+                    del self._actual_entries[deployment_location]
+
+    def _write_liveness_sentinel(self) -> None:
+        """Write a sentinel file to indicate that the agent is alive and grpc servers have been spun up.
+        """
+        pass
+
     def _check_for_image(self, metadata: CodeDeploymentMetadata):
         if self.requires_images and not metadata.image:
             raise Exception(
                 "Your agent's configuration requires you to specify an image. "
                 "Use the `--image` flag when specifying your location to tell the agent "
                 "which image to use to load your code."
             )
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.3.0/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.3.0/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.2.7
+Version: 1.3.0
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.2.7/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.3.0/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.2.7/setup.py` & `dagster_cloud-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.2.7",
-        "dagster-cloud-cli==1.2.7",
+        "dagster==1.3.0",
+        "dagster-cloud-cli==1.3.0",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.18.7",
+            "dagster_k8s==0.19.0",
         ],
-        "docker": ["docker", "dagster_docker==0.18.7"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.18.7"],
-        "ecs": ["dagster_aws==0.18.7", "boto3"],
+        "docker": ["docker", "dagster_docker==0.19.0"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.19.0"],
+        "ecs": ["dagster_aws==0.19.0", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```


# Comparing `tmp/globus-compute-endpoint-2.0.1a2.tar.gz` & `tmp/globus-compute-endpoint-2.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.1a2.tar", last modified: Tue Apr 18 21:51:21 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.1a3.tar", last modified: Tue Apr 18 22:06:06 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.1a2.tar` & `globus-compute-endpoint-2.0.1a3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.891209 globus-compute-endpoint-2.0.1a2/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a2/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1646 2023-04-18 21:51:21.891309 globus-compute-endpoint-2.0.1a2/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a2/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.875094 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    18802 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.877507 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    25351 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.878262 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.878549 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.878692 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.889230 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8401 2023-04-14 16:35:15.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.889389 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.889855 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.890593 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-18 21:17:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.875903 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1646 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2657 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-18 21:51:21.891612 globus-compute-endpoint-2.0.1a2/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3386 2023-04-18 21:17:41.000000 globus-compute-endpoint-2.0.1a2/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.891072 globus-compute-endpoint-2.0.1a2/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a2/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.902616 globus-compute-endpoint-2.0.1a3/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a3/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-18 22:06:06.902681 globus-compute-endpoint-2.0.1a3/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a3/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.896664 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    18802 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.898723 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    25351 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.899349 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.899591 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.899710 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.901128 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8401 2023-04-14 16:35:15.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.901248 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.901589 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.902175 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-18 22:04:21.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.897506 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2657 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-18 22:06:06.000000 globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-18 22:06:06.902937 globus-compute-endpoint-2.0.1a3/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3634 2023-04-18 22:04:18.000000 globus-compute-endpoint-2.0.1a3/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:06:06.902505 globus-compute-endpoint-2.0.1a3/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a3/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a3/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.1a2/LICENSE` & `globus-compute-endpoint-2.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/PKG-INFO` & `globus-compute-endpoint-2.0.1a3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a2
+Version: 2.0.1a3
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `globus-compute-endpoint-2.0.1a2/PyPI.md` & `globus-compute-endpoint-2.0.1a3/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a2"
+__version__ = "2.0.1a3"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a2
+Version: 2.0.1a3
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.1a3/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/setup.py` & `globus-compute-endpoint-2.0.1a3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk>=2.0.1a2",
+    "globus-compute-sdk>=2.0.1a3",
     "globus-compute-common==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
@@ -89,8 +89,12 @@
         ]
     },
     include_package_data=True,
     author="Globus Compute Team",
     author_email="support@globus.org",
     license="Apache License, Version 2.0",
     url="https://github.com/funcx-faas/funcx",
+    project_urls={
+        "Changelog": "https://globus-compute.readthedocs.io/en/latest/changelog.html",  # noqa: E501
+        "Upgrade to Globus Compute": "https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html",  # noqa: E501
+    },
 )
```

### Comparing `globus-compute-endpoint-2.0.1a2/tests/conftest.py` & `globus-compute-endpoint-2.0.1a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a2/tests/utils.py` & `globus-compute-endpoint-2.0.1a3/tests/utils.py`

 * *Files identical despite different names*


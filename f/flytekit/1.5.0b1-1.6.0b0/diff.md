# Comparing `tmp/flytekit-1.5.0b1.tar.gz` & `tmp/flytekit-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.5.0b1.tar", last modified: Wed Mar 29 18:58:29 2023, max compression
+gzip compressed data, was "flytekit-1.6.0b0.tar", last modified: Wed Apr 19 20:54:19 2023, max compression
```

## Comparing `flytekit-1.5.0b1.tar` & `flytekit-1.6.0b0.tar`

### file list

```diff
@@ -1,239 +1,244 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.956222 flytekit-1.5.0b1/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.956222 flytekit-1.5.0b1/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81942 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    26375 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.960222 flytekit-1.5.0b1/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    30288 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    35576 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    72988 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37299 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.964222 flytekit-1.5.0b1/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15166 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/interfaces/stats/taggable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.968222 flytekit-1.5.0b1/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    82798 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32227 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.956222 flytekit-1.5.0b1/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-29 18:58:20.000000 flytekit-1.5.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-29 18:58:29.972222 flytekit-1.5.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-03-29 18:58:29.000000 flytekit-1.5.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-19 20:54:16.000000 flytekit-1.6.0b0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.370920 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.370920 flytekit-1.6.0b0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    35808 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30894 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75336 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.374920 flytekit-1.6.0b0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/interfaces/stats/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.378920 flytekit-1.6.0b0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82901 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44333 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.366919 flytekit-1.6.0b0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:54:19.000000 flytekit-1.6.0b0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-19 20:54:06.000000 flytekit-1.6.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-19 20:54:19.382920 flytekit-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-19 20:54:16.000000 flytekit-1.6.0b0/setup.py
```

### Comparing `flytekit-1.5.0b1/LICENSE` & `flytekit-1.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/MANIFEST.in` & `flytekit-1.6.0b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/PKG-INFO` & `flytekit-1.6.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.5.0b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
->=3.8,<3.12 Description-Content-Type: text/markdown License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.8,<3.12
+Description-Content-Type: text/markdown License-File: LICENSE
                                  [Flyte Logo]
                          ****** Flytekit Python ******
             Flytekit Python is the Python SDK built on top of Flyte
                    **** Plugins  Â·  Contribution_Guide ****
 [![PyPI version fury.io](https://badge.fury.io/py/flytekit.svg)](https://
 pypi.python.org/pypi/flytekit/) [![PyPI download day](https://img.shields.io/
 pypi/dd/flytekit.svg)](https://pypi.python.org/pypi/flytekit/) [![PyPI download
```

### Comparing `flytekit-1.5.0b1/README.md` & `flytekit-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/__init__.py` & `flytekit-1.6.0b0/flytekit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
    kwtypes
    current_context
    ExecutionParameters
    FlyteContext
    map_task
    ~core.workflow.ImperativeWorkflow
    ~core.node_creation.create_node
+   ~core.promise.NodeOutput
    FlyteContextManager
 
 Running Locally
 ------------------
 Tasks and Workflows can both be locally run (assuming the relevant tasks are capable of local execution). This is useful for unit testing.
 
 
@@ -190,14 +191,16 @@
    Documentation
    SourceCode
 
 """
 import sys
 from typing import Generator
 
+from rich import traceback
+
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
 from flytekit.core.base_sql_task import SQLTask
 from flytekit.core.base_task import SecurityContext, TaskMetadata, kwtypes
@@ -233,15 +236,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.5.0b1"
+__version__ = "1.6.0b0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
@@ -292,7 +295,10 @@
     discovered_plugins = entry_points(group="flytekit.plugins")
     for p in discovered_plugins:
         p.load()
 
 
 # Load all implicit plugins
 load_implicit_plugins()
+
+# Pretty-print exception messages
+traceback.install(width=None, extra_lines=0)
```

### Comparing `flytekit-1.5.0b1/flytekit/bin/entrypoint.py` & `flytekit-1.6.0b0/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.0b0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.0b0/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/auth/keyring.py` & `flytekit-1.6.0b0/flytekit/clients/auth/keyring.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,30 +36,30 @@
             )
             _keyring.set_password(
                 credentials.for_endpoint,
                 KeyringStore._access_token_key,
                 credentials.access_token,
             )
         except NoKeyringError as e:
-            logging.warning(f"KeyRing not available, tokens will not be cached. Error: {e}")
+            logging.debug(f"KeyRing not available, tokens will not be cached. Error: {e}")
         return credentials
 
     @staticmethod
     def retrieve(for_endpoint: str) -> typing.Optional[Credentials]:
         try:
             refresh_token = _keyring.get_password(for_endpoint, KeyringStore._refresh_token_key)
             access_token = _keyring.get_password(for_endpoint, KeyringStore._access_token_key)
         except NoKeyringError as e:
-            logging.warning(f"KeyRing not available, tokens will not be cached. Error: {e}")
+            logging.debug(f"KeyRing not available, tokens will not be cached. Error: {e}")
             return None
 
         if not access_token:
             return None
         return Credentials(access_token, refresh_token, for_endpoint)
 
     @staticmethod
     def delete(for_endpoint: str):
         try:
             _keyring.delete_password(for_endpoint, KeyringStore._access_token_key)
             _keyring.delete_password(for_endpoint, KeyringStore._refresh_token_key)
         except NoKeyringError as e:
-            logging.warning(f"KeyRing not available, tokens will not be cached. Error: {e}")
+            logging.debug(f"KeyRing not available, tokens will not be cached. Error: {e}")
```

### Comparing `flytekit-1.5.0b1/flytekit/clients/auth/token_client.py` & `flytekit-1.6.0b0/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/auth_helper.py` & `flytekit-1.6.0b0/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/friendly.py` & `flytekit-1.6.0b0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.0b0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.0b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/helpers.py` & `flytekit-1.6.0b0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clients/raw.py` & `flytekit-1.6.0b0/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.0b0/flytekit/clis/flyte_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1163,15 +1163,14 @@
             else:
                 # If the commandline parameter urn is not supplied, and neither
                 # the input is from a pipe, it means the user is not using
                 # this command appropriately
                 raise _click.UsageError('Missing option "-u" / "--urn" or missing pipe inputs.')
         except KeyboardInterrupt:
             _sys.stdout.flush()
-            pass
     else:
         _terminate_one_execution(client, urn, cause)
 
 
 @_flyte_cli.command("list-executions", cls=_FlyteSubCommand)
 @_project_option
 @_domain_option
```

### Comparing `flytekit-1.5.0b1/flytekit/clis/helpers.py` & `flytekit-1.6.0b0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 import click
 import grpc
 from google.protobuf.json_format import MessageToJson
 
 from flytekit import configuration
 from flytekit.clis.sdk_in_container.backfill import backfill
+from flytekit.clis.sdk_in_container.build import build
 from flytekit.clis.sdk_in_container.constants import CTX_CONFIG_FILE, CTX_PACKAGES, CTX_VERBOSE
 from flytekit.clis.sdk_in_container.init import init
+from flytekit.clis.sdk_in_container.launchplan import launchplan
 from flytekit.clis.sdk_in_container.local_cache import local_cache
 from flytekit.clis.sdk_in_container.package import package
 from flytekit.clis.sdk_in_container.register import register
 from flytekit.clis.sdk_in_container.run import run
 from flytekit.clis.sdk_in_container.serialize import serialize
 from flytekit.configuration.internal import LocalSDK
 from flytekit.exceptions.base import FlyteException
@@ -128,11 +130,13 @@
 main.add_command(serialize)
 main.add_command(package)
 main.add_command(local_cache)
 main.add_command(init)
 main.add_command(run)
 main.add_command(register)
 main.add_command(backfill)
+main.add_command(build)
+main.add_command(launchplan)
 main.epilog
 
 if __name__ == "__main__":
     main()
```

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from flytekit.core.base_task import PythonTask
 from flytekit.core.context_manager import FlyteContext
 from flytekit.core.data_persistence import FileAccessProvider
 from flytekit.core.type_engine import TypeEngine
 from flytekit.core.workflow import PythonFunctionWorkflow, WorkflowBase
 from flytekit.models import literals
 from flytekit.models.interface import Variable
-from flytekit.models.literals import Blob, BlobMetadata, Primitive, Union
+from flytekit.models.literals import Blob, BlobMetadata, LiteralCollection, LiteralMap, Primitive, Union
 from flytekit.models.types import LiteralType, SimpleType
 from flytekit.remote.executions import FlyteWorkflowExecution
 from flytekit.tools import module_loader, script_mode
 from flytekit.tools.script_mode import _find_project_root
 from flytekit.tools.translator import Options
 
 REMOTE_FLAG_KEY = "remote"
@@ -211,32 +211,34 @@
         return self._click_type
 
     def is_bool(self) -> bool:
         if self._literal_type.simple:
             return self._literal_type.simple == SimpleType.BOOLEAN
         return False
 
-    def get_uri_for_dir(self, value: Directory, remote_filename: typing.Optional[str] = None):
+    def get_uri_for_dir(
+        self, ctx: typing.Optional[click.Context], value: Directory, remote_filename: typing.Optional[str] = None
+    ):
         uri = value.dir_path
 
         if self._remote and value.local:
             md5, _ = script_mode.hash_file(value.local_file)
             if not remote_filename:
                 remote_filename = value.local_file.name
-            df_remote_location = self._create_upload_fn(filename=remote_filename, content_md5=md5)
-            self._flyte_ctx.file_access.put_data(value.local_file, df_remote_location.signed_url)
-            uri = df_remote_location.native_url[: -len(remote_filename)]
+            remote = ctx.obj[FLYTE_REMOTE_INSTANCE_KEY]
+            _, native_url = remote.upload_file(value.local_file)
+            uri = native_url[: -len(remote_filename)]
 
         return uri
 
     def convert_to_structured_dataset(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: Directory
     ) -> Literal:
 
-        uri = self.get_uri_for_dir(value, "00000.parquet")
+        uri = self.get_uri_for_dir(ctx, value, "00000.parquet")
 
         lit = Literal(
             scalar=Scalar(
                 structured_dataset=literals.StructuredDataset(
                     uri=uri,
                     metadata=literals.StructuredDatasetMetadata(
                         structured_dataset_type=self._literal_type.structured_dataset_type
@@ -250,23 +252,21 @@
     def convert_to_blob(
         self,
         ctx: typing.Optional[click.Context],
         param: typing.Optional[click.Parameter],
         value: typing.Union[Directory, FileParam],
     ) -> Literal:
         if isinstance(value, Directory):
-            uri = self.get_uri_for_dir(value)
+            uri = self.get_uri_for_dir(ctx, value)
         else:
             uri = value.filepath
             if self._remote and value.local:
                 fp = pathlib.Path(value.filepath)
-                md5, _ = script_mode.hash_file(value.filepath)
-                df_remote_location = self._create_upload_fn(filename=fp.name, content_md5=md5)
-                self._flyte_ctx.file_access.put_data(fp, df_remote_location.signed_url)
-                uri = df_remote_location.native_url
+                remote = ctx.obj[FLYTE_REMOTE_INSTANCE_KEY]
+                _, uri = remote.upload_file(fp)
 
         lit = Literal(
             scalar=Scalar(
                 blob=Blob(
                     metadata=BlobMetadata(type=self._literal_type.blob),
                     uri=uri,
                 ),
@@ -304,22 +304,46 @@
     ) -> Literal:
         if self._literal_type.structured_dataset_type:
             return self.convert_to_structured_dataset(ctx, param, value)
 
         if self._literal_type.blob:
             return self.convert_to_blob(ctx, param, value)
 
-        if self._literal_type.collection_type or self._literal_type.map_value_type:
-            # TODO Does not support nested flytefile, flyteschema types
-            v = json.loads(value) if isinstance(value, str) else value
-            if self._literal_type.collection_type and not isinstance(v, list):
-                raise click.BadParameter(f"Expected json list '[...]', parsed value is {type(v)}")
-            if self._literal_type.map_value_type and not isinstance(v, dict):
-                raise click.BadParameter("Expected json map '{}', parsed value is {%s}" % type(v))
-            return TypeEngine.to_literal(self._flyte_ctx, v, self._python_type, self._literal_type)
+        if self._literal_type.collection_type:
+            python_value = json.loads(value) if isinstance(value, str) else value
+            if not isinstance(python_value, list):
+                raise click.BadParameter(f"Expected json list '[...]', parsed value is {type(python_value)}")
+            converter = FlyteLiteralConverter(
+                ctx,
+                self._flyte_ctx,
+                self._literal_type.collection_type,
+                type(python_value[0]),
+                self._create_upload_fn,
+            )
+            lt = Literal(collection=LiteralCollection([]))
+            for v in python_value:
+                click_val = converter._click_type.convert(v, param, ctx)
+                lt.collection.literals.append(converter.convert_to_literal(ctx, param, click_val))
+            return lt
+        if self._literal_type.map_value_type:
+            python_value = json.loads(value) if isinstance(value, str) else value
+            if not isinstance(python_value, dict):
+                raise click.BadParameter("Expected json map '{}', parsed value is {%s}" % type(python_value))
+            converter = FlyteLiteralConverter(
+                ctx,
+                self._flyte_ctx,
+                self._literal_type.map_value_type,
+                type(python_value[next(iter(python_value))]),
+                self._create_upload_fn,
+            )
+            lt = Literal(map=LiteralMap({}))
+            for k, v in python_value.items():
+                click_val = converter._click_type.convert(v, param, ctx)
+                lt.map.literals[k] = converter.convert_to_literal(ctx, param, click_val)
+            return lt
 
         if self._literal_type.union_type:
             return self.convert_to_union(ctx, param, value)
 
         if self._literal_type.simple or self._literal_type.enum_type:
             if self._literal_type.simple and self._literal_type.simple == SimpleType.STRUCT:
                 if self._python_type == dict:
```

### Comparing `flytekit-1.5.0b1/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.0b0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/configuration/__init__.py` & `flytekit-1.6.0b0/flytekit/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,20 +139,23 @@
 import re
 import tempfile
 import typing
 from dataclasses import dataclass, field
 from io import BytesIO
 from typing import Dict, List, Optional
 
+import yaml
 from dataclasses_json import dataclass_json
 from docker_image import reference
 
 from flytekit.configuration import internal as _internal
 from flytekit.configuration.default_images import DefaultImages
 from flytekit.configuration.file import ConfigEntry, ConfigFile, get_config_file, read_file_if_exists, set_if_exists
+from flytekit.image_spec import ImageSpec
+from flytekit.image_spec.image_spec import ImageBuildEngine
 from flytekit.loggers import logger
 
 PROJECT_PLACEHOLDER = "{{ registration.project }}"
 DOMAIN_PLACEHOLDER = "{{ registration.domain }}"
 VERSION_PLACEHOLDER = "{{ registration.version }}"
 DEFAULT_RUNTIME_PYTHON_INTERPRETER = "/opt/venv/bin/python3"
 DEFAULT_FLYTEKIT_ENTRYPOINT_FILELOC = "bin/entrypoint.py"
@@ -201,14 +204,21 @@
         like the sha of the latest commit.
 
         :param optional_tag:
         :param name:
         :param Text tag: e.g. somedocker.com/myimage:someversion123
         :rtype: Text
         """
+        if pathlib.Path(tag).is_file():
+            with open(tag, "r") as f:
+                image_spec_dict = yaml.safe_load(f)
+                image_spec = ImageSpec(**image_spec_dict)
+                ImageBuildEngine.build(image_spec)
+                tag = image_spec.image_name()
+
         ref = reference.Reference.parse(tag)
         if not optional_tag and ref["tag"] is None:
             raise AssertionError(f"Incorrectly formatted image {tag}, missing tag value")
         else:
             return Image(name=name, fqn=ref["name"], tag=ref["tag"])
 
 
@@ -695,25 +705,27 @@
         python_interpreter (Optional[str]): The python executable to use. This is used for spark tasks in out of
             container execution.
         entrypoint_settings (Optional[EntrypointSettings]): Information about the command, path and version of the
             entrypoint program.
         fast_serialization_settings (Optional[FastSerializationSettings]): If the code is being serialized so that it
             can be fast registered (and thus omit building a Docker image) this object contains additional parameters
             for serialization.
+        source_root (Optional[str]): The root directory of the source code.
     """
 
     image_config: ImageConfig
     project: typing.Optional[str] = None
     domain: typing.Optional[str] = None
     version: typing.Optional[str] = None
     env: Optional[Dict[str, str]] = None
     git_repo: Optional[str] = None
     python_interpreter: str = DEFAULT_RUNTIME_PYTHON_INTERPRETER
     flytekit_virtualenv_root: Optional[str] = None
     fast_serialization_settings: Optional[FastSerializationSettings] = None
+    source_root: Optional[str] = None
 
     def __post_init__(self):
         if self.flytekit_virtualenv_root is None:
             self.flytekit_virtualenv_root = self.venv_root_from_interpreter(self.python_interpreter)
 
     @property
     def entrypoint_settings(self) -> EntrypointSettings:
```

### Comparing `flytekit-1.5.0b1/flytekit/configuration/default_images.py` & `flytekit-1.6.0b0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/configuration/feature_flags.py` & `flytekit-1.6.0b0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/configuration/file.py` & `flytekit-1.6.0b0/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/configuration/internal.py` & `flytekit-1.6.0b0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/annotation.py` & `flytekit-1.6.0b0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/base_sql_task.py` & `flytekit-1.6.0b0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/base_task.py` & `flytekit-1.6.0b0/flytekit/core/base_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     create_and_link_node,
     create_task_output,
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.tracker import TrackedInstance
-from flytekit.core.type_engine import TypeEngine
+from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError
 from flytekit.deck.deck import Deck
 from flytekit.loggers import logger
 from flytekit.models import dynamic_job as _dynamic_job
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
 from flytekit.models import task as _task_model
 from flytekit.models.core import workflow as _workflow_model
@@ -241,20 +241,25 @@
         """
         # Unwrap the kwargs values. After this, we essentially have a LiteralMap
         # The reason why we need to do this is because the inputs during local execute can be of 2 types
         #  - Promises or native constants
         #  Promises as essentially inputs from previous task executions
         #  native constants are just bound to this specific task (default values for a task input)
         #  Also along with promises and constants, there could be dictionary or list of promises or constants
-        kwargs = translate_inputs_to_literals(
-            ctx,
-            incoming_values=kwargs,
-            flyte_interface_types=self.interface.inputs,
-            native_types=self.get_input_types(),  # type: ignore
-        )
+        try:
+            kwargs = translate_inputs_to_literals(
+                ctx,
+                incoming_values=kwargs,
+                flyte_interface_types=self.interface.inputs,
+                native_types=self.get_input_types(),  # type: ignore
+            )
+        except TypeTransformerFailedError as exc:
+            msg = f"Failed to convert inputs of task '{self.name}':\n  {exc}"
+            logger.error(msg)
+            raise TypeError(msg) from exc
         input_literal_map = _literal_models.LiteralMap(literals=kwargs)
 
         # if metadata.cache is set, check memoized version
         if self.metadata.cache:
             # TODO: how to get a nice `native_inputs` here?
             logger.info(
                 f"Checking cache for task named {self.name}, cache version {self.metadata.cache_version} "
@@ -511,15 +516,22 @@
             ctx.with_execution_state(
                 cast(ExecutionState, ctx.execution_state).with_params(user_space_params=new_user_params)
             )
             # type: ignore
         ) as exec_ctx:
             # TODO We could support default values here too - but not part of the plan right now
             # Translate the input literals to Python native
-            native_inputs = TypeEngine.literal_map_to_kwargs(exec_ctx, input_literal_map, self.python_interface.inputs)
+            try:
+                native_inputs = TypeEngine.literal_map_to_kwargs(
+                    exec_ctx, input_literal_map, self.python_interface.inputs
+                )
+            except Exception as exc:
+                msg = f"Failed to convert inputs of task '{self.name}':\n  {exc}"
+                logger.error(msg)
+                raise type(exc)(msg) from exc
 
             # TODO: Logger should auto inject the current context information to indicate if the task is running within
             #   a workflow or a subworkflow etc
             logger.info(f"Invoking {self.name} with inputs: {native_inputs}")
             try:
                 native_outputs = self.execute(**native_inputs)
             except Exception as e:
@@ -555,27 +567,28 @@
                 native_outputs_as_map = {
                     expected_output_names[i]: native_outputs[i] for i, _ in enumerate(native_outputs)
                 }
 
             # We manually construct a LiteralMap here because task inputs and outputs actually violate the assumption
             # built into the IDL that all the values of a literal map are of the same type.
             literals = {}
-            for k, v in native_outputs_as_map.items():
+            for i, (k, v) in enumerate(native_outputs_as_map.items()):
                 literal_type = self._outputs_interface[k].type
                 py_type = self.get_type_for_output_var(k, v)
 
                 if isinstance(v, tuple):
-                    raise TypeError(f"Output({k}) in task{self.name} received a tuple {v}, instead of {py_type}")
+                    raise TypeError(f"Output({k}) in task '{self.name}' received a tuple {v}, instead of {py_type}")
                 try:
                     literals[k] = TypeEngine.to_literal(exec_ctx, v, py_type, literal_type)
                 except Exception as e:
-                    logger.error(f"Failed to convert return value for var {k} with error {type(e)}: {e}")
-                    raise TypeError(
-                        f"Failed to convert return value for var {k} for function {self.name} with error {type(e)}: {e}"
-                    ) from e
+                    # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
+                    key = k if k != f"o{i}" else i
+                    msg = f"Failed to convert outputs of task '{self.name}' at position {key}:\n  {e}"
+                    logger.error(msg)
+                    raise TypeError(msg) from e
 
             if self._disable_deck is False:
                 INPUT = "input"
                 OUTPUT = "output"
 
                 input_deck = Deck(INPUT)
                 for k, v in native_inputs.items():
```

### Comparing `flytekit-1.5.0b1/flytekit/core/checkpointer.py` & `flytekit-1.6.0b0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/class_based_resolver.py` & `flytekit-1.6.0b0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/condition.py` & `flytekit-1.6.0b0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/constants.py` & `flytekit-1.6.0b0/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/container_task.py` & `flytekit-1.6.0b0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/context_manager.py` & `flytekit-1.6.0b0/flytekit/core/context_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,51 +325,52 @@
 
     def __getattr__(self, item: str) -> _GroupSecrets:
         """
         returns a new _GroupSecrets objects, that allows all keys within this group to be looked up like attributes
         """
         return self._GroupSecrets(item, self)
 
-    def get(self, group: str, key: str) -> str:
+    def get(self, group: str, key: Optional[str] = None, group_version: Optional[str] = None) -> str:
         """
         Retrieves a secret using the resolution order -> Env followed by file. If not found raises a ValueError
         """
-        self.check_group_key(group, key)
-        env_var = self.get_secrets_env_var(group, key)
-        fpath = self.get_secrets_file(group, key)
+        self.check_group_key(group)
+        env_var = self.get_secrets_env_var(group, key, group_version)
+        fpath = self.get_secrets_file(group, key, group_version)
         v = os.environ.get(env_var)
         if v is not None:
             return v
         if os.path.exists(fpath):
             with open(fpath, "r") as f:
                 return f.read().strip()
         raise ValueError(
             f"Unable to find secret for key {key} in group {group} " f"in Env Var:{env_var} and FilePath: {fpath}"
         )
 
-    def get_secrets_env_var(self, group: str, key: str) -> str:
+    def get_secrets_env_var(self, group: str, key: Optional[str] = None, group_version: Optional[str] = None) -> str:
         """
         Returns a string that matches the ENV Variable to look for the secrets
         """
-        self.check_group_key(group, key)
-        return f"{self._env_prefix}{group.upper()}_{key.upper()}"
+        self.check_group_key(group)
+        l = [k.upper() for k in filter(None, (group, group_version, key))]
+        return f"{self._env_prefix}{'_'.join(l)}"
 
-    def get_secrets_file(self, group: str, key: str) -> str:
+    def get_secrets_file(self, group: str, key: Optional[str] = None, group_version: Optional[str] = None) -> str:
         """
         Returns a path that matches the file to look for the secrets
         """
-        self.check_group_key(group, key)
-        return os.path.join(self._base_dir, group.lower(), f"{self._file_prefix}{key.lower()}")
+        self.check_group_key(group)
+        l = [k.lower() for k in filter(None, (group, group_version, key))]
+        l[-1] = f"{self._file_prefix}{l[-1]}"
+        return os.path.join(self._base_dir, *l)
 
     @staticmethod
-    def check_group_key(group: str, key: str):
+    def check_group_key(group: str):
         if group is None or group == "":
             raise ValueError("secrets group is a mandatory field.")
-        if key is None or key == "":
-            raise ValueError("secrets key is a mandatory field.")
 
 
 @dataclass(frozen=True)
 class CompilationState(object):
     """
     Compilation state is used during the compilation of a workflow or task. It stores the nodes that were
     created when walking through the workflow graph.
```

### Comparing `flytekit-1.5.0b1/flytekit/core/data_persistence.py` & `flytekit-1.6.0b0/flytekit/core/data_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
    UnsupportedPersistenceOp
 
 """
 import os
 import pathlib
 import tempfile
 import typing
-from typing import Union, cast
+from typing import Any, Dict, Union, cast
 from uuid import UUID
 
 import fsspec
 from fsspec.utils import get_protocol
 
 from flytekit import configuration
 from flytekit.configuration import DataConfig
@@ -42,15 +42,17 @@
 # for key and secret
 _FSSPEC_S3_KEY_ID = "key"
 _FSSPEC_S3_SECRET = "secret"
 _ANON = "anon"
 
 
 def s3_setup_args(s3_cfg: configuration.S3Config, anonymous: bool = False):
-    kwargs = {}
+    kwargs: Dict[str, Any] = {
+        "cache_regions": True,
+    }
     if s3_cfg.access_key_id:
         kwargs[_FSSPEC_S3_KEY_ID] = s3_cfg.access_key_id
 
     if s3_cfg.secret_access_key:
         kwargs[_FSSPEC_S3_SECRET] = s3_cfg.secret_access_key
 
     # S3fs takes this as a special arg
@@ -311,14 +313,15 @@
         we don't use the true local proxy if the remote path is a file://
 
         :param local_path:
         :param remote_path:
         :param is_multipart:
         """
         try:
+            local_path = str(local_path)
             with PerformanceTimer(f"Writing ({local_path} -> {remote_path})"):
                 self.put(cast(str, local_path), remote_path, recursive=is_multipart)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to put data from {local_path} to {remote_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             ) from ex
```

### Comparing `flytekit-1.5.0b1/flytekit/core/docstring.py` & `flytekit-1.6.0b0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.0b0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/gate.py` & `flytekit-1.6.0b0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/interface.py` & `flytekit-1.6.0b0/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/launch_plan.py` & `flytekit-1.6.0b0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/local_cache.py` & `flytekit-1.6.0b0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/map_task.py` & `flytekit-1.6.0b0/flytekit/core/map_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         :param bound_inputs: List[str] specifies a list of variable names within the interface of python_function_task,
               that are already bound and should not be considered as list inputs, but scalar values. This is mostly
               useful at runtime and is passed in by MapTaskResolver. This field is not required when a `partial` method
               is specified. The bound_vars will be auto-deduced from the `partial.keywords`.
         """
         self._partial = None
         if isinstance(python_function_task, functools.partial):
+            # TODO: We should be able to support partial tasks with lists as inputs
+            for arg in python_function_task.keywords.values():
+                if isinstance(arg, list):
+                    raise ValueError("Map tasks do not support partial tasks with lists as inputs. ")
             self._partial = python_function_task
             actual_task = self._partial.func
         else:
             actual_task = python_function_task
 
         if not isinstance(actual_task, PythonFunctionTask):
             raise ValueError("Map tasks can only compose of Python Functon Tasks currently")
```

### Comparing `flytekit-1.5.0b1/flytekit/core/mock_stats.py` & `flytekit-1.6.0b0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/node.py` & `flytekit-1.6.0b0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/node_creation.py` & `flytekit-1.6.0b0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/notification.py` & `flytekit-1.6.0b0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/pod_template.py` & `flytekit-1.6.0b0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/promise.py` & `flytekit-1.6.0b0/flytekit/core/promise.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     ExecutionParameters,
     ExecutionState,
     FlyteContext,
     FlyteContextManager,
 )
 from flytekit.core.interface import Interface
 from flytekit.core.node import Node
-from flytekit.core.type_engine import DictTransformer, ListTransformer, TypeEngine
+from flytekit.core.type_engine import DictTransformer, ListTransformer, TypeEngine, TypeTransformerFailedError
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
 from flytekit.models import literals as _literals_models
 from flytekit.models import types as _type_models
 from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
@@ -88,14 +88,20 @@
                 raise TypeError(f"Not a collection type {flyte_literal_type} but got a list {input_val}")
             try:
                 sub_type: type = ListTransformer.get_sub_type(python_type)
             except ValueError:
                 if len(input_val) == 0:
                     raise
                 sub_type = type(input_val[0])
+            # To maintain consistency between translate_inputs_to_literals and ListTransformer.to_literal for batchable types,
+            # directly call ListTransformer.to_literal to batch process the list items. This is necessary because processing
+            # each list item separately could lead to errors since ListTransformer.to_python_value may treat the literal
+            # as it is batched for batchable types.
+            if ListTransformer.is_batchable(python_type):
+                return TypeEngine.to_literal(ctx, input_val, python_type, lt)
             literal_list = [extract_value(ctx, v, sub_type, lt.collection_type) for v in input_val]
             return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=literal_list))
         elif isinstance(input_val, dict):
             lt = flyte_literal_type
             python_type = val_type
             if flyte_literal_type.union_type:
                 for i in range(len(flyte_literal_type.union_type.variants)):
@@ -137,15 +143,18 @@
 
     result = {}  # So as to not overwrite the input_kwargs
     for k, v in incoming_values.items():
         if k not in flyte_interface_types:
             raise ValueError(f"Received unexpected keyword argument {k}")
         var = flyte_interface_types[k]
         t = native_types[k]
-        result[k] = extract_value(ctx, v, t, var.type)
+        try:
+            result[k] = extract_value(ctx, v, t, var.type)
+        except TypeTransformerFailedError as exc:
+            raise TypeTransformerFailedError(f"Failed argument '{k}': {exc}") from exc
 
     return result
 
 
 def get_primitive_val(prim: Primitive) -> Any:
     for value in [
         prim.integer,
@@ -473,38 +482,44 @@
         raise ValueError("Interface of the entity is required to generate named outputs")
 
     if promises is None:
         return None
 
     if isinstance(promises, Promise):
         k, v = [(k, v) for k, v in entity_interface.outputs.items()][0]  # get output native type
+        # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
+        key = k if k != "o0" else 0
         try:
             return TypeEngine.to_python_value(ctx, promises.val, v)
         except Exception as e:
-            raise AssertionError(f"Failed to convert value of output {k}, expected type {v}.") from e
+            raise TypeError(
+                f"Failed to convert output in position {key} of value {promises.val}, expected type {v}."
+            ) from e
 
     if len(cast(Tuple[Promise], promises)) == 0:
         return None
 
     named_tuple_name = "DefaultNamedTupleOutput"
     if entity_interface.output_tuple_name:
         named_tuple_name = entity_interface.output_tuple_name
 
     outputs = {}
-    for p in cast(Tuple[Promise], promises):
+    for i, p in enumerate(cast(Tuple[Promise], promises)):
         if not isinstance(p, Promise):
             raise AssertionError(
                 "Workflow outputs can only be promises that are returned by tasks. Found a value of"
                 f"type {type(p)}. Workflows cannot return local variables or constants."
             )
         t = entity_interface.outputs[p.var]
         try:
             outputs[p.var] = TypeEngine.to_python_value(ctx, p.val, t)
         except Exception as e:
-            raise AssertionError(f"Failed to convert value of output {p.var}, expected type {t}.") from e
+            # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
+            key = p.var if p.var != f"o{i}" else i
+            raise TypeError(f"Failed to convert output in position {key} of value {p.val}, expected type {t}.") from e
 
     # Should this class be part of the Interface?
     nt = collections.namedtuple(named_tuple_name, list(outputs.keys()))  # type: ignore
     return nt(**outputs)
 
 
 # To create a class that is a named tuple, we might have to create namedtuplemeta and manipulate the tuple
@@ -1053,15 +1068,15 @@
             f"When calling tasks, only keyword args are supported. "
             f"Aborting execution as detected {len(args)} positional args {args}"
         )
     # Make sure arguments are part of interface
     for k, v in kwargs.items():
         if k not in cast(SupportsNodeCreation, entity).python_interface.inputs:
             raise ValueError(
-                f"Received unexpected keyword argument {k} in function {cast(SupportsNodeCreation, entity).name}"
+                f"Received unexpected keyword argument '{k}' in function '{cast(SupportsNodeCreation, entity).name}'"
             )
 
     ctx = FlyteContextManager.current_context()
     if ctx.compilation_state is not None and ctx.compilation_state.mode == 1:
         return create_and_link_node(ctx, entity=entity, **kwargs)
     elif ctx.execution_state is not None and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
         if ctx.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED:
```

### Comparing `flytekit-1.5.0b1/flytekit/core/python_auto_container.py` & `flytekit-1.6.0b0/flytekit/core/python_auto_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import importlib
 import re
 from abc import ABC
-from typing import Callable, Dict, List, Optional, TypeVar
+from typing import Callable, Dict, List, Optional, TypeVar, Union
 
 from flytekit.configuration import ImageConfig, SerializationSettings
 from flytekit.core.base_task import PythonTask, TaskMetadata, TaskResolverMixin
 from flytekit.core.context_manager import FlyteContextManager
 from flytekit.core.pod_template import PodTemplate
 from flytekit.core.resources import Resources, ResourceSpec
 from flytekit.core.tracked_abc import FlyteTrackedABC
 from flytekit.core.tracker import TrackedInstance, extract_task_module
 from flytekit.core.utils import _get_container_definition, _serialize_pod_spec
+from flytekit.image_spec.image_spec import ImageBuildEngine, ImageSpec
 from flytekit.loggers import logger
 from flytekit.models import task as _task_model
 from flytekit.models.security import Secret, SecurityContext
 
 T = TypeVar("T")
 _PRIMARY_CONTAINER_NAME_FIELD = "primary_container_name"
 
@@ -31,15 +32,15 @@
     """
 
     def __init__(
         self,
         name: str,
         task_config: T,
         task_type="python-task",
-        container_image: Optional[str] = None,
+        container_image: Optional[Union[str, ImageSpec]] = None,
         requests: Optional[Resources] = None,
         limits: Optional[Resources] = None,
         environment: Optional[Dict[str, str]] = None,
         task_resolver: Optional[TaskResolverMixin] = None,
         secret_requests: Optional[List[Secret]] = None,
         pod_template: Optional[PodTemplate] = None,
         pod_template_name: Optional[str] = None,
@@ -73,15 +74,15 @@
         sec_ctx = None
         if secret_requests:
             for s in secret_requests:
                 if not isinstance(s, Secret):
                     raise AssertionError(f"Secret {s} should be of type flytekit.Secret, received {type(s)}")
             sec_ctx = SecurityContext(secrets=secret_requests)
 
-        # pod_template_name overwrites the metedata.pod_template_name
+        # pod_template_name overwrites the metadata.pod_template_name
         kwargs["metadata"] = kwargs["metadata"] if "metadata" in kwargs else TaskMetadata()
         kwargs["metadata"].pod_template_name = pod_template_name
 
         super().__init__(
             task_type=task_type,
             name=name,
             task_config=task_config,
@@ -111,15 +112,15 @@
         self.pod_template = pod_template
 
     @property
     def task_resolver(self) -> TaskResolverMixin:
         return self._task_resolver
 
     @property
-    def container_image(self) -> Optional[str]:
+    def container_image(self) -> Optional[Union[str, ImageSpec]]:
         return self._container_image
 
     @property
     def resources(self) -> ResourceSpec:
         return self._resources
 
     def get_default_command(self, settings: SerializationSettings) -> List[str]:
@@ -176,14 +177,16 @@
             return self._get_container(settings)
 
     def _get_container(self, settings: SerializationSettings) -> _task_model.Container:
         env = {}
         for elem in (settings.env, self.environment):
             if elem:
                 env.update(elem)
+        if isinstance(self.container_image, ImageSpec):
+            self.container_image.source_root = settings.source_root
         return _get_container_definition(
             image=get_registerable_container_image(self.container_image, settings.image_config),
             command=[],
             args=self.get_command(settings=settings),
             data_loading_config=None,
             environment=env,
             storage_request=self.resources.requests.storage,
@@ -244,20 +247,24 @@
     def get_all_tasks(self) -> List[PythonAutoContainerTask]:  # type: ignore
         raise Exception("should not be needed")
 
 
 default_task_resolver = DefaultTaskResolver()
 
 
-def get_registerable_container_image(img: Optional[str], cfg: ImageConfig) -> str:
+def get_registerable_container_image(img: Optional[Union[str, ImageSpec]], cfg: ImageConfig) -> str:
     """
-    :param img: Configured image
+    :param img: Configured image or image spec
     :param cfg: Registration configuration
     :return:
     """
+    if isinstance(img, ImageSpec):
+        ImageBuildEngine.build(img)
+        return img.image_name()
+
     if img is not None and img != "":
         matches = _IMAGE_REPLACE_REGEX.findall(img)
         if matches is None or len(matches) == 0:
             return img
         for m in matches:
             if len(m) < 3:
                 raise AssertionError(
```

### Comparing `flytekit-1.5.0b1/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.0b0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/python_function_task.py` & `flytekit-1.6.0b0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/reference.py` & `flytekit-1.6.0b0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/reference_entity.py` & `flytekit-1.6.0b0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/resources.py` & `flytekit-1.6.0b0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/schedule.py` & `flytekit-1.6.0b0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/shim_task.py` & `flytekit-1.6.0b0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/task.py` & `flytekit-1.6.0b0/flytekit/core/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from flytekit.core.base_task import TaskMetadata, TaskResolverMixin
 from flytekit.core.interface import transform_function_to_interface
 from flytekit.core.pod_template import PodTemplate
 from flytekit.core.python_function_task import PythonFunctionTask
 from flytekit.core.reference_entity import ReferenceEntity, TaskReference
 from flytekit.core.resources import Resources
+from flytekit.image_spec.image_spec import ImageSpec
 from flytekit.models.documentation import Documentation
 from flytekit.models.security import Secret
 
 
 class TaskPlugins(object):
     """
     This is the TaskPlugins factory for task types that are derivative of PythonFunctionTask.
@@ -80,15 +81,15 @@
     cache: bool = False,
     cache_serialize: bool = False,
     cache_version: str = "",
     retries: int = 0,
     interruptible: Optional[bool] = None,
     deprecated: str = "",
     timeout: Union[_datetime.timedelta, int] = 0,
-    container_image: Optional[str] = None,
+    container_image: Optional[Union[str, ImageSpec]] = None,
     environment: Optional[Dict[str, str]] = None,
     requests: Optional[Resources] = None,
     limits: Optional[Resources] = None,
     secret_requests: Optional[List[Secret]] = None,
     execution_mode: PythonFunctionTask.ExecutionBehavior = PythonFunctionTask.ExecutionBehavior.DEFAULT,
     task_resolver: Optional[TaskResolverMixin] = None,
     docs: Optional[Documentation] = None,
```

### Comparing `flytekit-1.5.0b1/flytekit/core/testing.py` & `flytekit-1.6.0b0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/tracker.py` & `flytekit-1.6.0b0/flytekit/core/tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
             except ValueError as err:
                 # Empty pandas dataframes behave weirdly here such that calling `m.df` raises:
                 # ValueError: The truth value of a {type(self).__name__} is ambiguous. Use a.empty, a.bool(), a.item(),
                 #   a.any() or a.all()
                 # Since dataframes aren't registrable entities to begin with we swallow any errors they raise and
                 # continue looping through m.
                 logger.warning("Caught ValueError {} while attempting to auto-assign name".format(err))
-                pass
 
         logger.error(f"Could not find LHS for {self} in {self._instantiated_in}")
         raise _system_exceptions.FlyteSystemException(f"Error looking for LHS in {self._instantiated_in}")
 
 
 def isnested(func: Callable) -> bool:
     """
```

### Comparing `flytekit-1.5.0b1/flytekit/core/type_engine.py` & `flytekit-1.6.0b0/flytekit/core/type_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         """
         Indicates if the transformer wants type assertions to be enabled at the core type engine layer
         """
         return self._type_assertions_enabled
 
     def assert_type(self, t: Type[T], v: T):
         if not hasattr(t, "__origin__") and not isinstance(v, t):
-            raise TypeTransformerFailedError(f"Type of Val '{v}' is not an instance of {t}")
+            raise TypeTransformerFailedError(f"Expected value of type {t} but got '{v}' of type {type(v)}")
 
     @abstractmethod
     def get_literal_type(self, t: Type[T]) -> LiteralType:
         """
         Converts the python type to a Flyte LiteralType
         """
         raise NotImplementedError("Conversion to LiteralType should be implemented")
@@ -162,15 +162,17 @@
         self._from_literal_transformer = from_literal_transformer
 
     def get_literal_type(self, t: Optional[Type[T]] = None) -> LiteralType:
         return LiteralType.from_flyte_idl(self._lt.to_flyte_idl())
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
         if type(python_val) != self._type:
-            raise TypeTransformerFailedError(f"Expected value of type {self._type} but got type {type(python_val)}")
+            raise TypeTransformerFailedError(
+                f"Expected value of type {self._type} but got '{python_val}' of type {type(python_val)}"
+            )
         return self._to_literal_transformer(python_val)
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
         if get_origin(expected_python_type) is Annotated:
             expected_python_type = get_args(expected_python_type)[0]
 
         if expected_python_type != self._type:
@@ -181,15 +183,15 @@
         try:  # todo(maximsmol): this is quite ugly and each transformer should really check their Literal
             res = self._from_literal_transformer(lv)
             if type(res) != self._type:
                 raise TypeTransformerFailedError(f"Cannot convert literal {lv} to {self._type}")
             return res
         except AttributeError:
             # Assume that this is because a property on `lv` was None
-            raise TypeTransformerFailedError(f"Cannot convert literal {lv}")
+            raise TypeTransformerFailedError(f"Cannot convert literal {lv} to {self._type}")
 
     def guess_python_type(self, literal_type: LiteralType) -> Type[T]:
         if literal_type.simple is not None and literal_type.simple == self._lt.simple:
             return self.python_type
         raise ValueError(f"Transformer {self} cannot reverse {literal_type}")
 
 
@@ -860,15 +862,21 @@
         """
         Given a ``LiteralMap`` (usually an input into a task - intermediate), convert to kwargs for the task
         """
         if len(lm.literals) > len(python_types):
             raise ValueError(
                 f"Received more input values {len(lm.literals)}" f" than allowed by the input spec {len(python_types)}"
             )
-        return {k: TypeEngine.to_python_value(ctx, lm.literals[k], python_types[k]) for k, v in lm.literals.items()}
+        kwargs = {}
+        for i, k in enumerate(lm.literals):
+            try:
+                kwargs[k] = TypeEngine.to_python_value(ctx, lm.literals[k], python_types[k])
+            except TypeTransformerFailedError as exc:
+                raise TypeTransformerFailedError(f"Error converting input '{k}' at position {i}:\n  {exc}") from exc
+        return kwargs
 
     @classmethod
     def dict_to_literal_map(
         cls,
         ctx: FlyteContext,
         d: typing.Dict[str, typing.Any],
         type_hints: Optional[typing.Dict[str, type]] = None,
@@ -964,30 +972,67 @@
         """
         try:
             sub_type = TypeEngine.to_literal_type(self.get_sub_type(t))
             return _type_models.LiteralType(collection_type=sub_type)
         except Exception as e:
             raise ValueError(f"Type of Generic List type is not supported, {e}")
 
+    @staticmethod
+    def is_batchable(t: Type):
+        """
+        This function evaluates whether the provided type is batchable or not.
+        It returns True only if the type is either List or Annotated(List) and the List subtype is FlytePickle.
+        """
+        from flytekit.types.pickle import FlytePickle
+
+        if get_origin(t) is Annotated:
+            return ListTransformer.is_batchable(get_args(t)[0])
+        if get_origin(t) is list:
+            subtype = get_args(t)[0]
+            if subtype == FlytePickle or (hasattr(subtype, "__origin__") and subtype.__origin__ == FlytePickle):
+                return True
+        return False
+
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
         if type(python_val) != list:
             raise TypeTransformerFailedError("Expected a list")
 
-        t = self.get_sub_type(python_type)
-        lit_list = [TypeEngine.to_literal(ctx, x, t, expected.collection_type) for x in python_val]  # type: ignore
+        if ListTransformer.is_batchable(python_type):
+            from flytekit.types.pickle.pickle import BatchSize, FlytePickle
+
+            batchSize = len(python_val)  # default batch size
+            # parse annotated to get the number of items saved in a pickle file.
+            if get_origin(python_type) is Annotated:
+                for annotation in get_args(python_type)[1:]:
+                    if isinstance(annotation, BatchSize):
+                        batchSize = annotation.val
+                        break
+            lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batchSize], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batchSize)]  # type: ignore
+        else:
+            t = self.get_sub_type(python_type)
+            lit_list = [TypeEngine.to_literal(ctx, x, t, expected.collection_type) for x in python_val]  # type: ignore
         return Literal(collection=LiteralCollection(literals=lit_list))
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> typing.List[typing.Any]:  # type: ignore
         try:
             lits = lv.collection.literals
         except AttributeError:
             raise TypeTransformerFailedError()
+        if self.is_batchable(expected_python_type):
+            from flytekit.types.pickle import FlytePickle
 
-        st = self.get_sub_type(expected_python_type)
-        return [TypeEngine.to_python_value(ctx, x, st) for x in lits]
+            batch_list = [TypeEngine.to_python_value(ctx, batch, FlytePickle) for batch in lits]
+            if len(batch_list) > 0 and type(batch_list[0]) is list:
+                # Make it have backward compatibility. The upstream task may use old version of Flytekit that
+                # won't merge the elements in the list. Therefore, we should check if the batch_list[0] is the list first.
+                return [item for batch in batch_list for item in batch]
+            return batch_list
+        else:
+            st = self.get_sub_type(expected_python_type)
+            return [TypeEngine.to_python_value(ctx, x, st) for x in lits]
 
     def guess_python_type(self, literal_type: LiteralType) -> list:  # type: ignore
         if literal_type.collection_type:
             ct: Type = TypeEngine.guess_python_type(literal_type.collection_type)
             return typing.List[ct]  # type: ignore
         raise ValueError(f"List transformer cannot reverse {literal_type}")
 
@@ -1040,15 +1085,15 @@
 
         ucols = usdt.columns
         dcols = dsdt.columns
 
         if len(ucols) != len(dcols):
             return False
 
-        for (u, d) in zip(ucols, dcols):
+        for u, d in zip(ucols, dcols):
             if u.name != d.name:
                 return False
 
             if not _are_types_castable(u.literal_type, d.literal_type):
                 return False
 
         return True
```

### Comparing `flytekit-1.5.0b1/flytekit/core/type_helpers.py` & `flytekit-1.6.0b0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/utils.py` & `flytekit-1.6.0b0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/core/workflow.py` & `flytekit-1.6.0b0/flytekit/core/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.python_auto_container import PythonAutoContainerTask
 from flytekit.core.reference_entity import ReferenceEntity, WorkflowReference
 from flytekit.core.tracker import extract_task_module
-from flytekit.core.type_engine import TypeEngine
+from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.exceptions.user import FlyteValidationException, FlyteValueException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.documentation import Description, Documentation
@@ -256,29 +256,38 @@
         """
         Workflow needs to fill in default arguments before invoking the call handler.
         """
         # Get default arguments and override with kwargs passed in
         input_kwargs = self.python_interface.default_inputs_as_kwargs
         input_kwargs.update(kwargs)
         self.compile()
-        return flyte_entity_call_handler(self, *args, **input_kwargs)
+        try:
+            return flyte_entity_call_handler(self, *args, **input_kwargs)
+        except Exception as exc:
+            exc.args = (f"Encountered error while executing workflow '{self.name}':\n  {exc}", *exc.args[1:])
+            raise exc
 
     def execute(self, **kwargs):
         raise Exception("Should not be called")
 
     def compile(self, **kwargs):
         pass
 
     def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
         # This is done to support the invariant that Workflow local executions always work with Promise objects
         # holding Flyte literal values. Even in a wf, a user can call a sub-workflow with a Python native value.
         for k, v in kwargs.items():
             if not isinstance(v, Promise):
                 t = self.python_interface.inputs[k]
-                kwargs[k] = Promise(var=k, val=TypeEngine.to_literal(ctx, v, t, self.interface.inputs[k].type))
+                try:
+                    kwargs[k] = Promise(var=k, val=TypeEngine.to_literal(ctx, v, t, self.interface.inputs[k].type))
+                except TypeTransformerFailedError as exc:
+                    raise TypeError(
+                        f"Failed to convert input argument '{k}' of workflow '{self.name}':\n  {exc}"
+                    ) from exc
 
         # The output of this will always be a combination of Python native values and Promises containing Flyte
         # Literals.
         self.compile()
         function_outputs = self.execute(**kwargs)
 
         # First handle the empty return case.
```

### Comparing `flytekit-1.5.0b1/flytekit/deck/deck.py` & `flytekit-1.6.0b0/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/deck/html/template.html` & `flytekit-1.6.0b0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/deck/renderer.py` & `flytekit-1.6.0b0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/exceptions/scopes.py` & `flytekit-1.6.0b0/flytekit/exceptions/scopes.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,18 +190,21 @@
     we create here will only be handled within our system code so we don't need to worry about leaking weird exceptions
     to the user.
     """
     try:
         _CONTEXT_STACK.append(_USER_CONTEXT)
         if _is_base_context():
             # See comment at this location for system_entry_point
+            fn_name = wrapped.__name__
             try:
                 return wrapped(*args, **kwargs)
-            except FlyteScopedException as ex:
-                raise ex.value
+            except FlyteScopedException as exc:
+                raise exc.type(f"Error encountered while executing '{fn_name}':\n  {exc.value}") from exc
+            except Exception as exc:
+                raise type(exc)(f"Error encountered while executing '{fn_name}':\n  {exc}") from exc
         else:
             try:
                 return wrapped(*args, **kwargs)
             except FlyteScopedException as scoped:
                 raise scoped
             except _user_exceptions.FlyteUserException:
                 raise FlyteScopedUserException(*_exc_info())
```

### Comparing `flytekit-1.5.0b1/flytekit/exceptions/system.py` & `flytekit-1.6.0b0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/exceptions/user.py` & `flytekit-1.6.0b0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extend/__init__.py` & `flytekit-1.6.0b0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.0b0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.0b0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.0b0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/pytorch/native.py` & `flytekit-1.6.0b0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.0b0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/sklearn/native.py` & `flytekit-1.6.0b0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.0b0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/tasks/shell.py` & `flytekit-1.6.0b0/flytekit/extras/tasks/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import os
+import platform
 import string
 import subprocess
 import typing
 from dataclasses import dataclass
 
 import flytekit
 from flytekit.core.context_manager import ExecutionParameters
@@ -209,14 +210,17 @@
         gen_script = self._interpolizer.interpolate(self._script, inputs=kwargs, outputs=outputs)
         if self._debug:
             print("\n==============================================\n")
             print(gen_script)
             print("\n==============================================\n")
 
         try:
+            if platform.system() == "Windows" and os.environ.get("ComSpec") is None:
+                # https://github.com/python/cpython/issues/101283
+                os.environ["ComSpec"] = "C:\\Windows\\System32\\cmd.exe"
             subprocess.check_call(gen_script, shell=True)
         except subprocess.CalledProcessError as e:
             files = os.listdir(".")
             fstr = "\n-".join(files)
             logger.error(
                 f"Failed to Execute Script, return-code {e.returncode} \n"
                 f"StdErr: {e.stderr}\n"
@@ -352,15 +356,14 @@
         return None
 
 
 # The raw_shell_task is an instance of RawShellTask and wraps a 'pure' shell script
 # This utility function allows for the specification of env variables, arguments, and the actual script within the
 # workflow definition rather than at `RawShellTask` instantiation
 def get_raw_shell_task(name: str) -> RawShellTask:
-
     return RawShellTask(
         name=name,
         debug=True,
         inputs=flytekit.kwtypes(env=typing.Dict[str, str], script_args=str, script_file=str),
         output_locs=[
             OutputLocation(
                 var="out",
```

### Comparing `flytekit-1.5.0b1/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.0b0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.0b0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.0b0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.0b0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.0b0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/interfaces/random.py` & `flytekit-1.6.0b0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/interfaces/stats/client.py` & `flytekit-1.6.0b0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.0b0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/loggers.py` & `flytekit-1.6.0b0/flytekit/loggers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
 import os
 
 from pythonjsonlogger import jsonlogger
+from rich.console import Console
+from rich.logging import RichHandler
 
 # Note:
 # The environment variable controls exposed to affect the individual loggers should be considered to be beta.
 # The ux/api may change in the future.
 # At time of writing, the code was written to preserve existing default behavior
 # For now, assume this is the environment variable whose usage will remain unchanged and controls output for all
 # loggers defined in this file.
 LOGGING_ENV_VAR = "FLYTE_SDK_LOGGING_LEVEL"
+LOGGING_FMT_ENV_VAR = "FLYTE_SDK_LOGGING_FORMAT"
 
 # By default, the root flytekit logger to debug so everything is logged, but enable fine-tuning
 logger = logging.getLogger("flytekit")
 
 # Stop propagation so that configuration is isolated to this file (so that it doesn't matter what the
 # global Python root logger is set to).
 logger.propagate = False
@@ -29,16 +32,26 @@
 auth_logger = child_loggers["auth"]
 cli_logger = child_loggers["cli"]
 remote_logger = child_loggers["remote"]
 entrypoint_logger = child_loggers["entrypoint"]
 user_space_logger = child_loggers["user_space"]
 
 # create console handler
-ch = logging.StreamHandler()
-ch.setLevel(logging.DEBUG)
+try:
+    handler = RichHandler(
+        rich_tracebacks=True,
+        omit_repeated_times=False,
+        keywords=["[flytekit]"],
+        log_time_format="%Y-%m-%d %H:%M:%S,%f",
+        console=Console(width=os.get_terminal_size().columns),
+    )
+except OSError:
+    handler = logging.StreamHandler()
+
+handler.setLevel(logging.DEBUG)
 
 # Root logger control
 # Don't want to import the configuration library since that will cause all sorts of circular imports, let's
 # just use the environment variable if it's defined. Decide in the future when we implement better controls
 # if we should control with the channel or with the logger level.
 # The handler log level controls whether log statements will actually print to the screen
 flytekit_root_env_var = f"{LOGGING_ENV_VAR}_ROOT"
@@ -59,14 +72,18 @@
     else:
         if child_logger is user_space_logger:
             child_logger.setLevel(logging.INFO)
         else:
             child_logger.setLevel(logging.WARNING)
 
 # create formatter
-formatter = jsonlogger.JsonFormatter(fmt="%(asctime)s %(name)s %(levelname)s %(message)s")
+logging_fmt = os.environ.get(LOGGING_FMT_ENV_VAR, "json")
+if logging_fmt == "json":
+    formatter = jsonlogger.JsonFormatter(fmt="%(asctime)s %(name)s %(levelname)s %(message)s")
+else:
+    formatter = logging.Formatter(fmt="[%(name)s] %(message)s")
 
-# add formatter to ch
-ch.setFormatter(formatter)
+# add formatter to the handler
+handler.setFormatter(formatter)
 
 # add ch to logger
-logger.addHandler(ch)
+logger.addHandler(handler)
```

### Comparing `flytekit-1.5.0b1/flytekit/models/admin/common.py` & `flytekit-1.6.0b0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/admin/task_execution.py` & `flytekit-1.6.0b0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/admin/workflow.py` & `flytekit-1.6.0b0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/annotation.py` & `flytekit-1.6.0b0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/array_job.py` & `flytekit-1.6.0b0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/common.py` & `flytekit-1.6.0b0/flytekit/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc as _abc
 import json as _json
+import re
 
 from flyteidl.admin import common_pb2 as _common_pb2
 from google.protobuf import json_format as _json_format
 from google.protobuf import struct_pb2 as _struct
 
 
 class FlyteABCMeta(_abc.ABCMeta):
@@ -53,15 +54,16 @@
     def __hash__(self):
         return hash(self.to_flyte_idl().SerializeToString(deterministic=True))
 
     def short_string(self):
         """
         :rtype: Text
         """
-        return str(self.to_flyte_idl())
+        literal_str = re.sub(r"\s+", " ", str(self.to_flyte_idl())).strip()
+        return f"<FlyteLiteral {literal_str}>"
 
     def verbose_string(self):
         """
         :rtype: Text
         """
         return self.short_string()
```

### Comparing `flytekit-1.5.0b1/flytekit/models/core/catalog.py` & `flytekit-1.6.0b0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/compiler.py` & `flytekit-1.6.0b0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/condition.py` & `flytekit-1.6.0b0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/errors.py` & `flytekit-1.6.0b0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/execution.py` & `flytekit-1.6.0b0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/identifier.py` & `flytekit-1.6.0b0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/types.py` & `flytekit-1.6.0b0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/core/workflow.py` & `flytekit-1.6.0b0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/documentation.py` & `flytekit-1.6.0b0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/dynamic_job.py` & `flytekit-1.6.0b0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/execution.py` & `flytekit-1.6.0b0/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/filters.py` & `flytekit-1.6.0b0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/interface.py` & `flytekit-1.6.0b0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/launch_plan.py` & `flytekit-1.6.0b0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/literals.py` & `flytekit-1.6.0b0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/matchable_resource.py` & `flytekit-1.6.0b0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/named_entity.py` & `flytekit-1.6.0b0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/node_execution.py` & `flytekit-1.6.0b0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/presto.py` & `flytekit-1.6.0b0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/project.py` & `flytekit-1.6.0b0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/qubole.py` & `flytekit-1.6.0b0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/schedule.py` & `flytekit-1.6.0b0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/security.py` & `flytekit-1.6.0b0/flytekit/models/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,36 @@
         FILE = _sec.Secret.MountType.FILE
         """
         Use this for Secrets that cannot be injected into env-var or need to be available as a file
         Caution: May not be supported in all environments
         """
 
     group: str
-    key: str
+    key: Optional[str] = None
     group_version: Optional[str] = None
     mount_requirement: MountType = MountType.ANY
 
     def __post_init__(self):
         if self.group is None:
             raise ValueError("Group is a required parameter")
-        if self.key is None:
-            raise ValueError("Key is also a required parameter")
 
     def to_flyte_idl(self) -> _sec.Secret:
         return _sec.Secret(
             group=self.group,
             group_version=self.group_version,
             key=self.key,
             mount_requirement=self.mount_requirement.value,
         )
 
     @classmethod
     def from_flyte_idl(cls, pb2_object: _sec.Secret) -> "Secret":
         return cls(
             group=pb2_object.group,
             group_version=pb2_object.group_version if pb2_object.group_version else None,
-            key=pb2_object.key,
+            key=pb2_object.key if pb2_object.key else None,
             mount_requirement=Secret.MountType(pb2_object.mount_requirement),
         )
 
 
 @dataclass
 class OAuth2Client(_common.FlyteIdlEntity):
     client_id: str
```

### Comparing `flytekit-1.5.0b1/flytekit/models/task.py` & `flytekit-1.6.0b0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/types.py` & `flytekit-1.6.0b0/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/models/workflow_closure.py` & `flytekit-1.6.0b0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/remote/__init__.py` & `flytekit-1.6.0b0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/remote/backfill.py` & `flytekit-1.6.0b0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/remote/entities.py` & `flytekit-1.6.0b0/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/remote/executions.py` & `flytekit-1.6.0b0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/remote/lazy_entity.py` & `flytekit-1.6.0b0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/remote/remote.py` & `flytekit-1.6.0b0/flytekit/remote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,14 +617,18 @@
             serialization_settings = SerializationSettings(
                 ImageConfig.auto_default_image(),
                 project=self.default_project,
                 domain=self.default_domain,
                 version=version,
             )
             is_dummy_serialization_setting = True
+
+        if serialization_settings.version is None:
+            serialization_settings.version = version
+
         _ = get_serializable(m, settings=serialization_settings, entity=entity, options=options)
 
         ident = None
         for entity, cp_entity in m.items():
             if not isinstance(cp_entity, admin_workflow_models.WorkflowSpec) and is_dummy_serialization_setting:
                 # Only in the case of workflows can we use the dummy serialization settings.
                 raise user_exceptions.FlyteValueException(
@@ -706,17 +710,17 @@
         :return: md5_bytes, url
         """
         # Create a zip file containing all the entries.
         zip_file = fast_package(root, output, deref_symlinks)
         md5_bytes, _ = hash_file(pathlib.Path(zip_file))
 
         # Upload zip file to Admin using FlyteRemote.
-        return self._upload_file(pathlib.Path(zip_file))
+        return self.upload_file(pathlib.Path(zip_file))
 
-    def _upload_file(
+    def upload_file(
         self, to_upload: pathlib.Path, project: typing.Optional[str] = None, domain: typing.Optional[str] = None
     ) -> typing.Tuple[bytes, str]:
         """
         Function will use remote's client to hash and then upload the file using Admin's data proxy service.
 
         :param to_upload: Must be a single file
         :param project: Project to upload under, if not supplied will use the remote's default
@@ -816,15 +820,15 @@
         """
         if image_config is None:
             image_config = ImageConfig.auto_default_image()
 
         with tempfile.TemporaryDirectory() as tmp_dir:
             archive_fname = pathlib.Path(os.path.join(tmp_dir, "script_mode.tar.gz"))
             compress_scripts(source_path, str(archive_fname), module_name)
-            md5_bytes, upload_native_url = self._upload_file(
+            md5_bytes, upload_native_url = self.upload_file(
                 archive_fname, project or self.default_project, domain or self.default_domain
             )
 
         serialization_settings = SerializationSettings(
             project=project,
             domain=domain,
             image_config=image_config,
```

### Comparing `flytekit-1.5.0b1/flytekit/remote/remote_callable.py` & `flytekit-1.6.0b0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/testing/__init__.py` & `flytekit-1.6.0b0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/tools/fast_registration.py` & `flytekit-1.6.0b0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/tools/ignore.py` & `flytekit-1.6.0b0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/tools/module_loader.py` & `flytekit-1.6.0b0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/tools/repo.py` & `flytekit-1.6.0b0/flytekit/tools/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     See :py:class:`flytekit.models.core.identifier.ResourceType` to match the trailing index in the file name with the
     entity type.
     :param options:
     :param settings: SerializationSettings to be used
     :param pkgs: Dot-delimited Python packages/subpackages to look into for serialization.
     :param local_source_root: Where to start looking for the code.
     """
-
+    settings.source_root = local_source_root
     ctx = FlyteContextManager.current_context().with_serialization_settings(settings)
     with FlyteContextManager.with_context(ctx) as ctx:
         # Scan all modules. the act of loading populates the global singleton that contains all objects
         with module_loader.add_sys_path(local_source_root):
             click.secho(f"Loading packages {pkgs} under source root {local_source_root}", fg="yellow")
             module_loader.just_load_modules(pkgs=pkgs)
 
@@ -56,14 +56,16 @@
     local_source_root: typing.Optional[str] = None,
     folder: str = ".",
     options: typing.Optional[Options] = None,
 ):
     """
     Serialize the given set of python packages to a folder
     """
+    if folder is None:
+        folder = "."
     loaded_entities = serialize(pkgs, settings, local_source_root, options=options)
     persist_registrable_entities(loaded_entities, folder)
 
 
 def package(
     serializable_entities: typing.List[FlyteControlPlaneEntity],
     source: str = ".",
```

### Comparing `flytekit-1.5.0b1/flytekit/tools/script_mode.py` & `flytekit-1.6.0b0/flytekit/tools/script_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,20 @@
             if not chunk:
                 break
             h.update(chunk)
 
     return h.digest(), h.hexdigest()
 
 
-def _find_project_root(source_path) -> Path:
+def _find_project_root(source_path) -> str:
     """
     Find the root of the project.
     The root of the project is considered to be the first ancestor from source_path that does
     not contain a __init__.py file.
 
     N.B.: This assumption only holds for regular packages (as opposed to namespace packages)
     """
     # Start from the directory right above source_path
     path = Path(source_path).parent.resolve()
     while os.path.exists(os.path.join(path, "__init__.py")):
         path = path.parent
-    return path
+    return str(path)
```

### Comparing `flytekit-1.5.0b1/flytekit/tools/subprocess.py` & `flytekit-1.6.0b0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/tools/translator.py` & `flytekit-1.6.0b0/flytekit/tools/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,19 +659,14 @@
 
     elif isinstance(entity, LaunchPlan):
         cp_entity = get_serializable_launch_plan(entity_mapping, settings, entity, options=options)
 
     elif isinstance(entity, BranchNode):
         cp_entity = get_serializable_branch_node(entity_mapping, settings, entity, options)
 
-    elif isinstance(entity, GateNode):
-        import ipdb
-
-        ipdb.set_trace()
-
     elif isinstance(entity, FlyteTask) or isinstance(entity, FlyteWorkflow):
         if entity.should_register:
             if isinstance(entity, FlyteTask):
                 cp_entity = get_serializable_flyte_task(entity, settings)
             else:
                 if entity.should_register:
                     # We only add the tasks if the should register flag is set. This is to avoid adding
```

### Comparing `flytekit-1.5.0b1/flytekit/types/directory/__init__.py` & `flytekit-1.6.0b0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/directory/types.py` & `flytekit-1.6.0b0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/file/__init__.py` & `flytekit-1.6.0b0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/file/file.py` & `flytekit-1.6.0b0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.0b0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/pickle/pickle.py` & `flytekit-1.6.0b0/flytekit/types/pickle/pickle.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 
 T = typing.TypeVar("T")
 
 
+class BatchSize:
+    """
+    Flyte-specific object used to wrap the hash function for a specific type
+    """
+
+    def __init__(self, val: int):
+        self._val = val
+
+    @property
+    def val(self) -> int:
+        return self._val
+
+
 class FlytePickle(typing.Generic[T]):
     """
     This type is only used by flytekit internally. User should not use this type.
     Any type that flyte can't recognize will become FlytePickle
     """
 
     @classmethod
```

### Comparing `flytekit-1.5.0b1/flytekit/types/schema/types.py` & `flytekit-1.6.0b0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.0b0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/structured/__init__.py` & `flytekit-1.6.0b0/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.0b0/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/structured/bigquery.py` & `flytekit-1.6.0b0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.0b0/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.0b0/flytekit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.5.0b1 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
->=3.8,<3.12 Description-Content-Type: text/markdown License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.8,<3.12
+Description-Content-Type: text/markdown License-File: LICENSE
                                  [Flyte Logo]
                          ****** Flytekit Python ******
             Flytekit Python is the Python SDK built on top of Flyte
                    **** Plugins  Â·  Contribution_Guide ****
 [![PyPI version fury.io](https://badge.fury.io/py/flytekit.svg)](https://
 pypi.python.org/pypi/flytekit/) [![PyPI download day](https://img.shields.io/
 pypi/dd/flytekit.svg)](https://pypi.python.org/pypi/flytekit/) [![PyPI download
```

### Comparing `flytekit-1.5.0b1/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.0b0/flytekit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 flytekit/clis/__init__.py
 flytekit/clis/helpers.py
 flytekit/clis/flyte_cli/__init__.py
 flytekit/clis/flyte_cli/example.config
 flytekit/clis/flyte_cli/main.py
 flytekit/clis/sdk_in_container/__init__.py
 flytekit/clis/sdk_in_container/backfill.py
+flytekit/clis/sdk_in_container/build.py
 flytekit/clis/sdk_in_container/constants.py
 flytekit/clis/sdk_in_container/helpers.py
 flytekit/clis/sdk_in_container/init.py
+flytekit/clis/sdk_in_container/launchplan.py
 flytekit/clis/sdk_in_container/local_cache.py
 flytekit/clis/sdk_in_container/package.py
 flytekit/clis/sdk_in_container/pyflyte.py
 flytekit/clis/sdk_in_container/register.py
 flytekit/clis/sdk_in_container/run.py
 flytekit/clis/sdk_in_container/serialize.py
 flytekit/clis/sdk_in_container/utils.py
@@ -113,14 +115,16 @@
 flytekit/extras/sqlite3/__init__.py
 flytekit/extras/sqlite3/task.py
 flytekit/extras/tasks/__init__.py
 flytekit/extras/tasks/shell.py
 flytekit/extras/tensorflow/__init__.py
 flytekit/extras/tensorflow/model.py
 flytekit/extras/tensorflow/record.py
+flytekit/image_spec/__init__.py
+flytekit/image_spec/image_spec.py
 flytekit/interaction/__init__.py
 flytekit/interaction/parse_stdin.py
 flytekit/interfaces/__init__.py
 flytekit/interfaces/cli_identifiers.py
 flytekit/interfaces/random.py
 flytekit/interfaces/stats/__init__.py
 flytekit/interfaces/stats/client.py
```

### Comparing `flytekit-1.5.0b1/flytekit.egg-info/requires.txt` & `flytekit-1.6.0b0/flytekit.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 docker<7.0.0,>=4.0.0
 python-dateutil>=2.1
 grpcio<2.0,>=1.50.0
 grpcio-status<2.0,>=1.50.0
 importlib-metadata
 fsspec>=2023.3.0
 adlfs
-s3fs
+s3fs>=0.6.0
 gcsfs
 pyopenssl
 joblib
 python-json-logger>=2.0.0
 pytimeparse<2.0.0,>=1.1.8
 pytz
 pyyaml
@@ -36,10 +36,11 @@
 docstring-parser>=0.9.0
 diskcache>=5.2.1
 cloudpickle>=2.0.0
 cookiecutter>=1.7.3
 numpy
 gitpython
 kubernetes>=12.0.1
+rich
 
 [:python_version < "3.8.0"]
 singledispatchmethod
```

### Comparing `flytekit-1.5.0b1/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.0b0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.5.0b1/setup.py` & `flytekit-1.6.0b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.5.0b1"
+__version__ = "1.6.0b0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -41,15 +41,15 @@
         # Restrict grpcio and grpcio-status.  Version 1.50.0 pulls in a version of protobuf that is not compatible
         # with the old protobuf library (as described in https://developers.google.com/protocol-buffers/docs/news/2022-05-06)
         "grpcio>=1.50.0,<2.0",
         "grpcio-status>=1.50.0,<2.0",
         "importlib-metadata",
         "fsspec>=2023.3.0",
         "adlfs",
-        "s3fs",
+        "s3fs>=0.6.0",
         "gcsfs",
         "pyopenssl",
         "joblib",
         "python-json-logger>=2.0.0",
         "pytimeparse>=1.1.8,<2.0.0",
         "pytz",
         "pyyaml",
@@ -69,14 +69,15 @@
         "docstring-parser>=0.9.0",
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
         "numpy",
         "gitpython",
         "kubernetes>=12.0.1",
+        "rich",
     ],
     extras_require=extras_require,
     scripts=[
         "flytekit_scripts/flytekit_build_image.sh",
         "flytekit_scripts/flytekit_venv",
         "flytekit/bin/entrypoint.py",
     ],
@@ -85,14 +86,15 @@
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```


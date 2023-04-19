# Comparing `tmp/dagster-1.2.7.tar.gz` & `tmp/dagster-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.2.7.tar", last modified: Thu Apr 13 15:03:47 2023, max compression
+gzip compressed data, was "dagster-1.3.0.tar", last modified: Wed Apr 19 19:01:52 2023, max compression
```

## Comparing `dagster-1.2.7.tar` & `dagster-1.3.0.tar`

### file list

```diff
@@ -1,622 +1,625 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-13 15:03:06.000000 dagster-1.2.7/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:06.000000 dagster-1.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-13 15:03:06.000000 dagster-1.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-13 15:03:47.032711 dagster-1.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-04-13 15:03:06.000000 dagster-1.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster/
--rw-r--r--   0 root         (0) root         (0)    24945 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27129 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8207 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3456 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    33891 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5141 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19909 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28486 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14686 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18799 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16840 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.972711 dagster-1.2.7/dagster/_config/structured_config/
--rw-r--r--   0 root         (0) root         (0)    47857 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/structured_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6219 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/structured_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/structured_config/utils.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    16671 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.976711 dagster-1.2.7/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13519 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.976711 dagster-1.2.7/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2117 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7829 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28701 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10380 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)    22609 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_group.py
--rw-r--r--   0 root         (0) root         (0)     3817 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36853 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    43705 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    16164 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     4984 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    57573 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    23019 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     3067 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    15009 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45721 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10877 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20631 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    15887 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40311 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9563 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10261 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17814 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14491 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8349 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11709 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     7196 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    21501 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    33816 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21562 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10087 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8001 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    15897 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44446 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22927 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)    46465 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    16650 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7422 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    33294 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/mode.py
--rw-r--r--   0 root         (0) root         (0)    54997 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    21053 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11938 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     3307 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    20633 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    18471 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)    18917 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    44315 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    34900 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/pipeline_definition.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)     9054 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/preset.py
--rw-r--r--   0 root         (0) root         (0)    30644 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    23982 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    19566 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    19180 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8118 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    25150 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    14761 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    35086 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    32988 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10753 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    41375 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    13809 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    73361 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6232 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.988711 dagster-1.2.7/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    65032 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.992711 dagster-1.2.7/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41958 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    25196 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14370 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6082 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.992711 dagster-1.2.7/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22487 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    16287 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    27186 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27386 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    34437 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    43261 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    20099 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/context_creation_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     6480 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execute_job_result.py
--rw-r--r--   0 root         (0) root         (0)     9184 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8734 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14650 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23056 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7095 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12509 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16478 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27421 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10255 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    38667 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    60978 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15617 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    16031 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19527 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)    25987 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/results.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10333 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1136 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4175 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2855 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15452 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14347 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.996711 dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2874 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33996 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    33186 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    69236 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    11276 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4341 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)    17332 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     5205 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/pipeline_index.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   103980 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11309 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24286 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6413 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17327 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11050 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    18194 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.000712 dagster-1.2.7/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20631 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.004711 dagster-1.2.7/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4019 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12052 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14447 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)    17447 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/snap/pipeline_snapshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.008711 dagster-1.2.7/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.008711 dagster-1.2.7/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7205 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8073 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16259 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9579 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)    11527 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14277 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    77841 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7409 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18916 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)     9985 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    26222 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17376 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23190 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)    23993 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/pipeline_run.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16059 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8629 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46758 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.016712 dagster-1.2.7/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6818 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    19749 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3660 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     2885 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    10435 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14729 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15907 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27288 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    18680 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7393 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35947 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/utility_solids.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5451 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    26703 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.020712 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6882 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9084 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4422 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17377 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8371 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16312 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    35694 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2731 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.964711 dagster-1.2.7/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.024711 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11665 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    38179 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18538 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    22252 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5394 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    52644 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26106 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      638 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32009 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    33924 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.028711 dagster-1.2.7/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23212 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8687 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4238 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    23709 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    11139 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3290 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10483 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    23902 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:47.032711 dagster-1.2.7/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:03:06.000000 dagster-1.2.7/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:03:46.968711 dagster-1.2.7/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24855 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1290 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-13 15:03:46.000000 dagster-1.2.7/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-13 15:03:47.032711 dagster-1.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6429 2023-04-13 15:03:07.000000 dagster-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-19 19:01:29.000000 dagster-1.3.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-19 19:01:29.000000 dagster-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-19 19:01:29.000000 dagster-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-19 19:01:52.727803 dagster-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-04-19 19:01:29.000000 dagster-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster/
+-rw-r--r--   0 root         (0) root         (0)    25230 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.663803 dagster-1.3.0/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27263 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8207 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5718 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    33891 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5141 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19909 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.663803 dagster-1.3.0/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28486 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.663803 dagster-1.3.0/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14686 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18799 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    17554 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.667803 dagster-1.3.0/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    58020 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     6217 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    16671 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.667803 dagster-1.3.0/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13519 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.667803 dagster-1.3.0/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7997 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10380 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)    22609 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_group.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    36853 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    46445 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    17185 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    58973 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24065 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    15537 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45721 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10877 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20634 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    17905 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40545 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9563 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10731 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17810 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14491 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11914 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6695 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    20403 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39915 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31183 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21562 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16178 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44593 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22927 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)    46583 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18335 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7422 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32712 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/mode.py
+-rw-r--r--   0 root         (0) root         (0)    55735 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    21561 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    20633 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19242 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    18917 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    44376 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    34900 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/pipeline_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)     9054 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/preset.py
+-rw-r--r--   0 root         (0) root         (0)    30644 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    23982 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    19736 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    19180 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8118 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    25522 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    14975 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    37627 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    35100 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10753 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    43829 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    14153 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    73361 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15807 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    25453 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.679803 dagster-1.3.0/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    65032 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.683803 dagster-1.3.0/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:29.000000 dagster-1.3.0/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41958 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    25196 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14370 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.683803 dagster-1.3.0/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22487 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    27186 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27826 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    34437 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    43261 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    20099 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/context_creation_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execute_job_result.py
+-rw-r--r--   0 root         (0) root         (0)     9184 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8734 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14650 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23056 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7095 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16478 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27380 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10255 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    38667 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    60978 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15617 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    16031 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19527 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)    25987 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/results.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15452 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14347 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.687803 dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33996 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    33186 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    69685 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    11276 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)    17332 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/pipeline_index.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   104545 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11577 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24318 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17327 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11050 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    18194 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.691803 dagster-1.3.0/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.695803 dagster-1.3.0/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20631 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.695803 dagster-1.3.0/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4019 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12052 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14487 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)    17447 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/snap/pipeline_snapshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.699803 dagster-1.3.0/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.699803 dagster-1.3.0/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7205 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8073 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16259 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9579 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    11527 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14277 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     5090 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)    77841 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    18916 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9985 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    26262 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17376 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23190 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)    23993 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/pipeline_run.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15584 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8629 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46721 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.707803 dagster-1.3.0/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5344 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4095 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    19749 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14729 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15907 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27288 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18883 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7393 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/utility_solids.py
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5451 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    26703 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5450 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.711803 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6882 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9124 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17726 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8371 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/monitoring/monitoring_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16312 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    35694 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.655803 dagster-1.3.0/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.715803 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11665 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38179 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18538 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    22252 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    52644 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26106 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32009 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    33924 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.719803 dagster-1.3.0/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23212 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8687 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    23704 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9813 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    10483 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    23902 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.727803 dagster-1.3.0/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 19:01:30.000000 dagster-1.3.0/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:01:52.659803 dagster-1.3.0/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24986 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 19:01:52.000000 dagster-1.3.0/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-19 19:01:52.731804 dagster-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-04-19 19:01:30.000000 dagster-1.3.0/setup.py
```

### Comparing `dagster-1.2.7/COPYING` & `dagster-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/LICENSE` & `dagster-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/PKG-INFO` & `dagster-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.2.7
+Version: 1.3.0
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.2.7/README.md` & `dagster-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/__init__.py` & `dagster-1.3.0/dagster/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,40 +88,42 @@
 from dagster._config.field_utils import (
     EnvVar as EnvVar,
     Map as Map,
     Permissive as Permissive,
     Selector as Selector,
     Shape as Shape,
 )
-from dagster._config.source import (
-    BoolSource as BoolSource,
-    IntSource as IntSource,
-    StringSource as StringSource,
-)
-from dagster._config.structured_config import (
+from dagster._config.pythonic_config import (
     Config as Config,
     ConfigurableIOManager as ConfigurableIOManager,
     ConfigurableIOManagerFactory as ConfigurableIOManagerFactory,
     ConfigurableLegacyIOManagerAdapter as ConfigurableLegacyIOManagerAdapter,
-    ConfigurableLegacyResourceAdapter as ConfigurableLegacyResourceAdapter,
     ConfigurableResource as ConfigurableResource,
-    ConfigurableResourceFactory as ConfigurableResourceFactory,
+    IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
     PermissiveConfig as PermissiveConfig,
     ResourceDependency as ResourceDependency,
 )
+from dagster._config.source import (
+    BoolSource as BoolSource,
+    IntSource as IntSource,
+    StringSource as StringSource,
+)
 from dagster._core.definitions.asset_in import AssetIn as AssetIn
 from dagster._core.definitions.asset_out import AssetOut as AssetOut
 from dagster._core.definitions.asset_reconciliation_sensor import (
     build_asset_reconciliation_sensor as build_asset_reconciliation_sensor,
 )
 from dagster._core.definitions.asset_selection import AssetSelection as AssetSelection
 from dagster._core.definitions.asset_sensor_definition import (
     AssetSensorDefinition as AssetSensorDefinition,
 )
 from dagster._core.definitions.assets import AssetsDefinition as AssetsDefinition
+from dagster._core.definitions.auto_materialize_policy import (
+    AutoMaterializePolicy as AutoMaterializePolicy,
+)
 from dagster._core.definitions.composition import PendingNodeInvocation as PendingNodeInvocation
 from dagster._core.definitions.config import ConfigMapping as ConfigMapping
 from dagster._core.definitions.configurable import configured as configured
 from dagster._core.definitions.data_version import (
     DataProvenance as DataProvenance,
     DataVersion as DataVersion,
 )
@@ -296,15 +298,18 @@
 from dagster._core.definitions.resource_definition import (
     ResourceDefinition as ResourceDefinition,
     make_values_resource as make_values_resource,
     resource as resource,
 )
 from dagster._core.definitions.run_config import RunConfig as RunConfig
 from dagster._core.definitions.run_request import (
+    AddDynamicPartitionsRequest as AddDynamicPartitionsRequest,
+    DeleteDynamicPartitionsRequest as DeleteDynamicPartitionsRequest,
     RunRequest as RunRequest,
+    SensorResult as SensorResult,
     SkipReason as SkipReason,
 )
 from dagster._core.definitions.run_status_sensor_definition import (
     RunFailureSensorContext as RunFailureSensorContext,
     RunStatusSensorContext as RunStatusSensorContext,
     RunStatusSensorDefinition as RunStatusSensorDefinition,
     build_run_status_sensor_context as build_run_status_sensor_context,
@@ -475,15 +480,18 @@
     RunsFilter as RunsFilter,
 )
 from dagster._core.storage.root_input_manager import (
     RootInputManager as RootInputManager,
     RootInputManagerDefinition as RootInputManagerDefinition,
     root_input_manager as root_input_manager,
 )
-from dagster._core.storage.tags import MEMOIZED_RUN_TAG as MEMOIZED_RUN_TAG
+from dagster._core.storage.tags import (
+    MAX_RUNTIME_SECONDS_TAG as MAX_RUNTIME_SECONDS_TAG,
+    MEMOIZED_RUN_TAG as MEMOIZED_RUN_TAG,
+)
 from dagster._core.storage.upath_io_manager import UPathIOManager as UPathIOManager
 from dagster._core.types.config_schema import (
     DagsterTypeLoader as DagsterTypeLoader,
     dagster_type_loader as dagster_type_loader,
 )
 from dagster._core.types.dagster_type import (
     DagsterType as DagsterType,
```

### Comparing `dagster-1.2.7/dagster/_annotations.py` & `dagster-1.3.0/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/get_server_id.py` & `dagster-1.3.0/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/list_repositories.py` & `dagster-1.3.0/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/notebook_data.py` & `dagster-1.3.0/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.0/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/snapshot_partition.py` & `dagster-1.3.0/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/snapshot_pipeline.py` & `dagster-1.3.0/dagster/_api/snapshot_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/snapshot_repository.py` & `dagster-1.3.0/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/snapshot_schedule.py` & `dagster-1.3.0/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_api/snapshot_sensor.py` & `dagster-1.3.0/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_check/README.md` & `dagster-1.3.0/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_check/__init__.py` & `dagster-1.3.0/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/__init__.py` & `dagster-1.3.0/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/api.py` & `dagster-1.3.0/dagster/_cli/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -735,14 +735,17 @@
             else f"Dagster code server{code_desc}in process {os.getpid()}"
         )
 
         logger.info("Started %s", server_desc)
 
         try:
             server.serve()
+        except KeyboardInterrupt:
+            # Terminate cleanly on interrupt
+            logger.info("Code server was interrupted")
         finally:
             logger.info("Shutting down %s", server_desc)
 
 
 @api_cli.command(name="grpc-health-check", help="Check the status of a dagster GRPC server")
 @click.option(
     "--port",
```

### Comparing `dagster-1.2.7/dagster/_cli/asset.py` & `dagster-1.3.0/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/config_scaffolder.py` & `dagster-1.3.0/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/debug.py` & `dagster-1.3.0/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/dev.py` & `dagster-1.3.0/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/instance.py` & `dagster-1.3.0/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/job.py` & `dagster-1.3.0/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/load_handle.py` & `dagster-1.3.0/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/project.py` & `dagster-1.3.0/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/run.py` & `dagster-1.3.0/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/schedule.py` & `dagster-1.3.0/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/sensor.py` & `dagster-1.3.0/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/utils.py` & `dagster-1.3.0/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.0/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/__init__.py` & `dagster-1.3.0/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/config_schema.py` & `dagster-1.3.0/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/config_type.py` & `dagster-1.3.0/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/errors.py` & `dagster-1.3.0/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/evaluate_value_result.py` & `dagster-1.3.0/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/field.py` & `dagster-1.3.0/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/field_utils.py` & `dagster-1.3.0/dagster/_config/field_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -457,22 +457,24 @@
     if isinstance(potential_field, Field):
         return potential_field
 
     return Field(_convert_potential_type(original_root, potential_field, stack))
 
 
 def _config_dictionary_from_values_inner(obj: Any):
-    from dagster._config.structured_config import Config
+    from dagster._config.pythonic_config import Config
 
     if isinstance(obj, dict):
         return {k: _config_dictionary_from_values_inner(v) for k, v in obj.items() if v is not None}
     elif isinstance(obj, list):
         return [_config_dictionary_from_values_inner(v) for v in obj]
     elif isinstance(obj, EnvVar):
         return {"env": str(obj)}
+    elif isinstance(obj, IntEnvVar):
+        return {"env": obj.name}
     elif isinstance(obj, Config):
         return {
             k: _config_dictionary_from_values_inner(v)
             for k, v in obj._as_config_dict().items()  # noqa: SLF001
         }
     elif isinstance(obj, Enum):
         return obj.name
@@ -488,9 +490,33 @@
     and processing data structures such as dicts, lists, and structured Config classes.
     """
     assert ConfigTypeKind.is_shape(config_field.config_type.kind)
 
     return check.is_dict(_config_dictionary_from_values_inner(values))
 
 
+class IntEnvVar(int):
+    """Class used to represent an environment variable in the Dagster config system.
+
+    The environment variable will be resolved to an int value when the config is
+    loaded.
+    """
+
+    name: str
+
+    @classmethod
+    def create(cls, name: str) -> "IntEnvVar":
+        var = IntEnvVar(0)
+        var.name = name
+        return var
+
+
 class EnvVar(str):
-    pass
+    """Class used to represent an environment variable in the Dagster config system.
+
+    The environment variable will be resolved to a string value when the config is
+    loaded.
+    """
+
+    @classmethod
+    def int(cls, name: str) -> "IntEnvVar":
+        return IntEnvVar.create(name=name)
```

### Comparing `dagster-1.2.7/dagster/_config/post_process.py` & `dagster-1.3.0/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/primitive_mapping.py` & `dagster-1.3.0/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/snap.py` & `dagster-1.3.0/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/source.py` & `dagster-1.3.0/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/stack.py` & `dagster-1.3.0/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/structured_config/__init__.py` & `dagster-1.3.0/dagster/_config/pythonic_config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 import inspect
+import re
 from enum import Enum
 from typing import (
     AbstractSet,
     Any,
+    Callable,
     Dict,
     Generic,
     Iterable,
     Mapping,
     NamedTuple,
     Optional,
     Set,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from pydantic import ConstrainedFloat, ConstrainedInt, ConstrainedStr
-from typing_extensions import TypeAlias, get_args
+from typing_extensions import TypeAlias, TypeGuard, get_args
 
-from dagster import Enum as DagsterEnum
-from dagster._annotations import experimental
+from dagster import (
+    Enum as DagsterEnum,
+    Field as DagsterField,
+)
 from dagster._config.config_type import Array, ConfigFloatInstance, ConfigType, EnumValue, Noneable
 from dagster._config.field_utils import config_dictionary_from_values
 from dagster._config.post_process import resolve_defaults
+from dagster._config.pythonic_config.typing_utils import TypecheckAllowPartialResourceInitParams
 from dagster._config.source import BoolSource, IntSource, StringSource
-from dagster._config.structured_config.typing_utils import TypecheckAllowPartialResourceInitParams
 from dagster._config.validate import process_config, validate_config
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.definition_config_schema import (
     ConfiguredDefinitionConfigSchema,
     DefinitionConfigSchema,
 )
 from dagster._core.errors import (
     DagsterInvalidConfigDefinitionError,
     DagsterInvalidConfigError,
     DagsterInvalidDefinitionError,
+    DagsterInvalidInvocationError,
     DagsterInvalidPythonicConfigDefinitionError,
 )
 from dagster._core.execution.context.init import InitResourceContext
+from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX
+
+from .attach_other_object_to_context import (
+    IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
+)
 
 try:
     from functools import cached_property  # type: ignore  # (py37 compat)
 except ImportError:
 
     class cached_property:
         pass
@@ -71,14 +81,19 @@
 from dagster._core.storage.io_manager import IOManager, IOManagerDefinition
 
 from .typing_utils import BaseResourceMeta, LateBoundTypesForResourceTypeChecking
 from .utils import safe_is_subclass
 
 Self = TypeVar("Self", bound="ConfigurableResourceFactory")
 
+INTERNAL_MARKER = "__internal__"
+
+# ensure that this ends with the internal marker so we can do a single check
+assert CACHED_METHOD_FIELD_SUFFIX.endswith(INTERNAL_MARKER)
+
 
 class MakeConfigCacheable(BaseModel):
     """This class centralizes and implements all the chicanery we need in order
     to support caching decorators. If we decide this is a bad idea we can remove it
     all in one go.
     """
 
@@ -94,22 +109,62 @@
         frozen = True
 
     def __setattr__(self, name: str, value: Any):
         # This is a hack to allow us to set attributes on the class that are not part of the
         # config schema. Pydantic will normally raise an error if you try to set an attribute
         # that is not part of the schema.
 
-        if name.startswith("_") or name.endswith("_cache"):
+        if self._is_field_internal(name):
             object.__setattr__(self, name, value)
             return
 
-        return super().__setattr__(name, value)
+        try:
+            return super().__setattr__(name, value)
+        except (TypeError, ValueError) as e:
+            clsname = self.__class__.__name__
+            if "is immutable and does not support item assignment" in str(e):
+                if isinstance(self, ConfigurableResourceFactory):
+                    raise DagsterInvalidInvocationError(
+                        f"'{clsname}' is a Pythonic resource and does not support item assignment,"
+                        " as it inherits from 'pydantic.BaseModel' with frozen=True. If trying to"
+                        " maintain state on this resource, consider building a separate, stateful"
+                        " client class, and provide a method on the resource to construct and"
+                        " return the stateful client."
+                    ) from e
+                else:
+                    raise DagsterInvalidInvocationError(
+                        f"'{clsname}' is a Pythonic config class and does not support item"
+                        " assignment, as it inherits from 'pydantic.BaseModel' with frozen=True."
+                    ) from e
+            elif "object has no field" in str(e):
+                field_name = check.not_none(
+                    re.search(r"object has no field \"(.*)\"", str(e))
+                ).group(1)
+                if isinstance(self, ConfigurableResourceFactory):
+                    raise DagsterInvalidInvocationError(
+                        f"'{clsname}' is a Pythonic resource and does not support manipulating"
+                        f" undeclared attribute '{field_name}' as it inherits from"
+                        " 'pydantic.BaseModel' without extra=\"allow\". If trying to maintain"
+                        " state on this resource, consider building a separate, stateful client"
+                        " class, and provide a method on the resource to construct and return the"
+                        " stateful client."
+                    ) from e
+                else:
+                    raise DagsterInvalidInvocationError(
+                        f"'{clsname}' is a Pythonic config class and does not support manipulating"
+                        f" undeclared attribute '{field_name}' as it inherits from"
+                        " 'pydantic.BaseModel' without extra=\"allow\"."
+                    ) from e
+            else:
+                raise
+
+    def _is_field_internal(self, name: str) -> bool:
+        return name.endswith(INTERNAL_MARKER)
 
 
-@experimental
 class Config(MakeConfigCacheable):
     """Base class for Dagster configuration models."""
 
     def __init__(self, **config_dict) -> None:
         """This constructor is overridden to handle any remapping of raw config dicts to
         the appropriate config classes. For example, discriminated unions are represented
         in Dagster config as dicts with a single key, which is the discriminator value.
@@ -134,15 +189,15 @@
 
     def _as_config_dict(self) -> Mapping[str, Any]:
         """Returns a dictionary representation of this config object,
         ignoring any private fields.
         """
         output = {}
         for key, value in self.__dict__.items():
-            if key.startswith("_"):
+            if self._is_field_internal(key):
                 continue
             field = self.__fields__.get(key)
             if field and value is None and not _is_pydantic_field_required(field):
                 continue
             if field:
                 output[field.alias] = value
             else:
@@ -150,16 +205,23 @@
         return output
 
     @classmethod
     def to_config_schema(cls) -> DefinitionConfigSchema:
         """Converts the config structure represented by this class into a DefinitionConfigSchema."""
         return DefinitionConfigSchema(infer_schema_from_config_class(cls))
 
+    @classmethod
+    def to_fields_dict(cls) -> Dict[str, DagsterField]:
+        """Converts the config structure represented by this class into a dictionary of dagster.Fields.
+        This is useful when interacting with legacy code that expects a dictionary of fields but you
+        want the source of truth to be a config class.
+        """
+        return cast(Shape, cls.to_config_schema().as_field().config_type).fields
+
 
-@experimental
 class PermissiveConfig(Config):
     # Pydantic config for this class
     # Cannot use kwargs for base class as this is not support for pydantic<1.8
     class Config:
         extra = "allow"
 
     """
@@ -277,15 +339,17 @@
             nested_resource_required_keys.update(
                 _resolve_required_resource_keys_for_resource(v, resource_mapping)
             )
 
         resources, _ = separate_resource_params(self.__dict__)
         for v in resources.values():
             nested_resource_required_keys.update(
-                _resolve_required_resource_keys_for_resource(v, resource_mapping)
+                _resolve_required_resource_keys_for_resource(
+                    coerce_to_resource(v), resource_mapping
+                )
             )
 
         out = set(cast(Set[str], nested_partial_resource_keys.values())).union(
             nested_resource_required_keys
         )
         return out
 
@@ -386,26 +450,105 @@
         )
 
 
 def attach_resource_id_to_key_mapping(
     resource_def: Any, resource_id_to_key_mapping: Dict[ResourceId, str]
 ) -> Any:
     if isinstance(resource_def, (ConfigurableResourceFactory, PartialResource)):
+        defn = resource_def.get_resource_definition()
         return (
-            IOManagerWithKeyMapping(resource_def, resource_id_to_key_mapping)
-            if isinstance(resource_def, IOManagerDefinition)
-            else ResourceWithKeyMapping(resource_def, resource_id_to_key_mapping)
+            IOManagerWithKeyMapping(defn, resource_id_to_key_mapping)
+            if isinstance(defn, IOManagerDefinition)
+            else ResourceWithKeyMapping(defn, resource_id_to_key_mapping)
         )
     return resource_def
 
 
-@experimental
+CoercibleToResource: TypeAlias = Union[
+    ResourceDefinition, "ConfigurableResourceFactory", "PartialResource"
+]
+
+
+def is_coercible_to_resource(val: Any) -> TypeGuard[CoercibleToResource]:
+    return isinstance(val, (ResourceDefinition, ConfigurableResourceFactory, PartialResource))
+
+
+def coerce_to_resource(
+    coercible_to_resource: CoercibleToResource,
+) -> ResourceDefinition:
+    if isinstance(coercible_to_resource, (ConfigurableResourceFactory, PartialResource)):
+        return coercible_to_resource.get_resource_definition()
+    return coercible_to_resource
+
+
+class ConfigurableResourceFactoryResourceDefinition(ResourceDefinition, AllowDelayedDependencies):
+    def __init__(
+        self,
+        resource_fn: ResourceFunction,
+        config_schema: Any,
+        description: Optional[str],
+        resolve_resource_keys: Callable[[Mapping[int, str]], AbstractSet[str]],
+        nested_resources: Mapping[str, CoercibleToResource],
+    ):
+        super().__init__(
+            resource_fn=resource_fn, config_schema=config_schema, description=description
+        )
+        self._resolve_resource_keys = resolve_resource_keys
+        self._nested_resources = nested_resources
+
+    @property
+    def nested_resources(
+        self,
+    ) -> Mapping[str, CoercibleToResource]:
+        return self._nested_resources
+
+    def _resolve_required_resource_keys(
+        self, resource_mapping: Mapping[int, str]
+    ) -> AbstractSet[str]:
+        return self._resolve_resource_keys(resource_mapping)
+
+
+class ConfigurableIOManagerFactoryResourceDefinition(IOManagerDefinition, AllowDelayedDependencies):
+    def __init__(
+        self,
+        resource_fn: ResourceFunction,
+        config_schema: Any,
+        description: Optional[str],
+        resolve_resource_keys: Callable[[Mapping[int, str]], AbstractSet[str]],
+        nested_resources: Mapping[str, CoercibleToResource],
+    ):
+        super().__init__(
+            resource_fn=resource_fn, config_schema=config_schema, description=description
+        )
+        self._resolve_resource_keys = resolve_resource_keys
+        self._nested_resources = nested_resources
+
+    @property
+    def nested_resources(
+        self,
+    ) -> Mapping[str, CoercibleToResource]:
+        return self._nested_resources
+
+    def _resolve_required_resource_keys(
+        self, resource_mapping: Mapping[int, str]
+    ) -> AbstractSet[str]:
+        return self._resolve_resource_keys(resource_mapping)
+
+
+class ConfigurableResourceFactoryState(NamedTuple):
+    nested_partial_resources: Mapping[str, CoercibleToResource]
+    resolved_config_dict: Dict[str, Any]
+    config_schema: DefinitionConfigSchema
+    schema: DagsterField
+    nested_resources: Dict[str, CoercibleToResource]
+    resource_context: Optional[InitResourceContext]
+
+
 class ConfigurableResourceFactory(
     Generic[TResValue],
-    ResourceDefinition,
     Config,
     TypecheckAllowPartialResourceInitParams,
     AllowDelayedDependencies,
     ABC,
     metaclass=BaseResourceMeta,
 ):
     """Base class for creating and managing the lifecycle of Dagster resources that utilize structured config.
@@ -465,43 +608,70 @@
 
         # We pull the values from the Pydantic config object, which may cast values
         # to the correct type under the hood - useful in particular for enums
         casted_data_without_resources = {
             k: v for k, v in self._as_config_dict().items() if k in data_without_resources
         }
         resolved_config_dict = config_dictionary_from_values(casted_data_without_resources, schema)
-        curried_schema = _curry_config_schema(schema, resolved_config_dict)
 
-        # We keep track of any resources we depend on which are not fully configured
-        # so that we can retrieve them at runtime
-        self._nested_partial_resources: Mapping[str, ResourceDefinition] = {
-            k: v for k, v in resource_pointers.items() if (not _is_fully_configured(v))
-        }
+        self._state__internal__ = ConfigurableResourceFactoryState(
+            # We keep track of any resources we depend on which are not fully configured
+            # so that we can retrieve them at runtime
+            nested_partial_resources={
+                k: v for k, v in resource_pointers.items() if (not _is_fully_configured(v))
+            },
+            resolved_config_dict=resolved_config_dict,
+            # These are unfortunately named very similarily
+            config_schema=_curry_config_schema(schema, resolved_config_dict),
+            schema=schema,
+            nested_resources={k: v for k, v in resource_pointers.items()},
+            resource_context=None,
+        )
 
-        ResourceDefinition.__init__(
-            self,
-            resource_fn=self.initialize_and_run,
-            config_schema=curried_schema,
+    @property
+    def _schema(self):
+        return self._state__internal__.schema
+
+    @property
+    def _config_schema(self):
+        return self._state__internal__.config_schema
+
+    @property
+    def _nested_partial_resources(self):
+        return self._state__internal__.nested_partial_resources
+
+    @property
+    def _nested_resources(self):
+        return self._state__internal__.nested_resources
+
+    @property
+    def _resolved_config_dict(self):
+        return self._state__internal__.resolved_config_dict
+
+    def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
+        return ConfigurableResourceFactoryResourceDefinition(
+            resource_fn=self._initialize_and_run,
+            config_schema=self._config_schema,
             description=self.__doc__,
+            resolve_resource_keys=self._resolve_required_resource_keys,
+            nested_resources=self.nested_resources,
         )
-        self._resolved_config_dict = resolved_config_dict
-        self._schema = schema
-
-        self._nested_resources = {k: v for k, v in resource_pointers.items()}
 
     @abstractmethod
     def create_resource(self, context: InitResourceContext) -> TResValue:
         """Returns the object that this resource hands to user code, accessible by ops or assets
         through the context or resource parameters. This works like the function decorated
         with @resource when using function-based resources.
         """
         raise NotImplementedError()
 
     @property
-    def nested_resources(self) -> Mapping[str, ResourceDefinition]:
+    def nested_resources(
+        self,
+    ) -> Mapping[str, CoercibleToResource]:
         return self._nested_resources
 
     @classmethod
     def configure_at_launch(cls: "Type[Self]", **kwargs) -> "PartialResource[Self]":
         """Returns a partially initialized copy of the resource, with remaining config fields
         set at runtime.
         """
@@ -512,15 +682,19 @@
     ) -> "ConfigurableResourceFactory[TResValue]":
         """Returns a new instance of the resource with the given values.
         Used when initializing a resource at runtime.
         """
         # Since Resource extends BaseModel and is a dataclass, we know that the
         # signature of any __init__ method will always consist of the fields
         # of this class. We can therefore safely pass in the values as kwargs.
-        return self.__class__(**{**self._as_config_dict(), **values})
+        out = self.__class__(**{**self._as_config_dict(), **values})
+        out._state__internal__ = out._state__internal__._replace(  # noqa: SLF001
+            resource_context=self._state__internal__.resource_context
+        )
+        return out
 
     def _resolve_and_update_env_vars(self) -> "ConfigurableResourceFactory[TResValue]":
         """Processes the config dictionary to resolve any EnvVar values. This is called at runtime
         when the resource is initialized, so the user is only shown the error if they attempt to
         kick off a run relying on this resource.
 
         Returns a new instance of the resource.
@@ -550,38 +724,60 @@
                         "This ConfiguredResource contains unresolved partially-specified nested"
                         " resources, and so can only be initialized using a"
                         " InitResourceContextWithKeyMapping"
                     ),
                 ),
             )
             partial_resources_to_update = {
-                attr_name: context_with_mapping.resources_by_id[id(resource_def)]
-                for attr_name, resource_def in self._nested_partial_resources.items()
+                attr_name: context_with_mapping.resources_by_id[id(resource)]
+                for attr_name, resource in self._nested_partial_resources.items()
             }
 
         # Also evaluate any resources that are not partial
         resources_to_update, _ = separate_resource_params(self.__dict__)
         resources_to_update = {
-            attr_name: _call_resource_fn_with_default(resource_def, context)
-            for attr_name, resource_def in resources_to_update.items()
+            attr_name: _call_resource_fn_with_default(coerce_to_resource(resource), context)
+            for attr_name, resource in resources_to_update.items()
             if attr_name not in partial_resources_to_update
         }
 
         to_update = {**resources_to_update, **partial_resources_to_update}
         return self._with_updated_values(to_update)
 
-    def initialize_and_run(self, context: InitResourceContext) -> TResValue:
-        with_nested_resources = self._resolve_and_update_nested_resources(context)
-        with_env_vars = with_nested_resources._resolve_and_update_env_vars()  # noqa: SLF001
+    def with_resource_context(
+        self, resource_context: InitResourceContext
+    ) -> "ConfigurableResourceFactory[TResValue]":
+        """Returns a new instance of the resource with the given resource init context bound."""
+        # This utility is used to create a copy of this resource, without adjusting
+        # any values in this case
+        copy = self._with_updated_values({})
+        copy._state__internal__ = copy._state__internal__._replace(  # noqa: SLF001
+            resource_context=resource_context
+        )
+        return copy
+
+    def _initialize_and_run(self, context: InitResourceContext) -> TResValue:
+        updated_resource = (
+            self._resolve_and_update_nested_resources(context)  # noqa: SLF001
+            .with_resource_context(context)
+            ._resolve_and_update_env_vars()
+        )
 
-        return with_env_vars._create_object_fn(context)  # noqa: SLF001
+        return updated_resource._create_object_fn(context)  # noqa: SLF001
 
     def _create_object_fn(self, context: InitResourceContext) -> TResValue:
         return self.create_resource(context)
 
+    def get_resource_context(self) -> InitResourceContext:
+        """Returns the context that this resource was initialized with."""
+        return check.not_none(
+            self._state__internal__.resource_context,
+            additional_message="Attempted to get context before resource was initialized.",
+        )
+
     @classmethod
     def from_resource_context(cls, context: InitResourceContext) -> TResValue:
         """Creates a new instance of this resource from a populated InitResourceContext.
         Useful when creating a resource from a function-based resource, for backwards
         compatibility purposes.
 
         Example usage:
@@ -592,18 +788,17 @@
                 my_str: str
 
             @resource(config_schema=MyResource.to_config_schema())
             def my_resource(context: InitResourceContext) -> MyResource:
                 return MyResource.from_resource_context(context)
 
         """
-        return cls(**context.resource_config).create_resource(context)
+        return cls(**context.resource_config or {}).create_resource(context)
 
 
-@experimental
 class ConfigurableResource(ConfigurableResourceFactory[TResValue]):
     """Base class for Dagster resources that utilize structured config.
 
     This class is a subclass of both :py:class:`ResourceDefinition` and :py:class:`Config`.
 
     Example definition:
 
@@ -639,65 +834,87 @@
 
         For ConfigurableResource, this function will return itself, passing
         the actual ConfigurableResource object to user code.
         """
         return cast(TResValue, self)
 
 
-def _is_fully_configured(resource: ResourceDefinition) -> bool:
+def _is_fully_configured(resource: CoercibleToResource) -> bool:
+    actual_resource = coerce_to_resource(resource)
     res = (
         validate_config(
-            resource.config_schema.config_type,
-            resource.config_schema.default_value if resource.config_schema.default_provided else {},
+            actual_resource.config_schema.config_type,
+            actual_resource.config_schema.default_value
+            if actual_resource.config_schema.default_provided
+            else {},
         ).success
         is True
     )
 
     return res
 
 
-class PartialResource(
-    Generic[TResValue], ResourceDefinition, AllowDelayedDependencies, MakeConfigCacheable
-):
+class PartialResourceState(NamedTuple):
+    nested_partial_resources: Dict[str, CoercibleToResource]
+    config_schema: DagsterField
+    resource_fn: Callable[[InitResourceContext], Any]
+    description: Optional[str]
+    nested_resources: Dict[str, CoercibleToResource]
+
+
+class PartialResource(Generic[TResValue], AllowDelayedDependencies, MakeConfigCacheable):
     data: Dict[str, Any]
     resource_cls: Type[ConfigurableResourceFactory[TResValue]]
 
     def __init__(
         self, resource_cls: Type[ConfigurableResourceFactory[TResValue]], data: Dict[str, Any]
     ):
-        resource_pointers, data_without_resources = separate_resource_params(data)
+        resource_pointers, _data_without_resources = separate_resource_params(data)
 
         MakeConfigCacheable.__init__(self, data=data, resource_cls=resource_cls)  # type: ignore  # extends BaseModel, takes kwargs
 
-        # We keep track of any resources we depend on which are not fully configured
-        # so that we can retrieve them at runtime
-        self._nested_partial_resources: Dict[str, ResourceDefinition] = {
-            k: v for k, v in resource_pointers.items() if (not _is_fully_configured(v))
-        }
-
-        schema = infer_schema_from_config_class(
-            resource_cls, fields_to_omit=set(resource_pointers.keys())
-        )
-
         def resource_fn(context: InitResourceContext):
             instantiated = resource_cls(**context.resource_config, **data)
-            return instantiated.initialize_and_run(context)
+            return instantiated._initialize_and_run(context)  # noqa: SLF001
 
-        ResourceDefinition.__init__(
-            self,
+        self._state__internal__ = PartialResourceState(
+            # We keep track of any resources we depend on which are not fully configured
+            # so that we can retrieve them at runtime
+            nested_partial_resources={
+                k: v for k, v in resource_pointers.items() if (not _is_fully_configured(v))
+            },
+            config_schema=infer_schema_from_config_class(
+                resource_cls, fields_to_omit=set(resource_pointers.keys())
+            ),
             resource_fn=resource_fn,
-            config_schema=schema,
             description=resource_cls.__doc__,
+            nested_resources={k: v for k, v in resource_pointers.items()},
         )
 
-        self._nested_resources = {k: v for k, v in resource_pointers.items()}
+    # to make AllowDelayedDependencies work
+    @property
+    def _nested_partial_resources(
+        self,
+    ) -> Mapping[str, CoercibleToResource]:
+        return self._state__internal__.nested_partial_resources
 
     @property
-    def nested_resources(self) -> Mapping[str, ResourceDefinition]:
-        return self._nested_resources
+    def nested_resources(
+        self,
+    ) -> Mapping[str, CoercibleToResource]:
+        return self._state__internal__.nested_resources
+
+    def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
+        return ConfigurableResourceFactoryResourceDefinition(
+            resource_fn=self._state__internal__.resource_fn,
+            config_schema=self._state__internal__.config_schema,
+            description=self._state__internal__.description,
+            resolve_resource_keys=self._resolve_required_resource_keys,
+            nested_resources=self.nested_resources,
+        )
 
 
 ResourceOrPartial: TypeAlias = Union[
     ConfigurableResourceFactory[TResValue], PartialResource[TResValue]
 ]
 ResourceOrPartialOrValue: TypeAlias = Union[
     ConfigurableResourceFactory[TResValue],
@@ -706,27 +923,25 @@
     TResValue,
 ]
 
 
 V = TypeVar("V")
 
 
-@experimental
 class ResourceDependency(Generic[V]):
     def __set_name__(self, _owner, name):
         self._name = name
 
     def __get__(self, obj: "ConfigurableResourceFactory", __owner: Any) -> V:
         return getattr(obj, self._name)
 
     def __set__(self, obj: Optional[object], value: ResourceOrPartialOrValue[V]) -> None:
         setattr(obj, self._name, value)
 
 
-@experimental
 class ConfigurableLegacyResourceAdapter(ConfigurableResource, ABC):
     """Adapter base class for wrapping a decorated, function-style resource
     with structured config.
 
     To use this class, subclass it, define config schema fields using Pydantic,
     and implement the ``wrapped_resource`` method.
 
@@ -751,43 +966,39 @@
     """
 
     @property
     @abstractmethod
     def wrapped_resource(self) -> ResourceDefinition:
         raise NotImplementedError()
 
-    @property
-    def resource_fn(self) -> ResourceFunction:
-        return self.wrapped_resource.resource_fn
+    def get_resource_definition(self) -> ConfigurableResourceFactoryResourceDefinition:
+        return ConfigurableResourceFactoryResourceDefinition(
+            resource_fn=self.wrapped_resource.resource_fn,
+            config_schema=self._config_schema,
+            description=self.__doc__,
+            resolve_resource_keys=self._resolve_required_resource_keys,
+            nested_resources=self.nested_resources,
+        )
 
     def __call__(self, *args, **kwargs):
         return self.wrapped_resource(*args, **kwargs)
 
 
-@experimental
-class ConfigurableIOManagerFactory(
-    ConfigurableResourceFactory[TIOManagerValue], IOManagerDefinition
-):
+class ConfigurableIOManagerFactory(ConfigurableResourceFactory[TIOManagerValue]):
     """Base class for Dagster IO managers that utilize structured config. This base class
     is useful for cases in which the returned IO manager is not the same as the class itself
     (e.g. when it is a wrapper around the actual IO manager implementation).
 
     This class is a subclass of both :py:class:`IOManagerDefinition` and :py:class:`Config`.
     Implementers should provide an implementation of the :py:meth:`resource_function` method,
     which should return an instance of :py:class:`IOManager`.
     """
 
     def __init__(self, **data: Any):
         ConfigurableResourceFactory.__init__(self, **data)
-        IOManagerDefinition.__init__(
-            self,
-            resource_fn=self.initialize_and_run,
-            config_schema=self._config_schema,
-            description=self.__doc__,
-        )
 
     @abstractmethod
     def create_io_manager(self, context) -> TIOManagerValue:
         """Implement as one would implement a @io_manager decorator function."""
         raise NotImplementedError()
 
     def _create_object_fn(self, context: InitResourceContext) -> TIOManagerValue:
@@ -801,29 +1012,40 @@
     @classmethod
     def configure_at_launch(cls: "Type[Self]", **kwargs) -> "PartialIOManager[Self]":
         """Returns a partially initialized copy of the IO manager, with remaining config fields
         set at runtime.
         """
         return PartialIOManager(cls, data=kwargs)
 
+    def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
+        return ConfigurableIOManagerFactoryResourceDefinition(
+            resource_fn=self._initialize_and_run,
+            config_schema=self._config_schema,
+            description=self.__doc__,
+            resolve_resource_keys=self._resolve_required_resource_keys,
+            nested_resources=self.nested_resources,
+        )
+
 
-class PartialIOManager(Generic[TResValue], PartialResource[TResValue], IOManagerDefinition):
+class PartialIOManager(Generic[TResValue], PartialResource[TResValue]):
     def __init__(
         self, resource_cls: Type[ConfigurableResourceFactory[TResValue]], data: Dict[str, Any]
     ):
         PartialResource.__init__(self, resource_cls, data)
-        IOManagerDefinition.__init__(
-            self,
-            resource_fn=self._resource_fn,
-            config_schema=self._config_schema,
-            description=resource_cls.__doc__,
+
+    def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
+        return ConfigurableIOManagerFactoryResourceDefinition(
+            resource_fn=self._state__internal__.resource_fn,
+            config_schema=self._state__internal__.config_schema,
+            description=self._state__internal__.description,
+            resolve_resource_keys=self._resolve_required_resource_keys,
+            nested_resources=self._state__internal__.nested_resources,
         )
 
 
-@experimental
 class ConfigurableIOManager(ConfigurableIOManagerFactory, IOManager):
     """Base class for Dagster IO managers that utilize structured config.
 
     This class is a subclass of both :py:class:`IOManagerDefinition`, :py:class:`Config`,
     and :py:class:`IOManager`. Implementers must provide an implementation of the
     :py:meth:`handle_output` and :py:meth:`load_input` methods.
     """
@@ -927,22 +1149,23 @@
             config_type = _convert_pydantic_field(inner_field, model_cls=model_cls).config_type
         else:
             config_type = _config_type_for_pydantic_field(pydantic_field)
 
         wrapped_config_type = _wrap_config_type(
             shape_type=pydantic_field.shape, config_type=config_type, key_type=key_type
         )
+
         return Field(
             config=Noneable(wrapped_config_type)
             if pydantic_field.allow_none
             else wrapped_config_type,
             description=pydantic_field.field_info.description,
             is_required=_is_pydantic_field_required(pydantic_field),
             default_value=pydantic_field.default
-            if pydantic_field.default
+            if pydantic_field.default is not None
             else FIELD_NO_DEFAULT_PROVIDED,
         )
 
 
 def _config_type_for_pydantic_field(pydantic_field: ModelField) -> ConfigType:
     """Generates a Dagster ConfigType from a Pydantic field.
 
@@ -999,15 +1222,14 @@
     raise Exception(
         "pydantic.field.required is their UndefinedType sentinel value which we "
         "do not fully understand the semantics of right now. For the time being going "
         "to throw an error to figure see when we actually encounter this state."
     )
 
 
-@experimental
 class ConfigurableLegacyIOManagerAdapter(ConfigurableIOManagerFactory):
     """Adapter base class for wrapping a decorated, function-style I/O manager
     with structured config.
 
     To use this class, subclass it, define config schema fields using Pydantic,
     and implement the ``wrapped_io_manager`` method.
 
@@ -1038,17 +1260,22 @@
         raise NotImplementedError()
 
     def create_io_manager(self, context) -> IOManager:
         raise NotImplementedError(
             "Because we override resource_fn in the adapter, this is never called."
         )
 
-    @property
-    def resource_fn(self) -> ResourceFunction:
-        return self.wrapped_io_manager.resource_fn
+    def get_resource_definition(self) -> ConfigurableIOManagerFactoryResourceDefinition:
+        return ConfigurableIOManagerFactoryResourceDefinition(
+            resource_fn=self.wrapped_io_manager.resource_fn,
+            config_schema=self._config_schema,
+            description=self.__doc__,
+            resolve_resource_keys=self._resolve_required_resource_keys,
+            nested_resources=self.nested_resources,
+        )
 
 
 def _convert_pydantic_descriminated_union_field(pydantic_field: ModelField) -> Field:
     """Builds a Selector config field from a Pydantic field which is a descriminated union.
 
     For example:
 
@@ -1130,15 +1357,15 @@
     fields_to_omit: Optional[Set[str]] = None,
 ) -> Field:
     """Parses a structured config class and returns a corresponding Dagster config Field."""
     fields_to_omit = fields_to_omit or set()
 
     check.param_invariant(
         safe_is_subclass(model_cls, Config),
-        "Config type annotation must inherit from dagster._config.structured_config.Config",
+        "Config type annotation must inherit from dagster.Config",
     )
 
     fields = {}
     for pydantic_field in model_cls.__fields__.values():
         if pydantic_field.name not in fields_to_omit:
             if isinstance(pydantic_field.default, Field):
                 raise DagsterInvalidDefinitionError(
@@ -1163,25 +1390,25 @@
     shape_cls = Permissive if model_cls.__config__.extra == Extra.allow else Shape
 
     docstring = model_cls.__doc__.strip() if model_cls.__doc__ else None
     return Field(config=shape_cls(fields), description=description or docstring)
 
 
 class SeparatedResourceParams(NamedTuple):
-    resources: Dict[str, ResourceDefinition]
+    resources: Dict[str, CoercibleToResource]
     non_resources: Dict[str, Any]
 
 
 def separate_resource_params(data: Dict[str, Any]) -> SeparatedResourceParams:
     """Separates out the key/value inputs of fields in a structured config Resource class which
     are themselves Resources and those which are not.
     """
     return SeparatedResourceParams(
-        resources={k: v for k, v in data.items() if isinstance(v, ResourceDefinition)},
-        non_resources={k: v for k, v in data.items() if not isinstance(v, ResourceDefinition)},
+        resources={k: v for k, v in data.items() if is_coercible_to_resource(v)},
+        non_resources={k: v for k, v in data.items() if not is_coercible_to_resource(v)},
     )
 
 
 def _call_resource_fn_with_default(obj: ResourceDefinition, context: InitResourceContext) -> Any:
     if isinstance(obj.config_schema, ConfiguredDefinitionConfigSchema):
         value = cast(Dict[str, Any], obj.config_schema.resolve_config({}).value)
         context = context.replace_config(value["config"])
@@ -1203,25 +1430,25 @@
 def validate_resource_annotated_function(fn) -> None:
     """Validates any parameters on the decorated function that are annotated with
     :py:class:`dagster.ResourceDefinition`, raising a :py:class:`dagster.DagsterInvalidDefinitionError`
     if any are not also instances of :py:class:`dagster.ConfigurableResource` (these resources should
     instead be wrapped in the :py:func:`dagster.Resource` Annotation).
     """
     from dagster import DagsterInvalidDefinitionError
-    from dagster._config.structured_config import (
+    from dagster._config.pythonic_config import (
         ConfigurableResource,
         ConfigurableResourceFactory,
         TResValue,
     )
-    from dagster._config.structured_config.utils import safe_is_subclass
+    from dagster._config.pythonic_config.utils import safe_is_subclass
 
     malformed_params = [
         param
         for param in get_function_params(fn)
-        if safe_is_subclass(param.annotation, ResourceDefinition)
+        if safe_is_subclass(param.annotation, (ResourceDefinition, ConfigurableResourceFactory))
         and not safe_is_subclass(param.annotation, ConfigurableResource)
     ]
     if len(malformed_params) > 0:
         malformed_param = malformed_params[0]
         output_type = None
         if safe_is_subclass(malformed_param.annotation, ConfigurableResourceFactory):
             orig_bases = getattr(malformed_param.annotation, "__orig_bases__", None)
```

### Comparing `dagster-1.2.7/dagster/_config/structured_config/typing_utils.py` & `dagster-1.3.0/dagster/_config/pythonic_config/typing_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pydantic
 from pydantic import Field
 from typing_extensions import dataclass_transform, get_origin
 
 from .utils import safe_is_subclass
 
 if TYPE_CHECKING:
-    from dagster._config.structured_config import PartialResource
+    from dagster._config.pythonic_config import PartialResource
 
 
 # Since a metaclass is invoked by Resource before Resource or PartialResource is defined, we need to
 # define a temporary class to use as a placeholder for use in the initial metaclass invocation.
 #
 # These initial invocations will use the placeholder values, which is fine, since there's no
 # attributes on the Resource class which would be affected. The only time the metaclass will
```

### Comparing `dagster-1.2.7/dagster/_config/structured_config/utils.py` & `dagster-1.3.0/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/traversal_context.py` & `dagster-1.3.0/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/type_printer.py` & `dagster-1.3.0/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_config/validate.py` & `dagster-1.3.0/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/assets.py` & `dagster-1.3.0/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/code_pointer.py` & `dagster-1.3.0/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/container_context/config.py` & `dagster-1.3.0/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/debug.py` & `dagster-1.3.0/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/decorator_utils.py` & `dagster-1.3.0/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/__init__.py` & `dagster-1.3.0/dagster/_core/definitions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,19 @@
     resource as resource,
 )
 from .run_config_schema import (
     RunConfigSchema as RunConfigSchema,
     create_run_config_schema as create_run_config_schema,
 )
 from .run_request import (
+    AddDynamicPartitionsRequest as AddDynamicPartitionsRequest,
+    DeleteDynamicPartitionsRequest as DeleteDynamicPartitionsRequest,
     InstigatorType as InstigatorType,
     RunRequest as RunRequest,
+    SensorResult as SensorResult,
     SkipReason as SkipReason,
 )
 from .schedule_definition import (
     DefaultScheduleStatus as DefaultScheduleStatus,
     ScheduleDefinition as ScheduleDefinition,
     ScheduleEvaluationContext as ScheduleEvaluationContext,
 )
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.0/dagster/_core/definitions/asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
                 "Required neighbor information not set when creating this AssetGraph"
             )
         if asset_key in self._required_multi_asset_sets_by_key:
             return self._required_multi_asset_sets_by_key[asset_key]
         return set()
 
     def get_code_version(self, asset_key: AssetKey) -> Optional[str]:
-        return self._code_versions_by_key[asset_key]
+        return self._code_versions_by_key.get(asset_key)
 
     @cached_method
     def toposort_asset_keys(self) -> Sequence[AbstractSet[AssetKey]]:
         return [
             {key for key in level} for level in toposort.toposort(self._asset_dep_graph["upstream"])
         ]
 
@@ -525,14 +525,19 @@
                     ):
                         if child not in all_nodes:
                             queue.enqueue(child)
                             all_nodes.add(child)
 
         return result
 
+    def split_asset_keys_by_repository(
+        self, asset_keys: AbstractSet[AssetKey]
+    ) -> Sequence[AbstractSet[AssetKey]]:
+        return [asset_keys]
+
     def __hash__(self) -> int:
         return id(self)
 
     def __eq__(self, other: object) -> bool:
         return self is other
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.0/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_group.py` & `dagster-1.3.0/dagster/_core/definitions/asset_group.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_in.py` & `dagster-1.3.0/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.0/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_out.py` & `dagster-1.3.0/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.0/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.partition_mapping import IdentityPartitionMapping
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
 )
+from dagster._utils.backcompat import deprecation_warning
 from dagster._utils.schedules import cron_string_iterator
 
 from .asset_selection import AssetGraph, AssetSelection
 from .decorators.sensor_decorator import sensor
 from .partition import PartitionsDefinition, PartitionsSubset
 from .run_request import RunRequest
 from .sensor_definition import DefaultSensorStatus, SensorDefinition
@@ -49,15 +50,15 @@
     asset_graph: AssetGraph, asset_key: AssetKey
 ) -> Optional[AutoMaterializePolicy]:
     """For backcompat with pre-auto materialize policy graphs, assume a default scope of 1 day."""
     auto_materialize_policy = asset_graph.get_auto_materialize_policy(asset_key)
     if auto_materialize_policy is None:
         return AutoMaterializePolicy(
             on_missing=True,
-            on_upstream_data_newer=not bool(
+            on_new_parent_data=not bool(
                 asset_graph.get_downstream_freshness_policies(asset_key=asset_key)
             ),
             for_freshness=True,
             time_window_partition_scope_minutes=24 * 60,
         )
     return auto_materialize_policy
 
@@ -255,17 +256,24 @@
             if key not in asset_graph.non_source_asset_keys:
                 continue
 
             partitions_def = asset_graph.get_partitions_def(key)
             if partitions_def is None:
                 continue
 
-            materialized_or_requested_root_partitions_by_asset_key[
-                key
-            ] = partitions_def.deserialize_subset(serialized_subset)
+            try:
+                # in the case that the partitions def has changed, we may not be able to deserialize
+                # the corresponding subset. in this case, we just use an empty subset
+                materialized_or_requested_root_partitions_by_asset_key[
+                    key
+                ] = partitions_def.deserialize_subset(serialized_subset)
+            except:
+                materialized_or_requested_root_partitions_by_asset_key[
+                    key
+                ] = partitions_def.empty_subset()
         return cls(
             latest_storage_id=latest_storage_id,
             materialized_or_requested_root_asset_keys={
                 AssetKey.from_user_string(key_str)
                 for key_str in serialized_materialized_or_requested_root_asset_keys
             },
             materialized_or_requested_root_partitions_by_asset_key=materialized_or_requested_root_partitions_by_asset_key,
@@ -542,54 +550,67 @@
 
     backfill_target_asset_graph_subset = get_active_backfill_target_asset_graph_subset(
         asset_graph=asset_graph,
         instance=instance_queryer.instance,
     )
 
     def parents_will_be_reconciled(
+        asset_graph: AssetGraph,
         candidate: AssetKeyPartitionKey,
         to_reconcile: AbstractSet[AssetKeyPartitionKey],
     ) -> bool:
-        return all(
-            (
-                (
-                    parent in to_reconcile
-                    # if they don't have the same partitioning, then we can't launch a run that
-                    # targets both, so we need to wait until the parent is reconciled before
-                    # launching a run for the child
-                    and asset_graph.have_same_partitioning(parent.asset_key, candidate.asset_key)
-                    and parent.partition_key == candidate.partition_key
-                )
-                or (instance_queryer.is_reconciled(asset_partition=parent, asset_graph=asset_graph))
-            )
-            for parent in asset_graph.get_parents_partitions(
-                instance_queryer,
-                candidate.asset_key,
-                candidate.partition_key,
-            )
-        )
+        from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
+
+        for parent in asset_graph.get_parents_partitions(
+            instance_queryer,
+            candidate.asset_key,
+            candidate.partition_key,
+        ):
+            if instance_queryer.is_reconciled(asset_partition=parent, asset_graph=asset_graph):
+                continue
+
+            if not (
+                parent in to_reconcile
+                # if they don't have the same partitioning, then we can't launch a run that
+                # targets both, so we need to wait until the parent is reconciled before
+                # launching a run for the child
+                and asset_graph.have_same_partitioning(parent.asset_key, candidate.asset_key)
+                and parent.partition_key == candidate.partition_key
+            ):
+                return False
+
+            if isinstance(asset_graph, ExternalAssetGraph):
+                # if the parent is in a different repository, we can't launch a run that targets both,
+                # so we need to wait
+                if asset_graph.get_repository_handle(
+                    candidate.asset_key
+                ) is not asset_graph.get_repository_handle(parent.asset_key):
+                    return False
+
+        return True
 
     def should_reconcile_candidate(candidate: AssetKeyPartitionKey) -> bool:
         auto_materialize_policy = get_implicit_auto_materialize_policy(
             asset_graph=asset_graph, asset_key=candidate.asset_key
         )
         if auto_materialize_policy is None:
             return False
 
         return (
             auto_materialize_policy.on_missing
             and not instance_queryer.materialization_exists(asset_partition=candidate)
         ) or (
-            auto_materialize_policy.on_upstream_data_newer
+            auto_materialize_policy.on_new_parent_data
             and not instance_queryer.is_reconciled(
                 asset_partition=candidate, asset_graph=asset_graph
             )
         )
 
     def should_reconcile(
+        asset_graph: AssetGraph,
         candidates_unit: Iterable[AssetKeyPartitionKey],
         to_reconcile: AbstractSet[AssetKeyPartitionKey],
     ) -> bool:
         if any(
             # do not reconcile assets if they are not reconcilable
             not can_reconcile_candidate(candidate)
             # do not reconcile assets if an active backfill will update them
@@ -597,20 +618,23 @@
             # do not reconcile assets if they are not in the target selection
             or candidate.asset_key not in target_asset_keys
             for candidate in candidates_unit
         ):
             return False
 
         return all(
-            parents_will_be_reconciled(candidate, to_reconcile) for candidate in candidates_unit
+            parents_will_be_reconciled(asset_graph, candidate, to_reconcile)
+            for candidate in candidates_unit
         ) and any(should_reconcile_candidate(candidate) for candidate in candidates_unit)
 
     to_reconcile = asset_graph.bfs_filter_asset_partitions(
         instance_queryer,
-        should_reconcile,
+        lambda candidates_unit, to_reconcile: should_reconcile(
+            asset_graph, candidates_unit, to_reconcile
+        ),
         set(itertools.chain(never_materialized_or_requested_roots, stale_candidates)),
     )
 
     return (
         to_reconcile,
         newly_materialized_root_asset_keys,
         newly_materialized_root_partitions_by_asset_key,
@@ -688,35 +712,57 @@
 ) -> AbstractSet[AssetKeyPartitionKey]:
     """Returns a set of AssetKeyPartitionKeys to materialize in order to abide by the given
     FreshnessPolicies, as well as a set of AssetKeyPartitionKeys which will be materialized at
     some point within the plan window.
 
     Attempts to minimize the total number of asset executions.
     """
+    from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
+
     # now we have a full set of constraints, we can find solutions for them as we move down
     to_materialize: Set[AssetKeyPartitionKey] = set()
+    waiting_to_materialize: Set[AssetKey] = set()
     expected_data_time_by_key: Dict[AssetKey, Optional[datetime.datetime]] = {}
 
     for level in asset_graph.toposort_asset_keys():
         for key in level:
             if (
                 key not in target_asset_keys_and_parents
-                or key not in asset_graph.all_asset_keys
+                or key not in asset_graph.non_source_asset_keys
                 or not asset_graph.get_downstream_freshness_policies(asset_key=key)
             ):
                 continue
 
+            parents = asset_graph.get_parents(key)
+
+            if any(p in waiting_to_materialize for p in parents):
+                # we can't materialize this asset yet, because we're waiting on a parent
+                waiting_to_materialize.add(key)
+                continue
+
+            # if we're going to materialize a parent of this asset that's in a different repository,
+            # then we need to wait
+            if isinstance(asset_graph, ExternalAssetGraph):
+                repo = asset_graph.get_repository_handle(key)
+                if any(
+                    AssetKeyPartitionKey(p, None) in to_materialize
+                    and asset_graph.get_repository_handle(p) is not repo
+                    for p in parents
+                ):
+                    waiting_to_materialize.add(key)
+                    continue
+
             # figure out the current contents of this asset with respect to its constraints
             current_data_time = data_time_resolver.get_current_data_time(key, current_time)
 
             # figure out the expected data time of this asset if it were to be executed on this tick
             expected_data_time = min(
                 (
                     cast(datetime.datetime, expected_data_time_by_key[k])
-                    for k in asset_graph.get_parents(key)
+                    for k in parents
                     if k in expected_data_time_by_key and expected_data_time_by_key[k] is not None
                 ),
                 default=current_time,
             )
 
             if key in target_asset_keys:
                 # calculate the data times you would expect after all currently-executing runs
@@ -778,25 +824,14 @@
 ):
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
     current_time = pendulum.now("UTC")
 
     instance_queryer = CachingInstanceQueryer(instance=instance)
 
-    # if there is a auto materialize policy set in the selection, use that
-    if any(
-        asset_graph.get_auto_materialize_policy(target_key) is not None
-        for target_key in target_asset_keys
-    ):
-        target_asset_keys = {
-            target_key
-            for target_key in target_asset_keys
-            if asset_graph.get_auto_materialize_policy(target_key) is not None
-        }
-
     target_parent_asset_keys = {
         parent
         for target_asset_key in target_asset_keys
         for parent in asset_graph.get_parents(target_asset_key)
     }
     target_asset_keys_and_parents = target_asset_keys | target_parent_asset_keys
 
@@ -870,25 +905,26 @@
     ), asset_keys in assets_to_reconcile_by_partitions_def_partition_key.items():
         tags = {**(run_tags or {})}
         if partition_key is not None:
             if partitions_def is None:
                 check.failed("Partition key provided for unpartitioned asset")
             tags.update({**partitions_def.get_tags_for_partition_key(partition_key)})
 
-        # Do not call run_request.with_resolved_tags_and_config as the partition key is
-        # valid and there is no config.
-        # Calling with_resolved_tags_and_config is costly in asset reconciliation as it
-        # checks for valid partition keys.
-        run_requests.append(
-            RunRequest(
-                asset_selection=list(asset_keys),
-                partition_key=partition_key,
-                tags=tags,
+        for asset_keys_in_repo in asset_graph.split_asset_keys_by_repository(asset_keys):
+            run_requests.append(
+                # Do not call run_request.with_resolved_tags_and_config as the partition key is
+                # valid and there is no config.
+                # Calling with_resolved_tags_and_config is costly in asset reconciliation as it
+                # checks for valid partition keys.
+                RunRequest(
+                    asset_selection=list(asset_keys_in_repo),
+                    partition_key=partition_key,
+                    tags=tags,
+                )
             )
-        )
 
     return run_requests
 
 
 @experimental
 def build_asset_reconciliation_sensor(
     asset_selection: AssetSelection,
@@ -995,14 +1031,17 @@
               incorporate all of the required data, so no new runs will be kicked off until the
               following day.
 
 
     """
     check_valid_name(name)
     check.opt_mapping_param(run_tags, "run_tags", key_type=str, value_type=str)
+    deprecation_warning(
+        "build_asset_reconciliation_sensor", "1.4", "Use AutoMaterializePolicys instead."
+    )
 
     @sensor(
         name=name,
         asset_selection=asset_selection,
         minimum_interval_seconds=minimum_interval_seconds,
         description=description,
         default_status=default_status,
@@ -1010,17 +1049,33 @@
     def _sensor(context):
         asset_graph = context.repository_def.asset_graph
         cursor = (
             AssetReconciliationCursor.from_serialized(context.cursor, asset_graph)
             if context.cursor
             else AssetReconciliationCursor.empty()
         )
+
+        # if there is a auto materialize policy set in the selection, filter down to that. Otherwise, use the
+        # whole selection
+        target_asset_keys = asset_selection.resolve(asset_graph)
+        for target_key in target_asset_keys:
+            check.invariant(
+                asset_graph.get_auto_materialize_policy(target_key) is None,
+                (
+                    f"build_asset_reconciliation_sensor: Asset '{target_key.to_user_string()}' has"
+                    " an AutoMaterializePolicy set. This asset will be automatically materialized"
+                    " by the AssetDaemon, and should not be passed to this sensor. It's"
+                    " recommended to remove this sensor once you have migrated to the"
+                    " AutoMaterializePolicy api."
+                ),
+            )
+
         run_requests, updated_cursor = reconcile(
             asset_graph=asset_graph,
-            target_asset_keys=asset_selection.resolve(asset_graph),
+            target_asset_keys=target_asset_keys,
             instance=context.instance,
             cursor=cursor,
             run_tags=run_tags,
         )
 
         context.update_cursor(updated_cursor.serialize())
         return run_requests
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.0/dagster/_core/definitions/asset_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
             AssetSelection.groups("marketing") & AssetSelection.keys("leads").downstream()
 
             # Select all assets in a list of assets:
             AssetSelection.assets(*my_assets_list)
 
             # Select all assets except for those in group "marketing"
             AssetSelection.all() - AssetSelection.groups("marketing")
+
+            # Select all assets which are materialized by the same op as "projections":
+            AssetSelection.keys("projections").required_multi_asset_neighbors()
     """
 
     @public
     @staticmethod
     def all() -> "AllAssetSelection":
         """Returns a selection that includes all assets."""
         return AllAssetSelection()
@@ -152,14 +155,22 @@
 
         A sink asset is an asset that has no downstream dependencies within the asset selection.
         The sink asset can have downstream dependencies outside of the asset selection.
         """
         return SinkAssetSelection(self)
 
     @public
+    def required_multi_asset_neighbors(self) -> "RequiredNeighborsAssetSelection":
+        """Given an asset selection in which some assets are output from a mutli-asset compute op
+        which cannot be subset, returns a new asset selection that contains all of the assets
+        required to execute the original asset selection.
+        """
+        return RequiredNeighborsAssetSelection(self)
+
+    @public
     def roots(self) -> "RootAssetSelection":
         """Given an asset selection, returns a new asset selection that contains all of the root
         assets within the original asset selection.
 
         A root asset is an asset that has no upstream dependencies within the asset selection.
         The root asset can have downstream dependencies outside of the asset selection.
         """
@@ -297,14 +308,26 @@
         self._child = child
 
     def resolve_inner(self, asset_graph: AssetGraph) -> AbstractSet[AssetKey]:
         selection = self._child.resolve_inner(asset_graph)
         return fetch_sinks(asset_graph.asset_dep_graph, selection)
 
 
+class RequiredNeighborsAssetSelection(AssetSelection):
+    def __init__(self, child: AssetSelection):
+        self._child = child
+
+    def resolve_inner(self, asset_graph: AssetGraph) -> AbstractSet[AssetKey]:
+        selection = self._child.resolve_inner(asset_graph)
+        output = set(selection)
+        for asset_key in selection:
+            output.update(asset_graph.get_required_multi_asset_keys(asset_key))
+        return output
+
+
 class RootAssetSelection(AssetSelection):
     def __init__(self, child: AssetSelection):
         self._child = child
 
     def resolve_inner(self, asset_graph: AssetGraph) -> AbstractSet[AssetKey]:
         selection = self._child.resolve_inner(asset_graph)
         return fetch_sources(asset_graph.asset_dep_graph, selection)
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/assets.py` & `dagster-1.3.0/dagster/_core/definitions/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,23 +96,25 @@
         keys_by_output_name: Mapping[str, AssetKey],
         node_def: NodeDefinition,
         partitions_def: Optional[PartitionsDefinition] = None,
         partition_mappings: Optional[Mapping[AssetKey, PartitionMapping]] = None,
         asset_deps: Optional[Mapping[AssetKey, AbstractSet[AssetKey]]] = None,
         selected_asset_keys: Optional[AbstractSet[AssetKey]] = None,
         can_subset: bool = False,
-        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+        resource_defs: Optional[Mapping[str, object]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
         metadata_by_key: Optional[Mapping[AssetKey, ArbitraryMetadataMapping]] = None,
         freshness_policies_by_key: Optional[Mapping[AssetKey, FreshnessPolicy]] = None,
         auto_materialize_policies_by_key: Optional[Mapping[AssetKey, AutoMaterializePolicy]] = None,
         descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
         # if adding new fields, make sure to handle them in the with_attributes
         # and from_graph methods
     ):
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
         from .graph_definition import GraphDefinition
 
         if isinstance(node_def, GraphDefinition):
             _validate_graph_def(node_def)
 
         self._node_def = node_def
         self._keys_by_input_name = check.mapping_param(
@@ -155,15 +157,17 @@
             (
                 "The set of asset keys with dependencies specified in the asset_deps argument must "
                 "equal the set of asset keys produced by this AssetsDefinition. \n"
                 f"asset_deps keys: {set(self._asset_deps.keys())} \n"
                 f"expected keys: {all_asset_keys}"
             ),
         )
-        self._resource_defs = check.opt_mapping_param(resource_defs, "resource_defs")
+        self._resource_defs = wrap_resources_for_execution(
+            check.opt_mapping_param(resource_defs, "resource_defs")
+        )
 
         group_names_by_key = (
             check.mapping_param(group_names_by_key, "group_names_by_key")
             if group_names_by_key
             else {}
         )
         self._group_names_by_key = {}
@@ -714,14 +718,17 @@
         self,
         output_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         input_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
         freshness_policy: Optional[
             Union[FreshnessPolicy, Mapping[AssetKey, FreshnessPolicy]]
         ] = None,
+        auto_materialize_policy: Optional[
+            Union[AutoMaterializePolicy, Mapping[AssetKey, AutoMaterializePolicy]]
+        ] = None,
     ) -> "AssetsDefinition":
         output_asset_key_replacements = check.opt_mapping_param(
             output_asset_key_replacements,
             "output_asset_key_replacements",
             key_type=AssetKey,
             value_type=AssetKey,
         )
@@ -775,18 +782,39 @@
                 replaced_freshness_policy = self.freshness_policies_by_key.get(key)
 
             if replaced_freshness_policy:
                 replaced_freshness_policies_by_key[
                     output_asset_key_replacements.get(key, key)
                 ] = replaced_freshness_policy
 
-        replaced_auto_materialize_policies_by_key = {
-            output_asset_key_replacements.get(key, key): policy
-            for key, policy in self._auto_materialize_policies_by_key.items()
-        }
+        if auto_materialize_policy:
+            auto_materialize_policy_conflicts = (
+                self.auto_materialize_policies_by_key.keys()
+                if isinstance(auto_materialize_policy, AutoMaterializePolicy)
+                else (auto_materialize_policy.keys() & self.auto_materialize_policies_by_key.keys())
+            )
+            if auto_materialize_policy_conflicts:
+                raise DagsterInvalidDefinitionError(
+                    "AutoMaterializePolicy already exists on assets"
+                    f" {', '.join(key.to_string() for key in auto_materialize_policy_conflicts)}"
+                )
+
+        replaced_auto_materialize_policies_by_key = {}
+        for key in self.keys:
+            if isinstance(auto_materialize_policy, AutoMaterializePolicy):
+                replaced_auto_materialize_policy = auto_materialize_policy
+            elif auto_materialize_policy:
+                replaced_auto_materialize_policy = auto_materialize_policy.get(key)
+            else:
+                replaced_auto_materialize_policy = self.auto_materialize_policies_by_key.get(key)
+
+            if replaced_auto_materialize_policy:
+                replaced_auto_materialize_policies_by_key[
+                    output_asset_key_replacements.get(key, key)
+                ] = replaced_auto_materialize_policy
 
         replaced_descriptions_by_key = {
             output_asset_key_replacements.get(key, key): description
             for key, description in self._descriptions_by_key.items()
         }
 
         return self.__class__(
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/assets_job.py` & `dagster-1.3.0/dagster/_core/definitions/assets_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from typing import (
+    TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
@@ -39,14 +40,17 @@
 from .resource_requirement import ensure_requirements_satisfied
 from .source_asset import SourceAsset
 from .utils import DEFAULT_IO_MANAGER_KEY
 
 # Prefix for auto created jobs that are used to materialize assets
 ASSET_BASE_JOB_PREFIX = "__ASSET_JOB"
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.run_config import RunConfig
+
 
 def is_base_asset_job_name(name: str) -> bool:
     return name.startswith(ASSET_BASE_JOB_PREFIX)
 
 
 def get_base_asset_jobs(
     assets: Sequence[AssetsDefinition],
@@ -56,14 +60,20 @@
 ) -> Sequence[JobDefinition]:
     assets_by_partitions_def: Dict[
         Optional[PartitionsDefinition], List[AssetsDefinition]
     ] = defaultdict(list)
     for assets_def in assets:
         assets_by_partitions_def[assets_def.partitions_def].append(assets_def)
 
+    # We need to create "empty" jobs for each partitions def that is used by an observable but no
+    # materializable asset. They are empty because we don't assign the source asset to the `assets`,
+    # but rather the `source_assets` argument of `build_assets_job`.
+    for observable in [sa for sa in source_assets if sa.is_observable]:
+        if observable.partitions_def not in assets_by_partitions_def:
+            assets_by_partitions_def[observable.partitions_def] = []
     if len(assets_by_partitions_def.keys()) == 0 or assets_by_partitions_def.keys() == {None}:
         return [
             build_assets_job(
                 name=ASSET_BASE_JOB_PREFIX,
                 assets=assets,
                 source_assets=source_assets,
                 executor_def=executor_def,
@@ -74,37 +84,41 @@
         unpartitioned_assets = assets_by_partitions_def.get(None, [])
         partitioned_assets_by_partitions_def = {
             k: v for k, v in assets_by_partitions_def.items() if k is not None
         }
         jobs = []
 
         # sort to ensure some stability in the ordering
-        for i, (_, assets_with_partitions) in enumerate(
+        for i, (partitions_def, assets_with_partitions) in enumerate(
             sorted(partitioned_assets_by_partitions_def.items(), key=lambda item: repr(item[0]))
         ):
             jobs.append(
                 build_assets_job(
                     f"{ASSET_BASE_JOB_PREFIX}_{i}",
-                    assets=assets_with_partitions + unpartitioned_assets,
+                    assets=[*assets_with_partitions, *unpartitioned_assets],
                     source_assets=[*source_assets, *assets],
                     resource_defs=resource_defs,
                     executor_def=executor_def,
+                    # Only explicitly set partitions_def for observable-only jobs since it can't be
+                    # auto-detected from the passed assets (which is an empty list).
+                    partitions_def=partitions_def if len(assets_with_partitions) == 0 else None,
                 )
             )
-
         return jobs
 
 
 def build_assets_job(
     name: str,
     assets: Sequence[AssetsDefinition],
     source_assets: Optional[Sequence[Union[SourceAsset, AssetsDefinition]]] = None,
-    resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+    resource_defs: Optional[Mapping[str, object]] = None,
     description: Optional[str] = None,
-    config: Optional[Union[ConfigMapping, Mapping[str, object], PartitionedConfig[object]]] = None,
+    config: Optional[
+        Union[ConfigMapping, Mapping[str, object], PartitionedConfig[object], "RunConfig"]
+    ] = None,
     tags: Optional[Mapping[str, str]] = None,
     executor_def: Optional[ExecutorDefinition] = None,
     partitions_def: Optional[PartitionsDefinition[object]] = None,
     _asset_selection_data: Optional[AssetSelectionData] = None,
 ) -> JobDefinition:
     """Builds a job that materializes the given assets.
 
@@ -114,15 +128,15 @@
     Args:
         name (str): The name of the job.
         assets (List[AssetsDefinition]): A list of assets or
             multi-assets - usually constructed using the :py:func:`@asset` or :py:func:`@multi_asset`
             decorator.
         source_assets (Optional[Sequence[Union[SourceAsset, AssetsDefinition]]]): A list of
             assets that are not materialized by this job, but that assets in this job depend on.
-        resource_defs (Optional[Mapping[str, ResourceDefinition]]): Resource defs to be included in
+        resource_defs (Optional[Mapping[str, object]]): Resource defs to be included in
             this job.
         description (Optional[str]): A description of the job.
 
     Examples:
         .. code-block:: python
 
             @asset
@@ -134,27 +148,30 @@
                 return my_upstream_asset + 1
 
             my_assets_job = build_assets_job("my_assets_job", assets=[asset1, asset2])
 
     Returns:
         JobDefinition: A job that materializes the given assets.
     """
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
+
     check.str_param(name, "name")
     check.iterable_param(assets, "assets", of_type=(AssetsDefinition, SourceAsset))
     source_assets = check.opt_sequence_param(
         source_assets, "source_assets", of_type=(SourceAsset, AssetsDefinition)
     )
     check.opt_str_param(description, "description")
     check.opt_inst_param(_asset_selection_data, "_asset_selection_data", AssetSelectionData)
 
     # figure out what partitions (if any) exist for this job
     partitions_def = partitions_def or build_job_partitions_from_assets(assets)
 
     resource_defs = check.opt_mapping_param(resource_defs, "resource_defs")
     resource_defs = merge_dicts({DEFAULT_IO_MANAGER_KEY: default_job_io_manager}, resource_defs)
+    wrapped_resource_defs = wrap_resources_for_execution(resource_defs)
 
     # turn any AssetsDefinitions into SourceAssets
     resolved_source_assets: List[SourceAsset] = []
     for asset in source_assets or []:
         if isinstance(asset, AssetsDefinition):
             resolved_source_assets += asset.to_source_assets()
         elif isinstance(asset, SourceAsset):
@@ -185,15 +202,15 @@
         config=None,
     )
 
     asset_layer = AssetLayer.from_graph_and_assets_node_mapping(
         graph, assets_defs_by_node_handle, resolved_source_assets, resolved_asset_deps
     )
 
-    all_resource_defs = get_all_resource_defs(assets, resolved_source_assets, resource_defs)
+    all_resource_defs = get_all_resource_defs(assets, resolved_source_assets, wrapped_resource_defs)
 
     if _asset_selection_data:
         original_job = _asset_selection_data.parent_job_def
         return graph.to_job(
             resource_defs=all_resource_defs,
             config=config,
             tags=tags,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.0/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,70 @@
 import datetime
 from typing import NamedTuple, Optional
 
-from dagster._annotations import experimental
+from dagster._annotations import experimental, public
 from dagster._serdes.serdes import whitelist_for_serdes
 
 
 @experimental
 @whitelist_for_serdes
 class AutoMaterializePolicy(NamedTuple):
     """An AutoMaterializePolicy specifies how Dagster should attempt to keep an asset up-to-date.
 
     There are two main modes of reconciliation: eager and lazy.
 
-    Regardless of this selection, there are some cases where an asset / partition will never be
-    materialized:
-       - one or more of its parents is missing
-       - the partition is a time window partition with a start time that is more than
-            time_window_partition_scope older than the latest available time window partition. By
-            default, only the most recent time window partition will be materialized.
-
-    Outside of those cases...
+    Regardless of this selection an asset / partition will never be materialized if any of its
+    parents are missing.
 
     For eager reconciliation, an asset / partition will be (re)materialized when:
-       - it is missing
-       - it or any of its children have a FreshnessPolicy that require more up-to-date data than it
-            currently has
-       - any of its parent assets / partitions have been updated more recently than it has
+
+    - it is missing
+    - it or any of its children have a FreshnessPolicy that require more up-to-date data than it
+      currently has
+    - any of its parent assets / partitions have been updated more recently than it has
 
     For lazy reconciliation, an asset / partition will be (re)materialized when:
-       - it is missing
-       - it or any of its children have a FreshnessPolicy that require more up-to-date data than it
-            currently has
+
+    - it is missing
+    - it or any of its children have a FreshnessPolicy that require more up-to-date data than it
+      currently has
 
     In essence, an asset with eager reconciliation will always incorporate the most up-to-date
     version of its parents, while an asset with lazy reconciliation will only update when necessary
     in order to stay in line with the relevant FreshnessPolicies.
+
+    **Warning:**
+
+    Constructing an AutoMaterializePolicy directly is not recommended as the API is subject to change.
+    AutoMaterializePolicy.eager() and AutoMaterializePolicy.lazy() are the recommended API.
     """
 
     on_missing: bool
-    on_upstream_data_newer: bool
+    on_new_parent_data: bool
     for_freshness: bool
     time_window_partition_scope_minutes: Optional[float]
 
     @property
     def time_window_partition_scope(self) -> Optional[datetime.timedelta]:
         if self.time_window_partition_scope_minutes is None:
             return None
         return datetime.timedelta(minutes=self.time_window_partition_scope_minutes)
 
+    @public
     @staticmethod
-    def eager(
-        time_window_partition_scope: Optional[datetime.timedelta] = datetime.timedelta.resolution,
-    ) -> "AutoMaterializePolicy":
+    def eager() -> "AutoMaterializePolicy":
         return AutoMaterializePolicy(
             on_missing=True,
-            on_upstream_data_newer=True,
+            on_new_parent_data=True,
             for_freshness=True,
-            time_window_partition_scope_minutes=time_window_partition_scope.total_seconds() / 60
-            if time_window_partition_scope is not None
-            else None,
+            time_window_partition_scope_minutes=datetime.timedelta.resolution.total_seconds() / 60,
         )
 
+    @public
     @staticmethod
-    def lazy(
-        time_window_partition_scope: Optional[datetime.timedelta] = datetime.timedelta.resolution,
-    ) -> "AutoMaterializePolicy":
+    def lazy() -> "AutoMaterializePolicy":
         return AutoMaterializePolicy(
             on_missing=True,
-            on_upstream_data_newer=False,
+            on_new_parent_data=False,
             for_freshness=True,
-            time_window_partition_scope_minutes=time_window_partition_scope.total_seconds() / 60
-            if time_window_partition_scope is not None
-            else None,
+            time_window_partition_scope_minutes=datetime.timedelta.resolution.total_seconds() / 60,
         )
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.0/dagster/_core/definitions/cacheable_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import ABC, abstractmethod
 from typing import AbstractSet, Any, List, Mapping, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._config.field_utils import compute_fields_hash
 from dagster._core.definitions.assets import AssetsDefinition
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.metadata import MetadataUserInput
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.resource_requirement import ResourceAddable
 from dagster._serdes import whitelist_for_serdes
 from dagster._utils import hash_collection
@@ -152,22 +153,28 @@
         """
         if isinstance(prefix, str):
             prefix = [prefix]
         prefix = check.is_list(prefix, of_type=str)
         return PrefixOrGroupWrappedCacheableAssetsDefinition(self, prefix_for_all_assets=prefix)
 
     def with_attributes_for_all(
-        self, group_name: Optional[str], freshness_policy: Optional[FreshnessPolicy]
+        self,
+        group_name: Optional[str],
+        freshness_policy: Optional[FreshnessPolicy],
+        auto_materialize_policy: Optional[AutoMaterializePolicy],
     ) -> "CacheableAssetsDefinition":
         """Utility method which allows setting attributes for all assets in this
         CacheableAssetsDefinition, since the keys may not be known at the time of
         construction.
         """
         return PrefixOrGroupWrappedCacheableAssetsDefinition(
-            self, group_name_for_all_assets=group_name, freshness_policy=freshness_policy
+            self,
+            group_name_for_all_assets=group_name,
+            freshness_policy=freshness_policy,
+            auto_materialize_policy=auto_materialize_policy,
         )
 
 
 class WrappedCacheableAssetsDefinition(CacheableAssetsDefinition):
     """Wraps an instance of CacheableAssetsDefinition, applying transformed_assets_def to the
     generated AssetsDefinition objects. This lets e.g. users define resources on
     the cacheable assets at repo creation time which are not actually bound until
@@ -220,21 +227,25 @@
         input_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
         group_name_for_all_assets: Optional[str] = None,
         prefix_for_all_assets: Optional[List[str]] = None,
         freshness_policy: Optional[
             Union[FreshnessPolicy, Mapping[AssetKey, FreshnessPolicy]]
         ] = None,
+        auto_materialize_policy: Optional[
+            Union[AutoMaterializePolicy, Mapping[AssetKey, AutoMaterializePolicy]]
+        ] = None,
     ):
         self._output_asset_key_replacements = output_asset_key_replacements or {}
         self._input_asset_key_replacements = input_asset_key_replacements or {}
         self._group_names_by_key = group_names_by_key or {}
         self._group_name_for_all_assets = group_name_for_all_assets
         self._prefix_for_all_assets = prefix_for_all_assets
         self._freshness_policy = freshness_policy
+        self._auto_materialize_policy = auto_materialize_policy
 
         check.invariant(
             not (group_name_for_all_assets and group_names_by_key),
             "Cannot set both group_name_for_all_assets and group_names_by_key",
         )
         check.invariant(
             not (
@@ -320,14 +331,15 @@
             else self._input_asset_key_replacements
         )
         return assets_def.with_attributes(
             output_asset_key_replacements=output_asset_key_replacements,
             input_asset_key_replacements=input_asset_key_replacements,
             group_names_by_key=group_names_by_key,
             freshness_policy=self._freshness_policy,
+            auto_materialize_policy=self._auto_materialize_policy,
         )
 
 
 class ResourceWrappedCacheableAssetsDefinition(WrappedCacheableAssetsDefinition):
     """Represents a CacheableAssetsDefinition that has been wrapped with resources."""
 
     def __init__(
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/composition.py` & `dagster-1.3.0/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/config.py` & `dagster-1.3.0/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/configurable.py` & `dagster-1.3.0/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/data_time.py` & `dagster-1.3.0/dagster/_core/definitions/data_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,11 +486,11 @@
     ) -> Optional[float]:
         freshness_policy = self._asset_graph.freshness_policies_by_key.get(asset_key)
         if freshness_policy is None:
             raise DagsterInvariantViolationError(
                 "Cannot calculate minutes late for asset without a FreshnessPolicy"
             )
 
-        return freshness_policy.minutes_late(
+        return freshness_policy.minutes_overdue(
             data_time=self.get_current_data_time(asset_key, current_time=evaluation_time),
             evaluation_time=evaluation_time,
         )
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/data_version.py` & `dagster-1.3.0/dagster/_core/definitions/data_version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 from collections import OrderedDict
 from enum import Enum
 from hashlib import sha256
 from typing import (
     TYPE_CHECKING,
     Callable,
     Dict,
@@ -69,41 +70,46 @@
 
 class DataProvenance(
     NamedTuple(
         "_DataProvenance",
         [
             ("code_version", str),
             ("input_data_versions", Mapping["AssetKey", DataVersion]),
+            ("is_user_provided", bool),
         ],
     )
 ):
     """(Experimental) Provenance information for an asset materialization.
 
     Args:
         code_version (str): The code version of the op that generated a materialization.
         input_data_versions (Mapping[AssetKey, DataVersion]): The data versions of the
             inputs used to generate a materialization.
+        is_user_provided (bool): True if the data version was provided directly by the user, false
+            if it was generated by Dagster.
     """
 
     def __new__(
         cls,
         code_version: str,
         input_data_versions: Mapping["AssetKey", DataVersion],
+        is_user_provided: bool,
     ):
         from dagster._core.definitions.events import AssetKey
 
         return super(DataProvenance, cls).__new__(
             cls,
             code_version=check.str_param(code_version, "code_version"),
             input_data_versions=check.mapping_param(
                 input_data_versions,
                 "input_data_versions",
                 key_type=AssetKey,
                 value_type=DataVersion,
             ),
+            is_user_provided=check.bool_param(is_user_provided, "is_user_provided"),
         )
 
     @staticmethod
     def from_tags(tags: Mapping[str, str]) -> Optional[DataProvenance]:
         from dagster._core.definitions.events import AssetKey
 
         code_version = tags.get(CODE_VERSION_TAG)
@@ -112,15 +118,16 @@
         input_data_versions = {
             # Everything after the 2nd slash is the asset key
             AssetKey.from_user_string(k.split("/", maxsplit=2)[-1]): DataVersion(tags[k])
             for k, v in tags.items()
             if k.startswith(INPUT_DATA_VERSION_TAG_PREFIX)
             or k.startswith(_OLD_INPUT_DATA_VERSION_TAG_PREFIX)
         }
-        return DataProvenance(code_version, input_data_versions)
+        is_user_provided = tags.get(DATA_VERSION_IS_USER_PROVIDED_TAG) == "true"
+        return DataProvenance(code_version, input_data_versions, is_user_provided)
 
     @property
     @deprecated
     def input_logical_versions(self) -> Mapping["AssetKey", DataVersion]:
         return self.input_data_versions
 
 
@@ -130,14 +137,15 @@
 
 DATA_VERSION_TAG: Final[str] = "dagster/data_version"
 _OLD_DATA_VERSION_TAG: Final[str] = "dagster/logical_version"
 CODE_VERSION_TAG: Final[str] = "dagster/code_version"
 INPUT_DATA_VERSION_TAG_PREFIX: Final[str] = "dagster/input_data_version"
 _OLD_INPUT_DATA_VERSION_TAG_PREFIX: Final[str] = "dagster/input_logical_version"
 INPUT_EVENT_POINTER_TAG_PREFIX: Final[str] = "dagster/input_event_pointer"
+DATA_VERSION_IS_USER_PROVIDED_TAG = "dagster/data_version_is_user_provided"
 
 
 def read_input_data_version_from_tags(
     tags: Mapping[str, str], input_key: "AssetKey"
 ) -> Optional[DataVersion]:
     value = tags.get(
         get_input_data_version_tag(input_key, prefix=INPUT_DATA_VERSION_TAG_PREFIX)
@@ -218,19 +226,25 @@
 
 class StaleStatus(Enum):
     MISSING = "MISSING"
     STALE = "STALE"
     FRESH = "FRESH"
 
 
+@functools.total_ordering
 class StaleCauseCategory(Enum):
     CODE = "CODE"
     DATA = "DATA"
     DEPENDENCIES = "DEPENDENCIES"
 
+    def __lt__(self, other: "StaleCauseCategory"):
+        if self.__class__ is other.__class__:
+            return self.value < other.value
+        return NotImplemented
+
 
 class StaleCause(NamedTuple):
     key: AssetKey
     category: StaleCauseCategory
     reason: str
     dependency: Optional[AssetKey] = None
     children: Optional[Sequence["StaleCause"]] = None
@@ -303,22 +317,22 @@
 
         # only used if no provenance available
         materialization = check.not_none(self._get_latest_materialization_event(key=key))
         materialization_time = materialization.timestamp
 
         if provenance:
             if code_version and code_version != provenance.code_version:
-                yield StaleCause(key, StaleCauseCategory.CODE, "updated code version")
+                yield StaleCause(key, StaleCauseCategory.CODE, "has a new code version")
 
             removed_deps = set(provenance.input_data_versions.keys()) - set(dependency_keys)
             for dep_key in removed_deps:
                 yield StaleCause(
                     key,
                     StaleCauseCategory.DEPENDENCIES,
-                    "removed dependency",
+                    f"removed dependency on {dep_key.to_user_string()}",
                     dep_key,
                 )
 
         for dep_key in sorted(dependency_keys):
             if self._get_status(key=dep_key) == StaleStatus.STALE:
                 yield StaleCause(
                     key,
@@ -328,51 +342,63 @@
                     self._get_stale_causes(key=dep_key),
                 )
             elif provenance:
                 if dep_key not in provenance.input_data_versions:
                     yield StaleCause(
                         key,
                         StaleCauseCategory.DEPENDENCIES,
-                        "new dependency",
+                        f"has a new dependency on {dep_key.to_user_string()}",
                         dep_key,
                     )
                 elif provenance.input_data_versions[dep_key] != self._get_current_data_version(
                     key=dep_key
                 ):
+                    report_data_version = self.asset_graph.get_code_version(
+                        dep_key
+                    ) is not None or self._is_current_data_version_user_provided(key=dep_key)
                     yield StaleCause(
                         key,
                         StaleCauseCategory.DATA,
-                        "updated dependency data version",
+                        "has a new dependency data version"
+                        if report_data_version
+                        else "has a new dependency materialization",
                         dep_key,
                         [
                             StaleCause(
                                 dep_key,
                                 StaleCauseCategory.DATA,
-                                "updated data version",
+                                # Assets with no defined code version will get a new data version on
+                                # every materialization, so we just report new materialization for
+                                # this case since the user likely hasn't engaged with data versions.
+                                "has a new data version"
+                                if report_data_version
+                                else "has a new materialization",
                             )
                         ],
                     )
-            # if no provenance, then use materialization timestamps instead of versions
-            # this should be removable eventually since provenance is on all newer materializations
-            else:
+            # If no provenance and dep is a materializable asset, then use materialization
+            # timestamps instead of versions this should be removable eventually since
+            # provenance is on all newer materializations. If dep is a source, then we'll never
+            # provide a stale reason here.
+            elif not self.asset_graph.is_source(dep_key):
                 dep_materialization = self._get_latest_materialization_event(key=dep_key)
                 if dep_materialization is None:
                     # The input must be new if it has no materialization
-                    yield StaleCause(key, StaleCauseCategory.DATA, "new input", dep_key)
+                    yield StaleCause(key, StaleCauseCategory.DATA, "has a new input", dep_key)
                 elif dep_materialization.timestamp > materialization_time:
                     yield StaleCause(
                         key,
                         StaleCauseCategory.DATA,
-                        "updated dependency timestamp",
+                        "has a new dependency materialization",
                         dep_key,
                         [
                             StaleCause(
                                 dep_key,
                                 StaleCauseCategory.DATA,
-                                "updated timestamp",
+                                "has a new materialization",
                             )
                         ],
                     )
 
     @cached_method
     def _get_stale_root_causes(self, key: AssetKey) -> Sequence[StaleCause]:
         causes = self._get_stale_causes(key=key)
@@ -415,14 +441,22 @@
             return data_version or DEFAULT_DATA_VERSION
 
     @cached_method
     def _get_latest_materialization_event(self, *, key: AssetKey) -> Optional[EventLogEntry]:
         return self._instance.get_latest_materialization_event(key)
 
     @cached_method
+    def _is_current_data_version_user_provided(self, *, key: AssetKey) -> bool:
+        if self.asset_graph.is_source(key):
+            return True
+        else:
+            provenance = self._get_current_data_provenance(key=key)
+            return provenance is not None and provenance.is_user_provided
+
+    @cached_method
     def _get_current_data_provenance(self, *, key: AssetKey) -> Optional[DataProvenance]:
         materialization = self._get_latest_materialization_event(key=key)
         if materialization is None:
             return None
         else:
             return extract_data_provenance_from_entry(materialization)
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     ins: Optional[Mapping[str, AssetIn]] = ...,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = ...,
     metadata: Optional[Mapping[str, Any]] = ...,
     description: Optional[str] = ...,
     config_schema: Optional[UserConfigSchema] = None,
     required_resource_keys: Optional[Set[str]] = ...,
-    resource_defs: Optional[Mapping[str, ResourceDefinition]] = ...,
+    resource_defs: Optional[Mapping[str, object]] = ...,
     io_manager_def: Optional[IOManagerDefinition] = ...,
     io_manager_key: Optional[str] = ...,
     compute_kind: Optional[str] = ...,
     dagster_type: Optional[DagsterType] = ...,
     partitions_def: Optional[PartitionsDefinition[Any]] = ...,
     op_tags: Optional[Mapping[str, Any]] = ...,
     group_name: Optional[str] = ...,
@@ -89,15 +89,15 @@
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = None,
     metadata: Optional[ArbitraryMetadataMapping] = None,
     description: Optional[str] = None,
     config_schema: Optional[UserConfigSchema] = None,
     required_resource_keys: Optional[Set[str]] = None,
-    resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+    resource_defs: Optional[Mapping[str, object]] = None,
     io_manager_def: Optional[IOManagerDefinition] = None,
     io_manager_key: Optional[str] = None,
     compute_kind: Optional[str] = None,
     dagster_type: Optional[DagsterType] = None,
     partitions_def: Optional[PartitionsDefinition[Any]] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
     group_name: Optional[str] = None,
@@ -152,48 +152,51 @@
             compose the asset.
         op_tags (Optional[Dict[str, Any]]): A dictionary of tags for the op that computes the asset.
             Frameworks may expect and require certain metadata to be attached to a op. Values that
             are not strings will be json encoded and must meet the criteria that
             `json.loads(json.dumps(value)) == value`.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If not provided,
             the name "default" is used.
-        resource_defs (Optional[Mapping[str, ResourceDefinition]]):
-            (Experimental) A mapping of resource keys to resource definitions. These resources
+        resource_defs (Optional[Mapping[str, object]]):
+            (Experimental) A mapping of resource keys to resources. These resources
             will be initialized during execution, and can be accessed from the
             context within the body of the function.
         output_required (bool): Whether the decorated function will always materialize an asset.
             Defaults to True. If False, the function can return None, which will not be materialized to
             storage and will halt execution of downstream assets.
         freshness_policy (FreshnessPolicy): A constraint telling Dagster how often this asset is intended to be updated
             with respect to its root data.
-        auto_materialize_policy (AutoMaterializePolicy): (Experimental) This currently has no effect.
+        auto_materialize_policy (AutoMaterializePolicy): (Experimental) Configure Dagster to automatically materialize
+            this asset according to its FreshnessPolicy and when upstream dependencies change.
         retry_policy (Optional[RetryPolicy]): The retry policy for the op that computes the asset.
         code_version (Optional[str]): (Experimental) Version of the code that generates this asset. In
             general, versions should be set only for code that deterministically produces the same
             output when given the same inputs.
 
     Examples:
         .. code-block:: python
 
             @asset
             def my_asset(my_upstream_asset: int) -> int:
                 return my_upstream_asset + 1
     """
 
     def create_asset():
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
         return _Asset(
             name=cast(Optional[str], name),  # (mypy bug that it can't infer name is Optional[str])
             key_prefix=key_prefix,
             ins=ins,
             non_argument_deps=_make_asset_keys(non_argument_deps),
             metadata=metadata,
             description=description,
             config_schema=config_schema,
             required_resource_keys=required_resource_keys,
-            resource_defs=resource_defs,
+            resource_defs=wrap_resources_for_execution(resource_defs),
             io_manager=io_manager_def or io_manager_key,
             compute_kind=check.opt_str_param(compute_kind, "compute_kind"),
             dagster_type=dagster_type,
             partitions_def=partitions_def,
             op_tags=op_tags,
             group_name=group_name,
             output_required=output_required,
@@ -275,15 +278,15 @@
         self.output_required = output_required
         self.freshness_policy = freshness_policy
         self.retry_policy = retry_policy
         self.auto_materialize_policy = auto_materialize_policy
         self.code_version = code_version
 
     def __call__(self, fn: Callable) -> AssetsDefinition:
-        from dagster._config.structured_config import validate_resource_annotated_function
+        from dagster._config.pythonic_config import validate_resource_annotated_function
 
         validate_resource_annotated_function(fn)
         asset_name = self.name or fn.__name__
 
         asset_ins = build_asset_ins(fn, self.ins or {}, self.non_argument_deps)
 
         out_asset_key = AssetKey(list(filter(None, [*(self.key_prefix or []), asset_name])))
@@ -379,15 +382,15 @@
     config_schema: Optional[UserConfigSchema] = None,
     required_resource_keys: Optional[Set[str]] = None,
     compute_kind: Optional[str] = None,
     internal_asset_deps: Optional[Mapping[str, Set[AssetKey]]] = None,
     partitions_def: Optional[PartitionsDefinition[object]] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
     can_subset: bool = False,
-    resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+    resource_defs: Optional[Mapping[str, object]] = None,
     group_name: Optional[str] = None,
     retry_policy: Optional[RetryPolicy] = None,
     code_version: Optional[str] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Create a combined definition of multiple assets that are computed using the same op and same
     upstream assets.
 
@@ -416,36 +419,39 @@
             compose the assets.
         op_tags (Optional[Dict[str, Any]]): A dictionary of tags for the op that computes the asset.
             Frameworks may expect and require certain metadata to be attached to a op. Values that
             are not strings will be json encoded and must meet the criteria that
             `json.loads(json.dumps(value)) == value`.
         can_subset (bool): If this asset's computation can emit a subset of the asset
             keys based on the context.selected_assets argument. Defaults to False.
-        resource_defs (Optional[Mapping[str, ResourceDefinition]]):
-            (Experimental) A mapping of resource keys to resource definitions. These resources
+        resource_defs (Optional[Mapping[str, object]]):
+            (Experimental) A mapping of resource keys to resources. These resources
             will be initialized during execution, and can be accessed from the
             context within the body of the function.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. This
             group name will be applied to all assets produced by this multi_asset.
         retry_policy (Optional[RetryPolicy]): The retry policy for the op that computes the asset.
         code_version (Optional[str]): (Experimental) Version of the code encapsulated by the multi-asset. If set,
             this is used as a default code version for all defined assets.
     """
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
+
     if resource_defs is not None:
         experimental_arg_warning("resource_defs", "multi_asset")
 
     asset_deps = check.opt_mapping_param(
         internal_asset_deps, "internal_asset_deps", key_type=str, value_type=set
     )
     required_resource_keys = check.opt_set_param(
         required_resource_keys, "required_resource_keys", of_type=str
     )
-    resource_defs = check.opt_mapping_param(
-        resource_defs, "resource_defs", key_type=str, value_type=ResourceDefinition
+    resource_defs = wrap_resources_for_execution(
+        check.opt_mapping_param(resource_defs, "resource_defs", key_type=str)
     )
+
     _config_schema = check.opt_mapping_param(
         config_schema,
         "config_schema",
         additional_message="Only dicts are supported for asset config_schema.",
     )
 
     bare_required_resource_keys = set(required_resource_keys)
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.receive_processed_config_values = check.opt_bool_param(
             receive_processed_config_values, "receive_processed_config_values"
         )
 
     def __call__(self, fn: Callable[..., Any]) -> ConfigMapping:
         check.callable_param(fn, "fn")
 
-        from dagster._config.structured_config import (
+        from dagster._config.pythonic_config import (
             Config,
             infer_schema_from_config_annotation,
             safe_is_subclass,
         )
         from dagster._core.definitions.run_config import RunConfig
 
         config_fn_params = get_function_params(fn)
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,41 +13,44 @@
 from ..policy import RetryPolicy
 from ..resource_definition import ResourceDefinition
 from ..version_strategy import VersionStrategy
 
 if TYPE_CHECKING:
     from ..executor_definition import ExecutorDefinition
     from ..partition import PartitionedConfig, PartitionsDefinition
+    from ..run_config import RunConfig
 
 
 class _Job:
     def __init__(
         self,
         name: Optional[str] = None,
         description: Optional[str] = None,
         tags: Optional[Mapping[str, Any]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         config: Optional[
-            Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig[object]"]
+            Union[ConfigMapping, Mapping[str, Any], "RunConfig", "PartitionedConfig[object]"]
         ] = None,
         logger_defs: Optional[Mapping[str, LoggerDefinition]] = None,
         executor_def: Optional["ExecutorDefinition"] = None,
         hooks: Optional[AbstractSet[HookDefinition]] = None,
         op_retry_policy: Optional[RetryPolicy] = None,
         version_strategy: Optional[VersionStrategy] = None,
         partitions_def: Optional["PartitionsDefinition[object]"] = None,
         input_values: Optional[Mapping[str, object]] = None,
     ):
+        from dagster._core.definitions.run_config import convert_config_input
+
         self.name = name
         self.description = description
         self.tags = tags
         self.metadata = metadata
         self.resource_defs = resource_defs
-        self.config = config
+        self.config = convert_config_input(config)
         self.logger_defs = logger_defs
         self.executor_def = executor_def
         self.hooks = hooks
         self.op_retry_policy = op_retry_policy
         self.version_strategy = version_strategy
         self.partitions_def = partitions_def
         self.input_values = input_values
@@ -115,16 +118,16 @@
 
 
 @overload
 def job(
     *,
     name: Optional[str] = ...,
     description: Optional[str] = ...,
-    resource_defs: Optional[Mapping[str, ResourceDefinition]] = ...,
-    config: Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig[object]"] = ...,
+    resource_defs: Optional[Mapping[str, object]] = ...,
+    config: Union[ConfigMapping, Mapping[str, Any], "RunConfig", "PartitionedConfig[object]"] = ...,
     tags: Optional[Mapping[str, Any]] = ...,
     metadata: Optional[Mapping[str, RawMetadataValue]] = ...,
     logger_defs: Optional[Mapping[str, LoggerDefinition]] = ...,
     executor_def: Optional["ExecutorDefinition"] = ...,
     hooks: Optional[AbstractSet[HookDefinition]] = ...,
     op_retry_policy: Optional[RetryPolicy] = ...,
     version_strategy: Optional[VersionStrategy] = ...,
@@ -135,16 +138,18 @@
 
 
 def job(
     compose_fn: Optional[Callable[..., Any]] = None,
     *,
     name: Optional[str] = None,
     description: Optional[str] = None,
-    resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
-    config: Optional[Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig[object]"]] = None,
+    resource_defs: Optional[Mapping[str, object]] = None,
+    config: Optional[
+        Union[ConfigMapping, Mapping[str, Any], "RunConfig", "PartitionedConfig[object]"]
+    ] = None,
     tags: Optional[Mapping[str, Any]] = None,
     metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     logger_defs: Optional[Mapping[str, LoggerDefinition]] = None,
     executor_def: Optional["ExecutorDefinition"] = None,
     hooks: Optional[AbstractSet[HookDefinition]] = None,
     op_retry_policy: Optional[RetryPolicy] = None,
     version_strategy: Optional[VersionStrategy] = None,
@@ -158,28 +163,31 @@
 
     Args:
         compose_fn (Callable[..., Any]:
             The decorated function. The body should contain op or graph invocations. Unlike op
             functions, does not accept a context argument.
         name (Optional[str]):
             The name for the Job. Defaults to the name of the this graph.
-        resource_defs (Optional[Mapping[str, ResourceDefinition]]):
+        resource_defs (Optional[Mapping[str, object]]):
             Resources that are required by this graph for execution.
             If not defined, `io_manager` will default to filesystem.
         config:
             Describes how the job is parameterized at runtime.
 
             If no value is provided, then the schema for the job's run config is a standard
             format based on its ops and resources.
 
             If a dictionary is provided, then it must conform to the standard config schema, and
             it will be used as the job's run config for the job whenever the job is executed.
             The values provided will be viewable and editable in the Dagit playground, so be
             careful with secrets.
 
+            If a :py:class:`RunConfig` object is provided, then it will be used directly as the run config
+            for the job whenever the job is executed, similar to providing a dictionary.
+
             If a :py:class:`ConfigMapping` object is provided, then the schema for the job's run config is
             determined by the config mapping, and the ConfigMapping, which should return
             configuration in the standard format to configure the job.
 
             If a :py:class:`PartitionedConfig` object is provided, then it defines a discrete set of config
             values that can parameterize the pipeline, as well as a function for mapping those
             values to the base config. The values provided will be viewable and editable in the
@@ -224,18 +232,20 @@
             def job1():
                 add_one(return_one())
     """
     if compose_fn is not None:
         check.invariant(description is None)
         return _Job()(compose_fn)
 
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
+
     return _Job(
         name=name,
         description=description,
-        resource_defs=resource_defs,
+        resource_defs=wrap_resources_for_execution(resource_defs),
         config=config,
         tags=tags,
         metadata=metadata,
         logger_defs=logger_defs,
         executor_def=executor_def,
         hooks=hooks,
         op_retry_policy=op_retry_policy,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         # config will be checked within SolidDefinition
         self.config_schema = config_schema
 
         self.ins = check.opt_nullable_mapping_param(ins, "ins", key_type=str, value_type=In)
         self.out = out
 
     def __call__(self, fn: Callable[..., Any]) -> "OpDefinition":
-        from dagster._config.structured_config import validate_resource_annotated_function
+        from dagster._config.pythonic_config import validate_resource_annotated_function
 
         from ..op_definition import OpDefinition
 
         validate_resource_annotated_function(fn)
 
         if not self.name:
             self.name = fn.__name__
@@ -92,15 +92,15 @@
 
         if compute_fn.has_config_arg():
             check.param_invariant(
                 self.config_schema is None or self.config_schema == {},
                 "If the @op has a config arg, you cannot specify a config schema",
             )
 
-            from dagster._config.structured_config import infer_schema_from_config_annotation
+            from dagster._config.pythonic_config import infer_schema_from_config_annotation
 
             # Parse schema from the type annotation of the config arg
             config_arg = compute_fn.get_config_arg()
             config_arg_type = config_arg.annotation
             config_arg_default = config_arg.default
             self.config_schema = infer_schema_from_config_annotation(
                 config_arg_type, config_arg_default
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             that should execute when this schedule runs.
         default_status (DefaultScheduleStatus): Whether the schedule starts as running or not. The default
             status can be overridden from Dagit or via the GraphQL API.
         required_resource_keys (Optional[Set[str]]): The set of resource keys required by the schedule.
     """
 
     def inner(fn: RawScheduleEvaluationFunction) -> ScheduleDefinition:
-        from dagster._config.structured_config import validate_resource_annotated_function
+        from dagster._config.pythonic_config import validate_resource_annotated_function
 
         check.callable_param(fn, "fn")
         validate_resource_annotated_function(fn)
 
         schedule_name = name or fn.__name__
 
         validated_tags = None
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections.abc
 import inspect
 from functools import update_wrapper
-from typing import Callable, Optional, Sequence, Set, Union
+from typing import Any, Callable, Optional, Sequence, Set, Union
 
 import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.asset_selection import AssetSelection
 
 from ...errors import DagsterInvariantViolationError
 from ..asset_sensor_definition import AssetSensorDefinition
@@ -153,16 +153,16 @@
     """
     check.opt_str_param(name, "name")
 
     def inner(fn: AssetMaterializationFunction) -> AssetSensorDefinition:
         check.callable_param(fn, "fn")
         sensor_name = name or fn.__name__
 
-        def _wrapped_fn(context, event):
-            result = fn(context, event)
+        def _wrapped_fn(*args, **kwargs) -> Any:
+            result = fn(*args, **kwargs)
 
             if inspect.isgenerator(result) or isinstance(result, list):
                 for item in result:
                     yield item
             elif isinstance(result, (RunRequest, SkipReason)):
                 yield result
 
@@ -180,14 +180,18 @@
                     (
                         "Error in sensor {sensor_name}: Sensor unexpectedly returned output "
                         "{result} of type {type_}.  Should only return SkipReason or "
                         "RunRequest objects."
                     ).format(sensor_name=sensor_name, result=result, type_=type(result))
                 )
 
+        # Preserve any resource arguments from the underlying function, for when we inspect the
+        # wrapped function later on
+        _wrapped_fn.__signature__ = inspect.signature(fn)
+
         return AssetSensorDefinition(
             name=sensor_name,
             asset_key=asset_key,
             job_name=job_name,
             asset_materialization_fn=_wrapped_fn,
             minimum_interval_seconds=minimum_interval_seconds,
             description=description,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.0/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKeyPrefix
 from dagster._core.definitions.metadata import (
     MetadataUserInput,
 )
-from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.resource_annotation import get_resource_args
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.source_asset import SourceAsset, SourceAssetObserveFunction
 from dagster._core.storage.io_manager import IOManagerDefinition
 
 
 @overload
@@ -23,15 +22,14 @@
     *,
     name: Optional[str] = ...,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
     io_manager_def: Optional[IOManagerDefinition] = None,
     description: Optional[str] = None,
-    partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
     required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> "_ObservableSourceAsset":
     ...
 
 
@@ -41,15 +39,14 @@
     *,
     name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     metadata: Optional[MetadataUserInput] = None,
     io_manager_key: Optional[str] = None,
     io_manager_def: Optional[IOManagerDefinition] = None,
     description: Optional[str] = None,
-    partitions_def: Optional[PartitionsDefinition] = None,
     group_name: Optional[str] = None,
     required_resource_keys: Optional[AbstractSet[str]] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
 ) -> Union[SourceAsset, "_ObservableSourceAsset"]:
     """Create a `SourceAsset` with an associated observation function.
 
     The observation function of a source asset is wrapped inside of an op and can be executed as
@@ -67,16 +64,14 @@
             contains letters, numbers, and _) and may not contain python reserved keywords.
         metadata (Mapping[str, RawMetadataValue]): Metadata associated with the asset.
         io_manager_key (Optional[str]): The key for the IOManager that will be used to load the contents of
             the source asset when it's used as an input to other assets inside a job.
         io_manager_def (Optional[IOManagerDefinition]): (Experimental) The definition of the IOManager that will be used to load the contents of
             the source asset when it's used as an input to other assets inside a job.
         description (Optional[str]): The description of the asset.
-        partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
-            compose the source asset.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If not provided,
             the name "default" is used.
         required_resource_keys (Optional[Set[str]]): Set of resource keys required by the observe op.
         resource_defs (Optional[Mapping[str, ResourceDefinition]]): (Experimental) resource
             definitions that may be required by the :py:class:`dagster.IOManagerDefinition` provided in
             the `io_manager_def` argument.
         observe_fn (Optional[SourceAssetObserveFunction]) Observation function for the source asset.
@@ -87,15 +82,14 @@
     return _ObservableSourceAsset(
         name,
         key_prefix,
         metadata,
         io_manager_key,
         io_manager_def,
         description,
-        partitions_def,
         group_name,
         required_resource_keys,
         resource_defs,
     )
 
 
 class _ObservableSourceAsset:
@@ -103,30 +97,28 @@
         self,
         name: Optional[str] = None,
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         metadata: Optional[MetadataUserInput] = None,
         io_manager_key: Optional[str] = None,
         io_manager_def: Optional[IOManagerDefinition] = None,
         description: Optional[str] = None,
-        partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
         required_resource_keys: Optional[AbstractSet[str]] = None,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     ):
         self.name = name
         if isinstance(key_prefix, str):
             key_prefix = [key_prefix]
         elif key_prefix is None:
             key_prefix = []
         self.key_prefix = key_prefix
         self.metadata = metadata
         self.io_manager_key = io_manager_key
         self.io_manager_def = io_manager_def
         self.description = description
-        self.partitions_def = partitions_def
         self.group_name = group_name
         self.required_resource_keys = required_resource_keys
         self.resource_defs = resource_defs
 
     def __call__(self, observe_fn: SourceAssetObserveFunction) -> SourceAsset:
         source_asset_name = self.name or observe_fn.__name__
         source_asset_key = AssetKey([*self.key_prefix, source_asset_name])
@@ -144,13 +136,12 @@
 
         return SourceAsset(
             key=source_asset_key,
             metadata=self.metadata,
             io_manager_key=self.io_manager_key,
             io_manager_def=self.io_manager_def,
             description=self.description,
-            partitions_def=self.partitions_def,
             group_name=self.group_name,
             _required_resource_keys=resolved_resource_keys,
             resource_defs=self.resource_defs,
             observe_fn=observe_fn,
         )
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.0/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.0/dagster/_core/definitions/definitions_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import warnings
 from typing import (
     TYPE_CHECKING,
     Any,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Type,
     Union,
 )
 
 import dagster._check as check
-from dagster._annotations import experimental, public
-from dagster._config.structured_config import (
+from dagster._annotations import deprecated, experimental, public
+from dagster._config.pythonic_config import (
     attach_resource_id_to_key_mapping,
 )
 from dagster._core.definitions.events import AssetKey, CoercibleToAssetKey
 from dagster._core.definitions.executor_definition import ExecutorDefinition
 from dagster._core.definitions.logger_definition import LoggerDefinition
 from dagster._core.execution.build_resources import wrap_resources_for_execution
 from dagster._core.execution.with_resources import with_resources
@@ -232,48 +231,20 @@
         else {}
     )
 
     resource_defs = wrap_resources_for_execution(resources_with_key_mapping)
 
     check.opt_mapping_param(loggers, "loggers", key_type=str, value_type=LoggerDefinition)
 
-    if isinstance(jobs, BindResourcesToJobs):
-        # Binds top-level resources to jobs and any jobs attached to schedules or sensors
-        (
-            jobs_with_resources,
-            schedules_with_resources,
-            sensors_with_resources,
-        ) = _attach_resources_to_jobs_and_instigator_jobs(jobs, schedules, sensors, resource_defs)
-    else:
-        jobs_to_warn = _jobs_which_will_have_io_manager_replaced(jobs, resource_defs)
-        if jobs_to_warn:
-            jobs_text = ", ".join([f"`{job.name}`" for job in jobs_to_warn[:10]])
-            if len(jobs_to_warn) > 10:
-                jobs_text += f", and {len(jobs_to_warn) - 10} others"
-            warnings.warn(
-                f"""You have overridden the default `io_manager` on `Definitions`. One or more jobs utilize the default filesystem I/O manager. In the future, these jobs will use the `Definitions`-level override instead. To silence this warning, explicitly set the `io_manager` on the jobs in question:
-
-@job(resource_defs={{'io_manager': fs_io_manager}})
-def my_job():
-    ...
-    
-Alternatively, wrap the jobs input to `Definitions` with `BindResourceToJobs`:
-
-defs = Definitions(
-    jobs=BindResourcesToJobs([my_job, my_other_job, ...])
-)
-
-In later releases, this will be the default behavior, and `BindResourcesToJobs` will not be required.
-
-The following jobs are affected: {jobs_text}
-                """
-            )
-        jobs_with_resources = jobs or []
-        schedules_with_resources = schedules or []
-        sensors_with_resources = sensors or []
+    # Binds top-level resources to jobs and any jobs attached to schedules or sensors
+    (
+        jobs_with_resources,
+        schedules_with_resources,
+        sensors_with_resources,
+    ) = _attach_resources_to_jobs_and_instigator_jobs(jobs, schedules, sensors, resource_defs)
 
     @repository(
         name=name,
         default_executor_def=executor_def,
         default_logger_defs=loggers,
         _top_level_resources=resource_defs,
         _resource_key_mapping=resource_key_mapping,
@@ -285,16 +256,19 @@
             *(sensors_with_resources),
             *(jobs_with_resources),
         ]
 
     return created_repo
 
 
+@deprecated
 class BindResourcesToJobs(list):
-    pass
+    """Used to instruct Dagster to bind top-level resources to jobs and any jobs attached to schedules
+    and sensors. Now deprecated since this behavior is the default.
+    """
 
 
 class Definitions:
     """A set of definitions explicitly available and loadable by Dagster tools.
 
     Parameters:
         assets (Optional[Iterable[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]]):
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/dependency.py` & `dagster-1.3.0/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/events.py` & `dagster-1.3.0/dagster/_core/definitions/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from dagster._core.definitions.data_version import DataVersion
 from dagster._core.storage.tags import MULTIDIMENSIONAL_PARTITION_PREFIX, SYSTEM_TAG_PREFIX
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import NamedTupleSerializer
 from dagster._utils.backcompat import experimental_class_param_warning
 
 from .metadata import (
-    MetadataEntry,
     MetadataFieldSerializer,
     MetadataMapping,
     MetadataValue,
     RawMetadataValue,
     normalize_metadata,
 )
 from .utils import DEFAULT_OUTPUT, check_valid_name
@@ -230,41 +229,36 @@
     They are type-checked at op boundaries when their corresponding :py:class:`Out`
     or the downstream :py:class:`In` is typed.
 
     Args:
         value (Any): The value returned by the compute function.
         output_name (Optional[str]): Name of the corresponding out. (default:
             "result")
-        metadata_entries (Optional[MetadataEntry]):
-            (Deprecated) A set of metadata entries to attach to events related to this Output. Use
-            `metadata` instead.
         metadata (Optional[Dict[str, Union[str, float, int, MetadataValue]]]):
             Arbitrary metadata about the failure.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
         data_version (Optional[DataVersion]): (Experimental) A data version to manually set
             for the asset.
     """
 
     def __init__(
         self,
         value: T,
         output_name: Optional[str] = DEFAULT_OUTPUT,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         data_version: Optional[DataVersion] = None,
     ):
         self._value = value
         self._output_name = check.str_param(output_name, "output_name")
         if data_version is not None:
             experimental_class_param_warning("data_version", "Output")
         self._data_version = check.opt_inst_param(data_version, "data_version", DataVersion)
         self._metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
-            check.opt_sequence_param(metadata_entries, "metadata_entries", of_type=MetadataEntry),
         )
 
     @property
     def metadata(self) -> MetadataMapping:
         return self._metadata
 
     @public
@@ -305,37 +299,32 @@
         mapping_key (str):
             The key that uniquely identifies this dynamic value relative to its peers.
             This key will be used to identify the downstream ops when mapped, ie
             ``mapped_op[example_mapping_key]``
         output_name (Optional[str]):
             Name of the corresponding :py:class:`DynamicOut` defined on the op.
             (default: "result")
-        metadata_entries (Optional[MetadataEntry]):
-            (Deprecated) A set of metadata entries to attach to events related to this Output. Use
-            `metadata` instead.
         metadata (Optional[Dict[str, Union[str, float, int, MetadataValue]]]):
             Arbitrary metadata about the failure.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __init__(
         self,
         value: T,
         mapping_key: str,
         output_name: Optional[str] = DEFAULT_OUTPUT,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     ):
         self._mapping_key = check_valid_name(check.str_param(mapping_key, "mapping_key"))
         self._output_name = check.str_param(output_name, "output_name")
         self._value = value
         self._metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
-            check.opt_sequence_param(metadata_entries, "metadata_entries", of_type=MetadataEntry),
         )
 
     @property
     def metadata(self) -> Mapping[str, MetadataValue]:
         return self._metadata
 
     @public
@@ -359,29 +348,14 @@
             and self.value == other.value
             and self.output_name == other.output_name
             and self.mapping_key == other.mapping_key
             and self.metadata == other.metadata
         )
 
 
-# This is a temporary function to consolidate metadata normalization logic on event classes where
-# we've had to mangle the signature for backcompat reasons. Can be deleted when we remove
-# `metadata_entries`/`MetadataEntry`.
-def _normalize_event_metadata(
-    metadata: Optional[Union[Mapping[str, RawMetadataValue], Sequence[MetadataEntry]]] = None,
-    metadata_entries: Optional[Sequence[MetadataEntry]] = None,
-) -> MetadataMapping:
-    metadata_dict = metadata if isinstance(metadata, dict) else {}
-    metadata_entries = metadata if isinstance(metadata, list) else metadata_entries
-    return normalize_metadata(
-        check.opt_mapping_param(metadata_dict, "metadata_dict", key_type=str),
-        check.opt_sequence_param(metadata_entries, "metadata_entries", of_type=MetadataEntry),
-    )
-
-
 @whitelist_for_serdes(
     storage_field_names={"metadata": "metadata_entries"},
     field_serializers={"metadata": MetadataFieldSerializer},
 )
 class AssetObservation(
     NamedTuple(
         "_AssetObservation",
@@ -394,34 +368,31 @@
         ],
     )
 ):
     """Event that captures metadata about an asset at a point in time.
 
     Args:
         asset_key (Union[str, List[str], AssetKey]): A key to identify the asset.
-        metadata_entries (Optional[List[MetadataEntry]]): (Deprecated) Arbitrary metadata about the
-            asset. Use `metadata` instead.
         partition (Optional[str]): The name of a partition of the asset that the metadata
             corresponds to.
         tags (Optional[Mapping[str, str]]): A mapping containing system-populated tags for the
             observation. Users should not pass values into this argument.
         metadata (Optional[Dict[str, Union[str, float, int, MetadataValue]]]):
             Arbitrary metadata about the asset.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __new__(
         cls,
         asset_key: CoercibleToAssetKey,
         description: Optional[str] = None,
-        metadata: Optional[Union[Mapping[str, RawMetadataValue], Sequence[MetadataEntry]]] = None,
+        metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         partition: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
     ):
         if isinstance(asset_key, AssetKey):
             check.inst_param(asset_key, "asset_key", AssetKey)
         elif isinstance(asset_key, str):
             asset_key = AssetKey(parse_asset_key_string(asset_key))
         else:
             check.sequence_param(asset_key, "asset_key", of_type=str)
@@ -430,15 +401,17 @@
         tags = check.opt_mapping_param(tags, "tags", key_type=str, value_type=str)
         if any([not tag.startswith(SYSTEM_TAG_PREFIX) for tag in tags or {}]):
             check.failed(
                 "Users should not pass values into the tags argument for AssetMaterializations. "
                 "The tags argument is reserved for system-populated tags."
             )
 
-        metadata = _normalize_event_metadata(metadata, metadata_entries)
+        metadata = normalize_metadata(
+            check.opt_mapping_param(metadata, "metadata", key_type=str),
+        )
 
         return super(AssetObservation, cls).__new__(
             cls,
             asset_key=asset_key,
             description=check.opt_str_param(description, "description"),
             metadata=metadata,
             tags=tags,
@@ -493,34 +466,31 @@
     Op authors should use these events to organize metadata about the side effects of their
     computations, enabling tooling like the Assets dashboard in Dagit.
 
     Args:
         asset_key (Union[str, List[str], AssetKey]): A key to identify the materialized asset across
             job runs
         description (Optional[str]): A longer human-readable description of the materialized value.
-        metadata_entries (Optional[List[MetadataEntry]]): (Deprecated) Arbitrary
-            metadata about the materialized value. Use `metadata` instead.
         partition (Optional[str]): The name of the partition
             that was materialized.
         tags (Optional[Mapping[str, str]]): A mapping containing system-populated tags for the
             materialization. Users should not pass values into this argument.
         metadata (Optional[Dict[str, RawMetadataValue]]):
             Arbitrary metadata about the asset.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __new__(
         cls,
         asset_key: CoercibleToAssetKey,
         description: Optional[str] = None,
-        metadata: Optional[Union[Mapping[str, RawMetadataValue], Sequence[MetadataEntry]]] = None,
+        metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         partition: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
     ):
         from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionKey
 
         if isinstance(asset_key, AssetKey):
             check.inst_param(asset_key, "asset_key", AssetKey)
         elif isinstance(asset_key, str):
             asset_key = AssetKey(parse_asset_key_string(asset_key))
@@ -532,15 +502,17 @@
         invalid_tags = [tag for tag in tags or {} if not tag.startswith(SYSTEM_TAG_PREFIX)]
         if len(invalid_tags) > 0:
             check.failed(
                 f"Invalid tags: {tags} Users should not pass values into the tags argument for"
                 " AssetMaterializations. The tags argument is reserved for system-populated tags."
             )
 
-        metadata = _normalize_event_metadata(metadata, metadata_entries)
+        metadata = normalize_metadata(
+            check.opt_mapping_param(metadata, "metadata", key_type=str),
+        )
 
         partition = check.opt_str_param(partition, "partition")
 
         if not isinstance(partition, MultiPartitionKey):
             # When event log records are unpacked from storage, cast the partition key as a
             # MultiPartitionKey if multi-dimensional partition tags exist
             multi_dimensional_partitions = {
@@ -608,31 +580,30 @@
     Dagster framework (and the end user) that a data quality test has produced a (positive or
     negative) result.
 
     Args:
         success (bool): Whether the expectation passed or not.
         label (Optional[str]): Short display name for expectation. Defaults to "result".
         description (Optional[str]): A longer human-readable description of the expectation.
-        metadata_entries (Optional[List[MetadataEntry]]): (Deprecated) Arbitrary metadata about the
-            expectation. Use `metadata` instead.
         metadata (Optional[Dict[str, RawMetadataValue]]):
             Arbitrary metadata about the failure.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __new__(
         cls,
         success: bool,
         label: Optional[str] = None,
         description: Optional[str] = None,
-        metadata: Optional[Union[Mapping[str, RawMetadataValue], Sequence[MetadataEntry]]] = None,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
+        metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     ):
-        metadata = _normalize_event_metadata(metadata, metadata_entries)
+        metadata = normalize_metadata(
+            check.opt_mapping_param(metadata, "metadata", key_type=str),
+        )
 
         return super(ExpectationResult, cls).__new__(
             cls,
             success=check.bool_param(success, "success"),
             label=check.opt_str_param(label, "label", "result"),
             description=check.opt_str_param(description, "description"),
             metadata=metadata,
@@ -662,30 +633,29 @@
     :py:func:`PythonObjectDagsterType` API.)
 
     Solid compute functions should generally avoid yielding events of this type to avoid confusion.
 
     Args:
         success (bool): ``True`` if the type check succeeded, ``False`` otherwise.
         description (Optional[str]): A human-readable description of the type check.
-        metadata_entries (Optional[List[MetadataEntry]]): (Deprecated) Arbitrary metadata about the
-            type check. Use `metadata` instead.
         metadata (Optional[Dict[str, RawMetadataValue]]):
             Arbitrary metadata about the failure.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __new__(
         cls,
         success: bool,
         description: Optional[str] = None,
-        metadata: Optional[Union[Mapping[str, RawMetadataValue], Sequence[MetadataEntry]]] = None,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
+        metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     ):
-        metadata = _normalize_event_metadata(metadata, metadata_entries)
+        metadata = normalize_metadata(
+            check.opt_mapping_param(metadata, "metadata", key_type=str),
+        )
 
         return super(TypeCheck, cls).__new__(
             cls,
             success=check.bool_param(success, "success"),
             description=check.opt_str_param(description, "description"),
             metadata=metadata,
         )
@@ -696,37 +666,33 @@
 
     Raise events of this type from within op compute functions or custom type checks in order to
     indicate an unrecoverable failure in user code to the Dagster machinery and return
     structured metadata about the failure.
 
     Args:
         description (Optional[str]): A human-readable description of the failure.
-        metadata_entries (Optional[List[MetadataEntry]]): (Deprecated) Arbitrary metadata about the
-            failure. Use `metadata` instead.
         metadata (Optional[Dict[str, RawMetadataValue]]):
             Arbitrary metadata about the failure.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
         allow_retries (Optional[bool]):
             Whether this Failure should respect the retry policy or bypass it and immediately fail.
             Defaults to True, respecting the retry policy and allowing retries.
     """
 
     def __init__(
         self,
         description: Optional[str] = None,
-        metadata_entries: Optional[Sequence[MetadataEntry]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         allow_retries: Optional[bool] = None,
     ):
         super(Failure, self).__init__(description)
         self.description = check.opt_str_param(description, "description")
         self.metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
-            check.opt_sequence_param(metadata_entries, "metadata_entries", of_type=MetadataEntry),
         )
         self.allow_retries = check.opt_bool_param(allow_retries, "allow_retries", True)
 
 
 class RetryRequested(Exception):
     """An exception to raise from an op to indicate that it should be retried.
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.0/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.0/dagster/_core/definitions/external_asset_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,7 +222,18 @@
         """
         for job_name in sorted(self._asset_keys_by_job_name.keys()):
             if not job_name.startswith(ASSET_BASE_JOB_PREFIX):
                 continue
             if all(asset_key in self._asset_keys_by_job_name[job_name] for asset_key in asset_keys):
                 return job_name
         return None
+
+    def split_asset_keys_by_repository(
+        self, asset_keys: AbstractSet[AssetKey]
+    ) -> Sequence[AbstractSet[AssetKey]]:
+        asset_keys_by_repo = defaultdict(set)
+        for asset_key in asset_keys:
+            repo_handle = self.get_repository_handle(asset_key)
+            asset_keys_by_repo[(repo_handle.location_name, repo_handle.repository_name)].add(
+                asset_key
+            )
+        return list(asset_keys_by_repo.values())
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.0/dagster/_core/definitions/freshness_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,27 +144,27 @@
     def __reduce__(self):
         return (self._create, (self.maximum_lag_minutes, self.cron_schedule))
 
     @property
     def maximum_lag_delta(self) -> datetime.timedelta:
         return datetime.timedelta(minutes=self.maximum_lag_minutes)
 
-    def minutes_late(
+    def minutes_overdue(
         self,
         data_time: Optional[datetime.datetime],
         evaluation_time: datetime.datetime,
     ) -> Optional[float]:
         """Returns a number of minutes past the specified freshness policy that this asset currently
         is. If the asset is missing upstream data, or is not materialized at all, then it is unknown
-        how late it is, and this will return None.
+        how overdue it is, and this will return None.
 
         Args:
             data_time (Optional[datetime]): The timestamp of the data that was used to create the
                 current version of this asset.
-            evaluation_time (datetime): The time at which we're evaluating the lateness of this
+            evaluation_time (datetime): The time at which we're evaluating the overdueness of this
                 asset. Generally, this is the current time.
         """
         if data_time is None:
             return None
         if self.cron_schedule:
             # most recent cron schedule tick
             schedule_ticks = reverse_cron_string_iterator(
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.0/dagster/_core/definitions/graph_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing_extensions import Self
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.definitions.config import ConfigMapping
 from dagster._core.definitions.definition_config_schema import IDefinitionConfigSchema
 from dagster._core.definitions.policy import RetryPolicy
-from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvariantViolationError
 from dagster._core.selector.subset_selector import AssetSelectionData
 from dagster._core.types.dagster_type import (
     DagsterType,
     DagsterTypeKind,
     construct_dagster_type_dictionary,
 )
@@ -60,14 +59,15 @@
 
     from .asset_layer import AssetLayer
     from .composition import PendingNodeInvocation
     from .executor_definition import ExecutorDefinition
     from .job_definition import JobDefinition
     from .op_definition import OpDefinition
     from .partition import PartitionedConfig, PartitionsDefinition
+    from .run_config import RunConfig
     from .source_asset import SourceAsset
 
 T = TypeVar("T")
 
 
 def _check_node_defs_arg(
     graph_name: str, node_defs: Optional[Sequence[NodeDefinition]]
@@ -543,16 +543,18 @@
         return list(self._node_dict.keys())
 
     @public
     def to_job(
         self,
         name: Optional[str] = None,
         description: Optional[str] = None,
-        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
-        config: Optional[Union[ConfigMapping, Mapping[str, object], "PartitionedConfig[T]"]] = None,
+        resource_defs: Optional[Mapping[str, object]] = None,
+        config: Optional[
+            Union["RunConfig", ConfigMapping, Mapping[str, object], "PartitionedConfig[T]"]
+        ] = None,
         tags: Optional[Mapping[str, str]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         logger_defs: Optional[Mapping[str, LoggerDefinition]] = None,
         executor_def: Optional["ExecutorDefinition"] = None,
         hooks: Optional[AbstractSet[HookDefinition]] = None,
         op_retry_policy: Optional[RetryPolicy] = None,
         version_strategy: Optional[VersionStrategy] = None,
@@ -563,15 +565,15 @@
         _asset_selection_data: Optional[AssetSelectionData] = None,
     ) -> "JobDefinition":
         """Make this graph in to an executable Job by providing remaining components required for execution.
 
         Args:
             name (Optional[str]):
                 The name for the Job. Defaults to the name of the this graph.
-            resource_defs (Optional[Mapping [str, ResourceDefinition]]):
+            resource_defs (Optional[Mapping [str, object]]):
                 Resources that are required by this graph for execution.
                 If not defined, `io_manager` will default to filesystem.
             config:
                 Describes how the job is parameterized at runtime.
 
                 If no value is provided, then the schema for the job's run config is a standard
                 format based on its ops and resources.
@@ -616,21 +618,25 @@
                 will produce. Generally should not be set manually.
             input_values (Optional[Mapping[str, Any]]):
                 A dictionary that maps python objects to the top-level inputs of a job.
 
         Returns:
             JobDefinition
         """
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
         from .job_definition import JobDefinition
 
+        wrapped_resource_defs = wrap_resources_for_execution(resource_defs)
+
         return JobDefinition(
             name=name,
             description=description or self.description,
             graph_def=self,
-            resource_defs=resource_defs,
+            resource_defs=wrapped_resource_defs,
             logger_defs=logger_defs,
             executor_def=executor_def,
             config=config,
             partitions_def=partitions_def,
             tags=tags,
             metadata=metadata,
             hook_defs=hooks,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.0/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.0/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/inference.py` & `dagster-1.3.0/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/input.py` & `dagster-1.3.0/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.0/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/job_definition.py` & `dagster-1.3.0/dagster/_core/definitions/job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 from .preset import PresetDefinition
 from .resource_definition import ResourceDefinition
 from .run_request import RunRequest
 from .utils import DEFAULT_IO_MANAGER_KEY
 from .version_strategy import VersionStrategy
 
 if TYPE_CHECKING:
+    from dagster._core.definitions.run_config import RunConfig
     from dagster._core.execution.execute_in_process_result import ExecuteInProcessResult
     from dagster._core.execution.resources_init import InitResourceContext
     from dagster._core.instance import DagsterInstance
     from dagster._core.snap import PipelineSnapshot
 
 
 class JobDefinition(PipelineDefinition):
@@ -91,15 +92,17 @@
         self,
         *,
         graph_def: GraphDefinition,
         resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         executor_def: Optional[ExecutorDefinition] = None,
         logger_defs: Optional[Mapping[str, LoggerDefinition]] = None,
         name: Optional[str] = None,
-        config: Optional[Union[ConfigMapping, Mapping[str, object], PartitionedConfig]] = None,
+        config: Optional[
+            Union[ConfigMapping, Mapping[str, object], PartitionedConfig, "RunConfig"]
+        ] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         tags: Optional[Mapping[str, Any]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         hook_defs: Optional[AbstractSet[HookDefinition]] = None,
         op_retry_policy: Optional[RetryPolicy] = None,
         version_strategy: Optional[VersionStrategy] = None,
@@ -293,15 +296,15 @@
     @property
     def loggers(self) -> Mapping[str, LoggerDefinition]:
         return self.get_mode_definition().loggers
 
     @public
     def execute_in_process(
         self,
-        run_config: Optional[Mapping[str, Any]] = None,
+        run_config: Optional[Union[Mapping[str, Any], "RunConfig"]] = None,
         instance: Optional["DagsterInstance"] = None,
         partition_key: Optional[str] = None,
         raise_on_error: bool = True,
         op_selection: Optional[Sequence[str]] = None,
         asset_selection: Optional[Sequence[AssetKey]] = None,
         run_id: Optional[str] = None,
         input_values: Optional[Mapping[str, object]] = None,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.0/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import pkgutil
 from importlib import import_module
 from types import ModuleType
 from typing import Dict, Generator, Iterable, List, Optional, Sequence, Set, Tuple, Union
 
 import dagster._check as check
+from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.errors import DagsterInvalidDefinitionError
 
 from .assets import AssetsDefinition
 from .cacheable_assets import CacheableAssetsDefinition
 from .events import (
     AssetKey,
@@ -96,70 +97,80 @@
 
 def load_assets_from_modules(
     modules: Iterable[ModuleType],
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets and source assets from the given modules.
 
     Args:
         modules (Iterable[ModuleType]): The Python modules to look for assets inside.
         group_name (Optional[str]):
             Group name to apply to the loaded assets. The returned assets will be copies of the
             loaded objects, with the group name added.
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
+            to all the loaded assets.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset]]:
             A list containing assets and source assets defined in the given modules.
     """
     group_name = check.opt_str_param(group_name, "group_name")
     key_prefix = check_opt_coercible_to_asset_key_prefix_param(key_prefix, "key_prefix")
     freshness_policy = check.opt_inst_param(freshness_policy, "freshness_policy", FreshnessPolicy)
+    auto_materialize_policy = check.opt_inst_param(
+        auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
+    )
 
     (
         assets,
         source_assets,
         cacheable_assets,
     ) = assets_from_modules(modules)
 
     return assets_with_attributes(
         assets,
         source_assets,
         cacheable_assets,
         key_prefix=key_prefix,
         group_name=group_name,
         freshness_policy=freshness_policy,
+        auto_materialize_policy=auto_materialize_policy,
     )
 
 
 def load_assets_from_current_module(
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets, source assets, and cacheable assets from the module where
     this function is called.
 
     Args:
         group_name (Optional[str]):
             Group name to apply to the loaded assets. The returned assets will be copies of the
             loaded objects, with the group name added.
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
+            to all the loaded assets.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset, CachableAssetsDefinition]]:
             A list containing assets, source assets, and cacheable assets defined in the module.
     """
     caller = inspect.stack()[1]
     module = inspect.getmodule(caller[0])
@@ -167,14 +178,15 @@
         check.failed("Could not find a module for the caller")
 
     return load_assets_from_modules(
         [module],
         group_name=group_name,
         key_prefix=key_prefix,
         freshness_policy=freshness_policy,
+        auto_materialize_policy=auto_materialize_policy,
     )
 
 
 def assets_from_package_module(
     package_module: ModuleType,
     extra_source_assets: Optional[Sequence[SourceAsset]] = None,
 ) -> Tuple[Sequence[AssetsDefinition], Sequence[SourceAsset], Sequence[CacheableAssetsDefinition]]:
@@ -198,14 +210,15 @@
 
 def load_assets_from_package_module(
     package_module: ModuleType,
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets and source assets that includes all asset
     definitions, source assets, and cacheable assets in all sub-modules of the given package module.
 
     A package module is the result of importing a package.
 
     Args:
@@ -214,69 +227,79 @@
             Group name to apply to the loaded assets. The returned assets will be copies of the
             loaded objects, with the group name added.
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
+            to all the loaded assets.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
             A list containing assets, source assets, and cacheable assets defined in the module.
     """
     group_name = check.opt_str_param(group_name, "group_name")
     key_prefix = check_opt_coercible_to_asset_key_prefix_param(key_prefix, "key_prefix")
     freshness_policy = check.opt_inst_param(freshness_policy, "freshness_policy", FreshnessPolicy)
+    auto_materialize_policy = check.opt_inst_param(
+        auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
+    )
 
     (
         assets,
         source_assets,
         cacheable_assets,
     ) = assets_from_package_module(package_module)
     return assets_with_attributes(
         assets,
         source_assets,
         cacheable_assets,
         key_prefix=key_prefix,
         group_name=group_name,
         freshness_policy=freshness_policy,
+        auto_materialize_policy=auto_materialize_policy,
     )
 
 
 def load_assets_from_package_name(
     package_name: str,
     group_name: Optional[str] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     *,
     freshness_policy: Optional[FreshnessPolicy] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     """Constructs a list of assets, source assets, and cacheable assets that includes all asset
     definitions and source assets in all sub-modules of the given package.
 
     Args:
         package_name (str): The name of a Python package to look for assets inside.
         group_name (Optional[str]):
             Group name to apply to the loaded assets. The returned assets will be copies of the
             loaded objects, with the group name added.
         key_prefix (Optional[Union[str, Sequence[str]]]):
             Prefix to prepend to the keys of the loaded assets. The returned assets will be copies
             of the loaded objects, with the prefix prepended.
         freshness_policy (Optional[FreshnessPolicy]): FreshnessPolicy to apply to all the loaded
             assets.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): AutoMaterializePolicy to apply
+            to all the loaded assets.
 
     Returns:
         Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
             A list containing assets, source assets, and cacheable assets defined in the module.
     """
     package_module = import_module(package_name)
     return load_assets_from_package_module(
         package_module,
         group_name=group_name,
         key_prefix=key_prefix,
         freshness_policy=freshness_policy,
+        auto_materialize_policy=auto_materialize_policy,
     )
 
 
 def _find_modules_in_package(package_module: ModuleType) -> Iterable[ModuleType]:
     yield package_module
     package_path = package_module.__file__
     if package_path:
@@ -360,38 +383,44 @@
 def assets_with_attributes(
     assets_defs: Sequence[AssetsDefinition],
     source_assets: Sequence[SourceAsset],
     cacheable_assets: Sequence[CacheableAssetsDefinition],
     key_prefix: Optional[Sequence[str]],
     group_name: Optional[str],
     freshness_policy: Optional[FreshnessPolicy],
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
 ) -> Sequence[Union[AssetsDefinition, SourceAsset, CacheableAssetsDefinition]]:
     # There is a tricky edge case here where if a non-cacheable asset depends on a cacheable asset,
     # and the assets are prefixed, the non-cacheable asset's dependency will not be prefixed since
     # at prefix-time it is not known that its dependency is one of the cacheable assets.
     # https://github.com/dagster-io/dagster/pull/10389#pullrequestreview-1170913271
     if key_prefix:
         assets_defs = prefix_assets(assets_defs, key_prefix)
         cacheable_assets = [
             cached_asset.with_prefix_for_all(key_prefix) for cached_asset in cacheable_assets
         ]
 
-    if group_name or freshness_policy:
+    if group_name or freshness_policy or auto_materialize_policy:
         assets_defs = [
             asset.with_attributes(
                 group_names_by_key={asset_key: group_name for asset_key in asset.keys}
                 if group_name
                 else None,
                 freshness_policy=freshness_policy,
+                auto_materialize_policy=auto_materialize_policy,
             )
             for asset in assets_defs
         ]
         if group_name:
             source_assets = [
                 source_asset.with_group_name(group_name) for source_asset in source_assets
             ]
         cacheable_assets = [
-            cached_asset.with_attributes_for_all(group_name, freshness_policy=freshness_policy)
+            cached_asset.with_attributes_for_all(
+                group_name,
+                freshness_policy=freshness_policy,
+                auto_materialize_policy=auto_materialize_policy,
+            )
             for cached_asset in cacheable_assets
         ]
 
     return [*assets_defs, *source_assets, *cacheable_assets]
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.0/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.0/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/materialize.py` & `dagster-1.3.0/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.0/dagster/_core/definitions/metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     cast,
 )
 
 from typing_extensions import Self, TypeAlias, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
-from dagster._annotations import PublicAttr, experimental, public
+from dagster._annotations import PublicAttr, deprecated, experimental, public
 from dagster._core.errors import DagsterInvalidMetadata
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import (
     FieldSerializer,
     PackableValue,
     WhitelistMap,
     pack_value,
@@ -68,34 +68,16 @@
 # ########################
 # ##### NORMALIZATION
 # ########################
 
 
 def normalize_metadata(
     metadata: Mapping[str, RawMetadataValue],
-    metadata_entries: Optional[Sequence["MetadataEntry"]] = None,
     allow_invalid: bool = False,
 ) -> Mapping[str, "MetadataValue"]:
-    if metadata and metadata_entries:
-        raise DagsterInvalidMetadata(
-            "Attempted to provide both `metadata` and `metadata_entries` arguments to an event. "
-            "Must provide only one of the two."
-        )
-    elif metadata_entries:
-        deprecation_warning(
-            'Argument "metadata_entries"',
-            "1.0.0",
-            additional_warn_txt=(
-                "Use argument `metadata` instead. The `MetadataEntry` `description` attribute is"
-                " also deprecated-- argument `metadata` takes a label: value dictionary."
-            ),
-            stacklevel=4,  # to get the caller of `normalize_metadata`
-        )
-        return {entry.label: entry.value for entry in metadata_entries}
-
     # This is a stopgap measure to deal with unsupported metadata values, which occur when we try
     # to convert arbitrary metadata (on e.g. OutputDefinition) to a MetadataValue, which is required
     # for serialization. This will cause unsupported values to be silently replaced with a
     # string placeholder.
     normalized_metadata: Dict[str, MetadataValue] = {}
     for k, v in metadata.items():
         try:
@@ -147,18 +129,14 @@
 
     raise DagsterInvalidMetadata(
         f"Its type was {type(raw_value)}. Consider wrapping the value with the appropriate "
         "MetadataValue type."
     )
 
 
-def to_metadata_entries(metadata: Mapping[str, "MetadataValue"]) -> Sequence["MetadataEntry"]:
-    return [MetadataEntry(k, value=v) for k, v in metadata.items()]
-
-
 # ########################
 # ##### METADATA VALUE
 # ########################
 
 
 class MetadataValue(ABC, Generic[T_Packable]):
     """Utility class to wrap metadata values passed into Dagster events so that they can be
@@ -927,17 +905,21 @@
 
     @property
     def value(self) -> None:
         return None
 
 
 # ########################
-# ##### METADATA ENTRY
+# ##### METADATA BACKCOMPAT
 # ########################
 
+# Metadata used to be represented as a `List[MetadataEntry]`, but that class has been deleted. But
+# we still serialize metadata dicts to the serialized representation of `List[MetadataEntry]` for
+# backcompat purposes.
+
 
 class MetadataFieldSerializer(FieldSerializer):
     """Converts between metadata dict (new) and metadata entries list (old)."""
 
     storage_name = "metadata_entries"
     loaded_name = "metadata"
 
@@ -980,27 +962,30 @@
 
 T_MetadataValue = TypeVar("T_MetadataValue", bound=MetadataValue, covariant=True)
 
 
 # NOTE: This currently stores value in the `entry_data` NamedTuple attribute. In the next release,
 # we will change the name of the NamedTuple property to `value`, and need to implement custom
 # serialization so that it continues to be saved as `entry_data` for backcompat purposes.
+@deprecated
 @whitelist_for_serdes(storage_name="EventMetadataEntry")
 class MetadataEntry(
     NamedTuple(
         "_MetadataEntry",
         [
             ("label", PublicAttr[str]),
             ("description", PublicAttr[Optional[str]]),
             ("entry_data", PublicAttr[MetadataValue]),
         ],
     ),
     Generic[T_MetadataValue],
 ):
-    """The standard structure for describing metadata for Dagster events.
+    """A structure for describing metadata for Dagster events.
+
+    .. note:: This class is no longer usable in any Dagster API, and will be completely removed in 2.0.
 
     Lists of objects of this type can be passed as arguments to Dagster events and will be displayed
     in Dagit and other tooling.
 
     Should be yielded from within an IO manager to append metadata for a given input/output event.
     For other event types, passing a dict with `MetadataValue` values to the `metadata` argument
     is preferred.
@@ -1015,19 +1000,21 @@
     def __new__(
         cls,
         label: str,
         description: Optional[str] = None,
         entry_data: Optional["RawMetadataValue"] = None,
         value: Optional["RawMetadataValue"] = None,
     ):
-        if description is not None:
-            deprecation_warning(
-                'The "description" attribute on "MetadataEntry"',
-                "1.0.0",
-            )
+        deprecation_warning(
+            (
+                "The `MetadataEntry` class is deprecated. Please use a dict with `MetadataValue`"
+                " values instead."
+            ),
+            "2.0.0",
+        )
         value = cast(
             RawMetadataValue,
             canonicalize_backcompat_args(
                 new_val=value,
                 new_arg="value",
                 old_val=entry_data,
                 old_arg="entry_data",
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.0/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/mode.py` & `dagster-1.3.0/dagster/_core/definitions/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.0/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,43 +15,46 @@
     Set,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import experimental, public
-from dagster._core.decorator_utils import has_at_least_one_parameter
 from dagster._core.definitions.asset_selection import AssetSelection
 from dagster._core.definitions.assets import AssetsDefinition
 from dagster._core.definitions.partition import PartitionsDefinition
+from dagster._core.definitions.resource_annotation import get_resource_args
+from dagster._core.definitions.resource_definition import ResourceDefinition
+from dagster._core.definitions.scoped_resources_builder import ScopedResourcesBuilder
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
 )
 from dagster._core.instance import DagsterInstance
 from dagster._core.instance.ref import InstanceRef
 from dagster._utils import normalize_to_repository
 
-from ..decorator_utils import get_function_params
 from .events import AssetKey
 from .run_request import RunRequest, SensorResult, SkipReason
 from .sensor_definition import (
     DefaultSensorStatus,
     SensorDefinition,
     SensorEvaluationContext,
     SensorType,
+    get_context_param_name,
+    get_sensor_context_from_args_or_kwargs,
+    validate_and_get_resource_dict,
 )
 from .target import ExecutableDefinition
 from .utils import check_valid_name
 
 if TYPE_CHECKING:
     from dagster._core.definitions.definitions_class import Definitions
     from dagster._core.definitions.repository_definition import RepositoryDefinition
-    from dagster._core.events.log import EventLogEntry
     from dagster._core.storage.event_log.base import EventLogRecord
 
 MAX_NUM_UNCONSUMED_EVENTS = 25
 
 
 class MultiAssetSensorAssetCursorComponent(
     NamedTuple(
@@ -218,14 +221,15 @@
         last_completion_time: Optional[float],
         last_run_key: Optional[str],
         cursor: Optional[str],
         repository_name: Optional[str],
         repository_def: Optional["RepositoryDefinition"],
         monitored_assets: Union[Sequence[AssetKey], AssetSelection],
         instance: Optional[DagsterInstance] = None,
+        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
         definitions: Optional["Definitions"] = None,
     ):
         from dagster._core.definitions.definitions_class import Definitions
         from dagster._core.definitions.repository_definition import RepositoryDefinition
         from dagster._core.storage.event_log.base import EventLogRecord
 
         self._repository_def = normalize_to_repository(
@@ -266,14 +270,15 @@
             instance_ref=instance_ref,
             last_completion_time=last_completion_time,
             last_run_key=last_run_key,
             cursor=cursor,
             repository_name=repository_name,
             instance=instance,
             repository_def=repository_def,
+            resources=resource_defs,
         )
 
     def _cache_initial_unconsumed_events(self) -> None:
         from dagster._core.events import DagsterEventType
         from dagster._core.storage.event_log.base import EventRecordsFilter
 
         # This method caches the initial unconsumed events for each asset key. To generate the
@@ -374,53 +379,53 @@
                 not specified, the latest materialization will be fetched for all assets the
                 multi_asset_sensor monitors.
 
         Returns: Mapping of AssetKey to EventLogRecord where the EventLogRecord is the latest
             materialization event for the asset. If there is no materialization event for the asset,
             the value in the mapping will be None.
         """
-        from dagster._core.events import DagsterEventType
-        from dagster._core.storage.event_log.base import EventRecordsFilter
+        from dagster._core.storage.event_log.base import EventLogRecord
 
         # Do not evaluate unconsumed events, only events newer than the cursor
         # if there are no new events after the cursor, the cursor points to the most
         # recent event.
 
         if asset_keys is None:
             asset_keys = self._monitored_asset_keys
         else:
             asset_keys = check.opt_sequence_param(asset_keys, "asset_keys", of_type=AssetKey)
 
-        asset_event_records = {}
-        for a in asset_keys:
-            event_records = self.instance.get_event_records(
-                EventRecordsFilter(
-                    event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                    asset_key=a,
-                    after_cursor=self._get_cursor(a).latest_consumed_event_id,
-                ),
-                ascending=False,
-                limit=1,
-            )
+        asset_records = self.instance.get_asset_records(asset_keys)
 
-            asset_event_records[a] = next(iter(event_records), None)
+        asset_event_records: Dict[AssetKey, Optional[EventLogRecord]] = {
+            asset_key: None for asset_key in asset_keys
+        }
+        for record in asset_records:
+            if (
+                record.asset_entry.last_materialization_record
+                and record.asset_entry.last_materialization_record.storage_id
+                > (self._get_cursor(record.asset_entry.asset_key).latest_consumed_event_id or 0)
+            ):
+                asset_event_records[
+                    record.asset_entry.asset_key
+                ] = record.asset_entry.last_materialization_record
 
         return asset_event_records
 
     @public
     def materialization_records_for_key(
-        self, asset_key: AssetKey, limit: int
+        self, asset_key: AssetKey, limit: Optional[int] = None
     ) -> Iterable["EventLogRecord"]:
         """Fetches asset materialization event records for asset_key, with the earliest event first.
 
         Only fetches events after the latest consumed event ID for the given asset key.
 
         Args:
             asset_key (AssetKey): The asset to fetch materialization events for
-            limit (int): The number of events to fetch
+            limit (Optional[int]): The number of events to fetch
         """
         from dagster._core.events import DagsterEventType
         from dagster._core.storage.event_log.base import EventRecordsFilter
 
         asset_key = check.inst_param(asset_key, "asset_key", AssetKey)
         if asset_key not in self._assets_by_key:
             raise DagsterInvalidInvocationError(f"Asset key {asset_key} not monitored by sensor.")
@@ -931,14 +936,15 @@
     *,
     monitored_assets: Union[Sequence[AssetKey], AssetSelection],
     repository_def: Optional["RepositoryDefinition"] = None,
     instance: Optional[DagsterInstance] = None,
     cursor: Optional[str] = None,
     repository_name: Optional[str] = None,
     cursor_from_latest_materializations: bool = False,
+    resources: Optional[Mapping[str, object]] = None,
     definitions: Optional["Definitions"] = None,
 ) -> MultiAssetSensorEvaluationContext:
     """Builds multi asset sensor execution context for testing purposes using the provided parameters.
 
     This function can be used to provide a context to the invocation of a multi asset sensor definition. If
     provided, the dagster instance must be persistent; DagsterInstance.ephemeral() will result in an
     error.
@@ -951,14 +957,16 @@
             the sensor is defined in. Must provide `definitions` if this is not provided.
         instance (Optional[DagsterInstance]): The dagster instance configured to run the sensor.
         cursor (Optional[str]): A string cursor to provide to the evaluation of the sensor. Must be
             a dictionary of asset key strings to ints that has been converted to a json string
         repository_name (Optional[str]): The name of the repository that the sensor belongs to.
         cursor_from_latest_materializations (bool): If True, the cursor will be set to the latest
             materialization for each monitored asset. By default, set to False.
+        resources (Optional[Mapping[str, object]]): The resource definitions
+            to provide to the sensor.
         definitions (Optional[Definitions]): `Definitions` object that the sensor is defined in.
             Must provide `repository_def` if this is not provided.
 
     Examples:
         .. code-block:: python
 
             with instance_for_test() as instance:
@@ -967,14 +975,15 @@
                     instance=instance,
                 )
                 my_asset_sensor(context)
 
     """
     from dagster._core.definitions import RepositoryDefinition
     from dagster._core.definitions.definitions_class import Definitions
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
 
     check.opt_inst_param(instance, "instance", DagsterInstance)
     check.opt_str_param(cursor, "cursor")
     check.opt_str_param(repository_name, "repository_name")
     repository_def = normalize_to_repository(
         check.opt_inst_param(definitions, "definitions", Definitions),
         check.opt_inst_param(repository_def, "repository_def", RepositoryDefinition),
@@ -1013,32 +1022,33 @@
         last_completion_time=None,
         last_run_key=None,
         cursor=cursor,
         repository_name=repository_name,
         instance=instance,
         monitored_assets=monitored_assets,
         repository_def=repository_def,
+        resource_defs=wrap_resources_for_execution(resources),
     )
 
 
 AssetMaterializationFunctionReturn = Union[
     Iterator[Union[RunRequest, SkipReason, SensorResult]],
     Sequence[RunRequest],
     RunRequest,
     SkipReason,
     None,
     SensorResult,
 ]
 AssetMaterializationFunction = Callable[
-    ["SensorEvaluationContext", "EventLogEntry"],
+    ...,
     AssetMaterializationFunctionReturn,
 ]
 
 MultiAssetMaterializationFunction = Callable[
-    ["MultiAssetSensorEvaluationContext"],
+    ...,
     AssetMaterializationFunctionReturn,
 ]
 
 
 @experimental
 class MultiAssetSensorDefinition(SensorDefinition):
     """Define an asset sensor that initiates a set of runs based on the materialization of a list of
@@ -1078,36 +1088,59 @@
         asset_materialization_fn: MultiAssetMaterializationFunction,
         minimum_interval_seconds: Optional[int] = None,
         description: Optional[str] = None,
         job: Optional[ExecutableDefinition] = None,
         jobs: Optional[Sequence[ExecutableDefinition]] = None,
         default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
         request_assets: Optional[AssetSelection] = None,
+        required_resource_keys: Optional[Set[str]] = None,
     ):
+        resource_arg_names: Set[str] = {
+            arg.name for arg in get_resource_args(asset_materialization_fn)
+        }
+
+        combined_required_resource_keys = (
+            check.opt_set_param(required_resource_keys, "required_resource_keys", of_type=str)
+            | resource_arg_names
+        )
+
         def _wrap_asset_fn(materialization_fn):
             def _fn(context):
                 def _check_cursor_not_set(sensor_result: SensorResult):
                     if sensor_result.cursor:
                         raise DagsterInvariantViolationError(
                             "Cannot set cursor in a multi_asset_sensor. Cursor is set automatically"
                             " based on the latest materialization for each monitored asset."
                         )
 
-                multi_asset_sensor_context = MultiAssetSensorEvaluationContext(
+                resource_args_populated = validate_and_get_resource_dict(
+                    context.resources, name, resource_arg_names
+                )
+
+                with MultiAssetSensorEvaluationContext(
                     instance_ref=context.instance_ref,
                     last_completion_time=context.last_completion_time,
                     last_run_key=context.last_run_key,
                     cursor=context.cursor,
                     repository_name=context.repository_def.name,
                     repository_def=context.repository_def,
                     monitored_assets=monitored_assets,
                     instance=context.instance,
-                )
-
-                result = materialization_fn(multi_asset_sensor_context)
+                    resource_defs=context.resource_defs,
+                ) as multi_asset_sensor_context:
+                    context_param_name = get_context_param_name(materialization_fn)
+                    context_param = (
+                        {context_param_name: multi_asset_sensor_context}
+                        if context_param_name
+                        else {}
+                    )
+                    result = materialization_fn(
+                        **context_param,
+                        **resource_args_populated,
+                    )
                 if result is None:
                     return
 
                 # because the materialization_fn can yield results (see _wrapped_fn in multi_asset_sensor decorator),
                 # even if you return None in a sensor, it will still cause in inspect.isgenerator(result) to be True.
                 # So keep track to see if we actually return any values and should update the cursor
                 runs_yielded = False
@@ -1156,56 +1189,35 @@
             ),
             minimum_interval_seconds=minimum_interval_seconds,
             description=description,
             job=job,
             jobs=jobs,
             default_status=default_status,
             asset_selection=request_assets,
+            required_resource_keys=combined_required_resource_keys,
         )
 
-    def __call__(self, *args, **kwargs):
-        if has_at_least_one_parameter(self._raw_asset_materialization_fn):
-            if len(args) + len(kwargs) == 0:
-                raise DagsterInvalidInvocationError(
-                    "Sensor evaluation function expected context argument, but no context argument "
-                    "was provided when invoking."
-                )
-            if len(args) + len(kwargs) > 1:
-                raise DagsterInvalidInvocationError(
-                    "Sensor invocation received multiple arguments. Only a first "
-                    "positional context parameter should be provided when invoking."
-                )
-
-            context_param_name = get_function_params(self._raw_asset_materialization_fn)[0].name
-
-            if args:
-                context = check.inst_param(
-                    args[0], context_param_name, MultiAssetSensorEvaluationContext
-                )
-            else:
-                if context_param_name not in kwargs:
-                    raise DagsterInvalidInvocationError(
-                        f"Sensor invocation expected argument '{context_param_name}'."
-                    )
-                context = check.inst_param(
-                    kwargs[context_param_name],
-                    context_param_name,
-                    MultiAssetSensorEvaluationContext,
-                )
-
-            result = self._raw_asset_materialization_fn(context)
+    def __call__(self, *args, **kwargs) -> AssetMaterializationFunctionReturn:
+        context_param_name = get_context_param_name(self._raw_asset_materialization_fn)
+        context = get_sensor_context_from_args_or_kwargs(
+            self._raw_asset_materialization_fn,
+            args,
+            kwargs,
+            context_type=MultiAssetSensorEvaluationContext,
+        )
 
-        else:
-            if len(args) + len(kwargs) > 0:
-                raise DagsterInvalidInvocationError(
-                    "Sensor decorated function has no arguments, but arguments were provided to "
-                    "invocation."
-                )
+        resources = validate_and_get_resource_dict(
+            context.resources if context else ScopedResourcesBuilder.build_empty(),
+            self._name,
+            self._required_resource_keys,
+        )
 
-            result = self._raw_asset_materialization_fn()
+        context_param = {context_param_name: context} if context_param_name and context else {}
+        result = self._raw_asset_materialization_fn(**context_param, **resources)
 
-        context.update_cursor_after_evaluation()
+        if context:
+            context.update_cursor_after_evaluation()
         return result
 
     @property
     def sensor_type(self) -> SensorType:
         return SensorType.MULTI_ASSET
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.0/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import itertools
 from datetime import datetime
 from functools import reduce
 from typing import (
     Dict,
     Iterable,
     List,
@@ -210,14 +211,28 @@
             key=lambda x: x.name,
         )
 
     @property
     def partitions_subset_class(self) -> Type["PartitionsSubset"]:
         return MultiPartitionsSubset
 
+    def get_serializable_unique_identifier(
+        self, dynamic_partitions_store: Optional[DynamicPartitionsStore] = None
+    ) -> str:
+        return hashlib.sha1(
+            str(
+                {
+                    dim_def.name: dim_def.partitions_def.get_serializable_unique_identifier(
+                        dynamic_partitions_store
+                    )
+                    for dim_def in self.partitions_defs
+                }
+            ).encode("utf-8")
+        ).hexdigest()
+
     @property
     def partition_dimension_names(self) -> List[str]:
         return [dim_def.name for dim_def in self._partitions_defs]
 
     @property
     def partitions_defs(self) -> Sequence[PartitionDimensionDefinition]:
         return self._partitions_defs
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/node_container.py` & `dagster-1.3.0/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/node_definition.py` & `dagster-1.3.0/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/observe.py` & `dagster-1.3.0/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/op_definition.py` & `dagster-1.3.0/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.0/dagster/_core/definitions/op_invocation.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,63 +35,70 @@
     from .decorators.op_decorator import DecoratedOpFunction
     from .op_definition import OpDefinition
     from .output import OutputDefinition
 
 T = TypeVar("T")
 
 
-class InputsAndResources(NamedTuple):
+class SeparatedArgsKwargs(NamedTuple):
     input_args: Tuple[Any, ...]
     input_kwargs: Dict[str, Any]
     resources_by_param_name: Dict[str, Any]
+    config_arg: Any
 
 
 def _separate_args_and_kwargs(
     compute_fn: "DecoratedOpFunction",
     args: Tuple[Any, ...],
     kwargs: Dict[str, Any],
     resource_arg_mapping: Dict[str, Any],
-) -> InputsAndResources:
+) -> SeparatedArgsKwargs:
     """Given a decorated compute function, a set of args and kwargs, and set of resource param names,
     separates the set of resource inputs from op/asset inputs returns a tuple of the categorized
     args and kwargs.
 
     We use the remaining args and kwargs to cleanly invoke the compute function, and we use the
     extracted resource inputs to populate the execution context.
     """
-    resource_inputs_from_args_and_kwargs = {}
+    resources_from_args_and_kwargs = {}
     params = get_function_params(compute_fn.decorated_fn)
 
     adjusted_args = []
 
     params_without_context = params[1:] if compute_fn.has_context_arg() else params
 
+    config_arg = kwargs.get("config")
+
     # Get any (non-kw) args that correspond to resource inputs & strip them from the args list
     for i, arg in enumerate(args):
         param = params_without_context[i] if i < len(params_without_context) else None
         if param and param.kind != inspect.Parameter.KEYWORD_ONLY:
             if param.name in resource_arg_mapping:
-                resource_inputs_from_args_and_kwargs[param.name] = arg
+                resources_from_args_and_kwargs[param.name] = arg
+                continue
+            if param.name == "config":
+                config_arg = arg
                 continue
 
         adjusted_args.append(arg)
 
     # Get any kwargs that correspond to resource inputs & strip them from the kwargs dict
     for resource_arg in resource_arg_mapping:
         if resource_arg in kwargs:
-            resource_inputs_from_args_and_kwargs[resource_arg] = kwargs[resource_arg]
+            resources_from_args_and_kwargs[resource_arg] = kwargs[resource_arg]
 
     adjusted_kwargs = {
-        k: v for k, v in kwargs.items() if k not in resource_inputs_from_args_and_kwargs
+        k: v for k, v in kwargs.items() if k not in resources_from_args_and_kwargs and k != "config"
     }
 
-    return InputsAndResources(
+    return SeparatedArgsKwargs(
         input_args=tuple(adjusted_args),
         input_kwargs=adjusted_kwargs,
-        resources_by_param_name=resource_inputs_from_args_and_kwargs,
+        resources_by_param_name=resources_from_args_and_kwargs,
+        config_arg=config_arg,
     )
 
 
 def op_invocation_result(
     op_def_or_invocation: Union["OpDefinition", "PendingNodeInvocation[OpDefinition]"],
     context: Optional["UnboundOpExecutionContext"],
     *args,
@@ -104,26 +111,22 @@
 
     op_def = (
         op_def_or_invocation.node_def
         if isinstance(op_def_or_invocation, PendingNodeInvocation)
         else op_def_or_invocation
     )
 
-    _check_invocation_requirements(op_def, context)
-
     compute_fn = op_def.compute_fn
     if not isinstance(compute_fn, DecoratedOpFunction):
         check.failed("op invocation only works with decorated op fns")
 
     compute_fn = cast(DecoratedOpFunction, compute_fn)
 
     from ..execution.plan.compute_generator import invoke_compute_fn
 
-    context = context or build_op_context()
-
     resource_arg_mapping = {arg.name: arg.name for arg in compute_fn.get_resource_args()}
 
     # The user is allowed to invoke an op with an arbitrary mix of args and kwargs.
     # We ensure that these args and kwargs are correctly categorized as inputs, config, or resource objects and then validated.
     #
     # Depending on arg/kwarg type, we do various things:
     # - Any resources passed as parameters are also made available to user-defined code as part of the op execution context
@@ -133,23 +136,40 @@
     #
     # We recollect all the varying args/kwargs into a dictionary and invoke the user-defined function with kwargs only.
     extracted = _separate_args_and_kwargs(compute_fn, args, kwargs, resource_arg_mapping)
 
     input_args = extracted.input_args
     input_kwargs = extracted.input_kwargs
     resources_by_param_name = extracted.resources_by_param_name
+    config_input = extracted.config_arg
 
-    resources_provided_in_multiple_places = resources_by_param_name and context.resource_keys
+    resources_provided_in_multiple_places = (
+        resources_by_param_name and context and context.resource_keys
+    )
     if resources_provided_in_multiple_places:
         raise DagsterInvalidInvocationError("Cannot provide resources in both context and kwargs")
 
     if resources_by_param_name:
-        context = context.replace_resources(resources_by_param_name)
+        context = (context or build_op_context()).replace_resources(resources_by_param_name)
+
+    config_provided_in_multiple_places = config_input and context and context.op_config
+    if config_provided_in_multiple_places:
+        raise DagsterInvalidInvocationError("Cannot provide config in both context and kwargs")
+    if config_input:
+        from dagster._config.pythonic_config import Config
+
+        context = (context or build_op_context()).replace_config(
+            config_input._as_config_dict()  # noqa: SLF001
+            if isinstance(config_input, Config)
+            else config_input
+        )
+
+    _check_invocation_requirements(op_def, context)
 
-    bound_context = context.bind(op_def_or_invocation)
+    bound_context = (context or build_op_context()).bind(op_def_or_invocation)
 
     input_dict = _resolve_inputs(op_def, input_args, input_kwargs, bound_context)
 
     result = invoke_compute_fn(
         fn=compute_fn.decorated_fn,
         context=bound_context,
         kwargs=input_dict,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/output.py` & `dagster-1.3.0/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/partition.py` & `dagster-1.3.0/dagster/_core/definitions/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,17 +603,18 @@
     Examples:
         .. code-block:: python
 
             fruits = DynamicPartitionsDefinition(name="fruits")
 
             @sensor(job=my_job)
             def my_sensor(context):
-                context.instance.add_dynamic_partitions(fruits.name, [partition_key])
-                return RunRequest(partition_key=partition_key)
-
+                return SensorResult(
+                    run_requests=[RunRequest(partition_key="apple")],
+                    dynamic_partitions_requests=[fruits.build_add_request(["apple"])]
+                )
     """
 
     def __new__(
         cls,
         partition_fn: Optional[
             Callable[[Optional[datetime]], Union[Sequence[Partition], Sequence[str]]]
         ] = None,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.0/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.0/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/pipeline_base.py` & `dagster-1.3.0/dagster/_core/definitions/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/pipeline_definition.py` & `dagster-1.3.0/dagster/_core/definitions/pipeline_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/policy.py` & `dagster-1.3.0/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/preset.py` & `dagster-1.3.0/dagster/_core/definitions/preset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.0/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.0/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.0/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     Sequence,
     Set,
     Union,
     cast,
 )
 
 import dagster._check as check
-from dagster._config.structured_config import (
-    ConfigurableResource,
-    PartialResource,
+from dagster._config.pythonic_config import (
+    ConfigurableIOManagerFactoryResourceDefinition,
+    ConfigurableResourceFactoryResourceDefinition,
     ResourceWithKeyMapping,
-    separate_resource_params,
+    coerce_to_resource,
 )
 from dagster._core.definitions.asset_graph import AssetGraph
 from dagster._core.definitions.assets_job import (
     get_base_asset_jobs,
     is_base_asset_job_name,
 )
 from dagster._core.definitions.events import AssetKey
@@ -74,19 +74,25 @@
         if resource_def.config_schema.default_provided
         else {},
     )
 
     env_vars = _find_env_vars(config_schema_default)
 
     if isinstance(resource_def, ResourceWithKeyMapping) and isinstance(
-        resource_def.inner_resource, (ConfigurableResource, PartialResource)
+        resource_def.inner_resource,
+        (
+            ConfigurableIOManagerFactoryResourceDefinition,
+            ConfigurableResourceFactoryResourceDefinition,
+        ),
     ):
-        nested_resources = separate_resource_params(resource_def.inner_resource.__dict__).resources
+        nested_resources = resource_def.inner_resource.nested_resources
         for nested_resource in nested_resources.values():
-            env_vars = env_vars.union(_env_vars_from_resource_defaults(nested_resource))
+            env_vars = env_vars.union(
+                _env_vars_from_resource_defaults(coerce_to_resource(nested_resource))
+            )
 
     return env_vars
 
 
 def build_caching_repository_data_from_list(
     repository_definitions: Sequence[RepositoryListDefinition],
     default_executor_def: Optional[ExecutorDefinition] = None,
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.0/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.0/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.0/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.0/dagster/_core/definitions/resource_annotation.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,18 +11,20 @@
     return [param for param in get_function_params(fn) if _is_resource_annotated(param)]
 
 
 RESOURCE_PARAM_METADATA = "resource_param"
 
 
 def _is_resource_annotated(param: Parameter) -> bool:
+    from dagster._config.pythonic_config import ConfigurableResourceFactory
+
     extends_resource_definition = False
     try:
         extends_resource_definition = isinstance(param.annotation, type) and issubclass(
-            param.annotation, ResourceDefinition
+            param.annotation, (ResourceDefinition, ConfigurableResourceFactory)
         )
     except TypeError:
         # Using builtin Python types in python 3.9+ will raise a TypeError when using issubclass
         # even though the isinstance check will succeed (as will inspect.isclass), for example
         # list[dict[str, str]] will raise a TypeError
         pass
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.0/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.0/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.0/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/run_config.py` & `dagster-1.3.0/dagster/_core/definitions/run_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,23 @@
     TypeVar,
     Union,
     cast,
 )
 
 from typing_extensions import TypeAlias
 
-from dagster._annotations import experimental
 from dagster._config import (
     ALL_CONFIG_BUILTINS,
     ConfigType,
     Field,
     Permissive,
     Selector,
     Shape,
 )
-from dagster._config.structured_config import Config
+from dagster._config.pythonic_config import Config, config_dictionary_from_values
 from dagster._core.definitions.asset_layer import AssetLayer
 from dagster._core.definitions.executor_definition import (
     ExecutorDefinition,
     execute_in_process_executor,
     in_process_executor,
 )
 from dagster._core.definitions.input import InputDefinition
@@ -649,36 +648,46 @@
         type_dict_by_key[config_type.key] = config_type
 
     return type_dict_by_name, type_dict_by_key
 
 
 def _convert_config_classes(configs: Dict[str, Any]) -> Dict[str, Any]:
     return {
-        k: {"config": v._as_config_dict() if isinstance(v, Config) else v}  # noqa: SLF001
+        k: {
+            "config": config_dictionary_from_values(
+                v._as_config_dict(), v.to_config_schema().as_field()  # noqa: SLF001
+            )
+            if isinstance(v, Config)
+            else v
+        }
         for k, v in configs.items()
     }
 
 
-@experimental
 class RunConfig:
+    """RunConfig is a container for all the configuration that can be passed to a pipeline run."""
+
     def __init__(
         self,
         ops: Optional[Dict[str, Any]] = None,
         resources: Optional[Dict[str, Any]] = None,
         loggers: Optional[Dict[str, Any]] = None,
+        execution: Optional[Dict[str, Any]] = None,
     ):
         self.ops = check.opt_dict_param(ops, "ops")
         self.resources = check.opt_dict_param(resources, "resources")
         self.loggers = check.opt_dict_param(loggers, "loggers")
+        self.execution = check.opt_dict_param(execution, "execution")
 
     def to_config_dict(self):
         return {
             "loggers": self.loggers,
             "resources": _convert_config_classes(self.resources),
             "ops": _convert_config_classes(self.ops),
+            "execution": self.execution,
         }
 
 
 CoercibleToRunConfig: TypeAlias = Union[Dict[str, Any], RunConfig]
 
 T = TypeVar("T")
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.0/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/run_request.py` & `dagster-1.3.0/dagster/_core/definitions/run_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus
 from dagster._core.storage.tags import PARTITION_NAME_TAG
 from dagster._serdes.serdes import whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo
 
 if TYPE_CHECKING:
     from dagster._core.definitions.job_definition import JobDefinition
+    from dagster._core.definitions.run_config import RunConfig
     from dagster._core.definitions.unresolved_asset_job_definition import (
         UnresolvedAssetJobDefinition,
     )
 
 
 @whitelist_for_serdes(old_storage_names={"JobType"})
 class InstigatorType(Enum):
@@ -128,25 +129,29 @@
             job will be materialized. If the job does not materialize assets, this flag is ignored.
         partition_key (Optional[str]): The partition key for this run request.
     """
 
     def __new__(
         cls,
         run_key: Optional[str] = None,
-        run_config: Optional[Mapping[str, Any]] = None,
+        run_config: Optional[Union["RunConfig", Mapping[str, Any]]] = None,
         tags: Optional[Mapping[str, str]] = None,
         job_name: Optional[str] = None,
         asset_selection: Optional[Sequence[AssetKey]] = None,
         stale_assets_only: bool = False,
         partition_key: Optional[str] = None,
     ):
+        from dagster._core.definitions.run_config import convert_config_input
+
         return super(RunRequest, cls).__new__(
             cls,
             run_key=check.opt_str_param(run_key, "run_key"),
-            run_config=check.opt_mapping_param(run_config, "run_config", key_type=str),
+            run_config=check.opt_mapping_param(
+                convert_config_input(run_config), "run_config", key_type=str
+            ),
             tags=check.opt_mapping_param(tags, "tags", key_type=str, value_type=str),
             job_name=check.opt_str_param(job_name, "job_name"),
             asset_selection=check.opt_nullable_sequence_param(
                 asset_selection, "asset_selection", of_type=AssetKey
             ),
             stale_assets_only=check.bool_param(stale_assets_only, "stale_assets_only"),
             partition_key=check.opt_str_param(partition_key, "partition_key"),
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.0/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import logging
 import warnings
+from contextlib import ExitStack
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Callable,
     Iterator,
+    Mapping,
     NamedTuple,
     Optional,
     Sequence,
+    Set,
     Union,
     cast,
     overload,
 )
 
 import pendulum
 from typing_extensions import TypeAlias
 
 import dagster._check as check
 from dagster._annotations import public
-from dagster._core.decorator_utils import has_at_least_one_parameter
 from dagster._core.definitions.instigation_logger import InstigationLogger
+from dagster._core.definitions.resource_annotation import get_resource_args
+from dagster._core.definitions.scoped_resources_builder import Resources, ScopedResourcesBuilder
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
-    DagsterInvalidInvocationError,
     DagsterInvariantViolationError,
     RunStatusSensorExecutionError,
     user_code_error_boundary,
 )
 from dagster._core.events import PIPELINE_RUN_STATUS_TO_EVENT_TYPE, DagsterEvent
 from dagster._core.instance import DagsterInstance
 from dagster._core.storage.pipeline_run import DagsterRun, DagsterRunStatus, RunsFilter
@@ -37,45 +40,48 @@
 from dagster._serdes.errors import DeserializationError
 from dagster._serdes.serdes import deserialize_value
 from dagster._seven import JSONDecodeError
 from dagster._utils import utc_datetime_from_timestamp
 from dagster._utils.backcompat import deprecation_warning
 from dagster._utils.error import serializable_error_info_from_exc_info
 
-from ..decorator_utils import get_function_params
 from .graph_definition import GraphDefinition
 from .pipeline_definition import PipelineDefinition
 from .sensor_definition import (
     DefaultSensorStatus,
     PipelineRunReaction,
     RawSensorEvaluationFunctionReturn,
     RunRequest,
     SensorDefinition,
     SensorEvaluationContext,
     SensorResult,
     SensorType,
     SkipReason,
+    get_context_param_name,
+    get_sensor_context_from_args_or_kwargs,
+    validate_and_get_resource_dict,
 )
 from .target import ExecutableDefinition
 from .unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 
 if TYPE_CHECKING:
+    from dagster._core.definitions.resource_definition import ResourceDefinition
     from dagster._core.definitions.selector import (
         CodeLocationSelector,
         JobSelector,
         RepositorySelector,
     )
 
 RunStatusSensorEvaluationFunction: TypeAlias = Union[
-    Callable[[], RawSensorEvaluationFunctionReturn],
-    Callable[["RunStatusSensorContext"], RawSensorEvaluationFunctionReturn],
+    Callable[..., RawSensorEvaluationFunctionReturn],
+    Callable[..., RawSensorEvaluationFunctionReturn],
 ]
 RunFailureSensorEvaluationFn: TypeAlias = Union[
-    Callable[[], RawSensorEvaluationFunctionReturn],
-    Callable[["RunFailureSensorContext"], RawSensorEvaluationFunctionReturn],
+    Callable[..., RawSensorEvaluationFunctionReturn],
+    Callable[..., RawSensorEvaluationFunctionReturn],
 ]
 
 
 @whitelist_for_serdes(old_storage_names={"PipelineSensorCursor"})
 class RunStatusSensorCursor(
     NamedTuple(
         "_RunStatusSensorCursor",
@@ -112,32 +118,91 @@
         sensor_name (str): the name of the sensor.
         dagster_run (DagsterRun): the run of the job or pipeline.
         dagster_event (DagsterEvent): the event associated with the job or pipeline run status.
         instance (DagsterInstance): the current instance.
         log (logging.Logger): the logger for the given sensor evaluation
     """
 
-    def __init__(self, sensor_name, dagster_run, dagster_event, instance, context=None):
+    def __init__(
+        self,
+        sensor_name,
+        dagster_run,
+        dagster_event,
+        instance,
+        context: Optional[
+            SensorEvaluationContext
+        ] = None,  # deprecated arg, but we need to keep it for backcompat
+        resource_defs: Optional[Mapping[str, "ResourceDefinition"]] = None,
+        logger: Optional[logging.Logger] = None,
+    ) -> None:
+        self._exit_stack = ExitStack()
         self._sensor_name = check.str_param(sensor_name, "sensor_name")
         self._dagster_run = check.inst_param(dagster_run, "dagster_run", DagsterRun)
         self._dagster_event = check.inst_param(dagster_event, "dagster_event", DagsterEvent)
         self._instance = check.inst_param(instance, "instance", DagsterInstance)
-        self._context = check.opt_inst_param(context, "context", SensorEvaluationContext)
-        self._logger: Optional[logging.Logger] = None
+        self._logger: Optional[logging.Logger] = logger or (context.log if context else None)
+
+        # Wait to set resources unless they're accessed
+        self._resource_defs = resource_defs
+        self._resources = None
+        self._cm_scope_entered = False
 
-    def for_run_failure(self):
+    def for_run_failure(self) -> "RunFailureSensorContext":
         """Converts RunStatusSensorContext to RunFailureSensorContext."""
         return RunFailureSensorContext(
             sensor_name=self._sensor_name,
             dagster_run=self._dagster_run,
             dagster_event=self._dagster_event,
             instance=self._instance,
-            context=self._context,
+            logger=self._logger,
         )
 
+    @property
+    def resource_defs(self) -> Optional[Mapping[str, "ResourceDefinition"]]:
+        return self._resource_defs
+
+    @property
+    def resources(self) -> Resources:
+        from dagster._core.definitions.scoped_resources_builder import (
+            IContainsGenerator,
+        )
+        from dagster._core.execution.build_resources import build_resources
+
+        if not self._resources:
+            """
+            This is similar to what we do in e.g. the op context - we set up a resource
+            building context manager, and immediately enter it. This is so that in cases
+            where a user is not using any context-manager based resources, they don't
+            need to enter this SensorEvaluationContext themselves.
+
+            For example:
+
+            my_sensor(build_sensor_context(resources={"my_resource": my_non_cm_resource})
+
+            will work ok, but for a CM resource we must do
+
+            with build_sensor_context(resources={"my_resource": my_cm_resource}) as context:
+                my_sensor(context)
+            """
+
+            instance = self.instance if self._instance else None
+
+            resources_cm = build_resources(resources=self._resource_defs or {}, instance=instance)
+            self._resources = self._exit_stack.enter_context(resources_cm)
+
+            if isinstance(self._resources, IContainsGenerator) and not self._cm_scope_entered:
+                self._exit_stack.close()
+                raise DagsterInvariantViolationError(
+                    "At least one provided resource is a generator, but attempting to access"
+                    " resources outside of context manager scope. You can use the following syntax"
+                    " to open a context manager: `with build_schedule_context(...) as context:`"
+                )
+
+        return self._resources
+
     @public
     @property
     def sensor_name(self) -> str:
         return self._sensor_name
 
     @public
     @property
@@ -153,30 +218,35 @@
     @property
     def instance(self) -> DagsterInstance:
         return self._instance
 
     @public
     @property
     def log(self) -> logging.Logger:
-        if self._context:
-            return self._context.log
-
         if not self._logger:
             self._logger = InstigationLogger()
 
         return self._logger
 
     @property
     def pipeline_run(self) -> DagsterRun:
         warnings.warn(
             "`RunStatusSensorContext.pipeline_run` is deprecated as of 0.13.0; use "
             "`RunStatusSensorContext.dagster_run` instead."
         )
         return self.dagster_run
 
+    def __enter__(self) -> "RunStatusSensorContext":
+        self._cm_scope_entered = True
+        return self
+
+    def __exit__(self, *exc) -> None:
+        self._exit_stack.close()
+        self._logger = None
+
 
 class RunFailureSensorContext(RunStatusSensorContext):
     """The ``context`` object available to a decorated function of ``run_failure_sensor``.
 
     Attributes:
         sensor_name (str): the name of the sensor.
         dagster_run (DagsterRun): the failed pipeline run.
@@ -190,26 +260,29 @@
 
 def build_run_status_sensor_context(
     sensor_name: str,
     dagster_event: DagsterEvent,
     dagster_instance: DagsterInstance,
     dagster_run: DagsterRun,
     context: Optional[SensorEvaluationContext] = None,
+    resources: Optional[Mapping[str, object]] = None,
 ) -> RunStatusSensorContext:
     """Builds run status sensor context from provided parameters.
 
     This function can be used to provide the context argument when directly invoking a function
     decorated with `@run_status_sensor` or `@run_failure_sensor`, such as when writing unit tests.
 
     Args:
         sensor_name (str): The name of the sensor the context is being constructed for.
         dagster_event (DagsterEvent): A DagsterEvent with the same event type as the one that
             triggers the run_status_sensor
         dagster_instance (DagsterInstance): The dagster instance configured for the context.
         dagster_run (DagsterRun): DagsterRun object from running a job
+        resources (Optional[Mapping[str, object]]): A dictionary of resources to be made available
+            to the sensor.
 
     Examples:
         .. code-block:: python
 
             instance = DagsterInstance.ephemeral()
             result = my_job.execute_in_process(instance=instance)
 
@@ -220,20 +293,23 @@
                 sensor_name="run_status_sensor_to_invoke",
                 dagster_instance=instance,
                 dagster_run=dagster_run,
                 dagster_event=dagster_event,
             )
             run_status_sensor_to_invoke(context)
     """
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
+
     return RunStatusSensorContext(
         sensor_name=sensor_name,
         instance=dagster_instance,
         dagster_run=dagster_run,
         dagster_event=dagster_event,
-        context=context,
+        resource_defs=wrap_resources_for_execution(resources),
+        logger=context.log if context else None,
     )
 
 
 @overload
 def run_failure_sensor(
     name: RunFailureSensorEvaluationFn,
 ) -> SensorDefinition:
@@ -361,15 +437,15 @@
             monitored_jobs=jobs,
             monitor_all_repositories=monitor_all_repositories,
             default_status=default_status,
             request_job=request_job,
             request_jobs=request_jobs,
         )
         def _run_failure_sensor(context: RunStatusSensorContext):
-            return fn(context.for_run_failure())  # type: ignore  # fmt: skip
+            return fn(context.for_run_failure())  # fmt: skip
 
         return _run_failure_sensor
 
     # This case is for when decorator is used bare, without arguments
     if callable(name):
         return inner(name)
 
@@ -422,14 +498,15 @@
                 ]
             ]
         ] = None,
         monitor_all_repositories: bool = False,
         default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
         request_job: Optional[ExecutableDefinition] = None,
         request_jobs: Optional[Sequence[ExecutableDefinition]] = None,
+        required_resource_keys: Optional[Set[str]] = None,
     ):
         from dagster._core.definitions.selector import (
             CodeLocationSelector,
             JobSelector,
             RepositorySelector,
         )
         from dagster._core.event_api import RunShardedEventsCursor
@@ -450,14 +527,21 @@
                 RepositorySelector,
                 JobSelector,
                 CodeLocationSelector,
             ),
         )
         check.inst_param(default_status, "default_status", DefaultSensorStatus)
 
+        resource_arg_names: Set[str] = {arg.name for arg in get_resource_args(run_status_sensor_fn)}
+
+        combined_required_resource_keys = (
+            check.opt_set_param(required_resource_keys, "required_resource_keys", of_type=str)
+            | resource_arg_names
+        )
+
         # coerce CodeLocationSelectors to RepositorySelectors with repo name "__repository__"
         monitored_jobs = [
             job.to_repository_selector() if isinstance(job, CodeLocationSelector) else job
             for job in (monitored_jobs or [])
         ]
 
         self._run_status_sensor_fn = check.callable_param(
@@ -606,32 +690,39 @@
                             record_id=storage_id, update_timestamp=update_timestamp.isoformat()
                         ).to_json()
                     )
                     continue
 
                 serializable_error = None
 
+                resource_args_populated = validate_and_get_resource_dict(
+                    context.resources, name, resource_arg_names
+                )
+
                 try:
-                    with user_code_error_boundary(
+                    with RunStatusSensorContext(
+                        sensor_name=name,
+                        dagster_run=pipeline_run,
+                        dagster_event=event_log_entry.dagster_event,
+                        instance=context.instance,
+                        resource_defs=context.resource_defs,
+                        logger=context.log,
+                    ) as sensor_context, user_code_error_boundary(
                         RunStatusSensorExecutionError,
                         lambda: f'Error occurred during the execution sensor "{name}".',
                     ):
-                        if has_at_least_one_parameter(run_status_sensor_fn):
-                            # one user code invocation maps to one failure event
-                            sensor_return = run_status_sensor_fn(
-                                RunStatusSensorContext(
-                                    sensor_name=name,
-                                    dagster_run=pipeline_run,
-                                    dagster_event=event_log_entry.dagster_event,
-                                    instance=context.instance,
-                                    context=context,
-                                )
-                            )
-                        else:
-                            sensor_return = run_status_sensor_fn()  # type: ignore
+                        context_param_name = get_context_param_name(run_status_sensor_fn)
+                        context_param = (
+                            {context_param_name: sensor_context} if context_param_name else {}
+                        )
+
+                        sensor_return = run_status_sensor_fn(
+                            **context_param,
+                            **resource_args_populated,
+                        )
 
                         if sensor_return is not None:
                             context.update_cursor(
                                 RunStatusSensorCursor(
                                     record_id=storage_id,
                                     update_timestamp=update_timestamp.isoformat(),
                                 ).to_json()
@@ -679,57 +770,33 @@
             name=name,
             evaluation_fn=_wrapped_fn,
             minimum_interval_seconds=minimum_interval_seconds,
             description=description,
             default_status=default_status,
             job=request_job,
             jobs=request_jobs,
+            required_resource_keys=combined_required_resource_keys,
         )
 
-    def __call__(self, *args, **kwargs):
-        if has_at_least_one_parameter(self._run_status_sensor_fn):
-            if len(args) + len(kwargs) == 0:
-                raise DagsterInvalidInvocationError(
-                    "Run status sensor function expected context argument, but no context argument "
-                    "was provided when invoking."
-                )
-            if len(args) + len(kwargs) > 1:
-                raise DagsterInvalidInvocationError(
-                    "Run status sensor invocation received multiple arguments. Only a first "
-                    "positional context parameter should be provided when invoking."
-                )
-
-            context_param_name = get_function_params(self._run_status_sensor_fn)[0].name
-
-            if args:
-                context = check.opt_inst_param(args[0], context_param_name, RunStatusSensorContext)
-            else:
-                if context_param_name not in kwargs:
-                    raise DagsterInvalidInvocationError(
-                        f"Run status sensor invocation expected argument '{context_param_name}'."
-                    )
-                context = check.opt_inst_param(
-                    kwargs[context_param_name], context_param_name, RunStatusSensorContext
-                )
-
-            if not context:
-                raise DagsterInvalidInvocationError(
-                    "Context must be provided for direct invocation of run status sensor."
-                )
-
-            return self._run_status_sensor_fn(context)
-
-        else:
-            if len(args) + len(kwargs) > 0:
-                raise DagsterInvalidInvocationError(
-                    "Run status sensor decorated function has no arguments, but arguments were "
-                    "provided to invocation."
-                )
+    def __call__(self, *args, **kwargs) -> RawSensorEvaluationFunctionReturn:
+        context_param_name = get_context_param_name(self._run_status_sensor_fn)
+        context = get_sensor_context_from_args_or_kwargs(
+            self._run_status_sensor_fn,
+            args,
+            kwargs,
+            context_type=RunStatusSensorContext,
+        )
+        context_param = {context_param_name: context} if context_param_name and context else {}
 
-            return self._run_status_sensor_fn()
+        resources = validate_and_get_resource_dict(
+            context.resources if context else ScopedResourcesBuilder.build_empty(),
+            self._name,
+            self._required_resource_keys,
+        )
+        return self._run_status_sensor_fn(**context_param, **resources)
 
     @property
     def sensor_type(self) -> SensorType:
         return SensorType.RUN_STATUS
 
 
 def run_status_sensor(
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.0/dagster/_core/definitions/schedule_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,43 +90,63 @@
 ) -> "ScheduleEvaluationContext":
     """Based on the passed resource function and the arguments passed to it, returns the
     user-passed ScheduleEvaluationContext or creates one if it is not passed.
 
     Raises an exception if the user passes more than one argument or if the user-provided
     function requires a context parameter but none is passed.
     """
+    from dagster._config.pythonic_config import is_coercible_to_resource
     from dagster._core.definitions.sensor_definition import get_context_param_name
 
     context_param_name = get_context_param_name(fn)
 
-    if len(args) + len(kwargs) > 1:
+    kwarg_keys_non_resource = set(kwargs.keys()) - {param.name for param in get_resource_args(fn)}
+    if len(args) + len(kwarg_keys_non_resource) > 1:
         raise DagsterInvalidInvocationError(
-            "Schedule invocation received multiple arguments. Only a first "
-            "positional context parameter should be provided."
+            "Schedule invocation received multiple non-resource arguments. Only a first "
+            "positional context parameter should be provided when invoking."
+        )
+
+    if any(is_coercible_to_resource(arg) for arg in args):
+        raise DagsterInvalidInvocationError(
+            "If directly invoking a schedule, you may not provide resources as"
+            " positional arguments, only as keyword arguments."
         )
 
     context: Optional[ScheduleEvaluationContext] = None
 
     if len(args) > 0:
         context = check.opt_inst(args[0], ScheduleEvaluationContext)
     elif len(kwargs) > 0:
         if context_param_name and context_param_name not in kwargs:
             raise DagsterInvalidInvocationError(
                 f"Schedule invocation expected argument '{context_param_name}'."
             )
-        context_param_name = context_param_name or list(kwargs.keys())[0]
-        context = check.opt_inst(kwargs.get(context_param_name), ScheduleEvaluationContext)
+        context = check.opt_inst(
+            kwargs.get(context_param_name or "context"), ScheduleEvaluationContext
+        )
     elif context_param_name:
         # If the context parameter is present but no value was provided, we error
         raise DagsterInvalidInvocationError(
             "Schedule evaluation function expected context argument, but no context argument "
             "was provided when invoking."
         )
 
-    return context or build_schedule_context()
+    context = context or build_schedule_context()
+    resource_args_from_kwargs = {}
+
+    resource_args = {param.name for param in get_resource_args(fn)}
+    for resource_arg in resource_args:
+        if resource_arg in kwargs:
+            resource_args_from_kwargs[resource_arg] = kwargs[resource_arg]
+
+    if resource_args_from_kwargs:
+        return context.merge_resources(resource_args_from_kwargs)
+
+    return context
 
 
 class ScheduleEvaluationContext:
     """The context object available as the first argument various functions defined on a :py:class:`dagster.ScheduleDefinition`.
 
     A `ScheduleEvaluationContext` object is passed as the first argument to ``run_config_fn``, ``tags_fn``,
     and ``should_execute``.
@@ -212,14 +232,18 @@
         return self
 
     def __exit__(self, *exc) -> None:
         self._exit_stack.close()
         self._logger = None
 
     @property
+    def resource_defs(self) -> Optional[Mapping[str, "ResourceDefinition"]]:
+        return self._resource_defs
+
+    @property
     def resources(self) -> Resources:
         from dagster._core.definitions.scoped_resources_builder import (
             IContainsGenerator,
         )
         from dagster._core.execution.build_resources import build_resources
 
         if not self._resources:
@@ -234,14 +258,38 @@
                     "At least one provided resource is a generator, but attempting to access"
                     " resources outside of context manager scope. You can use the following syntax"
                     " to open a context manager: `with build_sensor_context(...) as context:`"
                 )
 
         return self._resources
 
+    def merge_resources(self, resources_dict: Mapping[str, Any]) -> "ScheduleEvaluationContext":
+        """Merge the specified resources into this context.
+        This method is intended to be used by the Dagster framework, and should not be called by user code.
+
+        Args:
+            resources_dict (Mapping[str, Any]): The resources to replace in the context.
+        """
+        check.invariant(
+            self._resources is None, "Cannot merge resources in context that has been initialized."
+        )
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
+        return ScheduleEvaluationContext(
+            instance_ref=self._instance_ref,
+            scheduled_execution_time=self._scheduled_execution_time,
+            repository_name=self._repository_name,
+            schedule_name=self._schedule_name,
+            resources={
+                **(self._resource_defs or {}),
+                **wrap_resources_for_execution(resources_dict),
+            },
+            repository_def=self._repository_def,
+        )
+
     @public
     @property
     def instance(self) -> "DagsterInstance":
         # self._instance_ref should only ever be None when this ScheduleEvaluationContext was
         # constructed under test.
         if not self._instance_ref:
             raise DagsterInvariantViolationError(
@@ -317,15 +365,15 @@
     wrapped_fn: Callable[[ScheduleEvaluationContext], RunRequestIterator]
     has_context_arg: bool
 
 
 def build_schedule_context(
     instance: Optional[DagsterInstance] = None,
     scheduled_execution_time: Optional[datetime] = None,
-    resources: Optional[Mapping[str, "ResourceDefinition"]] = None,
+    resources: Optional[Mapping[str, object]] = None,
     repository_def: Optional["RepositoryDefinition"] = None,
 ) -> ScheduleEvaluationContext:
     """Builds schedule execution context using the provided parameters.
 
     The instance provided to ``build_schedule_context`` must be persistent;
     DagsterInstance.ephemeral() will result in an error.
 
@@ -337,22 +385,24 @@
 
     Examples:
         .. code-block:: python
 
             context = build_schedule_context(instance)
 
     """
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
+
     check.opt_inst_param(instance, "instance", DagsterInstance)
 
     return ScheduleEvaluationContext(
         instance_ref=instance.get_ref() if instance and instance.is_persistent else None,
         scheduled_execution_time=check.opt_inst_param(
             scheduled_execution_time, "scheduled_execution_time", datetime
         ),
-        resources=resources,
+        resources=wrap_resources_for_execution(resources),
         repository_def=repository_def,
     )
 
 
 @whitelist_for_serdes
 class ScheduleExecutionData(
     NamedTuple(
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.0/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     incompatible with type annotations on its own due to its dynamic attributes, so this tag class
     provides a workaround.
     """
 
     def __getattr__(self, name: str) -> Any:
         raise DagsterUnknownResourceError(name)
 
+    @property
+    def _original_resource_dict(self) -> Mapping[str, object]:
+        raise NotImplementedError()
+
 
 class ScopedResourcesBuilder(
     NamedTuple(
         "_ScopedResourcesBuilder",
         [("resource_instance_dict", Mapping[str, object]), ("contains_generator", bool)],
     )
 ):
@@ -51,14 +55,16 @@
             resource_instance_dict=check.opt_mapping_param(
                 resource_instance_dict, "resource_instance_dict", key_type=str
             ),
             contains_generator=contains_generator,
         )
 
     def build(self, required_resource_keys: Optional[AbstractSet[str]]) -> Resources:
+        from dagster._config.pythonic_config import IAttachDifferentObjectToOpContext
+
         """We dynamically create a type that has the resource keys as properties, to enable dotting into
         the resources from a context.
 
         For example, given:
 
         resources = {'foo': <some resource>, 'bar': <some other resource>}
 
@@ -74,32 +80,50 @@
         # because we are building a context for steps that we are not going to execute (e.g. in the
         # resume/retry case, in order to generate copy intermediates events)
         resource_instance_dict = {
             key: self.resource_instance_dict[key]
             for key in required_resource_keys
             if key in self.resource_instance_dict
         }
+        resources_to_attach_to_context = {
+            k: (
+                v.get_object_to_set_on_execution_context()
+                if isinstance(v, IAttachDifferentObjectToOpContext)
+                else v
+            )
+            for k, v in resource_instance_dict.items()
+        }
 
         # If any of the resources are generators, add the IContainsGenerator subclass to flag that
         # this is the case.
         if self.contains_generator:
 
             class _ScopedResourcesContainsGenerator(
                 namedtuple(
-                    "_ScopedResourcesContainsGenerator", list(resource_instance_dict.keys())
+                    "_ScopedResourcesContainsGenerator",
+                    list(resources_to_attach_to_context.keys()),
                 ),
                 Resources,
                 IContainsGenerator,
             ):
-                ...
+                @property
+                def _original_resource_dict(self) -> Mapping[str, object]:
+                    return resource_instance_dict
 
-            return _ScopedResourcesContainsGenerator(**resource_instance_dict)  # type: ignore[call-arg]
+            return _ScopedResourcesContainsGenerator(**resources_to_attach_to_context)  # type: ignore[call-arg]
 
         else:
 
             class _ScopedResources(
-                namedtuple("_ScopedResources", list(resource_instance_dict.keys())),
+                namedtuple("_ScopedResources", list(resources_to_attach_to_context.keys())),
                 Resources,
             ):
-                ...
-
-            return _ScopedResources(**resource_instance_dict)  # type: ignore[call-arg]
+                @property
+                def _original_resource_dict(self) -> Mapping[str, object]:
+                    return resource_instance_dict
+
+            return _ScopedResources(**resources_to_attach_to_context)  # type: ignore[call-arg]
+
+    @classmethod
+    def build_empty(cls) -> Resources:
+        """Returns an empty Resources object, equivalent to ScopedResourcesBuilder().build(None)."""
+        return cls().build(None)
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/selector.py` & `dagster-1.3.0/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.0/dagster/_core/definitions/sensor_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     Iterator,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
+    Tuple,
+    Type,
+    TypeVar,
     Union,
     cast,
 )
 
 import pendulum
 from typing_extensions import TypeAlias
 
@@ -180,14 +183,46 @@
         return self
 
     def __exit__(self, *exc) -> None:
         self._exit_stack.close()
         self._logger = None
 
     @property
+    def resource_defs(self) -> Optional[Mapping[str, "ResourceDefinition"]]:
+        return self._resource_defs
+
+    def merge_resources(self, resources_dict: Mapping[str, Any]) -> "SensorEvaluationContext":
+        """Merge the specified resources into this context.
+
+        This method is intended to be used by the Dagster framework, and should not be called by user code.
+
+        Args:
+            resources_dict (Mapping[str, Any]): The resources to replace in the context.
+        """
+        check.invariant(
+            self._resources is None, "Cannot merge resources in context that has been initialized."
+        )
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
+        return SensorEvaluationContext(
+            instance_ref=self._instance_ref,
+            last_completion_time=self._last_completion_time,
+            last_run_key=self._last_run_key,
+            cursor=self._cursor,
+            repository_name=self._repository_name,
+            repository_def=self._repository_def,
+            instance=self._instance,
+            sensor_name=self._sensor_name,
+            resources={
+                **(self._resource_defs or {}),
+                **wrap_resources_for_execution(resources_dict),
+            },
+        )
+
+    @property
     def resources(self) -> Resources:
         from dagster._core.definitions.scoped_resources_builder import (
             IContainsGenerator,
         )
         from dagster._core.execution.build_resources import build_resources
 
         if not self._resources:
@@ -337,65 +372,27 @@
     resource_params = {param.name for param in get_resource_args(fn)}
 
     return next(
         (param.name for param in get_function_params(fn) if param.name not in resource_params), None
     )
 
 
-def _validate_and_get_resource_dict(
-    context: SensorEvaluationContext, sensor_name: str, required_resource_keys: Set[str]
+def validate_and_get_resource_dict(
+    resources: Resources, sensor_name: str, required_resource_keys: Set[str]
 ) -> Dict[str, Any]:
     """Validates that the context has all the required resources and returns a dictionary of
     resource key to resource object.
     """
     for k in required_resource_keys:
-        if not hasattr(context.resources, k):
+        if not hasattr(resources, k):
             raise DagsterInvalidDefinitionError(
                 f"Resource with key '{k}' required by sensor '{sensor_name}' was not provided."
             )
 
-    return {k: getattr(context.resources, k) for k in required_resource_keys}
-
-
-def get_or_create_sensor_context(
-    fn: Callable, *args: Any, **kwargs: Any
-) -> SensorEvaluationContext:
-    """Based on the passed resource function and the arguments passed to it, returns the
-    user-passed SensorEvaluationContext or creates one if it is not passed.
-
-    Raises an exception if the user passes more than one argument or if the user-provided
-    function requires a context parameter but none is passed.
-    """
-    context_param_name_if_present = get_context_param_name(fn)
-
-    if len(args) + len(kwargs) > 1:
-        raise DagsterInvalidInvocationError(
-            "Sensor invocation received multiple arguments. Only a first "
-            "positional context parameter should be provided when invoking."
-        )
-
-    context: Optional[SensorEvaluationContext] = None
-
-    if len(args) > 0:
-        context = check.opt_inst(args[0], SensorEvaluationContext)
-    elif len(kwargs) > 0:
-        if context_param_name_if_present and context_param_name_if_present not in kwargs:
-            raise DagsterInvalidInvocationError(
-                f"Sensor invocation expected argument '{context_param_name_if_present}'."
-            )
-        context_param_name_if_present = context_param_name_if_present or list(kwargs.keys())[0]
-        context = check.opt_inst(kwargs.get(context_param_name_if_present), SensorEvaluationContext)
-    elif context_param_name_if_present:
-        # If the context parameter is present but no value was provided, we error
-        raise DagsterInvalidInvocationError(
-            "Sensor evaluation function expected context argument, but no context argument "
-            "was provided when invoking."
-        )
-
-    return context or build_sensor_context()
+    return {k: getattr(resources, k) for k in required_resource_keys}
 
 
 def _check_dynamic_partitions_requests(
     dynamic_partitions_requests: Sequence[
         Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]
     ],
 ) -> None:
@@ -493,15 +490,15 @@
         description: Optional[str] = None,
         job: Optional[ExecutableDefinition] = None,
         jobs: Optional[Sequence[ExecutableDefinition]] = None,
         default_status: DefaultSensorStatus = DefaultSensorStatus.STOPPED,
         asset_selection: Optional[AssetSelection] = None,
         required_resource_keys: Optional[Set[str]] = None,
     ):
-        from dagster._config.structured_config import validate_resource_annotated_function
+        from dagster._config.pythonic_config import validate_resource_annotated_function
 
         if evaluation_fn is None:
             raise DagsterInvalidDefinitionError("Must provide evaluation_fn to SensorDefinition.")
 
         if (
             sum(
                 [
@@ -581,16 +578,16 @@
         context_param_name_if_present = get_context_param_name(self._raw_fn)
         context = get_or_create_sensor_context(self._raw_fn, *args, **kwargs)
 
         context_param = (
             {context_param_name_if_present: context} if context_param_name_if_present else {}
         )
 
-        resources = _validate_and_get_resource_dict(
-            context, self.name, self._required_resource_keys
+        resources = validate_and_get_resource_dict(
+            context.resources, self.name, self._required_resource_keys
         )
         return self._raw_fn(**context_param, **resources)
 
     @public
     @property
     def required_resource_keys(self) -> Set[str]:
         return self._required_resource_keys
@@ -906,16 +903,16 @@
 def wrap_sensor_evaluation(
     sensor_name: str,
     fn: RawSensorEvaluationFunction,
 ) -> SensorEvaluationFunction:
     resource_arg_names: Set[str] = {arg.name for arg in get_resource_args(fn)}
 
     def _wrapped_fn(context: SensorEvaluationContext):
-        resource_args_populated = _validate_and_get_resource_dict(
-            context, sensor_name, resource_arg_names
+        resource_args_populated = validate_and_get_resource_dict(
+            context.resources, sensor_name, resource_arg_names
         )
 
         context_param_name_if_present = get_context_param_name(fn)
         context_param = (
             {context_param_name_if_present: context} if context_param_name_if_present else {}
         )
         result = fn(**context_param, **resource_args_populated)
@@ -940,15 +937,15 @@
 
 def build_sensor_context(
     instance: Optional[DagsterInstance] = None,
     cursor: Optional[str] = None,
     repository_name: Optional[str] = None,
     repository_def: Optional["RepositoryDefinition"] = None,
     sensor_name: Optional[str] = None,
-    resources: Optional[Mapping[str, "ResourceDefinition"]] = None,
+    resources: Optional[Mapping[str, object]] = None,
     definitions: Optional["Definitions"] = None,
 ) -> SensorEvaluationContext:
     """Builds sensor execution context using the provided parameters.
 
     This function can be used to provide a context to the invocation of a sensor definition.If
     provided, the dagster instance must be persistent; DagsterInstance.ephemeral() will result in an
     error.
@@ -972,14 +969,15 @@
 
             context = build_sensor_context()
             my_sensor(context)
 
     """
     from dagster._core.definitions.definitions_class import Definitions
     from dagster._core.definitions.repository_definition import RepositoryDefinition
+    from dagster._core.execution.build_resources import wrap_resources_for_execution
 
     check.opt_inst_param(instance, "instance", DagsterInstance)
     check.opt_str_param(cursor, "cursor")
     check.opt_str_param(repository_name, "repository_name")
     repository_def = normalize_to_repository(
         check.opt_inst_param(definitions, "definitions", Definitions),
         check.opt_inst_param(repository_def, "repository_def", RepositoryDefinition),
@@ -991,16 +989,96 @@
         last_completion_time=None,
         last_run_key=None,
         cursor=cursor,
         repository_name=repository_name,
         instance=instance,
         repository_def=repository_def,
         sensor_name=sensor_name,
-        resources=resources,
+        resources=wrap_resources_for_execution(resources),
+    )
+
+
+T = TypeVar("T")
+
+
+def get_sensor_context_from_args_or_kwargs(
+    fn: Callable,
+    args: Tuple[Any],
+    kwargs: Dict[str, Any],
+    context_type: Type[T],
+) -> Optional[T]:
+    from dagster._config.pythonic_config import is_coercible_to_resource
+
+    context_param_name = get_context_param_name(fn)
+
+    kwarg_keys_non_resource = set(kwargs.keys()) - {param.name for param in get_resource_args(fn)}
+    if len(args) + len(kwarg_keys_non_resource) > 1:
+        raise DagsterInvalidInvocationError(
+            "Sensor invocation received multiple non-resource arguments. Only a first "
+            "positional context parameter should be provided when invoking."
+        )
+
+    if any(is_coercible_to_resource(arg) for arg in args):
+        raise DagsterInvalidInvocationError(
+            "If directly invoking a sensor, you may not provide resources as"
+            " positional"
+            " arguments, only as keyword arguments."
+        )
+
+    context: Optional[T] = None
+
+    if len(args) > 0:
+        context = check.opt_inst(args[0], context_type)
+    elif len(kwargs) > 0:
+        if context_param_name and context_param_name not in kwargs:
+            raise DagsterInvalidInvocationError(
+                f"Sensor invocation expected argument '{context_param_name}'."
+            )
+        context = check.opt_inst(kwargs.get(context_param_name or "context"), context_type)
+    elif context_param_name:
+        # If the context parameter is present but no value was provided, we error
+        raise DagsterInvalidInvocationError(
+            "Sensor evaluation function expected context argument, but no context argument "
+            "was provided when invoking."
+        )
+
+    return context
+
+
+def get_or_create_sensor_context(
+    fn: Callable,
+    *args: Any,
+    **kwargs: Any,
+) -> SensorEvaluationContext:
+    """Based on the passed resource function and the arguments passed to it, returns the
+    user-passed SensorEvaluationContext or creates one if it is not passed.
+
+    Raises an exception if the user passes more than one argument or if the user-provided
+    function requires a context parameter but none is passed.
+    """
+    context = (
+        get_sensor_context_from_args_or_kwargs(
+            fn,
+            args,
+            kwargs,
+            context_type=SensorEvaluationContext,
+        )
+        or build_sensor_context()
     )
+    resource_args_from_kwargs = {}
+
+    resource_args = {param.name for param in get_resource_args(fn)}
+    for resource_arg in resource_args:
+        if resource_arg in kwargs:
+            resource_args_from_kwargs[resource_arg] = kwargs[resource_arg]
+
+    if resource_args_from_kwargs:
+        return context.merge_resources(resource_args_from_kwargs)
+
+    return context
 
 
 def _run_requests_with_base_asset_jobs(
     run_requests: Iterable[RunRequest],
     context: SensorEvaluationContext,
     outer_asset_selection: AssetSelection,
 ) -> Sequence[RunRequest]:
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/source_asset.py` & `dagster-1.3.0/dagster/_core/definitions/source_asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,35 +90,44 @@
         key: CoercibleToAssetKey,
         metadata: Optional[ArbitraryMetadataMapping] = None,
         io_manager_key: Optional[str] = None,
         io_manager_def: Optional[IOManagerDefinition] = None,
         description: Optional[str] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         group_name: Optional[str] = None,
-        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
+        resource_defs: Optional[Mapping[str, object]] = None,
         observe_fn: Optional[SourceAssetObserveFunction] = None,
         # This is currently private because it is necessary for source asset observation functions,
         # but we have not yet decided on a final API for associated one or more ops with a source
         # asset. If we were to make this public, then we would have a canonical public
         # `required_resource_keys` used for observation that might end up conflicting with a set of
         # required resource keys for a different operation.
         _required_resource_keys: Optional[AbstractSet[str]] = None,
         # Add additional fields to with_resources and with_group below
     ):
+        from dagster._core.execution.build_resources import wrap_resources_for_execution
+
+        if partitions_def is not None and observe_fn is not None:
+            raise DagsterInvalidDefinitionError(
+                "Cannot specify a `partitions_def` for an observable source asset."
+            )
+
         if resource_defs is not None:
             experimental_arg_warning("resource_defs", "SourceAsset.__new__")
 
         if io_manager_def is not None:
             experimental_arg_warning("io_manager_def", "SourceAsset.__new__")
 
         self.key = AssetKey.from_coerceable(key)
         metadata = check.opt_mapping_param(metadata, "metadata", key_type=str)
         self.raw_metadata = metadata
         self.metadata = normalize_metadata(metadata, allow_invalid=True)
-        self.resource_defs = dict(check.opt_mapping_param(resource_defs, "resource_defs"))
+        self.resource_defs = wrap_resources_for_execution(
+            dict(check.opt_mapping_param(resource_defs, "resource_defs"))
+        )
         self._io_manager_def = check.opt_inst_param(
             io_manager_def, "io_manager_def", IOManagerDefinition
         )
         if self._io_manager_def:
             if not io_manager_key:
                 io_manager_key = self.key.to_python_identifier("io_manager")
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.0/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/target.py` & `dagster-1.3.0/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.0/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.0/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.0/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         JobDefinition,
         PartitionedConfig,
         PartitionsDefinition,
         SourceAsset,
     )
     from dagster._core.definitions.asset_graph import InternalAssetGraph
     from dagster._core.definitions.asset_selection import CoercibleToAssetSelection
+    from dagster._core.definitions.run_config import RunConfig
 
 
 class UnresolvedAssetJobDefinition(
     NamedTuple(
         "_UnresolvedAssetJobDefinition",
         [
             ("name", str),
@@ -43,15 +44,17 @@
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         selection: "AssetSelection",
-        config: Optional[Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig"]] = None,
+        config: Optional[
+            Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig", "RunConfig"]
+        ] = None,
         description: Optional[str] = None,
         tags: Optional[Mapping[str, Any]] = None,
         partitions_def: Optional["PartitionsDefinition"] = None,
         executor_def: Optional["ExecutorDefinition"] = None,
     ):
         from dagster._core.definitions import (
             AssetSelection,
@@ -237,15 +240,17 @@
             executor_def=self.executor_def or default_executor_def,
         )
 
 
 def define_asset_job(
     name: str,
     selection: Optional["CoercibleToAssetSelection"] = None,
-    config: Optional[Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig[object]"]] = None,
+    config: Optional[
+        Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig[object]", "RunConfig"]
+    ] = None,
     description: Optional[str] = None,
     tags: Optional[Mapping[str, Any]] = None,
     partitions_def: Optional["PartitionsDefinition[Any]"] = None,
     executor_def: Optional["ExecutorDefinition"] = None,
 ) -> UnresolvedAssetJobDefinition:
     """Creates a definition of a job which will either materialize a selection of assets or observe
     a selection of source assets. This will only be resolved to a JobDefinition once placed in a
```

### Comparing `dagster-1.2.7/dagster/_core/definitions/utils.py` & `dagster-1.3.0/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.0/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/errors.py` & `dagster-1.3.0/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/event_api.py` & `dagster-1.3.0/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/events/__init__.py` & `dagster-1.3.0/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/events/log.py` & `dagster-1.3.0/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/events/utils.py` & `dagster-1.3.0/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/api.py` & `dagster-1.3.0/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.0/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/backfill.py` & `dagster-1.3.0/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/build_resources.py` & `dagster-1.3.0/dagster/_core/execution/build_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,21 +110,25 @@
             )
         finally:
             list(resources_manager.generate_teardown_events())
 
 
 def wrap_resources_for_execution(
     resources: Optional[Mapping[str, Any]] = None
-) -> Mapping[str, ResourceDefinition]:
+) -> Dict[str, ResourceDefinition]:
+    from dagster._config.pythonic_config import ConfigurableResourceFactory, PartialResource
+
     resources = check.opt_mapping_param(resources, "resources", key_type=str)
     resource_defs = {}
     # Wrap instantiated resource values in a resource definition.
     # If an instantiated IO manager is provided, wrap it in an IO manager definition.
     for resource_key, resource in resources.items():
-        if isinstance(resource, ResourceDefinition):
+        if isinstance(resource, (ConfigurableResourceFactory, PartialResource)):
+            resource_defs[resource_key] = resource.get_resource_definition()
+        elif isinstance(resource, ResourceDefinition):
             resource_defs[resource_key] = resource
         elif isinstance(resource, IOManager):
             resource_defs[resource_key] = IOManagerDefinition.hardcoded_io_manager(resource)
         else:
             resource_defs[resource_key] = ResourceDefinition.hardcoded_resource(resource)
 
     return resource_defs
```

### Comparing `dagster-1.2.7/dagster/_core/execution/compute_logs.py` & `dagster-1.3.0/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/compute.py` & `dagster-1.3.0/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/hook.py` & `dagster-1.3.0/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/init.py` & `dagster-1.3.0/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/input.py` & `dagster-1.3.0/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/invocation.py` & `dagster-1.3.0/dagster/_core/execution/context/invocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,25 @@
             resources_config=self._resources_config,
             instance=self._instance,
             partition_key=self._partition_key,
             mapping_key=self._mapping_key,
             assets_def=self._assets_def,
         )
 
+    def replace_config(self, config: Mapping[str, Any]) -> "UnboundOpExecutionContext":
+        return UnboundOpExecutionContext(
+            op_config=config,
+            resources_dict=self._resource_defs,
+            resources_config=self._resources_config,
+            instance=self._instance,
+            partition_key=self._partition_key,
+            mapping_key=self._mapping_key,
+            assets_def=self._assets_def,
+        )
+
 
 def _validate_resource_requirements(
     resource_defs: Mapping[str, ResourceDefinition], op_def: OpDefinition
 ) -> None:
     """Validate correctness of resources against required resource keys."""
     if cast(DecoratedOpFunction, op_def.compute_fn).has_context_arg():
         for requirement in op_def.get_resource_requirements():
```

### Comparing `dagster-1.2.7/dagster/_core/execution/context/logger.py` & `dagster-1.3.0/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/output.py` & `dagster-1.3.0/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context/system.py` & `dagster-1.3.0/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/context_creation_pipeline.py` & `dagster-1.3.0/dagster/_core/execution/context_creation_pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.0/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.0/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/execute_job_result.py` & `dagster-1.3.0/dagster/_core/execution/execute_job_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/execution_result.py` & `dagster-1.3.0/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/host_mode.py` & `dagster-1.3.0/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/job_backfill.py` & `dagster-1.3.0/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/memoization.py` & `dagster-1.3.0/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/active.py` & `dagster-1.3.0/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/compute.py` & `dagster-1.3.0/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.0/dagster/_core/execution/plan/compute_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Type,
     Union,
     cast,
 )
 
 from typing_extensions import get_args
 
-from dagster._config.structured_config import Config
+from dagster._config.pythonic_config import Config
 from dagster._core.definitions import (
     AssetMaterialization,
     DynamicOutput,
     ExpectationResult,
     Output,
     OutputDefinition,
 )
@@ -107,15 +107,17 @@
         # config_arg_cls is either a Config class or a primitive type
         if issubclass(config_arg_cls, Config):
             args_to_pass["config"] = config_arg_cls(**context.op_config)
         else:
             args_to_pass["config"] = context.op_config
     if resource_args:
         for resource_name, arg_name in resource_args.items():
-            args_to_pass[arg_name] = getattr(context.resources, resource_name)
+            args_to_pass[arg_name] = context.resources._original_resource_dict[  # noqa: SLF001
+                resource_name
+            ]
 
     return fn(context, **args_to_pass) if context_arg_provided else fn(**args_to_pass)
 
 
 def _coerce_solid_compute_fn_to_iterator(
     fn, output_defs, context, context_arg_provided, kwargs, config_arg_class, resource_arg_mapping
 ):
```

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.0/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.0/dagster/_core/execution/plan/execute_step.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     ExpectationResult,
     Output,
     OutputDefinition,
     TypeCheck,
 )
 from dagster._core.definitions.data_version import (
     CODE_VERSION_TAG,
+    DATA_VERSION_IS_USER_PROVIDED_TAG,
     DATA_VERSION_TAG,
     DEFAULT_DATA_VERSION,
     DataVersion,
     compute_logical_data_version,
     extract_data_version_from_entry,
     get_input_data_version_tag,
     get_input_event_pointer_tag,
 )
 from dagster._core.definitions.decorators.op_decorator import DecoratedOpFunction
 from dagster._core.definitions.events import DynamicOutput
 from dagster._core.definitions.metadata import (
-    MetadataEntry,
     MetadataValue,
     normalize_metadata,
 )
 from dagster._core.definitions.multi_dimensional_partitions import (
     MultiPartitionKey,
     get_tags_from_multi_partition_key,
 )
@@ -471,15 +471,17 @@
             compute_logical_data_version(
                 code_version,
                 {k: meta["data_version"] for k, meta in input_provenance_data.items()},
             )
             if output.data_version is None
             else output.data_version
         )
-        tags = _build_data_version_tags(data_version, code_version, input_provenance_data)
+        tags = _build_data_version_tags(
+            data_version, code_version, input_provenance_data, output.data_version is not None
+        )
         if not step_context.has_data_version(asset_key):
             data_version = DataVersion(tags[DATA_VERSION_TAG])
             step_context.set_data_version(asset_key, data_version)
     else:
         tags = {}
 
     backfill_id = step_context.get_tag(BACKFILL_ID_TAG)
@@ -547,23 +549,26 @@
     return input_provenance
 
 
 def _build_data_version_tags(
     data_version: DataVersion,
     code_version: str,
     input_provenance_data: Mapping[AssetKey, _InputProvenanceData],
+    data_version_is_user_provided: bool,
 ) -> Dict[str, str]:
     tags: Dict[str, str] = {}
     tags[CODE_VERSION_TAG] = code_version
     for key, meta in input_provenance_data.items():
         tags[get_input_data_version_tag(key)] = meta["data_version"].value
         tags[get_input_event_pointer_tag(key)] = (
             str(meta["storage_id"]) if meta["storage_id"] else "NULL"
         )
     tags[DATA_VERSION_TAG] = data_version.value
+    if data_version_is_user_provided:
+        tags[DATA_VERSION_IS_USER_PROVIDED_TAG] = "true"
     return tags
 
 
 def _store_output(
     step_context: StepExecutionContext,
     step_output_handle: StepOutputHandle,
     output: Union[Output, DynamicOutput],
@@ -607,29 +612,24 @@
             yield event
 
         manager_metadata = {**manager_metadata, **output_context.consume_logged_metadata()}
         if isinstance(elt, DagsterEvent):
             yield elt
         elif isinstance(elt, AssetMaterialization):
             manager_materializations.append(elt)
-        elif isinstance(elt, MetadataEntry):  # should remove this?
-            experimental_functionality_warning(
-                "Yielding metadata from an IOManager's handle_output() function"
-            )
-            manager_metadata[elt.label] = elt.value
         elif isinstance(elt, dict):  # should remove this?
             experimental_functionality_warning(
                 "Yielding metadata from an IOManager's handle_output() function"
             )
             manager_metadata = {**manager_metadata, **normalize_metadata(elt)}
         else:
             raise DagsterInvariantViolationError(
                 f"IO manager on output {output_def.name} has returned "
                 f"value {elt} of type {type(elt).__name__}. The return type can only be "
-                "one of AssetMaterialization, MetadataEntry."
+                "one of AssetMaterialization, Dict[str, MetadataValue]."
             )
 
     for event in output_context.consume_events():
         yield event
 
     manager_metadata = {**manager_metadata, **output_context.consume_logged_metadata()}
     # do not alter explicitly created AssetMaterializations
```

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.0/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/handle.py` & `dagster-1.3.0/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.0/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.0/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/objects.py` & `dagster-1.3.0/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.0/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/plan.py` & `dagster-1.3.0/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/state.py` & `dagster-1.3.0/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/step.py` & `dagster-1.3.0/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/plan/utils.py` & `dagster-1.3.0/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.0/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.0/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/resources_init.py` & `dagster-1.3.0/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/results.py` & `dagster-1.3.0/dagster/_core/execution/results.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/retries.py` & `dagster-1.3.0/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.0/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/stats.py` & `dagster-1.3.0/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/tags.py` & `dagster-1.3.0/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.0/dagster/_core/execution/validate_run_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Any, Mapping, Optional
+from typing import Any, Mapping, Optional, Union
 
 import dagster._check as check
 from dagster._core.definitions import JobDefinition
-from dagster._core.definitions.run_config import convert_config_input
+from dagster._core.definitions.run_config import RunConfig, convert_config_input
 from dagster._core.system_config.objects import ResolvedRunConfig
 
 
 def validate_run_config(
     job_def: JobDefinition,
-    run_config: Optional[Mapping[str, Any]] = None,
+    run_config: Optional[Union[Mapping[str, Any], RunConfig]] = None,
 ) -> Mapping[str, Any]:
     """Function to validate a provided run config blob against a given job.
 
     If validation is successful, this function will return a dictionary representation of the
     validated config actually used during execution.
 
     Args:
```

### Comparing `dagster-1.2.7/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.0/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/execution/with_resources.py` & `dagster-1.3.0/dagster/_core/execution/with_resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import Any, Iterable, List, Mapping, Optional, Sequence, TypeVar, cast
 
 from dagster import _check as check
+from dagster._core.execution.build_resources import wrap_resources_for_execution
 from dagster._utils.merger import merge_dicts
 
 from ..._config import Shape
-from ..definitions import ResourceDefinition
 from ..definitions.resource_requirement import ResourceAddable
 from ..definitions.utils import DEFAULT_IO_MANAGER_KEY
 from ..errors import DagsterInvalidConfigError, DagsterInvalidInvocationError
 
 T = TypeVar("T", bound=ResourceAddable)
 
 
 def with_resources(
     definitions: Iterable[T],
-    resource_defs: Mapping[str, ResourceDefinition],
+    resource_defs: Mapping[str, object],
     resource_config_by_key: Optional[Mapping[str, Any]] = None,
 ) -> Sequence[T]:
     """Adds dagster resources to copies of resource-requiring dagster definitions.
 
     An error will be thrown if any provided definitions have a conflicting
     resource definition provided for a key provided to resource_defs. Resource
     config can be provided, with keys in the config dictionary corresponding to
     the keys for each resource definition. If any definition has unsatisfied
     resource keys after applying with_resources, an error will be thrown.
 
     Args:
         definitions (Iterable[ResourceAddable]): Dagster definitions to provide resources to.
-        resource_defs (Mapping[str, ResourceDefinition]):
-            Mapping of resource keys to ResourceDefinition objects to satisfy
+        resource_defs (Mapping[str, object]):
+            Mapping of resource keys to objects to satisfy
             resource requirements of provided dagster definitions.
         resource_config_by_key (Optional[Mapping[str, Any]]):
             Specifies config for provided resources. The key in this dictionary
             corresponds to configuring the same key in the resource_defs
             dictionary.
 
     Examples:
@@ -69,16 +69,19 @@
     )
 
     check.mapping_param(resource_defs, "resource_defs")
     resource_config_by_key = check.opt_mapping_param(
         resource_config_by_key, "resource_config_by_key"
     )
 
-    resource_defs = merge_dicts(
-        {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema}, resource_defs
+    resource_defs = wrap_resources_for_execution(
+        merge_dicts(
+            {DEFAULT_IO_MANAGER_KEY: default_job_io_manager_with_fs_io_manager_schema},
+            resource_defs,
+        )
     )
 
     for key, resource_def in resource_defs.items():
         if key in resource_config_by_key:
             resource_config = resource_config_by_key[key]
             if not isinstance(resource_config, dict) or "config" not in resource_config:
                 raise DagsterInvalidInvocationError(
```

### Comparing `dagster-1.2.7/dagster/_core/executor/base.py` & `dagster-1.3.0/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.0/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/executor/in_process.py` & `dagster-1.3.0/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/executor/init.py` & `dagster-1.3.0/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/executor/multiprocess.py` & `dagster-1.3.0/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.0/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.0/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/__init__.py` & `dagster-1.3.0/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/code_location.py` & `dagster-1.3.0/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/external.py` & `dagster-1.3.0/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/external_data.py` & `dagster-1.3.0/dagster/_core/host_representation/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 import pendulum
 from typing_extensions import Final
 
 from dagster import (
     StaticPartitionsDefinition,
     _check as check,
 )
+from dagster._config.pythonic_config import (
+    ConfigurableIOManagerFactoryResourceDefinition,
+    ConfigurableResourceFactoryResourceDefinition,
+    ResourceWithKeyMapping,
+)
 from dagster._config.snap import (
     ConfigFieldSnap,
     ConfigSchemaSnapshot,
     snap_from_config_type,
 )
-from dagster._config.structured_config import (
-    ConfigurableResource,
-    PartialResource,
-    ResourceWithKeyMapping,
-)
 from dagster._core.definitions import (
     JobDefinition,
     PartitionsDefinition,
     PipelineDefinition,
     PresetDefinition,
     RepositoryDefinition,
     ScheduleDefinition,
@@ -1380,14 +1380,16 @@
     for source_asset in source_assets_by_key.values():
         if source_asset.key not in node_defs_by_asset_key:
             job_names = (
                 [
                     job_def.name
                     for job_def in pipelines
                     if source_asset.key in job_def.asset_layer.source_assets_by_key
+                    and source_asset.partitions_def is None
+                    or source_asset.partitions_def == job_def.partitions_def  # type: ignore
                 ]
                 if source_asset.node_def is not None
                 else []
             )
             asset_nodes.append(
                 ExternalAssetNode(
                     asset_key=source_asset.key,
@@ -1528,33 +1530,40 @@
 
 def _get_nested_resources(
     resource_def: ResourceDefinition, resource_key_mapping: Mapping[int, str]
 ) -> Mapping[str, NestedResource]:
     if isinstance(resource_def, ResourceWithKeyMapping):
         resource_def = resource_def.wrapped_resource
 
-    return (
-        {
+    # ConfigurableResources may have "anonymous" nested resources, which are not
+    # explicitly specified as top-level resources
+    if isinstance(
+        resource_def,
+        (
+            ConfigurableResourceFactoryResourceDefinition,
+            ConfigurableIOManagerFactoryResourceDefinition,
+        ),
+    ):
+        return {
             k: (
                 NestedResource(
                     NestedResourceType.TOP_LEVEL, resource_key_mapping[id(nested_resource)]
                 )
                 if id(nested_resource) in resource_key_mapping
                 else NestedResource(
                     NestedResourceType.ANONYMOUS, nested_resource.__class__.__name__
                 )
             )
             for k, nested_resource in resource_def.nested_resources.items()
         }
-        if isinstance(resource_def, (ConfigurableResource, PartialResource))
-        else {
+    else:
+        return {
             k: NestedResource(NestedResourceType.TOP_LEVEL, k)
             for k in resource_def.required_resource_keys
         }
-    )
 
 
 def external_resource_data_from_def(
     name: str,
     resource_def: ResourceDefinition,
     nested_resources: Mapping[str, NestedResource],
     parent_resources: Mapping[str, str],
```

### Comparing `dagster-1.2.7/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.0/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.0/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/handle.py` & `dagster-1.3.0/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/historical.py` & `dagster-1.3.0/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/origin.py` & `dagster-1.3.0/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/pipeline_index.py` & `dagster-1.3.0/dagster/_core/host_representation/pipeline_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/host_representation/represented.py` & `dagster-1.3.0/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/instance/__init__.py` & `dagster-1.3.0/dagster/_core/instance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
         InstigatorTick,
         TickData,
         TickStatus,
     )
     from dagster._core.secrets import SecretsLoader
     from dagster._core.snap import ExecutionPlanSnapshot, PipelineSnapshot
     from dagster._core.storage.compute_log_manager import ComputeLogManager
+    from dagster._core.storage.daemon_cursor import DaemonCursorStorage
     from dagster._core.storage.event_log import EventLogStorage
     from dagster._core.storage.event_log.base import (
         AssetRecord,
         EventLogConnection,
         EventLogRecord,
         EventRecordsFilter,
     )
@@ -418,35 +419,29 @@
                     " max_resume_run_attempts to 0 to use run monitoring. Any runs with a failed"
                     " run worker will be marked as failed, but will not be resumed."
                 ),
             )
 
         if self.run_retries_enabled:
             check.invariant(
-                self.run_storage.supports_kvs(),
-                (
-                    "Run retries are enabled, but the configured run storage does not support them."
-                    " Consider switching to Postgres or Mysql."
-                ),
-            )
-            check.invariant(
                 self.event_log_storage.supports_event_consumer_queries(),
                 (
                     "Run retries are enabled, but the configured event log storage does not support"
                     " them. Consider switching to Postgres or Mysql."
                 ),
             )
 
     # ctors
 
     @public
     @staticmethod
     def ephemeral(
         tempdir: Optional[str] = None,
         preload: Optional[Sequence["DebugRunPayload"]] = None,
+        settings: Optional[Dict] = None,
     ) -> "DagsterInstance":
         from dagster._core.launcher.sync_in_memory_run_launcher import SyncInMemoryRunLauncher
         from dagster._core.run_coordinator import DefaultRunCoordinator
         from dagster._core.storage.event_log import InMemoryEventLogStorage
         from dagster._core.storage.noop_compute_log_manager import NoOpComputeLogManager
         from dagster._core.storage.root import LocalArtifactStorage, TemporaryLocalArtifactStorage
         from dagster._core.storage.runs import InMemoryRunStorage
@@ -460,14 +455,15 @@
             instance_type=InstanceType.EPHEMERAL,
             local_artifact_storage=local_storage,
             run_storage=InMemoryRunStorage(preload=preload),
             event_storage=InMemoryEventLogStorage(preload=preload),
             compute_log_manager=NoOpComputeLogManager(),
             run_coordinator=DefaultRunCoordinator(),
             run_launcher=SyncInMemoryRunLauncher(),
+            settings=settings,
         )
 
     @public
     @staticmethod
     def get() -> "DagsterInstance":
         dagster_home_path = os.getenv("DAGSTER_HOME")
 
@@ -661,14 +657,18 @@
     def run_storage(self) -> "RunStorage":
         return self._run_storage
 
     @property
     def event_log_storage(self) -> "EventLogStorage":
         return self._event_storage
 
+    @property
+    def daemon_cursor_storage(self) -> "DaemonCursorStorage":
+        return self._run_storage
+
     # schedule storage
 
     @property
     def schedule_storage(self) -> Optional["ScheduleStorage"]:
         return self._schedule_storage
 
     @property
@@ -791,14 +791,26 @@
     def run_retries_enabled(self) -> bool:
         return self.get_settings("run_retries").get("enabled", False)
 
     @property
     def run_retries_max_retries(self) -> int:
         return self.get_settings("run_retries").get("max_retries")
 
+    @property
+    def auto_materialize_enabled(self) -> bool:
+        return self.get_settings("auto_materialize").get("enabled", True)
+
+    @property
+    def auto_materialize_minimum_interval_seconds(self) -> int:
+        return self.get_settings("auto_materialize").get("minimum_interval_seconds")
+
+    @property
+    def auto_materialize_run_tags(self) -> Dict[str, str]:
+        return self.get_settings("auto_materialize").get("run_tags", {})
+
     # python logs
 
     @property
     def managed_python_loggers(self) -> Sequence[str]:
         python_log_settings = self.get_settings("python_logs") or {}
         loggers: Sequence[str] = python_log_settings.get("managed_python_loggers", [])
         return loggers
@@ -2423,14 +2435,15 @@
 
     def wipe_daemon_heartbeats(self) -> None:
         self._run_storage.wipe_daemon_heartbeats()
 
     def get_required_daemon_types(self) -> Sequence[str]:
         from dagster._core.run_coordinator import QueuedRunCoordinator
         from dagster._core.scheduler import DagsterDaemonScheduler
+        from dagster._daemon.asset_daemon import AssetDaemon
         from dagster._daemon.auto_run_reexecution.event_log_consumer import EventLogConsumerDaemon
         from dagster._daemon.daemon import (
             BackfillDaemon,
             MonitoringDaemon,
             SchedulerDaemon,
             SensorDaemon,
         )
@@ -2446,14 +2459,16 @@
             daemons.append(SchedulerDaemon.daemon_type())
         if isinstance(self.run_coordinator, QueuedRunCoordinator):
             daemons.append(QueuedRunCoordinatorDaemon.daemon_type())
         if self.run_monitoring_enabled:
             daemons.append(MonitoringDaemon.daemon_type())
         if self.run_retries_enabled:
             daemons.append(EventLogConsumerDaemon.daemon_type())
+        if self.auto_materialize_enabled:
+            daemons.append(AssetDaemon.daemon_type())
         return daemons
 
     def get_daemon_statuses(
         self, daemon_types: Optional[Sequence[str]] = None
     ) -> Mapping[str, "DaemonStatus"]:
         """Get the current status of the daemons. If daemon_types aren't provided, defaults to all
         required types. Returns a dict of daemon type to status.
```

### Comparing `dagster-1.2.7/dagster/_core/instance/config.py` & `dagster-1.3.0/dagster/_core/instance/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,8 +321,15 @@
             },
             is_required=False,
         ),
         "secrets": secrets_loader_config_schema(),
         "retention": retention_config_schema(),
         "sensors": sensors_daemon_config(),
         "schedules": schedules_daemon_config(),
+        "auto_materialize": Field(
+            {
+                "enabled": Field(Bool, is_required=False),
+                "minimum_interval_seconds": Field(int, is_required=False),
+                "run_tags": Field(dict, is_required=False),
+            }
+        ),
     }
```

### Comparing `dagster-1.2.7/dagster/_core/instance/ref.py` & `dagster-1.3.0/dagster/_core/instance/ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,14 +449,15 @@
             "run_monitoring",
             "run_retries",
             "code_servers",
             "retention",
             "sensors",
             "schedules",
             "nux",
+            "auto_materialize",
         }
         settings = {key: config_value.get(key) for key in settings_keys if config_value.get(key)}
 
         return InstanceRef(
             local_artifact_storage_data=local_artifact_storage_data,  # type: ignore  # (possible none)
             run_storage_data=run_storage_data,
             event_storage_data=event_storage_data,
```

### Comparing `dagster-1.2.7/dagster/_core/instance_for_test.py` & `dagster-1.3.0/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/launcher/base.py` & `dagster-1.3.0/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.0/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.0/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/log_manager.py` & `dagster-1.3.0/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/nux.py` & `dagster-1.3.0/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/origin.py` & `dagster-1.3.0/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/run_coordinator/base.py` & `dagster-1.3.0/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.0/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.0/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/scheduler/__init__.py` & `dagster-1.3.0/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/scheduler/execution.py` & `dagster-1.3.0/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/scheduler/instigation.py` & `dagster-1.3.0/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.0/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/secrets/env_file.py` & `dagster-1.3.0/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/selector/subset_selector.py` & `dagster-1.3.0/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/__init__.py` & `dagster-1.3.0/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/config_types.py` & `dagster-1.3.0/dagster/_core/snap/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/dagster_types.py` & `dagster-1.3.0/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.0/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.0/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/mode.py` & `dagster-1.3.0/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/snap/node.py` & `dagster-1.3.0/dagster/_core/snap/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     ):
         return super(InputDefSnap, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             dagster_type_key=check.str_param(dagster_type_key, "dagster_type_key"),
             description=check.opt_str_param(description, "description"),
             metadata=normalize_metadata(
-                check.opt_mapping_param(metadata, "metadata", key_type=str)
+                check.opt_mapping_param(metadata, "metadata", key_type=str), allow_invalid=True
             ),
         )
 
 
 @whitelist_for_serdes(
     storage_field_names={"metadata": "metadata_entries"},
     field_serializers={"metadata": MetadataFieldSerializer},
@@ -88,15 +88,15 @@
         return super(OutputDefSnap, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             dagster_type_key=check.str_param(dagster_type_key, "dagster_type_key"),
             description=check.opt_str_param(description, "description"),
             is_required=check.bool_param(is_required, "is_required"),
             metadata=normalize_metadata(
-                check.opt_mapping_param(metadata, "metadata", key_type=str)
+                check.opt_mapping_param(metadata, "metadata", key_type=str), allow_invalid=True
             ),
             is_dynamic=check.bool_param(is_dynamic, "is_dynamic"),
         )
 
 
 @whitelist_for_serdes(storage_field_names={"mapped_node_name": "mapped_solid_name"})
 class OutputMappingSnap(
```

### Comparing `dagster-1.2.7/dagster/_core/snap/pipeline_snapshot.py` & `dagster-1.3.0/dagster/_core/snap/pipeline_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.0/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/README.md` & `dagster-1.3.0/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/env.py` & `dagster-1.3.0/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.0/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/base_storage.py` & `dagster-1.3.0/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.0/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.0/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.0/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.0/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/config.py` & `dagster-1.3.0/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.0/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.0/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/base.py` & `dagster-1.3.0/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.0/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.0/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.0/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.0/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.3.0/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/file_manager.py` & `dagster-1.3.0/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.0/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/input_manager.py` & `dagster-1.3.0/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/io_manager.py` & `dagster-1.3.0/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.0/dagster/_core/storage/legacy_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,19 +323,19 @@
 
     def update_backfill(self, partition_backfill: "PartitionBackfill") -> None:
         return self._storage.run_storage.update_backfill(partition_backfill)
 
     def get_run_partition_data(self, runs_filter: "RunsFilter") -> Sequence["RunPartitionData"]:
         return self._storage.run_storage.get_run_partition_data(runs_filter)
 
-    def kvs_get(self, keys: Set[str]) -> Mapping[str, str]:
-        return self._storage.run_storage.kvs_get(keys)
+    def get_cursor_values(self, keys: Set[str]) -> Mapping[str, str]:
+        return self._storage.run_storage.get_cursor_values(keys)
 
-    def kvs_set(self, pairs: Mapping[str, str]) -> None:
-        return self._storage.run_storage.kvs_set(pairs)
+    def set_cursor_values(self, pairs: Mapping[str, str]) -> None:
+        return self._storage.run_storage.set_cursor_values(pairs)
 
     def replace_job_origin(self, run: "DagsterRun", job_origin: "ExternalPipelineOrigin") -> None:
         return self._storage.run_storage.replace_job_origin(run, job_origin)
 
 
 class LegacyEventLogStorage(EventLogStorage, ConfigurableClass):
     def __init__(self, storage: DagsterStorage, inst_data: Optional[ConfigurableClassData] = None):
```

### Comparing `dagster-1.2.7/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.0/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.0/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.0/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/migration/utils.py` & `dagster-1.3.0/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.0/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/output_manager.py` & `dagster-1.3.0/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.0/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/pipeline_run.py` & `dagster-1.3.0/dagster/_core/storage/pipeline_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/root.py` & `dagster-1.3.0/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.0/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/base.py` & `dagster-1.3.0/dagster/_core/storage/runs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,26 @@
     RunsFilter,
     TagBucket,
 )
 from dagster._core.storage.sql import AlembicVersion
 from dagster._daemon.types import DaemonHeartbeat
 from dagster._utils import PrintFn
 
+from ..daemon_cursor import DaemonCursorStorage
+
 if TYPE_CHECKING:
     from dagster._core.host_representation.origin import ExternalPipelineOrigin
 
 
 class RunGroupInfo(TypedDict):
     count: int
     runs: Sequence[DagsterRun]
 
 
-class RunStorage(ABC, MayHaveInstanceWeakref[T_DagsterInstance]):
+class RunStorage(ABC, MayHaveInstanceWeakref[T_DagsterInstance], DaemonCursorStorage):
     """Abstract base class for storing pipeline run history.
 
     Note that run storages using SQL databases as backing stores should implement
     :py:class:`~dagster._core.storage.runs.SqlRunStorage`.
 
     Users should not directly instantiate concrete subclasses of this class; they are instantiated
     by internal machinery when ``dagit`` and ``dagster-graphql`` load, based on the values in the
@@ -397,26 +399,10 @@
     @abstractmethod
     def update_backfill(self, partition_backfill: PartitionBackfill):
         """Update a partition backfill in run storage."""
 
     def alembic_version(self) -> Optional[AlembicVersion]:
         return None
 
-    # Key Value Storage
-    #
-    # Stores arbitrary key-value pairs. Currently used for the cursor for the auto-reexecution
-    # deamon. Bundled into run storage for convenience.
-
-    def supports_kvs(self) -> bool:
-        return True
-
-    @abstractmethod
-    def kvs_get(self, keys: Set[str]) -> Mapping[str, str]:
-        """Retrieve the value for a given key in the current deployment."""
-
-    @abstractmethod
-    def kvs_set(self, pairs: Mapping[str, str]) -> None:
-        """Set the value for a given key in the current deployment."""
-
     @abstractmethod
     def replace_job_origin(self, run: "DagsterRun", job_origin: "ExternalPipelineOrigin") -> None:
         ...
```

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.0/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/migration.py` & `dagster-1.3.0/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/schema.py` & `dagster-1.3.0/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.0/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1133,29 +1133,26 @@
                 .where(BulkActionsTable.c.key == backfill_id)
                 .values(
                     status=partition_backfill.status.value,
                     body=serialize_value(partition_backfill),
                 )
             )
 
-    def supports_kvs(self) -> bool:
-        return True
-
-    def kvs_get(self, keys: Set[str]) -> Mapping[str, str]:
+    def get_cursor_values(self, keys: Set[str]) -> Mapping[str, str]:
         check.set_param(keys, "keys", of_type=str)
 
         with self.connect() as conn:
             rows = conn.execute(
                 db.select([KeyValueStoreTable.c.key, KeyValueStoreTable.c.value]).where(
                     KeyValueStoreTable.c.key.in_(keys)
                 ),
             )
             return {row.key: row.value for row in rows}
 
-    def kvs_set(self, pairs: Mapping[str, str]) -> None:
+    def set_cursor_values(self, pairs: Mapping[str, str]) -> None:
         check.mapping_param(pairs, "pairs", key_type=str, value_type=str)
         db_values = [{"key": k, "value": v} for k, v in pairs.items()]
 
         with self.connect() as conn:
             try:
                 conn.execute(KeyValueStoreTable.insert().values(db_values))
             except db_exc.IntegrityError:
```

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/schedules/base.py` & `dagster-1.3.0/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.0/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.0/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.0/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/sql.py` & `dagster-1.3.0/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/sqlite.py` & `dagster-1.3.0/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.0/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/tags.py` & `dagster-1.3.0/dagster/_core/storage/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 MAX_RETRIES_TAG = f"{SYSTEM_TAG_PREFIX}max_retries"
 RETRY_NUMBER_TAG = f"{SYSTEM_TAG_PREFIX}retry_number"
 RETRY_STRATEGY_TAG = f"{SYSTEM_TAG_PREFIX}retry_strategy"
 
 MAX_RUNTIME_SECONDS_TAG = f"{SYSTEM_TAG_PREFIX}max_runtime"
 
+CREATED_BY_TAG = f"{SYSTEM_TAG_PREFIX}created_by"
+
 USER_EDITABLE_SYSTEM_TAGS = [
     PRIORITY_TAG,
     MAX_RETRIES_TAG,
     RETRY_STRATEGY_TAG,
     MAX_RUNTIME_SECONDS_TAG,
 ]
```

### Comparing `dagster-1.2.7/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.0/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.0/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.0/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/system_config/objects.py` & `dagster-1.3.0/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/telemetry.py` & `dagster-1.3.0/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/telemetry_upload.py` & `dagster-1.3.0/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/test_utils.py` & `dagster-1.3.0/dagster/_core/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     Iterator,
     Mapping,
     NamedTuple,
     NoReturn,
     Optional,
     Sequence,
     TypeVar,
+    Union,
+    cast,
 )
 
 import pendulum
 from typing_extensions import Self
 
 from dagster import (
     Permissive,
@@ -466,19 +468,24 @@
 
 def get_mocked_system_timezone() -> Optional[str]:
     return _mocked_system_timezone["timezone"]
 
 
 # Test utility for creating a test workspace for a function
 class InProcessTestWorkspaceLoadTarget(WorkspaceLoadTarget):
-    def __init__(self, origin: InProcessCodeLocationOrigin):
-        self._origin = origin
+    def __init__(
+        self, origin: Union[InProcessCodeLocationOrigin, Sequence[InProcessCodeLocationOrigin]]
+    ):
+        self._origins = cast(
+            Sequence[InProcessCodeLocationOrigin],
+            origin if isinstance(origin, list) else [origin],
+        )
 
     def create_origins(self) -> Sequence[InProcessCodeLocationOrigin]:
-        return [self._origin]
+        return self._origins
 
 
 @contextmanager
 def in_process_test_workspace(
     instance: DagsterInstance,
     loadable_target_origin: LoadableTargetOrigin,
     container_image: Optional[str] = None,
```

### Comparing `dagster-1.2.7/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.0/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/config_schema.py` & `dagster-1.3.0/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/dagster_type.py` & `dagster-1.3.0/dagster/_core/types/dagster_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from dagster._config import (
     Array,
     ConfigType,
     Noneable as ConfigNoneable,
 )
 from dagster._core.definitions.events import DynamicOutput, Output, TypeCheck
 from dagster._core.definitions.metadata import (
-    MetadataEntry,
     MetadataValue,
     RawMetadataValue,
     normalize_metadata,
 )
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvariantViolationError
 from dagster._serdes import whitelist_for_serdes
 from dagster._seven import is_subclass
@@ -107,15 +106,14 @@
         name: t.Optional[str] = None,
         is_builtin: bool = False,
         description: t.Optional[str] = None,
         loader: t.Optional[DagsterTypeLoader] = None,
         required_resource_keys: t.Optional[t.Set[str]] = None,
         kind: DagsterTypeKind = DagsterTypeKind.REGULAR,
         typing_type: t.Any = t.Any,
-        metadata_entries: t.Optional[t.Sequence[MetadataEntry]] = None,
         metadata: t.Optional[t.Mapping[str, RawMetadataValue]] = None,
     ):
         check.opt_str_param(key, "key")
         check.opt_str_param(name, "name")
 
         check.invariant(not (name is None and key is None), "Must set key or name")
         if name is None:
@@ -153,15 +151,14 @@
 
         self.kind = check.inst_param(kind, "kind", DagsterTypeKind)
 
         self._typing_type = typing_type
 
         self._metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
-            check.opt_list_param(metadata_entries, "metadata_entries", of_type=MetadataEntry),
         )
 
     @public
     def type_check(self, context: "TypeCheckContext", value: object) -> TypeCheck:
         retval = self._type_check_fn(context, value)
 
         if not isinstance(retval, (bool, TypeCheck)):
```

### Comparing `dagster-1.2.7/dagster/_core/types/decorator.py` & `dagster-1.3.0/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.0/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.0/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/python_dict.py` & `dagster-1.3.0/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/python_set.py` & `dagster-1.3.0/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/python_tuple.py` & `dagster-1.3.0/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/types/transform_typing.py` & `dagster-1.3.0/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/utility_solids.py` & `dagster-1.3.0/dagster/_core/utility_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/utils.py` & `dagster-1.3.0/dagster/_core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             )
             warnings.warn(message)
     else:
         target_version = library_version_from_core_version(__version__)
         if library_version != target_version:
             message = (
                 f"Found version mismatch between `dagster` ({__version__}) "
-                f"expected library version ({target_version} "
+                f"expected library version ({target_version}) "
                 f"and `{library_name}` ({library_version})."
             )
             warnings.warn(message)
 
 
 def parse_env_var(env_var_str: str) -> Tuple[str, str]:
     if "=" in env_var_str:
```

### Comparing `dagster-1.2.7/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.0/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/workspace/config_schema.py` & `dagster-1.3.0/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/workspace/context.py` & `dagster-1.3.0/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/workspace/load.py` & `dagster-1.3.0/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/workspace/load_target.py` & `dagster-1.3.0/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_core/workspace/permissions.py` & `dagster-1.3.0/dagster/_core/workspace/permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     DELETE_PIPELINE_RUN = "delete_pipeline_run"
     RELOAD_REPOSITORY_LOCATION = "reload_repository_location"
     RELOAD_WORKSPACE = "reload_workspace"
     WIPE_ASSETS = "wipe_assets"
     LAUNCH_PARTITION_BACKFILL = "launch_partition_backfill"
     CANCEL_PARTITION_BACKFILL = "cancel_partition_backfill"
     EDIT_DYNAMIC_PARTITIONS = "edit_dynamic_partitions"
+    TOGGLE_AUTO_MATERIALIZE = "toggle_auto_materialize"
 
     def __str__(self) -> str:
         return str.__str__(self)
 
 
 VIEWER_PERMISSIONS: Dict[str, bool] = {
     Permissions.LAUNCH_PIPELINE_EXECUTION: False,
@@ -34,14 +35,15 @@
     Permissions.DELETE_PIPELINE_RUN: False,
     Permissions.RELOAD_REPOSITORY_LOCATION: False,
     Permissions.RELOAD_WORKSPACE: False,
     Permissions.WIPE_ASSETS: False,
     Permissions.LAUNCH_PARTITION_BACKFILL: False,
     Permissions.CANCEL_PARTITION_BACKFILL: False,
     Permissions.EDIT_DYNAMIC_PARTITIONS: False,
+    Permissions.TOGGLE_AUTO_MATERIALIZE: False,
 }
 
 EDITOR_PERMISSIONS: Dict[str, bool] = {
     Permissions.LAUNCH_PIPELINE_EXECUTION: True,
     Permissions.LAUNCH_PIPELINE_REEXECUTION: True,
     Permissions.START_SCHEDULE: True,
     Permissions.STOP_RUNNING_SCHEDULE: True,
@@ -51,14 +53,15 @@
     Permissions.DELETE_PIPELINE_RUN: True,
     Permissions.RELOAD_REPOSITORY_LOCATION: True,
     Permissions.RELOAD_WORKSPACE: True,
     Permissions.WIPE_ASSETS: True,
     Permissions.LAUNCH_PARTITION_BACKFILL: True,
     Permissions.CANCEL_PARTITION_BACKFILL: True,
     Permissions.EDIT_DYNAMIC_PARTITIONS: True,
+    Permissions.TOGGLE_AUTO_MATERIALIZE: True,
 }
 
 LOCATION_SCOPED_PERMISSIONS = {
     Permissions.LAUNCH_PIPELINE_EXECUTION,
     Permissions.LAUNCH_PIPELINE_REEXECUTION,
     Permissions.START_SCHEDULE,
     Permissions.STOP_RUNNING_SCHEDULE,
```

### Comparing `dagster-1.2.7/dagster/_core/workspace/workspace.py` & `dagster-1.3.0/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/__init__.py` & `dagster-1.3.0/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 def _fetch_persisted_cursors(
     instance: DagsterInstance, event_types: Sequence[DagsterEventType], logger: logging.Logger
 ) -> Dict[DagsterEventType, Optional[int]]:
     check.inst_param(instance, "instance", DagsterInstance)
     check.sequence_param(event_types, "event_types", of_type=DagsterEventType)
 
     # get the persisted cursor for each event type
-    persisted_cursors = instance.run_storage.kvs_get(
+    persisted_cursors = instance.daemon_cursor_storage.get_cursor_values(
         {_create_cursor_key(event_type) for event_type in event_types}
     )
 
     fetched_cursors: Dict[DagsterEventType, Optional[int]] = {}
     for event_type in event_types:
         raw_cursor_value = persisted_cursors.get(_create_cursor_key(event_type))
 
@@ -130,15 +130,15 @@
 
 
 def _persist_cursors(instance: DagsterInstance, cursors: Mapping[DagsterEventType, int]) -> None:
     check.inst_param(instance, "instance", DagsterInstance)
     check.mapping_param(cursors, "cursors", key_type=DagsterEventType, value_type=int)
 
     if cursors:
-        instance.run_storage.kvs_set(
+        instance.daemon_cursor_storage.set_cursor_values(
             {
                 _create_cursor_key(event_type): str(cursor_value)
                 for event_type, cursor_value in cursors.items()
             }
         )
```

### Comparing `dagster-1.2.7/dagster/_daemon/backfill.py` & `dagster-1.3.0/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/cli/__init__.py` & `dagster-1.3.0/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/controller.py` & `dagster-1.3.0/dagster/_daemon/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing_extensions import Self
 
 import dagster._check as check
 from dagster._core.host_representation.grpc_server_registry import GrpcServerRegistry
 from dagster._core.instance import DagsterInstance
 from dagster._core.workspace.context import IWorkspaceProcessContext, WorkspaceProcessContext
 from dagster._core.workspace.load_target import WorkspaceLoadTarget
+from dagster._daemon.asset_daemon import AssetDaemon
 from dagster._daemon.auto_run_reexecution.event_log_consumer import EventLogConsumerDaemon
 from dagster._daemon.daemon import (
     BackfillDaemon,
     DagsterDaemon,
     MonitoringDaemon,
     SchedulerDaemon,
     SensorDaemon,
@@ -330,14 +331,20 @@
         )
     elif daemon_type == BackfillDaemon.daemon_type():
         return BackfillDaemon(interval_seconds=DEFAULT_DAEMON_INTERVAL_SECONDS)
     elif daemon_type == MonitoringDaemon.daemon_type():
         return MonitoringDaemon(interval_seconds=instance.run_monitoring_poll_interval_seconds)
     elif daemon_type == EventLogConsumerDaemon.daemon_type():
         return EventLogConsumerDaemon()
+    elif daemon_type == AssetDaemon.daemon_type():
+        return AssetDaemon(
+            interval_seconds=instance.auto_materialize_minimum_interval_seconds
+            if instance.auto_materialize_minimum_interval_seconds is not None
+            else DEFAULT_DAEMON_INTERVAL_SECONDS
+        )
     else:
         raise Exception(f"Unexpected daemon type {daemon_type}")
 
 
 def all_daemons_healthy(
     instance: DagsterInstance,
     curr_time_seconds: Optional[float] = None,
```

### Comparing `dagster-1.2.7/dagster/_daemon/daemon.py` & `dagster-1.3.0/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.0/dagster/_daemon/monitoring/monitoring_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/sensor.py` & `dagster-1.3.0/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/types.py` & `dagster-1.3.0/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_daemon/workspace.py` & `dagster-1.3.0/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_generate/download.py` & `dagster-1.3.0/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_generate/generate.py` & `dagster-1.3.0/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.0/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.0/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/__init__.py` & `dagster-1.3.0/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/client.py` & `dagster-1.3.0/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/compile.py` & `dagster-1.3.0/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/impl.py` & `dagster-1.3.0/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/protos/api.proto` & `dagster-1.3.0/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/server.py` & `dagster-1.3.0/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/server_watcher.py` & `dagster-1.3.0/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/types.py` & `dagster-1.3.0/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_grpc/utils.py` & `dagster-1.3.0/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_legacy/__init__.py` & `dagster-1.3.0/dagster/_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_loggers/__init__.py` & `dagster-1.3.0/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_module_alias_map.py` & `dagster-1.3.0/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_scheduler/scheduler.py` & `dagster-1.3.0/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_scheduler/stale.py` & `dagster-1.3.0/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_serdes/__init__.py` & `dagster-1.3.0/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_serdes/config_class.py` & `dagster-1.3.0/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_serdes/ipc.py` & `dagster-1.3.0/dagster/_serdes/ipc.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,39 +193,25 @@
             message = _process_line(file_pointer)
 
 
 # Windows subprocess termination utilities
 # https://stefan.sofa-rockers.org/2013/08/15/handling-sub-process-hierarchies-python-linux-os-x/
 
 
-def _preexec_fn():
-    # See: https://bugs.python.org/issue14892 - prevent lines like "import readline" from hanging
-    # in the subprocess
-    signal.signal(signal.SIGTTOU, signal.SIG_IGN)
-
-    # the new subprocess will be in its own process group so that CTRL-Cing the parent process
-    # doesn't immediately interrupt the child process as well.
-    os.setpgrp()
-
-
 def open_ipc_subprocess(parts: Sequence[str], **kwargs: object) -> Popen[bytes]:
     """Sets the correct flags to support graceful termination."""
     check.list_param(parts, "parts", str)
 
     creationflags = 0
-    preexec_fn = None
     if sys.platform == "win32":
         creationflags = subprocess.CREATE_NEW_PROCESS_GROUP
-    else:
-        # Works on all UNIX systems (but not WASI, see: https://docs.python.org/3/library/os.html#os.setpgrp)
-        preexec_fn = _preexec_fn
+
     return subprocess.Popen(
         parts,
         creationflags=creationflags,
-        preexec_fn=preexec_fn,
         **kwargs,
     )
 
 
 def interrupt_ipc_subprocess(proc: Popen[bytes]) -> None:
     """Send CTRL_BREAK on Windows, SIGINT on other platforms."""
     if sys.platform == "win32":
```

### Comparing `dagster-1.2.7/dagster/_serdes/serdes.py` & `dagster-1.3.0/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_serdes/utils.py` & `dagster-1.3.0/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_seven/__init__.py` & `dagster-1.3.0/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_seven/abc.py` & `dagster-1.3.0/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_seven/compat/pendulum.py` & `dagster-1.3.0/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/__init__.py` & `dagster-1.3.0/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/alert.py` & `dagster-1.3.0/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/backcompat.py` & `dagster-1.3.0/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/backoff.py` & `dagster-1.3.0/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/cached_method.py` & `dagster-1.3.0/dagster/_utils/cached_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 class _Sentinel:
     ...
 
 
 NO_VALUE_IN_CACHE_SENTINEL: Final = _Sentinel()
 NO_ARGS_HASH_VALUE = 0
 
+CACHED_METHOD_FIELD_SUFFIX = "_cached__internal__"
+
 
 def cached_method(method: Callable[Concatenate[S, P], T]) -> Callable[Concatenate[S, P], T]:
     """Caches the results of a method call.
 
     Usage:
 
         .. code-block:: python
@@ -53,15 +55,15 @@
 
     With this decorator, the first two would point to the same cache entry, and non-kwarg arguments
     are not allowed.
     """
 
     @wraps(method)
     def helper(self: S, *args: P.args, **kwargs: P.kwargs) -> T:
-        cache_attr_name = method.__name__ + "_cache"
+        cache_attr_name = method.__name__ + CACHED_METHOD_FIELD_SUFFIX
         if not hasattr(self, cache_attr_name):
             cache: Dict[Hashable, T] = {}
             setattr(self, cache_attr_name, cache)
         else:
             cache = getattr(self, cache_attr_name)
 
         key = _make_key(args, kwargs)
```

### Comparing `dagster-1.2.7/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.0/dagster/_utils/caching_instance_queryer.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,24 +301,25 @@
                     EventRecordsFilter(
                         event_type=DagsterEventType.ASSET_OBSERVATION,
                         asset_key=asset_key,
                         before_cursor=before_cursor,
                     ),
                     ascending=False,
                 )
-            )
+            ),
+            None,
         )
 
     @cached_method
     def next_version_record(
         self,
         *,
         asset_key: AssetKey,
         after_cursor: Optional[int],
-        data_version: DataVersion,
+        data_version: Optional[DataVersion],
     ) -> Optional["EventLogRecord"]:
         from dagster._core.event_api import EventRecordsFilter
 
         for record in self.instance.get_event_records(
             EventRecordsFilter(
                 event_type=DagsterEventType.ASSET_OBSERVATION,
                 asset_key=asset_key,
@@ -348,19 +349,19 @@
         """
         previous_version_record = self.get_observation_record(
             asset_key=observable_source_asset_key,
             # we're looking for if a new version exists after `after_cursor`, so we need to know
             # what the version was before `after_cursor`
             before_cursor=after_cursor,
         )
-        if previous_version_record is None:
-            return False
-        previous_version = extract_data_version_from_entry(previous_version_record.event_log_entry)
-        if previous_version is None:
-            return False
+        previous_version = (
+            extract_data_version_from_entry(previous_version_record.event_log_entry)
+            if previous_version_record is not None
+            else None
+        )
 
         next_version_record = self.next_version_record(
             asset_key=observable_source_asset_key,
             after_cursor=after_cursor,
             data_version=previous_version,
         )
         return next_version_record is not None
```

### Comparing `dagster-1.2.7/dagster/_utils/dagster_type.py` & `dagster-1.3.0/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/error.py` & `dagster-1.3.0/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/external.py` & `dagster-1.3.0/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/forked_pdb.py` & `dagster-1.3.0/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/hosted_user_process.py` & `dagster-1.3.0/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/indenting_printer.py` & `dagster-1.3.0/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/interrupts.py` & `dagster-1.3.0/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/log.py` & `dagster-1.3.0/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/merger.py` & `dagster-1.3.0/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/net.py` & `dagster-1.3.0/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/schedules.py` & `dagster-1.3.0/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/tags.py` & `dagster-1.3.0/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/temp_file.py` & `dagster-1.3.0/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/test/__init__.py` & `dagster-1.3.0/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.0/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.0/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.0/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/timing.py` & `dagster-1.3.0/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/typing_api.py` & `dagster-1.3.0/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster/_utils/yaml_utils.py` & `dagster-1.3.0/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/dagster.egg-info/PKG-INFO` & `dagster-1.3.0/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.2.7
+Version: 1.3.0
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.2.7/dagster.egg-info/SOURCES.txt` & `dagster-1.3.0/dagster.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,18 @@
 dagster/_config/primitive_mapping.py
 dagster/_config/snap.py
 dagster/_config/source.py
 dagster/_config/stack.py
 dagster/_config/traversal_context.py
 dagster/_config/type_printer.py
 dagster/_config/validate.py
-dagster/_config/structured_config/__init__.py
-dagster/_config/structured_config/typing_utils.py
-dagster/_config/structured_config/utils.py
+dagster/_config/pythonic_config/__init__.py
+dagster/_config/pythonic_config/attach_other_object_to_context.py
+dagster/_config/pythonic_config/typing_utils.py
+dagster/_config/pythonic_config/utils.py
 dagster/_core/__init__.py
 dagster/_core/assets.py
 dagster/_core/code_pointer.py
 dagster/_core/debug.py
 dagster/_core/decorator_utils.py
 dagster/_core/errors.py
 dagster/_core/event_api.py
@@ -288,14 +289,15 @@
 dagster/_core/storage/__init__.py
 dagster/_core/storage/asset_value_loader.py
 dagster/_core/storage/base_storage.py
 dagster/_core/storage/captured_log_manager.py
 dagster/_core/storage/cloud_storage_compute_log_manager.py
 dagster/_core/storage/compute_log_manager.py
 dagster/_core/storage/config.py
+dagster/_core/storage/daemon_cursor.py
 dagster/_core/storage/db_io_manager.py
 dagster/_core/storage/file_manager.py
 dagster/_core/storage/fs_io_manager.py
 dagster/_core/storage/input_manager.py
 dagster/_core/storage/io_manager.py
 dagster/_core/storage/legacy_storage.py
 dagster/_core/storage/local_compute_log_manager.py
@@ -444,14 +446,15 @@
 dagster/_core/workspace/context.py
 dagster/_core/workspace/load.py
 dagster/_core/workspace/load_target.py
 dagster/_core/workspace/permissions.py
 dagster/_core/workspace/workspace.py
 dagster/_daemon/__init__.py
 dagster/_daemon/__main__.py
+dagster/_daemon/asset_daemon.py
 dagster/_daemon/backfill.py
 dagster/_daemon/controller.py
 dagster/_daemon/daemon.py
 dagster/_daemon/sensor.py
 dagster/_daemon/types.py
 dagster/_daemon/workspace.py
 dagster/_daemon/auto_run_reexecution/__init__.py
```

### Comparing `dagster-1.2.7/dagster.egg-info/requires.txt` & `dagster-1.3.0/dagster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dagster-1.2.7/setup.py` & `dagster-1.3.0/setup.py`

 * *Files identical despite different names*


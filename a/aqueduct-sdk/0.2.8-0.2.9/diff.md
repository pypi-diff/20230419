# Comparing `tmp/aqueduct-sdk-0.2.8.tar.gz` & `tmp/aqueduct-sdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.2.8.tar", last modified: Wed Mar 29 16:47:06 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.2.9.tar", last modified: Wed Apr  5 19:17:31 2023, max compression
```

## Comparing `aqueduct-sdk-0.2.8.tar` & `aqueduct-sdk-0.2.9.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.978033 aqueduct-sdk-0.2.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5995 2023-03-29 16:47:06.978033 aqueduct-sdk-0.2.8/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.958033 aqueduct-sdk-0.2.8/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1474 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.958033 aqueduct-sdk-0.2.8/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3551 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11574 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6632 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24898 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.962033 aqueduct-sdk-0.2.8/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21791 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6404 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7033 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/backend/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30654 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.962033 aqueduct-sdk-0.2.8/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6211 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45150 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4450 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8272 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.962033 aqueduct-sdk-0.2.8/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/globals/dag.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.966033 aqueduct-sdk-0.2.8/aqueduct/integrations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/airflow_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/aws_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11711 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/databricks_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7231 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/dynamic_k8s_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4767 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/google_sheets_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      469 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/k8s_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      472 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/lambda_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8850 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/mongodb_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8924 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/s3_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/salesforce_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3208 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/spark_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11770 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/integrations/sql_integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.970033 aqueduct-sdk-0.2.8/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1733 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2814 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2279 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/models/integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7459 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.970033 aqueduct-sdk-0.2.8/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15599 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.974033 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.974033 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.974033 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6072 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.974033 aqueduct-sdk-0.2.8/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.8/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11395 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7700 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.974033 aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5995 2023-03-29 16:47:06.000000 aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-03-29 16:47:06.000000 aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-29 16:47:06.000000 aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      287 2023-03-29 16:47:06.000000 aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-03-29 16:47:06.000000 aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:47:06.978033 aqueduct-sdk-0.2.8/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      286 2023-03-28 21:01:21.000000 aqueduct-sdk-0.2.8/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-29 16:47:06.978033 aqueduct-sdk-0.2.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1104 2023-03-28 21:04:23.000000 aqueduct-sdk-0.2.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6944 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1474 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/artifacts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/base_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/bool_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/generic_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11574 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/numeric_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6632 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/preview.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/system_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24898 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/artifacts/table_artifact.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22951 2023-04-04 21:44:50.000000 aqueduct-sdk-0.2.9/aqueduct/backend/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6404 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/backend/response_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7033 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/backend/response_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32293 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/constants/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/constants/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6511 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/constants/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/constants/exports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/constants/metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    45150 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/decorator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3637 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/error.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4450 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/flow_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8272 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/github.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.028932 aqueduct-sdk-0.2.9/aqueduct/globals/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      323 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/globals/dag.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/integrations/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      485 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/airflow_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      659 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/aws_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11711 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/connect_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/databricks_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7231 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/dynamic_k8s_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4767 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/google_sheets_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      469 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/k8s_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      472 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/lambda_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8850 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/mongodb_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8924 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/s3_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/salesforce_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3208 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/save.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/spark_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11770 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/integrations/sql_integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      507 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1733 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2814 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/models/dag_rules.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2279 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/models/integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7459 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/models/operators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/schedule.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/connect_config_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/dag_delta_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/dag_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/decorator_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/enum_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/flow_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/helpers_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/metric_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/naming_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15599 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/serialization_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/python_function.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.032932 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6072 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/tests/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/type_annotations.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/aqueduct/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/dag_deltas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.2.9/aqueduct/utils/describe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/format.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/function_packaging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/local_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/naming.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14431 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/type_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7700 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/aqueduct/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6944 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3121 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-05 19:17:31.000000 aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-10.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-7.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-8.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-04-04 21:43:24.000000 aqueduct-sdk-0.2.9/requirements/python-3-9.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-05 19:17:31.036932 aqueduct-sdk-0.2.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1104 2023-04-04 22:01:25.000000 aqueduct-sdk-0.2.9/setup.py
```

### Comparing `aqueduct-sdk-0.2.8/PKG-INFO` & `aqueduct-sdk-0.2.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python SDK for the Aqueduct prediction infrastructure
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [<img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "35%" />](https://www.aqueducthq.com)
 
-## Aqueduct: The easiest way to run ML on any cloud infrastructure
+## Aqueduct: The easiest way to run ML on any cloud
 
+[![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
 
-**Aqueduct enables you to define, deploy and monitor robust ML pipelines on any cloud infrastructure.** Check out our [quickstart guide](https://docs.aqueducthq.com/quickstart-guide)!
+**Aqueduct enables you to easily run machine learning tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
-Aqueduct gives you a simple Python-native API to define machine learning pipelines, the ability to deploy those pipelines on your existing infrastructure (e.g., Spark, Kubernetes, Lambda), and visibility into the code, data, and metadata associated with your workflows. 
-Aqueduct is fully open-source and runs securely in your cloud.
+Aqueduct is an open-source MLOps framework that allows you to define ML tasks in vanilla Python, run those tasks on any infrastructure you'd like to use, and gain visibility into the execution and performance of your ML. **[See what tools Aqueduct works with. →](https://aqueducthq.com/integrations/)**
+
+Here's how you can get started: 
 
-You can install Aqueduct via `pip`:
 ```bash
 pip3 install aqueduct-ml
 aqueduct start
 ```
 
-Now, we can create our first workflow:
-
-```python
-from aqueduct import Client, op, metric
-
-client = Client()
+### How it works
 
-@op
-def transform_data(reviews):
-    reviews['strlen'] = reviews['review'].str.len()
-    return reviews
+Aqueduct's Python native API allows you to define ML tasks in regular Python code. You can connect Aqueduct to your existing cloud infrastructure ([docs](https://docs.aqueducthq.com/integrations)), and Aqueduct will seamlessly move your code from your laptop to the cloud or between different cloud infrastructure layers. 
 
+<!--- TODO(vikram): Modify this once we add support for switching into/out of Databricks in a single workflow. --->
+For example, we can define a pipeline that trains a model on Kubernetes using a GPU and validates that model in AWS Lambda in a few lines of Python: 
 
-demo_db = client.integration("aqueduct_demo")
-reviews_table = demo_db.sql("select * from hotel_reviews;")
-
-strlen_table = transform_data(reviews_table)
-demo_db.save(strlen_table, "strlen_table", "replace)
+```python
+@op(
+  engine='eks-us-east-2', 
+  resources={'gpu_resource_name': 'nvidia.com/gpu'}
+)
+def train(features):
+  return model.train(features)
+
+@metric(engine='lambda-us-east-2')
+def validate(model):
+    return validation_test(model)
 
-client.publish_flow(name="review_strlen", artifacts=[strlen_table])
+validate(train(features))
 ```
 
-Once we've created a workflow, we can view that workflow in the Aqueduct UI: 
+Once you publish this workflow to Aqueduct, you can see it on the UI: 
 
-![image](https://user-images.githubusercontent.com/867892/196529730-3c9582d5-8692-495d-a7df-8eb62ddf305f.png)
+![image](https://user-images.githubusercontent.com/867892/228295996-4ba3de23-3106-431d-93a9-afd8d77a707b.png)
+
+To see how to build your first workflow, check out our **[quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 ## Why Aqueduct?
 
-The engineering required to get data science & machine learning projects in production slows down data teams. Aqueduct automates away that engineering and allows you to define robust data & ML pipelines in a few lines of code and run them anywhere.
+MLOps has become a [tangled mess of siloed infrastructure](https://aqueducthq.com/post/the-mlops-knot/). Most teams need to set up and operate many different cloud infrastructure tools to run ML effectively, but these tools have disparate APIs and interoperate poorly.
+
+Aqueduct provides a single interface to running machine learning tasks on your existing cloud infrastructure — Kubernetes, Spark, Lambda, etc. From the same Python API, you can run code across any or all of these systems seamlessly and gain visibility into how your code is performing.
 
 * **Python-native pipeline API**: Aqueduct’s API allows you define your workflows in vanilla Python, so you can get code into production quickly and effectively. No more DSLs or YAML configs to worry about.
 * **Integrated with your infrastructure**: Workflows defined in Aqueduct can run on any cloud infrastructure you use, like Kubernetes, Spark, Airflow, or AWS Lambda. You can get all the benefits of Aqueduct without having to rip-and-replace your existing tooling.
 * **Centralized visibility into code, data, & metadata**: Once your workflows are in production, you need to know what’s running, whether it’s working, and when it breaks. Aqueduct gives you visibility into what code, data, metrics, and metadata are generated by each workflow run, so you can have confidence that your pipelines work as expected — and know immediately when they don’t.
-* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that nothing is ever leaving your cloud.
+* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that your data and code are secure.
 
 ## Overview & Examples
 
 The core abstraction in Aqueduct is a [Workflow](https://docs.aqueducthq.com/workflows), which is a sequence of [Artifacts](https://docs.aqueducthq.com/artifacts) (data) that are transformed by [Operators](https://docs.aqueducthq.com/operators) (compute). 
 The input Artifact(s) for a Workflow is typically loaded from a database, and the output Artifact(s) are typically persisted back to a database. 
 Each Workflow can either be run on a fixed schedule or triggered on-demand.
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct/__init__.py` & `aqueduct-sdk-0.2.9/aqueduct/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/base_artifact.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/bool_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,28 +44,31 @@
 
 def create_param_artifact(
     dag: DAG,
     param_name: str,
     default: Any,
     description: str,
     explicitly_named: bool,
+    is_local_data: bool = False,
 ) -> BaseArtifact:
     """Creates a parameter operator and return an artifact that can be fed into other operators.
 
     Args:
         dag:
             The dag to check for collisions against.
         param_name:
             The name for the parameter.
         default:
             The default value for the new parameter.
         description:
             A description for the parameter.
         explicitly_named:
             Whether this parameter was explicitly created with `client.create_param()`.
+        is_local_data:
+            Whether this parameter comes from a local data source.
     """
     if default is None:
         raise InvalidUserArgumentException("Parameter default value cannot be None.")
 
     artifact_type = infer_artifact_type(default)
     param_spec = construct_param_spec(default, artifact_type)
     operator_id = generate_uuid()
@@ -85,13 +88,14 @@
                 ),
                 output_artifacts=[
                     ArtifactMetadata(
                         id=output_artifact_id,
                         name=sanitize_artifact_name(param_name),
                         type=artifact_type,
                         explicitly_named=explicitly_named,
+                        from_local_data=is_local_data,
                     ),
                 ],
             ),
         ],
     )
     return to_artifact_class(dag, output_artifact_id, artifact_type, default)
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/generic_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/numeric_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/preview.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.2.9/aqueduct/artifacts/table_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.2.9/aqueduct/backend/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import requests
 from aqueduct.constants.enums import ExecutionStatus, K8sClusterActionType, RuntimeType, ServiceType
 from aqueduct.error import (
     AqueductError,
     ClientValidationError,
     InternalServerError,
     InvalidRequestError,
+    InvalidUserActionException,
     NoConnectedIntegrationsException,
     ResourceNotFoundError,
     UnprocessableEntityError,
 )
 from aqueduct.logger import logger
 from aqueduct.models.dag import DAG
 from aqueduct.models.integration import Integration, IntegrationInfo
@@ -36,14 +37,18 @@
     ListWorkflowSavedObjectsResponse,
     PreviewResponse,
     RegisterAirflowWorkflowResponse,
     RegisterWorkflowResponse,
     SavedObjectUpdate,
 )
 
+# The maximum http request size is capped at 32 MB. DAG containing
+# local data parameter(s) should not go beyond this value.
+MAX_REQUEST_BODY_SIZE = 32 << 20
+
 
 class APIClient:
     """
     Internal client class used to send requests to the aqueduct cluster.
     """
 
     HTTP_PREFIX = "http://"
@@ -399,14 +404,22 @@
             A PreviewResponse object, parsed from the preview endpoint's response.
         """
         headers = self._generate_auth_headers()
         body = {
             "dag": dag.json(exclude_none=True),
         }
 
+        if len(body["dag"]) > MAX_REQUEST_BODY_SIZE and any(
+            artifact_metadata.from_local_data for artifact_metadata in list(dag.artifacts.values())
+        ):
+            raise InvalidUserActionException(
+                "Local Data after serialization is too large. Aqueduct uses json serialization. The maximum size of workflow with local data is %s in bytes, the current size is %s in bytes."
+                % (MAX_REQUEST_BODY_SIZE, len(body["dag"]))
+            )
+
         files: Dict[str, IO[Any]] = {}
         for op in dag.list_operators():
             file = op.file()
             if file:
                 files[str(op.id)] = io.BytesIO(file)
 
         url = self.construct_full_url(self.PREVIEW_ROUTE)
@@ -448,14 +461,22 @@
         headers = self._generate_auth_headers()
         # This header value will be string "True" or "False"
         headers.update({"run-now": str(run_now)})
         body = {
             "dag": dag.json(exclude_none=True),
         }
 
+        if len(body["dag"]) > MAX_REQUEST_BODY_SIZE and any(
+            artifact_metadata.from_local_data for artifact_metadata in list(dag.artifacts.values())
+        ):
+            raise InvalidUserActionException(
+                "Local Data after serialization is too large. Aqueduct uses json serialization. The maximum size of workflow with local data is %s in bytes, the current size is %s in bytes."
+                % (MAX_REQUEST_BODY_SIZE, len(body["dag"]))
+            )
+
         files: Dict[str, IO[Any]] = {}
         for op in dag.list_operators():
             file = op.file()
             if file:
                 files[str(op.id)] = io.BytesIO(file)
 
         return headers, body, files
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.2.9/aqueduct/backend/response_helpers.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/backend/response_models.py` & `aqueduct-sdk-0.2.9/aqueduct/backend/response_models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/client.py` & `aqueduct-sdk-0.2.9/aqueduct/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 from aqueduct.models.integration import Integration, IntegrationInfo
 from aqueduct.models.operators import ParamSpec
 from aqueduct.utils.dag_deltas import (
     SubgraphDAGDelta,
     apply_deltas_to_dag,
     validate_overwriting_parameters,
 )
-from aqueduct.utils.serialization import deserialize
+from aqueduct.utils.local_data import validate_local_data
+from aqueduct.utils.serialization import deserialize, extract_val_from_local_data
 from aqueduct.utils.type_inference import _base64_string_to_bytes, infer_artifact_type
 from aqueduct.utils.utils import (
     construct_param_spec,
     find_flow_with_user_supplied_id_and_name,
     generate_engine_config,
     generate_flow_schedule,
     generate_ui_url,
@@ -174,37 +175,60 @@
 
         Returns:
             A github integration object linked to the repo and branch.
 
         """
         return Github(repo_url=repo, branch=branch)
 
-    def create_param(self, name: str, default: Any, description: str = "") -> BaseArtifact:
+    def create_param(
+        self,
+        name: str,
+        default: Any,
+        description: str = "",
+        use_local: bool = False,
+        as_type: Optional[ArtifactType] = None,
+        format: Optional[str] = None,
+    ) -> BaseArtifact:
         """Creates a parameter artifact that can be fed into other operators.
 
         Parameter values are configurable at runtime.
 
         Args:
             name:
                 The name to assign this parameter.
             default:
                 The default value to give this parameter, if no value is provided.
-                Every parameter must have a default.
+                Every parameter must have a default. If we decide to use local data,
+                a path to the local data file must be specified.
             description:
                 A description of what this parameter represents.
-
+            use_local:
+                Whether this parameter uses local data source or not.
+            as_type:
+                The expected type of the local data. Only supported types are ArtifactType.TABLE and ArtifactType.IMAGE.
+            format:
+                If local data type is ArtifactType.TABLE, the user has to specify the table format.
+                We currently support "json", "csv", and "parquet".
         Returns:
             A parameter artifact.
         """
+        if use_local:
+            if not isinstance(default, str):
+                raise InvalidUserArgumentException(
+                    "The default value must be a path to local data."
+                )
+            validate_local_data(default, as_type, format)
+            default = extract_val_from_local_data(default, as_type, format)
         return create_param_artifact(
             self._dag,
             name,
             default,
             description,
             explicitly_named=True,
+            is_local_data=use_local,
         )
 
     def connect_integration(
         self,
         name: str,
         service: Union[str, ServiceType],
         config: Union[Dict[str, str], IntegrationConfig],
@@ -423,14 +447,15 @@
         engine: Optional[str] = None,
         artifacts: Optional[Union[BaseArtifact, List[BaseArtifact]]] = None,
         metrics: Optional[List[NumericArtifact]] = None,
         checks: Optional[List[BoolArtifact]] = None,
         k_latest_runs: Optional[int] = None,
         source_flow: Optional[Union[Flow, str, uuid.UUID]] = None,
         run_now: Optional[bool] = None,
+        use_local: Optional[bool] = False,
     ) -> Flow:
         """Uploads and kicks off the given flow in the system.
 
         If a flow already exists with the same name, the existing flow will be updated
         to this new state.
 
         The default execution engine of the flow is Aqueduct. In order to specify which
@@ -470,14 +495,16 @@
                 this bound are garbage collected. Defaults to persisting all runs.
             source_flow:
                 Used to identify the source flow for this flow. This can be identified
                 via an object (Flow), name (str), or id (str or uuid).
             run_now:
                 Used to specify if the flow should run immediately at publish time. The default
                 behavior is 'True'.
+            use_local:
+                Must be set if any artifact in the flow is derived from local data.
 
         Raises:
             InvalidUserArgumentException:
                 An invalid combination of parameters was provided.
             InvalidCronStringException:
                 An error occurred because the supplied schedule is invalid.
             IncompleteFlowException:
@@ -578,14 +605,20 @@
                     include_saves=True,
                     include_metrics=implicitly_include_metrics,
                     include_checks=implicitly_include_checks,
                 ),
             ],
             make_copy=True,
         )
+        if not use_local and any(
+            artifact_metadata.from_local_data for artifact_metadata in list(dag.artifacts.values())
+        ):
+            raise InvalidUserActionException(
+                "Cannot create a flow with local data. Consider setting `use_local` to True to publish a workflow with local data parameters."
+            )
         dag.metadata = Metadata(
             name=name,
             description=description,
             schedule=flow_schedule,
             retention_policy=retention_policy,
         )
         dag.set_engine_config(
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct/constants/enums.py` & `aqueduct-sdk-0.2.9/aqueduct/constants/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,14 +226,27 @@
     ACTIVE = "Active"
     # The cluster is being deleted.
     TERMINATING = "Terminating"
     # The cluster is terminated.
     TERMINATED = "Terminated"
 
 
+class LocalDataTableFormat(str, Enum, metaclass=MetaEnum):
+    CSV = "CSV"
+    JSON = "JSON"
+    PARQUET = "Parquet"
+
+
+class LocalDataSerializationType(str, Enum, metaclass=MetaEnum):
+    CSV_TABLE = "csv_table"
+    JSON_TABLE = "json_table"
+    PARQUET_TABLE = "parquet_table"
+    IMAGE = "image"
+
+
 class K8sClusterActionType(str, Enum, metaclass=MetaEnum):
     CREATE = "create"
     UPDATE = "update"
     DELETE = "delete"
     FORCE_DELETE = "force-delete"
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct/decorator.py` & `aqueduct-sdk-0.2.9/aqueduct/decorator.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/error.py` & `aqueduct-sdk-0.2.9/aqueduct/error.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/flow.py` & `aqueduct-sdk-0.2.9/aqueduct/flow.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/flow_run.py` & `aqueduct-sdk-0.2.9/aqueduct/flow_run.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/github.py` & `aqueduct-sdk-0.2.9/aqueduct/github.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/aws_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/aws_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/connect_config.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/connect_config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/dynamic_k8s_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/dynamic_k8s_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/google_sheets_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/google_sheets_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/mongodb_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/mongodb_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/parameters.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/s3_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/s3_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/salesforce_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/salesforce_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/save.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/save.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/integrations/sql_integration.py` & `aqueduct-sdk-0.2.9/aqueduct/integrations/sql_integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/models/config.py` & `aqueduct-sdk-0.2.9/aqueduct/models/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/models/dag.py` & `aqueduct-sdk-0.2.9/aqueduct/models/dag.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.2.9/aqueduct/models/dag_rules.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/models/integration.py` & `aqueduct-sdk-0.2.9/aqueduct/models/integration.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/models/operators.py` & `aqueduct-sdk-0.2.9/aqueduct/models/operators.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/schedule.py` & `aqueduct-sdk-0.2.9/aqueduct/schedule.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/tests/utils.py` & `aqueduct-sdk-0.2.9/aqueduct/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/dag_deltas.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/describe.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/naming.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/serialization.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 import json
 import os
 import shutil
 from typing import Any, Callable, Dict, List, Optional, Union, cast
 
 import cloudpickle as pickle
 import pandas as pd
-from aqueduct.constants.enums import ArtifactType, S3SerializationType, SerializationType
+from aqueduct.constants.enums import (
+    ArtifactType,
+    LocalDataSerializationType,
+    LocalDataTableFormat,
+    S3SerializationType,
+    SerializationType,
+)
+from aqueduct.utils.local_data import _convert_to_local_data_table_format
 from aqueduct.utils.type_inference import infer_artifact_type
 from bson import json_util as bson_json_util
 from PIL import Image
 from pydantic import BaseModel
 
 from .format import DEFAULT_ENCODING
 from .function_packaging import _make_temp_dir
@@ -64,14 +71,30 @@
     return content.decode(DEFAULT_ENCODING)
 
 
 def _read_bytes_content(content: bytes) -> bytes:
     return content
 
 
+def _read_local_csv_table_content(path: str) -> Any:
+    return pd.read_csv(path)
+
+
+def _read_local_json_table_content(path: str) -> Any:
+    return pd.read_json(path, orient="table")
+
+
+def _read_local_parquet_table_content(path: str) -> Any:
+    return pd.read_parquet(path)
+
+
+def _read_local_image_content(path: str) -> Any:
+    return Image.open(path)
+
+
 # Returns a tf.keras.Model type. We don't assume that every user has it installed,
 # so we return "Any" type.
 def _read_tf_keras_model(content: bytes) -> Any:
     temp_model_dir = None
     try:
         temp_model_dir = _make_temp_dir()
         model_file_path = os.path.join(temp_model_dir, _TEMP_KERAS_MODEL_NAME)
@@ -94,14 +117,22 @@
     SerializationType.IMAGE: _read_image_content,
     SerializationType.STRING: _read_string_content,
     SerializationType.BYTES: _read_bytes_content,
     SerializationType.TF_KERAS: _read_tf_keras_model,
     SerializationType.BSON_TABLE: _read_bson_table_content,
 }
 
+# Not intended for use outside of `deserialize()`.
+__local_data_deserialization_function_mapping: Dict[str, Callable[[str], Any]] = {
+    LocalDataSerializationType.CSV_TABLE: _read_local_csv_table_content,
+    LocalDataSerializationType.JSON_TABLE: _read_local_json_table_content,
+    LocalDataSerializationType.PARQUET_TABLE: _read_local_parquet_table_content,
+    LocalDataSerializationType.IMAGE: _read_local_image_content,
+}
+
 
 def check_and_fetch_pickled_collection_format(
     serialization_type: Union[SerializationType, S3SerializationType],
     deserialized_val: Any,
 ) -> Optional[PickleableCollectionSerializationFormat]:
     """If a value that has undergone one round of deserialization is in the form of a
     `PickleableCollectionSerializationFormat`, we will load up that class and return it.
@@ -158,14 +189,34 @@
     # We wanted to keep the readability of json, particularly for the UI, so we decided to distinguish
     # between the two here using the expected artifact type, at deserialization time.
     if artifact_type == ArtifactType.TUPLE:
         return tuple(deserialized_val)
     return deserialized_val
 
 
+def deserialize_from_local_data(
+    serialization_type: LocalDataSerializationType,
+    artifact_type: ArtifactType,
+    path: str,
+) -> Any:
+    """Deserializes a file object with specified path into the appropriate python object.
+
+    Handles serialization for local data.
+    """
+    deserialization_function_mapping = __local_data_deserialization_function_mapping
+    if serialization_type not in deserialization_function_mapping:
+        raise Exception("Unsupported serialization type %s" % serialization_type)
+
+    deserialized_val = deserialization_function_mapping[serialization_type](path)
+
+    if artifact_type == ArtifactType.TUPLE:
+        return tuple(deserialized_val)
+    return deserialized_val
+
+
 def _write_table_output(output: pd.DataFrame) -> bytes:
     # This serialization format should also be consistent with go code in
     # src/golang/lib/workflow/artifact/artifact.go SampleContent() method.
     output_str = cast(str, output.to_json(orient="table", date_format="iso", index=False))
     return output_str.encode(DEFAULT_ENCODING)
 
 
@@ -296,7 +347,38 @@
     else:
         raise Exception("Unsupported artifact type %s" % artifact_type)
 
     assert serialization_type is not None, (
         "Unimplemented case for artifact type `%s`" % artifact_type
     )
     return serialization_type
+
+
+def extract_val_from_local_data(
+    path: str, as_type: Optional[ArtifactType], format: Optional[str]
+) -> Any:
+    """Extract value of specified type in Local Data."""
+    artifact_type = as_type
+    local_data_path = path
+    local_data_format = _convert_to_local_data_table_format(format)
+    if artifact_type == ArtifactType.TABLE:
+        if local_data_format == LocalDataTableFormat.CSV:
+            deserialized_val = deserialize_from_local_data(
+                LocalDataSerializationType.CSV_TABLE, artifact_type, local_data_path
+            )
+        elif local_data_format == LocalDataTableFormat.JSON:
+            deserialized_val = deserialize_from_local_data(
+                LocalDataSerializationType.JSON_TABLE, artifact_type, local_data_path
+            )
+        elif local_data_format == LocalDataTableFormat.PARQUET:
+            deserialized_val = deserialize_from_local_data(
+                LocalDataSerializationType.PARQUET_TABLE, artifact_type, local_data_path
+            )
+        else:
+            raise Exception("Unsupported file format %s" % format)
+    elif artifact_type == ArtifactType.IMAGE:
+        deserialized_val = deserialize_from_local_data(
+            LocalDataSerializationType.IMAGE, artifact_type, local_data_path
+        )
+    else:
+        raise Exception("Unsupported artifact type %s" % artifact_type)
+    return deserialized_val
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct/utils/utils.py` & `aqueduct-sdk-0.2.9/aqueduct/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python SDK for the Aqueduct prediction infrastructure
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [<img src="https://aqueduct-public-assets-bucket.s3.us-east-2.amazonaws.com/webapp/logos/aqueduct-logo-two-tone/1x/aqueduct-logo-two-tone-1x.png" width= "35%" />](https://www.aqueducthq.com)
 
-## Aqueduct: The easiest way to run ML on any cloud infrastructure
+## Aqueduct: The easiest way to run ML on any cloud
 
+[![Start Sandbox](https://img.shields.io/static/v1?label=%20&logo=github&message=Start%20Sandbox&color=black)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=496844646)
 [![Downloads](https://pepy.tech/badge/aqueduct-ml/month)](https://pypi.org/project/aqueduct-ml/)
 [![Slack](https://img.shields.io/static/v1.svg?label=chat&message=on%20slack&color=27b1ff&style=flat)](https://join.slack.com/t/aqueductusers/shared_invite/zt-11hby91cx-cpmgfK0qfXqEYXv25hqD6A)
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/aqueducthq/aqueduct/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/aqueduct-ml.svg)](https://pypi.org/project/aqueduct-ml/)
 [![Tests](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/aqueducthq/aqueduct/actions/workflows/integration-tests.yml)
 
-**Aqueduct enables you to define, deploy and monitor robust ML pipelines on any cloud infrastructure.** Check out our [quickstart guide](https://docs.aqueducthq.com/quickstart-guide)!
+**Aqueduct enables you to easily run machine learning tasks on any cloud infrastructure. [Check out our quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
-Aqueduct gives you a simple Python-native API to define machine learning pipelines, the ability to deploy those pipelines on your existing infrastructure (e.g., Spark, Kubernetes, Lambda), and visibility into the code, data, and metadata associated with your workflows. 
-Aqueduct is fully open-source and runs securely in your cloud.
+Aqueduct is an open-source MLOps framework that allows you to define ML tasks in vanilla Python, run those tasks on any infrastructure you'd like to use, and gain visibility into the execution and performance of your ML. **[See what tools Aqueduct works with. →](https://aqueducthq.com/integrations/)**
+
+Here's how you can get started: 
 
-You can install Aqueduct via `pip`:
 ```bash
 pip3 install aqueduct-ml
 aqueduct start
 ```
 
-Now, we can create our first workflow:
-
-```python
-from aqueduct import Client, op, metric
-
-client = Client()
+### How it works
 
-@op
-def transform_data(reviews):
-    reviews['strlen'] = reviews['review'].str.len()
-    return reviews
+Aqueduct's Python native API allows you to define ML tasks in regular Python code. You can connect Aqueduct to your existing cloud infrastructure ([docs](https://docs.aqueducthq.com/integrations)), and Aqueduct will seamlessly move your code from your laptop to the cloud or between different cloud infrastructure layers. 
 
+<!--- TODO(vikram): Modify this once we add support for switching into/out of Databricks in a single workflow. --->
+For example, we can define a pipeline that trains a model on Kubernetes using a GPU and validates that model in AWS Lambda in a few lines of Python: 
 
-demo_db = client.integration("aqueduct_demo")
-reviews_table = demo_db.sql("select * from hotel_reviews;")
-
-strlen_table = transform_data(reviews_table)
-demo_db.save(strlen_table, "strlen_table", "replace)
+```python
+@op(
+  engine='eks-us-east-2', 
+  resources={'gpu_resource_name': 'nvidia.com/gpu'}
+)
+def train(features):
+  return model.train(features)
+
+@metric(engine='lambda-us-east-2')
+def validate(model):
+    return validation_test(model)
 
-client.publish_flow(name="review_strlen", artifacts=[strlen_table])
+validate(train(features))
 ```
 
-Once we've created a workflow, we can view that workflow in the Aqueduct UI: 
+Once you publish this workflow to Aqueduct, you can see it on the UI: 
 
-![image](https://user-images.githubusercontent.com/867892/196529730-3c9582d5-8692-495d-a7df-8eb62ddf305f.png)
+![image](https://user-images.githubusercontent.com/867892/228295996-4ba3de23-3106-431d-93a9-afd8d77a707b.png)
+
+To see how to build your first workflow, check out our **[quickstart guide! →](https://docs.aqueducthq.com/quickstart-guide)**
 
 ## Why Aqueduct?
 
-The engineering required to get data science & machine learning projects in production slows down data teams. Aqueduct automates away that engineering and allows you to define robust data & ML pipelines in a few lines of code and run them anywhere.
+MLOps has become a [tangled mess of siloed infrastructure](https://aqueducthq.com/post/the-mlops-knot/). Most teams need to set up and operate many different cloud infrastructure tools to run ML effectively, but these tools have disparate APIs and interoperate poorly.
+
+Aqueduct provides a single interface to running machine learning tasks on your existing cloud infrastructure — Kubernetes, Spark, Lambda, etc. From the same Python API, you can run code across any or all of these systems seamlessly and gain visibility into how your code is performing.
 
 * **Python-native pipeline API**: Aqueduct’s API allows you define your workflows in vanilla Python, so you can get code into production quickly and effectively. No more DSLs or YAML configs to worry about.
 * **Integrated with your infrastructure**: Workflows defined in Aqueduct can run on any cloud infrastructure you use, like Kubernetes, Spark, Airflow, or AWS Lambda. You can get all the benefits of Aqueduct without having to rip-and-replace your existing tooling.
 * **Centralized visibility into code, data, & metadata**: Once your workflows are in production, you need to know what’s running, whether it’s working, and when it breaks. Aqueduct gives you visibility into what code, data, metrics, and metadata are generated by each workflow run, so you can have confidence that your pipelines work as expected — and know immediately when they don’t.
-* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that nothing is ever leaving your cloud.
+* **Runs securely in your cloud**: Aqueduct is fully open-source and runs in any Unix environment. It runs entirely in your cloud and on your infrastructure, so you can be confident that your data and code are secure.
 
 ## Overview & Examples
 
 The core abstraction in Aqueduct is a [Workflow](https://docs.aqueducthq.com/workflows), which is a sequence of [Artifacts](https://docs.aqueducthq.com/artifacts) (data) that are transformed by [Operators](https://docs.aqueducthq.com/operators) (compute). 
 The input Artifact(s) for a Workflow is typically loaded from a database, and the output Artifact(s) are typically persisted back to a database. 
 Each Workflow can either be run on a fixed schedule or triggered on-demand.
```

### Comparing `aqueduct-sdk-0.2.8/aqueduct_sdk.egg-info/SOURCES.txt` & `aqueduct-sdk-0.2.9/aqueduct_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
 aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
 aqueduct/utils/__init__.py
 aqueduct/utils/dag_deltas.py
 aqueduct/utils/describe.py
 aqueduct/utils/format.py
 aqueduct/utils/function_packaging.py
+aqueduct/utils/local_data.py
 aqueduct/utils/naming.py
 aqueduct/utils/serialization.py
 aqueduct/utils/type_inference.py
 aqueduct/utils/utils.py
 aqueduct_sdk.egg-info/PKG-INFO
 aqueduct_sdk.egg-info/SOURCES.txt
 aqueduct_sdk.egg-info/dependency_links.txt
```

### Comparing `aqueduct-sdk-0.2.8/setup.py` & `aqueduct-sdk-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 else:
     raise Exception(
         "Python Version %s.%s not supported" % (sys.version_info[0], sys.version_info[1])
     )
 
 setuptools.setup(
     name="aqueduct-sdk",
-    version="0.2.8",
+    version="0.2.9",
     author="Aqueduct, Inc.",
     author_email="hello@aqueducthq.com",
     description="Python SDK for the Aqueduct prediction infrastructure",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aqueducthq/aqueduct",
     license="Apache License 2.0",
```


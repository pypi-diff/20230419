# Comparing `tmp/aqueduct-ml-0.2.8.tar.gz` & `tmp/aqueduct-ml-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.2.8.tar", last modified: Wed Mar 29 16:50:05 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.2.9.tar", last modified: Wed Apr  5 19:18:44 2023, max compression
```

## Comparing `aqueduct-ml-0.2.8.tar` & `aqueduct-ml-0.2.9.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.757942 aqueduct-ml-0.2.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5975 2023-03-29 16:50:05.757942 aqueduct-ml-0.2.8/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.729942 aqueduct-ml-0.2.8/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.729942 aqueduct-ml-0.2.8/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.729942 aqueduct-ml-0.2.8/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.733942 aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.733942 aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.733942 aqueduct-ml-0.2.8/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.737942 aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.737942 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.741942 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2795 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12959 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8183 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.741942 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5473 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.745942 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.749942 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15071 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.749942 aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.753942 aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8793 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9678 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.753942 aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.753942 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7496 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.757942 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      787 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-03-28 21:01:21.000000 aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.757942 aqueduct-ml-0.2.8/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5975 2023-03-29 16:50:05.000000 aqueduct-ml-0.2.8/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5729 2023-03-29 16:50:05.000000 aqueduct-ml-0.2.8/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-29 16:50:05.000000 aqueduct-ml-0.2.8/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-03-29 16:50:05.000000 aqueduct-ml-0.2.8/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-03-29 16:50:05.000000 aqueduct-ml-0.2.8/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-29 16:50:05.757942 aqueduct-ml-0.2.8/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29101 2023-03-28 21:04:23.000000 aqueduct-ml-0.2.8/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-03-28 21:04:23.000000 aqueduct-ml-0.2.8/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-29 16:50:05.757942 aqueduct-ml-0.2.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-03-28 21:04:23.000000 aqueduct-ml-0.2.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6924 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/operators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.153672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/athena.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2795 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/connector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12959 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/relational.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8183 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5473 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15071 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1471 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.157672 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8793 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/execute_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9678 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/execute_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7496 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      787 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/storage.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/timer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-04-04 21:43:24.000000 aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6924 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5729 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-04-05 19:18:44.000000 aqueduct-ml-0.2.9/aqueduct_ml.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/bin/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29101 2023-04-04 22:01:25.000000 aqueduct-ml-0.2.9/bin/aqueduct
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-04-04 22:01:25.000000 aqueduct-ml-0.2.9/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-05 19:18:44.161672 aqueduct-ml-0.2.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-04-04 22:01:25.000000 aqueduct-ml-0.2.9/setup.py
```

### Comparing `aqueduct-ml-0.2.8/PKG-INFO` & `aqueduct-ml-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
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

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.2.9/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.2.9/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/common.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/load.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/main.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/execute_data.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/execute_function.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/execute_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.2.9/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.2.9/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,79 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prediction Infrastructure for Data Scientists
 Home-page: https://www.aqueducthq.com/
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

### Comparing `aqueduct-ml-0.2.8/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.2.9/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.2.8/bin/aqueduct` & `aqueduct-ml-0.2.9/bin/aqueduct`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import distro
 import requests
 import yaml
 from packaging.version import parse as parse_version
 from tqdm import tqdm
 
-SCHEMA_VERSION = "24"
+SCHEMA_VERSION = "25"
 CHUNK_SIZE = 4096
 
 # Connector Package Version Bounds
 PYMONGO_VERSION_BOUND = "<=4.3.3"
 PSYCOPG2_VERSION_BOUND = "<=2.9.5"
 BIGQUERY_VERSION_BOUND = "<=3.5.0"
 SNOWFLAKE_VERSION_BOUND = "<=1.4.4"
@@ -33,15 +33,15 @@
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.2.8"
+package_version = "0.2.9"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
```

### Comparing `aqueduct-ml-0.2.8/setup.py` & `aqueduct-ml-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = open("requirements.txt").read().strip().split("\n")
 
 readme_path = Path(os.environ["PWD"], "../../README.md")
 long_description = open(readme_path).read()
 
 setup(
     name="aqueduct-ml",
-    version="0.2.8",
+    version="0.2.9",
     install_requires=install_requires,
     scripts=["bin/aqueduct"],
     packages=find_packages(),
     description="Prediction Infrastructure for Data Scientists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.aqueducthq.com/",
```


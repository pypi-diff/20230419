# Comparing `tmp/airflow_db_logger-2.0.3.tar.gz` & `tmp/airflow_db_logger-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_db_logger-2.0.3.tar", last modified: Wed Aug 17 21:20:50 2022, max compression
+gzip compressed data, was "airflow_db_logger-2.1.0.tar", last modified: Wed Apr 19 20:14:46 2023, max compression
```

## Comparing `airflow_db_logger-2.0.3.tar` & `airflow_db_logger-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 21:20:50.080812 airflow_db_logger-2.0.3/
--rwxr-xr-x   0 runner    (1001) docker     (121)       18 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-08-17 21:20:50.080812 airflow_db_logger-2.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     5609 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      138 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 21:20:50.080812 airflow_db_logger-2.0.3/airflow_db_logger/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2257 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1554 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/airflow_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10937 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1303 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2948 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/data.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       45 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16613 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1589 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/shell_logging_config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1757 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 21:20:50.080812 airflow_db_logger-2.0.3/airflow_db_logger/writers/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3807 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/writers/gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2501 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/writers/local.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      665 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/airflow_db_logger/writers/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 21:20:50.080812 airflow_db_logger-2.0.3/airflow_db_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-08-17 21:20:50.000000 airflow_db_logger-2.0.3/airflow_db_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-08-17 21:20:50.000000 airflow_db_logger-2.0.3/airflow_db_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 21:20:50.000000 airflow_db_logger-2.0.3/airflow_db_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-17 21:20:50.000000 airflow_db_logger-2.0.3/airflow_db_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-17 21:20:50.000000 airflow_db_logger-2.0.3/airflow_db_logger.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       67 2022-08-17 21:20:50.080812 airflow_db_logger-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1056 2022-08-17 21:20:38.000000 airflow_db_logger-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       18 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5623 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/airflow_db_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/airflow_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11247 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17091 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/shell_logging_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/airflow_db_logger/writers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3807 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/writers/gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2500 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/writers/local.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/airflow_db_logger/writers/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 20:14:46.000000 airflow_db_logger-2.1.0/airflow_db_logger.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       67 2023-04-19 20:14:46.562790 airflow_db_logger-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-04-19 20:14:31.000000 airflow_db_logger-2.1.0/setup.py
```

### Comparing `airflow_db_logger-2.0.3/README.md` & `airflow_db_logger-2.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 Add to airflow.cfg,
 
 ```ini
 [core or logging(airflow 2)]
 logging_config_class = airflow_db_logger.LOGGING_CONFIG
 
 [db_logger]
-SQL_ALCHEMY_CONN=
-SQL_ALCHEMY_SCHEMA=
-SQL_ALCHEMY_POOL_ENABLED=True
-SQL_ALCHEMY_POOL_SIZE=5
-SQL_ALCHEMY_MAX_OVERFLOW=1
-SQL_ALCHEMY_POOL_RECYCLE=1800
-SQL_ALCHEMY_POOL_PRE_PING=True
-SQL_ENGINE_ENCODING=utf-8
+sql_alchemy_conn =
+sql_alchemy_schema =
+sql_alchemy_pool_enabled = true
+sql_alchemy_pool_size = 5
+sql_alchemy_max_overflow = 1
+sql_alchemy_pool_recycle = 1800
+sql_alchemy_pool_pre_ping = true
+sql_engine_encoding = utf-8
 ```
 
 Or use the airflow builtin envs,
 
 ```shell
 export AIRFLOW__DB_LOGGER_[config value name]="my_value"
 ```
@@ -58,35 +58,35 @@
 # Config
 
 Uses the airflow config, under the section `db_logger`. You can add a section to the airflow
 configuration of apply these values using envs, like so,
 
 | section                                  | description                                               | type/values | default                     |
 | ---------------------------------------- | --------------------------------------------------------- | ----------- | --------------------------- |
-| [db_logger].`SQL_ALCHEMY_CONN`           | The sqlalchemy connection string                          | `string`    | [core].`SQL_ALCHEMY_CONN`   |
-| [db_logger].`SQL_ALCHEMY_CONN_ARGS`      | The sqlalchemy connection args                            | `string`    | None                        |
-| [db_logger].`SQL_ALCHEMY_SCHEMA`         | The schema where to put the logging tables.               | `string`    | [core].`SQL_ALCHEMY_SCHEMA` |
-| [db_logger].`SQL_ALCHEMY_POOL_ENABLED`   | If true enable sql alchemy pool                           | `boolean`   | True                        |
-| [db_logger].`SQL_ALCHEMY_POOL_SIZE`      | The size of the sqlalchemy pool.                          | `int`       | 5                           |
-| [db_logger].`SQL_ALCHEMY_MAX_OVERFLOW`   | The max overflow for sqlalchemy                           | `int`       | 1                           |
-| [db_logger].`SQL_ALCHEMY_POOL_RECYCLE`   | The pool recycle time                                     | `int`       | 1800                        |
-| [db_logger].`SQL_ALCHEMY_POOL_PRE_PING`  | If true, do a ping at the connection start.               | `boolean`   | true                        |
-| [db_logger].`SQL_ENGINE_ENCODING`        | THe encoding for the sql engine                           | `string`    | utf-8                       |
+| [db_logger].`sql_alchemy_conn`           | The sqlalchemy connection string                          | `string`    | [core].`sql_alchemy_conn`   |
+| [db_logger].`sql_alchemy_conn_args`      | The sqlalchemy connection args                            | `string`    | None                        |
+| [db_logger].`sql_alchemy_schema`         | The schema where to put the logging tables.               | `string`    | [core].`sql_alchemy_schema` |
+| [db_logger].`sql_alchemy_pool_enabled`   | If true enable sql alchemy pool                           | `boolean`   | True                        |
+| [db_logger].`sql_alchemy_pool_size`      | The size of the sqlalchemy pool.                          | `int`       | 5                           |
+| [db_logger].`sql_alchemy_max_overflow`   | The max overflow for sqlalchemy                           | `int`       | 1                           |
+| [db_logger].`sql_alchemy_pool_recycle`   | The pool recycle time                                     | `int`       | 1800                        |
+| [db_logger].`sql_alchemy_pool_pre_ping`  | If true, do a ping at the connection start.               | `boolean`   | true                        |
+| [db_logger].`sql_engine_encoding`        | THe encoding for the sql engine                           | `string`    | utf-8                       |
 |                                          |                                                           |             |
-| [db_logger].`SHOW_REVERSE_ORDER`         | Show logs in reverse order in airflow log ui              | bool        | false                       |
-| [db_logger].`CREATE_INDEXES`             | If true create db indexis                                 | bool        | false                       |
-| [db_logger].`GOOGLE_APP_CREDS_PATH`      | The credentials file path for google bucket writing (gcs) | `string`    | None                        |
-| [db_logger].`WRITE_TO_GCS_BUCKET`        | The gcs bucket to write to                                | `string`    | None                        |
-| [db_logger].`WRITE_TO_GCS_PROJECT_ID`    | The gcs project to write to                               | `string`    | None                        |
-| [db_logger].`WRITE_TO_FILES`             | If true, writes the log also to files                     | false       | None                        |
-| [db_logger].`WRITE_TO_SHELL`             | Output the logs to shell as well                          | false       | None                        |
-| [db_logger].`WRITE_DAG_PROCESSING_TO_DB` | Write all dag processing to database (a lot)              | `string`    | utf-8                       |
-| [db_logger].`CONSOLE_FORMATTER`          | the formatter to use for teh console                      | `string`    | airflow_coloured            |
-| [db_logger].`TASK_FORMATTER`             | the formatter to use for the task                         | `string`    | airflow                     |
-| [db_logger].`PROCESSER_LOG_LEVEL`        | The log level to use for dag processing                   | `string`    | "WARN"                      |
+| [db_logger].`show_reverse_order`         | Show logs in reverse order in airflow log ui              | bool        | false                       |
+| [db_logger].`create_indexes`             | If true create db indexis                                 | bool        | false                       |
+| [db_logger].`google_app_creds_path`      | The credentials file path for google bucket writing (gcs) | `string`    | None                        |
+| [db_logger].`write_to_gcs_bucket`        | The gcs bucket to write to                                | `string`    | None                        |
+| [db_logger].`write_to_gcs_project_id`    | The gcs project to write to                               | `string`    | None                        |
+| [db_logger].`write_to_files`             | If true, writes the log also to files                     | false       | None                        |
+| [db_logger].`write_to_shell`             | Output the logs to shell as well                          | false       | None                        |
+| [db_logger].`write_dag_processing_to_db` | Write all dag processing to database (a lot)              | `string`    | utf-8                       |
+| [db_logger].`console_formatter`          | the formatter to use for teh console                      | `string`    | airflow_coloured            |
+| [db_logger].`task_formatter`             | the formatter to use for the task                         | `string`    | airflow                     |
+| [db_logger].`processer_log_level`        | The log level to use for dag processing                   | `string`    | "WARN"                      |
 
 # Maintenance
 
 You can use the built in airflow operator to do cleanup. for example cleanup of logs older than 30 days,
 
 ```python
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/__init__.py` & `airflow_db_logger-2.1.0/airflow_db_logger/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,53 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
-__title__ = "airflow_db_logger"
-__author__ = "Zav Shotan"
 
-import sys
-import os
 from copy import deepcopy
-import airflow_db_logger.consts as consts
-
-
-LOGGING_CONFIG = consts.DB_LOGGER_LOGGING_CONFIG
-AIRFLOW_DEFAULT_LOGGING_CONFIG = consts.get_default_loggin_config()
 
+from airflow.config_templates.airflow_local_settings import DEFAULT_LOGGING_CONFIG
 from airflow_db_logger.config import (  # noqa
     check_cli_for_init_db,  # noqa: E402
     DB_LOGGER_TASK_FORMATTER,  # noqa: E402
     DB_LOGGER_CONSOLE_FORMATTER,  # noqa: E402
     DB_LOGGER_WRITE_DAG_PROCESSING_TO_DB,  # noqa: E402
     DB_LOGGER_PROCESSER_LOG_LEVEL,
-    airflow_db_logger_log,
 )
 
 
-def update_config_from_defaults():
-    consts.IS_DB_LOGGER_LOADING_CONFIG
-
-    if consts.IS_DB_LOGGER_LOADING_CONFIG is True:
-        return
-
-    # Remove any other loads.
-    try:
-        consts.IS_DB_LOGGER_LOADING_CONFIG = True
+def create_logging_config():
+    config = deepcopy(DEFAULT_LOGGING_CONFIG)
+    processor_handler_config = {
+        "class": "airflow_db_logger.handlers.StreamHandler",
+        "formatter": DB_LOGGER_CONSOLE_FORMATTER,
+        "level": DB_LOGGER_PROCESSER_LOG_LEVEL,
+    }
 
+    if DB_LOGGER_WRITE_DAG_PROCESSING_TO_DB:
         processor_handler_config = {
-            "class": "airflow_db_logger.handlers.StreamHandler",
+            "class": "airflow_db_logger.handlers.DBProcessLogHandler",
             "formatter": DB_LOGGER_CONSOLE_FORMATTER,
             "level": DB_LOGGER_PROCESSER_LOG_LEVEL,
         }
 
-        if DB_LOGGER_WRITE_DAG_PROCESSING_TO_DB:
-            processor_handler_config = {
-                "class": "airflow_db_logger.handlers.DBProcessLogHandler",
-                "formatter": DB_LOGGER_CONSOLE_FORMATTER,
-                "level": DB_LOGGER_PROCESSER_LOG_LEVEL,
-            }
-
-        LOGGING_CONFIG.update(deepcopy(AIRFLOW_DEFAULT_LOGGING_CONFIG))
-        LOGGING_CONFIG["handlers"] = {
-            "console": {
-                "class": "airflow_db_logger.handlers.StreamHandler",
-                "formatter": DB_LOGGER_CONSOLE_FORMATTER,
-            },
-            "task": {
-                "class": "airflow_db_logger.handlers.DBTaskLogHandler",
-                "formatter": DB_LOGGER_TASK_FORMATTER,
-            },
-            "processor": processor_handler_config,
-        }
+    config["handlers"] = {
+        "console": {
+            "class": "airflow_db_logger.handlers.StreamHandler",
+            "formatter": DB_LOGGER_CONSOLE_FORMATTER,
+        },
+        "task": {
+            "class": "airflow_db_logger.handlers.DBTaskLogHandler",
+            "formatter": DB_LOGGER_TASK_FORMATTER,
+        },
+        "processor": processor_handler_config,
+    }
+    return config
 
-        loggers = LOGGING_CONFIG.get("loggers", {})
 
-        # for logger_name in loggers.keys():
-        #     loggers[logger_name]["level"] = LOG_LEVEL
+LOGGING_CONFIG = create_logging_config()
 
-        # Checking for database initialization
-        check_cli_for_init_db()
+# Checking for database initialization
+check_cli_for_init_db()
 
-    finally:
-        consts.IS_DB_LOGGER_LOADING_CONFIG = False
 
+if __name__ == "__main__":
+    import json
 
-update_config_from_defaults()
-# airflow_db_logger_log.info("airflow_db_logger initialized")
+    print(json.dumps(LOGGING_CONFIG, indent=2))
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/airflow_utils.py` & `airflow_db_logger-2.1.0/airflow_db_logger/airflow_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import airflow
 from datetime import datetime
 from airflow import settings
-from airflow.operators.python_operator import PythonOperator
+from airflow.operators.python import PythonOperator
 from sqlalchemy.orm import Session, Query
 
 from airflow_db_logger.config import DBLoggerSession
 from airflow_db_logger.data import TaskExecutionLogRecord, DagFileProcessingLogRecord, LoggerModelBase
 
 
 def create_clean_old_logs_task(
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/config.py` & `airflow_db_logger-2.1.0/airflow_db_logger/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 import os
 import logging
-import warnings
 import colorlog
 from typing import Union, List
 from typing import Type
 from enum import Enum
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker, scoped_session
 from sqlalchemy.pool import NullPool, QueuePool
@@ -26,34 +25,40 @@
         val = conf.get(*args, **kwargs)
     except AirflowConfigException:
         val = None
     log.level = old_level
     return val
 
 
+def __add_core(*collections):
+    if AIRFLOW_MAJOR_VERSION < 1:
+        collections = ["core", *collections]
+    return collections
+
+
 def get(
     key: str,
     default=None,
     otype: Type = None,
     allow_empty: bool = False,
     collection: Union[str, List[str]] = None,
 ):
-    collection = collection or "db_logger"
-    collection = collection if isinstance(collection, list) else [collection]
-    otype = otype or str if default is None else default.__class__
     collection = collection or AIRFLOW_CONFIG_SECTION_NAME
+    if isinstance(collection, str):
+        collection = [collection]
+    assert all(isinstance(v, str) for v in collection), ValueError("Collection must be a string or a list of strings")
+    collection = [v for v in collection if len(v.strip()) > 0]
+    assert len(collection) > 0, ValueError("Collection must be a non empty string or list of non empty strings")
+
+    otype = otype or str if default is None else default.__class__
     for col in collection:
         val = conf_get_no_warnings_no_errors(col, key)
         if val is not None:
             break
 
-    assert all([isinstance(v, str) for v in collection]), AirflowConfigException(
-        "Collection must be a non empty string or a collection of non empty strings"
-    )
-
     if issubclass(otype, Enum):
         allow_empty = False
 
     value_is_empty = val is None or (isinstance(val, str) and len(val.strip()) == 0)
 
     if not allow_empty and value_is_empty:
         assert default is not None, AirflowConfigException(
@@ -69,38 +74,38 @@
         val = val.strip()
         return otype(val.strip())
     else:
         return otype(val)
 
 
 # Loading airflow parameters
-LOG_LEVEL = get(collection=["logging", "core"], key="logging_level").upper()
-FILENAME_TEMPLATE = get(collection=["logging", "core"], key="LOG_FILENAME_TEMPLATE")
+LOG_LEVEL = get(collection=__add_core("logging"), key="logging_level").upper()
+FILENAME_TEMPLATE = get(collection=__add_core("logging"), key="LOG_FILENAME_TEMPLATE")
 AIRFLOW_EXECUTOR = get(collection="core", key="executor")
 IS_RUNNING_DEBUG_EXECUTOR = AIRFLOW_EXECUTOR == "DebugExecutor"
-IS_USING_COLORED_CONSOLE = get(collection=["logging", "core"], key="colored_console_log").lower() == "true"
+IS_USING_COLORED_CONSOLE = get(collection=__add_core("logging"), key="colored_console_log").lower() == "true"
 DAGS_FOLDER = os.path.expanduser(get(collection="core", key="dags_folder"))
-BASE_LOG_FOLDER = os.path.expanduser(get(collection=["logging", "core"], key="base_log_folder"))
+BASE_LOG_FOLDER = os.path.expanduser(get(collection=__add_core("logging"), key="base_log_folder"))
 
 # Loading sql parameters
-SQL_ALCHEMY_CONN = get(collection=["core", "database"], key="sql_alchemy_conn", allow_empty=False)
-SQL_ALCHEMY_SCHEMA = get(collection=["core", "database"], key="sql_alchemy_schema", allow_empty=True)
+SQL_ALCHEMY_CONN = get(collection=__add_core("database"), key="sql_alchemy_conn", allow_empty=False)
+SQL_ALCHEMY_SCHEMA = get(collection=__add_core("database"), key="sql_alchemy_schema", allow_empty=True)
 
 TASK_LOG_FILENAME_TEMPLATE = (
     get(
-        collection="core",
+        collection=__add_core("logging"),
         key="LOG_FILENAME_TEMPLATE",
         default="{{ ti.dag_id }}/{{ ti.task_id }}/{{ ts }}/{{ try_number }}.log",
     )
     .replace("{{{{", "{{")
     .replace("}}}}", "}}")
 )
 PROCESS_LOG_FILENAME_TEMPLATE = (
     get(
-        collection="core",
+        collection=__add_core("logging"),
         key="log_processor_filename_template",
         default="{{ filename }}.log",
     )
     .replace("{{{{", "{{")
     .replace("}}}}", "}}")
 )
 
@@ -113,15 +118,15 @@
 DB_LOGGER_WRITE_DAG_PROCESSING_TO_DB = get("write_dag_processing_to_db", False)
 
 DB_LOGGER_SQL_ALCHEMY_POOL_ENABLED = get("sql_alchemy_pool_enabled", False)
 DB_LOGGER_SQL_ALCHEMY_POOL_SIZE = get("sql_alchemy_pool_size", 5)
 DB_LOGGER_SQL_ALCHEMY_MAX_OVERFLOW = get("sql_alchemy_max_overflow", 1)
 DB_LOGGER_SQL_ALCHEMY_POOL_RECYCLE = get("sql_alchemy_pool_recycle", 1800)
 DB_LOGGER_SQL_ALCHEMY_POOL_PRE_PING = get("sql_alchemy_pool_pre_ping", True)
-DB_LOGGER_SQL_ENGINE_ENCODING = get("sql_engine_encoding", "utf-8")
+DB_LOGGER_SQL_ENGINE_ENCODING = get("sql_engine_encoding", None, allow_empty=True)
 
 DB_LOGGER_GOOGLE_APP_CREDS_PATH = get("google_application_credentials", default=None, allow_empty=True, otype=str)
 # A bucket path, requires google-cloud-storage to be installed.
 DB_LOGGER_WRITE_TO_GCS_BUCKET = get("write_to_gcs_bucket", default=None, allow_empty=True, otype=str)
 DB_LOGGER_WRITE_TO_GCS_PROJECT_ID = get("write_to_gcs_project_id", default=None, allow_empty=True, otype=str)
 DB_LOGGER_WRITE_TO_GCS_MULTI_FILE_LOG = get("write_to_gcs_multi_file_log", default=False)
 DB_LOGGER_PROCESSER_LOG_LEVEL = get("processer_log_level", default="WARN", allow_empty=True, otype=str)
@@ -138,15 +143,14 @@
 logging.basicConfig(level=LOG_LEVEL)
 
 logging.debug(f"DBLogger is connecting to: {DB_LOGGER_SQL_ALCHEMY_CONNECTION}/{DB_LOGGER_SQL_ALCHEMY_SCHEMA}")
 logging.debug(f"DBLogger indexes: {DB_LOGGER_CREATE_INDEXES}")
 
 
 def create_db_logger_sqlalchemy_engine():
-
     # Configuring the db_logger sql engine.
     engine_args = {}
     if DB_LOGGER_SQL_ALCHEMY_POOL_ENABLED:
         # Copied from airflow main repo.
 
         # Pool size engine args not supported by sqlite.
         # If no config value is defined for the pool size, select a reasonable value.
@@ -199,17 +203,20 @@
             if len(value) == 0 or len(key) == 0:
                 continue
             engine_args[key] = value
 
     # Allow the user to specify an encoding for their DB otherwise default
     # to utf-8 so jobs & users with non-latin1 characters can still use
     # us.
-    engine_args["encoding"] = DB_LOGGER_SQL_ENGINE_ENCODING
-    # For Python2 we get back a newstr and need a str
-    engine_args["encoding"] = engine_args["encoding"].__str__()
+    if DB_LOGGER_SQL_ENGINE_ENCODING:
+        engine_args["encoding"] = DB_LOGGER_SQL_ENGINE_ENCODING
+
+    # DEPRECATED:
+    # # For Python2 we get back a newstr and need a str
+    # engine_args["encoding"] = engine_args["encoding"].__str__()
 
     return create_engine(DB_LOGGER_SQL_ALCHEMY_CONNECTION, **engine_args)
 
 
 # The main db session. Used in all logging.
 DB_LOGGER_ENGINE = create_db_logger_sqlalchemy_engine()
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/data.py` & `airflow_db_logger-2.1.0/airflow_db_logger/data.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/handlers.py` & `airflow_db_logger-2.1.0/airflow_db_logger/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 import traceback
+import warnings
 import os
 import sys
 from typing import Dict, List, Union
 from zthreading.events import EventHandler, Event
 from airflow.utils.helpers import parse_template_string
 from airflow.models import TaskInstance
+from airflow.utils.context import AirflowContextDeprecationWarning
 from sqlalchemy import asc, desc
-import traceback
 
 from airflow_db_logger.exceptions import DBLoggerException
 from airflow_db_logger.utils import get_calling_frame_objects_by_type
 from airflow_db_logger.data import TaskExecutionLogRecord, DagFileProcessingLogRecord
 from airflow_db_logger.config import (
     LOG_LEVEL,
     DBLoggerSession,
     DAGS_FOLDER,
     IS_RUNNING_DEBUG_EXECUTOR,
-    IS_USING_COLORED_CONSOLE,
     DB_LOGGER_SHOW_REVERSE_ORDER,
     TASK_LOG_FILENAME_TEMPLATE,
     PROCESS_LOG_FILENAME_TEMPLATE,
     DB_LOGGER_WRITE_TO_FILES,
     DB_LOGGER_WRITE_TO_GCS_BUCKET,
     DB_LOGGER_WRITE_TO_SHELL,
     AIRFLOW_MAJOR_VERSION,
@@ -32,14 +32,15 @@
 class ExecutionLogTaskContextInfo:
     def __init__(self, task_instance: TaskInstance):
         super().__init__()
         self.dag_id = task_instance.dag_id
         self.task_id = task_instance.task_id
         self.execution_date = task_instance.execution_date
         self.try_number = task_instance.try_number
+        self.map_index = 0
 
 
 class DBLoggingEventHandler(EventHandler):
     log_event_name: str = "log"
     flush_event_name: str = "flush"
     close_event_name: str = "close"
 
@@ -207,15 +208,22 @@
     def _render_logfile_subpath(self):
         """Returns the task log sub filepath"""
         if self.filename_jinja_template:
             # render as jinja
             jinja_context = self._task_instance.get_template_context()
             jinja_context["ti"] = self.task_context_info
             jinja_context["try_number"] = self.task_context_info.try_number
-            return self.filename_jinja_template.render(**jinja_context)
+            with warnings.catch_warnings():
+                # Render should not have warnings here, since the render should
+                # just throw an error if errored.
+                warnings.filterwarnings(
+                    action="ignore",
+                    category=AirflowContextDeprecationWarning,
+                )
+                return self.filename_jinja_template.render(**jinja_context)
         else:
             # render direct
             return self.filename_template.format(
                 dag_id=self.task_context_info.dag_id,
                 task_id=self.task_context_info.task_id,
                 execution_date=self.task_context_info.execution_date.isoformat(),
                 try_number=self.task_context_info.try_number,
@@ -260,15 +268,15 @@
                 )
 
                 self.db_session.add(db_record)
                 self.db_session.commit()
             except Exception:
                 try:
                     self.db_session.rollback()
-                except:
+                except Exception:
                     pass
                 airflow_db_logger_log.error(traceback.format_exc())
 
         super().emit(record)
 
     def read(
         self,
@@ -308,15 +316,18 @@
                 return logs
             else:
                 try_numbers = [try_number]
 
             logs_by_try_number: Dict[int, List[TaskExecutionLogRecord]] = dict()
 
             airflow_db_logger_log.info(
-                f"Reading logs: {task_instance.dag_id}/{task_instance.task_id} {try_numbers} {{{task_instance.execution_date}}}"
+                (
+                    f"Reading logs: {task_instance.dag_id}/{task_instance.task_id} {try_numbers}"
+                    f" {{{task_instance.execution_date}}}"
+                )
             )
 
             log_records_query = (
                 db_session.query(TaskExecutionLogRecord)
                 .filter(TaskExecutionLogRecord.dag_id == task_instance.dag_id)
                 .filter(TaskExecutionLogRecord.task_id == task_instance.task_id)
                 .filter(TaskExecutionLogRecord.execution_date == task_instance.execution_date)
@@ -367,15 +378,15 @@
         except Exception:
             if db_session:
                 try:
                     db_session.rollback()
                 except Exception:
                     pass
             airflow_db_logger_log.error(traceback.format_exc())
-            return [f"An error occurred while connecting to the database:\n" + f"{traceback.format_exc()}"], [
+            return [f"An error occurred while connecting to the database:\n{traceback.format_exc()}"], [
                 {"end_of_log": True}
             ]
         finally:
             if db_session:
                 db_session.close()
 
 
@@ -456,13 +467,13 @@
         try:
             db_record = DagFileProcessingLogRecord(self._log_filepath, db_record_message)
             self.db_session.add(db_record)
             self.db_session.commit()
         except Exception:
             try:
                 self.db_session.rollback()
-            except:
+            except Exception:
                 pass
             airflow_db_logger_log.error(f"Error while attempting to log ({self._log_filepath}): {db_record_message}")
             airflow_db_logger_log.error(traceback.format_exc())
 
         super().emit(record)
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/operators.py` & `airflow_db_logger-2.1.0/airflow_db_logger/operators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from datetime import datetime
 from typing import Any
 from sqlalchemy.orm import Session, Query
 
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.models import BaseOperator
 from airflow_db_logger.config import AIRFLOW_MAJOR_VERSION
-from airflow_db_logger.exceptions import DBLoggerException
-from airflow_db_logger.data import DagFileProcessingLogRecord, TaskExecutionLogRecord, LoggerModelBase
+from airflow_db_logger.data import DagFileProcessingLogRecord, TaskExecutionLogRecord
 
 if AIRFLOW_MAJOR_VERSION > 1:
     from airflow.utils.session import provide_session
 else:
     from airflow.utils.db import provide_session
 
 
@@ -20,14 +19,23 @@
         task_id: str,
         up_to: datetime,
         since: datetime = None,
         include_task_logs=True,
         include_operations_log=True,
         **kwargs,
     ) -> None:
+        """Cleanup db_logger database logs
+
+        Args:
+            task_id (str): The id of the task.
+            up_to (datetime): Any log before this date will be deleted.
+            since (datetime, optional): Start from this date. Defaults to None.
+            include_task_logs (bool, optional): If true, then clean task logs. Defaults to True.
+            include_operations_log (bool, optional): If true, then clean operations log. Defaults to True.
+        """
         assert isinstance(up_to, datetime), ValueError("up_to must be of type datetime")
 
         super().__init__(task_id=task_id, **kwargs)
 
         assert include_operations_log or include_task_logs, ValueError(
             "Either include_operations_log or include_task_logs must be true"
         )
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/shell_logging_config.py` & `airflow_db_logger-2.1.0/airflow_db_logger/shell_logging_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-import sys
 import logging
 
 LOG_FORMAT_HEADER = "[%(asctime)s][%(levelname)7s]"
 LOG_FORMAT = LOG_FORMAT_HEADER + " %(message)s"
 
 
 def create_shell_logging_config(
     level=logging.INFO, format: str = LOG_FORMAT, handler_class: str = "airflow_db_logger.handlers.StreamHandler"
 ):
-    return {
+    from airflow.version import version as AIRFLOW_VERSION
+
+    AIRFLOW_VERSION_PARTS = AIRFLOW_VERSION.split(".")
+    AIRFLOW_VERSION_PARTS = [int(v) for v in AIRFLOW_VERSION_PARTS]
+
+    AIRFLOW_MAJOR_VERSION = AIRFLOW_VERSION_PARTS[0]
+
+    config = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
             "shell": {"format": LOG_FORMAT},
         },
         "handlers": {
             "console": {
@@ -34,23 +40,32 @@
                 "level": level,
                 "propagate": False,
             },
             "airflow.task": {
                 "handlers": ["task"],
                 "level": level,
                 "propagate": False,
+                "filters": ["mask_secrets"],
             },
             "flask_appbuilder": {
                 "handler": ["console"],
                 "level": level,
                 "propagate": True,
             },
         },
         "root": {
             "handlers": ["console"],
             "level": level,
+            "filters": ["mask_secrets"],
+        },
+        "filters": {
+            "mask_secrets": {
+                "()": "airflow.utils.log.secrets_masker.SecretsMasker",
+            }
         },
     }
 
+    return config
+
 
 SIMPLE_LOGGING_CONFIG = create_shell_logging_config(logging.INFO, handler_class="logging.StreamHandler")
 LOGGING_CONFIG = create_shell_logging_config(logging.INFO)
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/utils.py` & `airflow_db_logger-2.1.0/airflow_db_logger/utils.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/writers/gcs.py` & `airflow_db_logger-2.1.0/airflow_db_logger/writers/gcs.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/writers/local.py` & `airflow_db_logger-2.1.0/airflow_db_logger/writers/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
 class DBLogFileWriter(DBLogStreamWriter):
     def __init__(self) -> None:
         super().__init__()
         self._pending_loggers: Dict[str, DBLogFileCollectionWriter] = WeakValueDictionary()
 
     def get_file_collection_writer(self, filename: str):
-
         if filename not in self._pending_loggers:
             logger = DBLogFileCollectionWriter(filename)
             self._pending_loggers[filename] = logger
             return logger
         else:
             return self._pending_loggers[filename]
```

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger/writers/shell.py` & `airflow_db_logger-2.1.0/airflow_db_logger/writers/shell.py`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-2.0.3/airflow_db_logger.egg-info/SOURCES.txt` & `airflow_db_logger-2.1.0/airflow_db_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow_db_logger-2.0.3/setup.py` & `airflow_db_logger-2.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def get_version():
     version_file_path = os.path.join(here, "package_version.txt")
     if not os.path.isfile(version_file_path):
-        return "debug"
+        return "0.0.0"
     version = None
     with open(version_file_path, "r") as raw:
         version = raw.read()
 
     return version
 
 
@@ -27,13 +27,12 @@
     author="Zav Shotan",
     author_email="",
     url="https://github.com/LamaAni/AirflowDBLogger",
     packages=["airflow_db_logger", "airflow_db_logger/writers"],
     platforms="any",
     license="docs/LICENSE",
     install_requires=[
-        "sqlalchemy>=0.23.1",
         "zthreading>=0.1.15",
     ],
     python_requires=">=3.6",
     include_package_data=True,
 )
```


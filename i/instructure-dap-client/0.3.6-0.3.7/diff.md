# Comparing `tmp/instructure-dap-client-0.3.6.tar.gz` & `tmp/instructure-dap-client-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructure-dap-client-0.3.6.tar", last modified: Fri Apr  7 12:35:42 2023, max compression
+gzip compressed data, was "instructure-dap-client-0.3.7.tar", last modified: Wed Apr 19 18:01:45 2023, max compression
```

## Comparing `instructure-dap-client-0.3.6.tar` & `instructure-dap-client-0.3.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.343059 instructure-dap-client-0.3.6/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.6/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18505 2023-04-07 12:35:42.343255 instructure-dap-client-0.3.6/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    17706 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.321272 instructure-dap-client-0.3.6/dap/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       22 2023-04-07 12:35:01.000000 instructure-dap-client-0.3.6/dap/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4382 2023-04-04 13:12:06.000000 instructure-dap-client-0.3.6/dap/__main__.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.323633 instructure-dap-client-0.3.6/dap/actions/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/actions/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/actions/drop_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/actions/init_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/actions/sync_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    20570 2023-04-04 13:08:40.000000 instructure-dap-client-0.3.6/dap/api.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2980 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.6/dap/arguments.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.330824 instructure-dap-client-0.3.6/dap/commands/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.6/dap/commands/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      457 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/commands/abstract_db_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/base.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.6/dap/commands/commands.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2611 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.6/dap/commands/commonargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/dbargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/dropdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1361 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/initdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/queryargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1695 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/syncdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/commands/timestampargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/concurrency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2920 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/dap_error.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18455 2023-04-04 13:07:56.000000 instructure-dap-client-0.3.6/dap/dap_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.335472 instructure-dap-client-0.3.6/dap/database/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/database/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2316 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.6/dap/database/base_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.6/dap/database/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.6/dap/database/database_errors.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3401 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/database/database_operations.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2720 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/database/init_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3661 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/database/sync_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5759 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.6/dap/downloader.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      669 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.6/dap/log.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.336969 instructure-dap-client-0.3.6/dap/model/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.6/dap/model/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8026 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.6/dap/model/meta_table.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6184 2023-04-04 12:03:12.000000 instructure-dap-client-0.3.6/dap/model/metadata.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      850 2023-04-04 12:03:12.000000 instructure-dap-client-0.3.6/dap/networking.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.6/dap/payload.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.338161 instructure-dap-client-0.3.6/dap/replicator/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.6/dap/replicator/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2550 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/replicator/sql.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/timer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1450 2023-03-27 20:20:03.000000 instructure-dap-client-0.3.6/dap/timestamp.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2869 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.6/dap/type_conversion.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-07 12:35:42.342427 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18505 2023-04-07 12:35:42.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1327 2023-04-07 12:35:42.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-07 12:35:42.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-04-07 12:35:42.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/entry_points.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      151 2023-04-07 12:35:42.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-04-07 12:35:42.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-07 12:35:41.000000 instructure-dap-client-0.3.6/instructure_dap_client.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.6/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1170 2023-04-07 12:35:42.344222 instructure-dap-client-0.3.6/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.6/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.378236 instructure-dap-client-0.3.7/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.7/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18505 2023-04-19 18:01:45.378531 instructure-dap-client-0.3.7/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    17706 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.344117 instructure-dap-client-0.3.7/dap/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       22 2023-04-19 07:04:39.000000 instructure-dap-client-0.3.7/dap/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4382 2023-04-04 13:12:06.000000 instructure-dap-client-0.3.7/dap/__main__.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.346893 instructure-dap-client-0.3.7/dap/actions/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/actions/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/actions/drop_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/actions/init_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/actions/sync_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    20570 2023-04-04 13:08:40.000000 instructure-dap-client-0.3.7/dap/api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2980 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.7/dap/arguments.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.359203 instructure-dap-client-0.3.7/dap/commands/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.7/dap/commands/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      457 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/commands/abstract_db_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/base.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.7/dap/commands/commands.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2611 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.7/dap/commands/commonargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/dbargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/dropdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1361 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/initdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/queryargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1695 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/syncdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/commands/timestampargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/concurrency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2920 2023-04-14 16:20:35.000000 instructure-dap-client-0.3.7/dap/dap_error.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18455 2023-04-04 13:07:56.000000 instructure-dap-client-0.3.7/dap/dap_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.367048 instructure-dap-client-0.3.7/dap/database/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/database/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2316 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/database/base_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/database/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/database/database_errors.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3835 2023-04-19 07:03:02.000000 instructure-dap-client-0.3.7/dap/database/database_operations.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2720 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/database/init_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3661 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/database/sync_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5759 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/downloader.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      669 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.7/dap/log.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.369231 instructure-dap-client-0.3.7/dap/model/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.7/dap/model/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8026 2023-04-07 11:44:25.000000 instructure-dap-client-0.3.7/dap/model/meta_table.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6184 2023-04-04 12:03:12.000000 instructure-dap-client-0.3.7/dap/model/metadata.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      850 2023-04-04 12:03:12.000000 instructure-dap-client-0.3.7/dap/networking.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.7/dap/payload.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.371003 instructure-dap-client-0.3.7/dap/replicator/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.7/dap/replicator/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2550 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/replicator/sql.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.7/dap/timer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1450 2023-03-27 20:20:03.000000 instructure-dap-client-0.3.7/dap/timestamp.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6740 2023-04-19 16:25:38.000000 instructure-dap-client-0.3.7/dap/type_conversion.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-04-19 18:01:45.377575 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18505 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1327 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/entry_points.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      151 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-04-19 18:01:45.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-04-19 18:01:44.000000 instructure-dap-client-0.3.7/instructure_dap_client.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.7/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1170 2023-04-19 18:01:45.379676 instructure-dap-client-0.3.7/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.7/setup.py
```

### Comparing `instructure-dap-client-0.3.6/LICENSE` & `instructure-dap-client-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/PKG-INFO` & `instructure-dap-client-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.6
+Version: 0.3.7
 Summary: Data Access Platform client library
 Author: Levente Hunyadi
 Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `instructure-dap-client-0.3.6/README.md` & `instructure-dap-client-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/__main__.py` & `instructure-dap-client-0.3.7/dap/__main__.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/actions/drop_db.py` & `instructure-dap-client-0.3.7/dap/actions/drop_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/actions/init_db.py` & `instructure-dap-client-0.3.7/dap/actions/init_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/actions/sync_db.py` & `instructure-dap-client-0.3.7/dap/actions/sync_db.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/api.py` & `instructure-dap-client-0.3.7/dap/api.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/arguments.py` & `instructure-dap-client-0.3.7/dap/arguments.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/base.py` & `instructure-dap-client-0.3.7/dap/commands/base.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/commands.py` & `instructure-dap-client-0.3.7/dap/commands/commands.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/commonargs.py` & `instructure-dap-client-0.3.7/dap/commands/commonargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/dropdb_command.py` & `instructure-dap-client-0.3.7/dap/commands/dropdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/initdb_command.py` & `instructure-dap-client-0.3.7/dap/commands/initdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/queryargs.py` & `instructure-dap-client-0.3.7/dap/commands/queryargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/syncdb_command.py` & `instructure-dap-client-0.3.7/dap/commands/syncdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/commands/timestampargs.py` & `instructure-dap-client-0.3.7/dap/commands/timestampargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/concurrency.py` & `instructure-dap-client-0.3.7/dap/concurrency.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/dap_error.py` & `instructure-dap-client-0.3.7/dap/dap_error.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/dap_types.py` & `instructure-dap-client-0.3.7/dap/dap_types.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/database/base_processor.py` & `instructure-dap-client-0.3.7/dap/database/base_processor.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/database/connection.py` & `instructure-dap-client-0.3.7/dap/database/connection.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/database/database_errors.py` & `instructure-dap-client-0.3.7/dap/database/database_errors.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/database/database_operations.py` & `instructure-dap-client-0.3.7/dap/database/database_operations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, Generic, List, Tuple, TypeVar
 
 import asyncpg
-from sqlalchemy import Delete, Table, bindparam
+from sqlalchemy import BindParameter, Delete, Table, bindparam
 from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.sql.dml import Insert
 
 from ..timer import Timer
 from .base_processor import ContextAwareObject
 from .connection import DatabaseSession
 from .database_errors import DatabaseConnectionError
@@ -71,16 +71,29 @@
 
 
 class DatabaseUpsert(DatabaseOperation[Dict[str, Any]]):
     async def _execute(self) -> None:
         if not self._records:
             return
 
-        upsert_statement: Insert = insert(self._table_def).on_conflict_do_update(  # type: ignore
-            constraint=self._table_def.primary_key, set_=self._table_def.c
+        values_clause: Dict[str, BindParameter] = {}
+        for col in self._table_def.columns:
+            values_clause[col.name] = bindparam(col.name)
+
+        set_clause: Dict[str, BindParameter] = {}
+        for col in self._table_def.columns:
+            if not col.primary_key:
+                set_clause[col.name] = bindparam(col.name)
+
+        upsert_statement: Insert = (
+            insert(self._table_def)  # type: ignore
+            .values(values_clause)
+            .on_conflict_do_update(
+                constraint=self._table_def.primary_key, set_=set_clause
+            )
         )
 
         async with Timer(
             f"upserting {len(self._records)} records from {self._context}"
         ):
             async with self._connection.context() as conn:
                 await conn.execute(
```

### Comparing `instructure-dap-client-0.3.6/dap/database/init_processor.py` & `instructure-dap-client-0.3.7/dap/database/init_processor.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/database/sync_processor.py` & `instructure-dap-client-0.3.7/dap/database/sync_processor.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/downloader.py` & `instructure-dap-client-0.3.7/dap/downloader.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/log.py` & `instructure-dap-client-0.3.7/dap/log.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/model/meta_table.py` & `instructure-dap-client-0.3.7/dap/model/meta_table.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/model/metadata.py` & `instructure-dap-client-0.3.7/dap/model/metadata.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/networking.py` & `instructure-dap-client-0.3.7/dap/networking.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/payload.py` & `instructure-dap-client-0.3.7/dap/payload.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/replicator/sql.py` & `instructure-dap-client-0.3.7/dap/replicator/sql.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/timer.py` & `instructure-dap-client-0.3.7/dap/timer.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/dap/timestamp.py` & `instructure-dap-client-0.3.7/dap/timestamp.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/instructure_dap_client.egg-info/PKG-INFO` & `instructure-dap-client-0.3.7/instructure_dap_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.6
+Version: 0.3.7
 Summary: Data Access Platform client library
 Author: Levente Hunyadi
 Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

### Comparing `instructure-dap-client-0.3.6/instructure_dap_client.egg-info/SOURCES.txt` & `instructure-dap-client-0.3.7/instructure_dap_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.6/setup.cfg` & `instructure-dap-client-0.3.7/setup.cfg`

 * *Files identical despite different names*


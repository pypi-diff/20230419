# Comparing `tmp/bsl-appcli-1.3.6.tar.gz` & `tmp/bsl-appcli-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsl-appcli-1.3.6.tar", last modified: Mon Jan 24 01:21:46 2022, max compression
+gzip compressed data, was "bsl-appcli-1.4.0.tar", last modified: Wed Apr 19 04:06:31 2023, max compression
```

## Comparing `bsl-appcli-1.3.6.tar` & `bsl-appcli-1.4.0.tar`

### file list

```diff
@@ -1,60 +1,99 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    38088 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    31960 2022-01-24 01:13:07.000000 bsl-appcli-1.3.6/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.310031 bsl-appcli-1.3.6/appcli/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.310031 bsl-appcli-1.3.6/appcli/backup_manager/
--rw-rw-r--   0 tom       (1000) tom       (1000)    21984 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/backup_manager/backup_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8376 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/backup_manager/remote_strategy.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    12970 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/cli_builder.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/commands/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1340 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/appcli_command.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8352 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/backup_manager_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9275 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/configure_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8075 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/configure_template_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2391 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/debug_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1916 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/encrypt_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2400 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/init_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4276 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/install_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3284 2022-01-11 01:58:28.000000 bsl-appcli-1.3.6/appcli/commands/launcher_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2065 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/commands/migrate_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9313 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/commands/service_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2805 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/commands/task_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1305 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/commands/version_cli.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/common/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1556 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/common/data_class_extensions.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/configuration/
--rw-rw-r--   0 tom       (1000) tom       (1000)    13729 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/configuration/configuration_dir_state.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    25497 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/configuration_manager.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/crypto/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3987 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/crypto/cipher.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1783 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/crypto/crypto.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3086 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/functions.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/git_repositories/
--rw-rw-r--   0 tom       (1000) tom       (1000)     8026 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/git_repositories/git_repositories.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9871 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/keycloak_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1157 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/logger.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/models/
--rw-rw-r--   0 tom       (1000) tom       (1000)     4916 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/models/cli_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7592 2022-01-24 01:13:07.000000 bsl-appcli-1.3.6/appcli/models/configuration.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    26098 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/orchestrators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2658 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/string_transformer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/appcli/templates/
--rw-rw-r--   0 tom       (1000) tom       (1000)      196 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/templates/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3344 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/appcli/templates/installer.j2
--rw-rw-r--   0 tom       (1000) tom       (1000)     3391 2022-01-11 01:59:10.000000 bsl-appcli-1.3.6/appcli/templates/launcher.j2
--rw-rw-r--   0 tom       (1000) tom       (1000)     4064 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/appcli/variables_manager.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/bsl_appcli.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    38088 2022-01-24 01:21:46.000000 bsl-appcli-1.3.6/bsl_appcli.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1292 2022-01-24 01:21:46.000000 bsl-appcli-1.3.6/bsl_appcli.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2022-01-24 01:21:46.000000 bsl-appcli-1.3.6/bsl_appcli.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      303 2022-01-24 01:21:46.000000 bsl-appcli-1.3.6/bsl_appcli.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       13 2022-01-24 01:21:46.000000 bsl-appcli-1.3.6/bsl_appcli.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)     2244 2022-01-21 04:45:44.000000 bsl-appcli-1.3.6/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.310031 bsl-appcli-1.3.6/tests/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.310031 bsl-appcli-1.3.6/tests/resources/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.310031 bsl-appcli-1.3.6/tests/resources/templates/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.310031 bsl-appcli-1.3.6/tests/resources/templates/baseline/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2022-01-24 01:21:46.314031 bsl-appcli-1.3.6/tests/resources/templates/baseline/nesting/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2022-01-11 01:37:20.000000 bsl-appcli-1.3.6/tests/resources/templates/baseline/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.539481 bsl-appcli-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-04-19 04:06:31.539481 bsl-appcli-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/appcli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/appcli/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    22873 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/backup_manager/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/backup_manager/remote_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/cli_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/appcli_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/backup_manager_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/configure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/configure_template_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/debug_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/encrypt_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/init_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/install_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/launcher_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/migrate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/service_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/task_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/commands/version_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/common/data_class_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/configuration/configuration_dir_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/crypto/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/git_repositories/git_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/keycloak_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/models/cli_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28248 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/orchestrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/appcli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/templates/installer.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/templates/launcher.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/appcli/variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/bsl_appcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36266 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 04:06:31.000000 bsl-appcli-1.4.0/bsl_appcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 04:06:31.539481 bsl-appcli-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/backup_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    36535 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/backup_manager/test_backup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/cipher/test_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands/test_install_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands_task/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands_task/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands_task/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/commands_task/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/commands_task/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands_task/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/commands_task/test_commands_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration/test_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/expected_generated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_manager/expected_generated/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_manager/expected_generated/nesting/nested_baseline_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.531481 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/baseline/nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_manager/resources/templates/baseline/nesting/nested_baseline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_manager/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/configuration_state/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/configuration_state/test_configuration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/crypto/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/git_repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/git_repositories/test_git_repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/string_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/string_transformer/test_string_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/variables_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/variables_manager/test_variables_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:31.535481 bsl-appcli-1.4.0/tests/version/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-19 04:05:34.000000 bsl-appcli-1.4.0/tests/version/test_version.py
```

### Comparing `bsl-appcli-1.3.6/PKG-INFO` & `bsl-appcli-1.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,732 +1,850 @@
-Metadata-Version: 2.1
-Name: bsl-appcli
-Version: 1.3.6
-Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
-Home-page: https://www.brightsparklabs.com
-Author: brightSPARK Labs
-Author-email: enquire@brightsparklabs.com
-License: MIT License
-Description: # BSL Application CLI Library
-        
-        ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
-        
-        A library for adding CLI interfaces to applications in the brightSPARK Labs style.
-        
-        ## Overview
-        
-        This library can be leveraged to add a standardised CLI capability to applications to:
-        
-        - Handle system lifecycle events for services (`service [start|shutdown]`).
-        - Allow running arbitrary short-lived tasks (`task run`).
-        - Manage configuration (`configure`).
-        - Upgrade to a newer version of the application (`upgrade|migrate`).
-        - And more.
-        
-        The CLI is designed to run within a Docker container and launch other Docker containers (i.e.
-        Docker-in-Docker). This is generally managed via a `docker-compose.yml` file.
-        
-        The library exposes the following environment variables to the `docker-compose.yml` file:
-        
-        - `APP_VERSION` - the version of containers to launch.
-        - `<APP_NAME>_CONFIG_DIR` - the directory containing configuration files.
-        - `<APP_NAME>_DATA_DIR` - the directory containing data produced/consumed by the system.
-        - `<APP_NAME>_GENERATED_CONFIG_DIR` - the directory containing configuration files generated from
-          the templates in `<APP_NAME>_CONFIG_DIR`.
-        - `<APP_NAME>_ENVIRONMENT` - the deployment environment the system is running in. For example
-          `production` or `staging`. This allows multiple instances of the application to run on the same
-          Docker daemon. Defaults to `production`.
-        
-        Note: the `APP_NAME` variable is derived from the `app_name` passed in to the `Configuration` object in the
-        main python entrypoint to the application. In order for the application to work, the `app_name` is forced to conform
-        with the shell variable name standard: `[a-zA-Z_][a-zA-Z_0-9]*`. Any characters that do not fit this regex will be
-        replaced with `_`. See:
-        (https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable)
-        (https://linuxhint.com/bash-variable-name-rules-legal-illegal/)
-        
-        The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
-        variables within the `settings.yml` file as described in the Installation section.
-        
-        Stack variables can be set within the `stack-settings.yml` file as described in the
-        `Build configuration template directories` section.
-        
-        ## Installation
-        
-        ### Add the library to your python CLI application
-        
-            pip install git+https://github.com/brightsparklabs/appcli.git@<VERSION>
-        
-        ### Define the CLI for your application `myapp`
-        
-        _Note for appcli version 1.1.3 and below_: Import paths to access to appcli
-        internal classes and methods is now by a full path, rather than being exposed
-        at the root. This was done to allow access to all methods and classes using
-        python3 implicit namespaced packages.
-        
-            # filename: myapp.py
-        
-            #!/usr/bin/env python3
-            # # -*- coding: utf-8 -*-
-        
-            # standard libraries
-            import os
-            import sys
-            from pathlib import Path
-        
-            # vendor libraries
-            from appcli.cli_builder import create_cli
-            from appcli.models.configuration import Configuration
-            from appcli.orchestrators import DockerComposeOrchestrator
-        
-            # ------------------------------------------------------------------------------
-            # CONSTANTS
-            # ------------------------------------------------------------------------------
-        
-            # directory containing this script
-            BASE_DIR = os.path.dirname(os.path.realpath(__file__))
-        
-            # ------------------------------------------------------------------------------
-            # PRIVATE METHODS
-            # ------------------------------------------------------------------------------
-        
-            def main():
-                configuration = Configuration(
-                    app_name='myapp',
-                    docker_image='brightsparklabs/myapp',
-                    seed_app_configuration_file=Path(BASE_DIR, 'resources/settings.yml'),
-                    stack_configuration_file=Path(BASE_DIR, 'resources/stack-settings.yml'),
-                    baseline_templates_dir=Path(BASE_DIR, 'resources/templates/baseline'),
-                    configurable_templates_dir=Path(BASE_DIR, 'resources/templates/configurable'),
-                    orchestrator=DockerComposeOrchestrator(
-                        docker_compose_file = Path('docker-compose.yml'),
-                        docker_compose_override_directory = Path('docker-compose.override.d/'),
-                        docker_compose_task_file = Path('docker-compose.tasks.yml'),
-                        docker_compose_task_override_directory = Path(
-                            'docker-compose.tasks.override.d/'
-                        ),
-                    ),
-                    mandatory_additional_data_dirs=['EXTRA_DATA',],
-                    mandatory_additional_env_variables=['ENV_VAR_2',],
-                )
-                cli = create_cli(configuration)
-                cli()
-        
-            # ------------------------------------------------------------------------------
-            # ENTRYPOINT
-            # ------------------------------------------------------------------------------
-        
-            if __name__ == '__main__':
-                main()
-        
-        #### Custom Commands
-        
-        You can specify some custom top-level commands by adding click commands or command groups to the configuration object.
-        Assuming 'web' is the name of the service in the docker-compose.yml file which you wish to exec against, we can create
-        three custom commands in the following example:
-        
-        - `myapp ls-root` which lists the contents of the root directory within the `web` service container and prints it out.
-        - `myapp ls-root-to-file` which lists the contents of the root directory within the `web` service container and dumps to file within the container.
-        - `myapp tee-file` which takes some text and `tee`s it into another file the `web` service container.
-        
-        ```python
-        
-        def get_ls_root_command(orchestrator: DockerComposeOrchestrator):
-            @click.command(
-                help="List files in the root directory",
-            )
-            @click.pass_context
-            def ls_root(ctx: click.Context):
-        
-                # Equivalent command within the container:
-                # `ls -alh`
-                cli_context: CliContext = ctx.obj
-                output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
-                print(output.stdout.decode())
-        
-            return ls_root
-        
-        def get_tee_file_command(orchestrator: DockerComposeOrchestrator):
-            @click.command(
-                help="Tee some text into a file",
-            )
-            @click.pass_context
-            def tee_file(ctx: click.Context):
-        
-                # Equivalent command within the container:
-                # `echo "Some data to tee into the custom file" | tee /ls-root.txt`
-                cli_context: CliContext = ctx.obj
-                output: CompletedProcess = orchestrator.exec(cli_context, "web", ["tee", "/my_custom_file.txt"], stdin_input="Some data to tee into the custom file")
-        
-            return tee_file
-        
-        def get_ls_root_to_file_command(orchestrator: DockerComposeOrchestrator):
-            @click.command(
-                help="List files in the root directory and tee to file",
-            )
-            @click.pass_context
-            def ls_root_to_file(ctx: click.Context):
-        
-                # Equivalent command within the container:
-                # `ls -alh | tee /ls-root.txt`
-                cli_context: CliContext = ctx.obj
-                output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
-                data = output.stdout.decode()
-                orchestrator.exec(cli_context, "web", ["tee", "/ls-root.txt"], stdin_input=data)
-        
-            return ls_root_to_file
-        
-        def main():
-            orchestrator = DockerComposeOrchestrator(Path("docker-compose.yml"))
-            configuration = Configuration(
-                app_name="appcli_nginx",
-                docker_image="thomas-anderson-bsl/appcli-nginx",
-                seed_app_configuration_file=Path(BASE_DIR, "resources/settings.yml"),
-                stack_configuration_file=Path(BASE_DIR, "resources/stack-settings.yml"),
-                baseline_templates_dir=Path(BASE_DIR, "resources/templates/baseline"),
-                configurable_templates_dir=Path(BASE_DIR, "resources/templates/configurable"),
-                orchestrator=orchestrator,
-                custom_commands={get_tee_file_command(orchestrator),get_ls_root_command(orchestrator),get_ls_root_to_file_command(orchestrator)}
-            )
-            cli = create_cli(configuration)
-            cli()
-        
-        ```
-        
-        ### Build configuration template directories
-        
-        - Store any Jinja2 variable definitions you wish to use in your configuration
-          template files in `resources/settings.yml`.
-        - Store any appcli stack specific keys in `resources/stack-settings.yml`.
-        - Store your `docker-compose.yml`/`docker-compose.yml.j2` file in `resources/templates/baseline/`.
-        - Configuration files (Jinja2 compatible templates or otherwise) can be stored in one
-          of two locations:
-          - `resources/templates/baseline` - for templates which the end user **is not** expected to modify.
-          - `resources/templates/configurable` - for templates which the end user is expected to modify.
-        
-        ### Configure application backup
-        
-        Appcli's `backup` command creates backups of configuration and data of an application, stored locally in the
-        backup directory. The settings for backups are configured through entries in a `backups` block in `stack-settings.yml`.
-        
-        The available keys for entries in the `backups` block are:
-        
-        | key            | Description                                                                                                       |
-        | -------------- | ----------------------------------------------------------------------------------------------------------------- |
-        | name           | The name of the backup. Must be unique between backup definitions and use `kebab-case`.                           |
-        | backup_limit   | The number of local backups to keep. Set to `0` to disable rolling deletion.                                      |
-        | file_filter    | The file_filter contains lists of glob patterns used to specify what files to include or exclude from the backup. |
-        | frequency      | The cron-like frequency at which backups will execute.                                                            |
-        | remote_backups | The list of remote backup strategies.                                                                             |
-        
-            # filename: stack-settings.yml
-        
-            backups:
-              - name: "full"
-                backup_limit: 0
-                file_filter:
-                  data_dir:
-                    include_list:
-                    exclude_list:
-                  conf_dir:
-                    include_list:
-                    exclude_list:
-                frequency: "* * *"
-                remote_backups:
-        
-        #### Backup name
-        
-        The backup `name` is a short descriptive name for the backup definition.
-        To avoid problems, we _highly_ recommend `name` be:
-        
-        - unique between items in the `backups` list
-        - use `kebab-case`
-        
-        Examples of good names:
-        
-        - `full`
-        - `conf-only`
-        - `audit-logs`
-        
-        Without a unique `name`, backups from different items in `backups` will
-        overwrite each other without warning.
-        
-        Using `kebab-case` is necessary to avoid some issues with `click` and filesystem
-        naming issues.
-        
-        When using the `backup` command, you are able to supply the name
-        of the backup to run. If you have a backup `name` with a space in it, the `click`
-        library cannot interpret the name as a whole string (even with quotes), so you
-        will be unable to run the backup individually.
-        
-        If the backup `name` doesn't use `kebab-case`, it may use some characters that
-        are incompatible with file and directory naming conventions. Appcli will
-        automatically slugify the name to something compatible, but this may cause
-        collisions in the folder names of backups to be taken which will lead to backups
-        being overwritten. e.g. `s3#1` and `s3&1` will both translate internally to
-        `s3-1`.
-        
-        #### Backup limit
-        
-        A rolling deletion strategy is used to remove local backups, in order to keep `backup_limit` number of backups.
-        
-        If more than `backup_limit` number of backups exist in the backup directory, the oldest backups will be deleted.
-        
-        Set this value to `0` to keep all backups.
-        
-        #### File filter
-        
-        The `file_filter` block enables filtering of files to backup from `conf` and `data` directories. For more details
-        including examples, see [here](/README_BACKUP_FILE_FILTER.md).
-        
-            # filename: stack-settings.yml
-            # Includes all log files from data dir only
-        
-            backups:
-              - name: "full"
-                backup_limit: 0
-                file_filter:
-                  data_dir:
-                    include_list:
-                      - "**/*.log"
-                    exclude_list:
-                    conf_dir:
-                      include_list:
-                      exclude_list:
-                        - "**/*"
-                frequency: "* * *"
-                remote_backups:
-        
-        #### Freqency
-        
-        Appcli supports limiting individual backups to run on only specific days using a cron-like frequency filter.
-        
-        When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
-        today's date. Only strategies whose `frequency` pattern match today's date will execute.
-        
-        The input pattern `pattern` is prefixed with `"* * "` and is used as a standard cron expression to
-        check for a match. i.e. `"* * $pattern"`.
-        
-        Examples:
-        
-        - `"* * *"` (cron equivalent `"* * * * *"`) will always run.
-        - `"* * 0"` (cron equivalent `"* * * * 0"`) will only run on Sunday.
-        - `"1 */3 *"` (cron equivalent `"* * 1 */3 *"`) will only run on the first day-of-month of every 3rd month.
-        
-        #### Remote backup
-        
-        Appcli supports pushing local backups to remote storage. The list of strategies for pushing to remote storage are
-        defined within the `remote_backups` block.
-        
-        The available keys for every remote backup strategy are:
-        
-        | key           | Description                                                                                                 |
-        | ------------- | ----------------------------------------------------------------------------------------------------------- |
-        | name          | A short name or description used to describe this backup.                                                   |
-        | strategy_type | The type of this backup, must match an implemented remote backup strategy.                                  |
-        | frequency     | The cron-like frequency at which remote backups will execute. Behaves the same as local backup `frequency`. |
-        | configuration | Custom configuration block that is specific to each remote backup strategy.                                 |
-        
-        N.B. remote backups will only run for a local backup that has run. Therefore the `frequency` of the local backup
-        will apply first, followed by the `frequency` of the remote backup. This means that it's possible to write a remote
-        backup frequency that will never execute. e.g. Local `* * 0` and remote `* * 1`.
-        
-        ##### Strategies
-        
-        ###### AWS S3 remote strategy
-        
-        To use S3 remote backup, set `strategy_type` to `S3`.
-        The available configuration keys for an S3 backup are:
-        
-        | key         | Description                                                                                                                 |
-        | ----------- | --------------------------------------------------------------------------------------------------------------------------- |
-        | bucket_name | The name of the bucket to upload to.                                                                                        |
-        | access_key  | The AWS Access key ID for the account to upload with.                                                                       |
-        | secret_key  | The AWS Secret access key for the account to upload with. The value _must_ be encrypted using the appcli `encrypt` command. |
-        | bucket_path | The path in the S3 bucket to upload to. Set this to an empty string to upload to the root of the bucket.                    |
-        | tags        | Key value pairs of tags to set on the backup object.                                                                        |
-        
-            # filename: stack-settings.yml
-        
-            backups:
-              - name: "full_backup"
-                backup_limit: 0
-                remote_backups:
-                - name: "weekly_S3"
-                  strategy_type: "S3"
-                  frequency: "* * 0"
-                  configuration:
-                    bucket_name: "aws.s3.bucket"
-                    access_key: "aws_access_key"
-                    secret_key: "enc:id=1:encrypted_text:end"
-                    bucket_path: "bucket/path"
-                    tags:
-                      frequency: "weekly"
-                      type: "data"
-        
-        ### Restoring a remote backup
-        
-        To restore from a remote backup:
-        
-        1. Acquire the remote backup (`.tgz` file) that you wish to restore. For S3 this can be done by downloading the backup from the specified bucket.
-        2. Place the backup `myapp_date.tgz` file in the backup directory. By default this will be `/opt/brightsparklabs/${APP_NAME}/production/backup/`
-        3. Confirm that appcli can access the backup by running the `view-backups` command
-        4. Run the restore command `./myapp restore BACKUP_FILE.tgz` e.g. `./myapp restore APP_2021-02-02T10:55:48+00:00.tgz`. The restore process will trigger a backup.
-        
-        ### Define a container for your CLI application
-        
-            # filename: Dockerfile
-        
-            FROM brightsparklabs/appcli
-        
-            ENTRYPOINT ["./myapp.py"]
-            WORKDIR /app
-        
-            # install compose if using it as the orchestrator
-            RUN pip install docker-compose
-        
-            COPY requirements.txt .
-            RUN pip install --requirement requirements.txt
-            COPY src .
-        
-            ARG APP_VERSION=latest
-            ENV APP_VERSION=${APP_VERSION}
-        
-        ### Build the container
-        
-            # sh
-            docker build -t brightsparklabs/myapp --build-arg APP_VERSION=latest .
-        
-        ### (Optional) Login to private Docker registries and pass through credentials
-        
-        It is possible to login to private Docker registries on the host, and pass through credentials to
-        the CLI container run by the launcher script. This enables pulling and running Docker images from
-        private Docker registries.
-        
-        Login using:
-        
-            docker login ${REGISTRY_URL}
-        
-        The credentials file path can be passed as an option via `--docker-credentials-file` or `-p` to the
-        `myapp` container.
-        
-        ### View the installer script
-        
-            # sh
-            docker run --rm brightsparklabs/myapp:<version> install
-        
-            # or if using a private registry for images
-            docker run --rm brightsparklabs/myapp:<version> --docker-credentials-file ~/.docker/config.json install
-        
-        While it is not mandatory to view the script before running, it is highly recommended.
-        
-        ### Run the installer script
-        
-            # sh
-            docker run --rm brightsparklabs/myapp:<version> install | sudo bash
-        
-        The above will use the following defaults:
-        
-        - `environment` => `production`.
-        - `install-dir` => `/opt/brightsparklabs/${APP_NAME}/production/`.
-        - `configuration-dir` => `/opt/brightsparklabs/${APP_NAME}/production/conf/`.
-        - `data-dir` => `/opt/brightsparklabs/${APP_NAME}/production/data/`.
-        - `backup-dir` => `/opt/brightsparklabs/${APP_NAME}/production/backup/`.
-        
-        You can modify any of the above if desired. E.g.
-        
-            # sh
-            docker run --rm brightsparklabs/myapp:<version> \
-                --environment "uat" \
-                --configuration-dir /etc/myapp \
-                --data-dir /mnt/data/myapp \
-                install --install-dir ${HOME}/apps/myapp \
-            | sudo bash
-        
-        Where:
-        
-        - `--environment` defines the environment name for the deployment. This allows multiple instances of
-          the application to be present on the same host.
-          Defaults to `production`.
-        - `--install-dir` defines the base path for launcher and the default locations for the configuration
-          and data directories if they are not overrideen (see below).
-          Defaults to `/opt/brightsparklabs/${APP_NAME}/${ENVIRONMENT}/` (where `${ENVIRONMENT}` is defined
-          by `--environment` above).
-        - `--configuration-dir` defines the path to the configuration directory.
-          Defaults to `${INSTALL_DIR}/conf/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
-        - `--data-dir` defines the path to the data directory.
-          Defaults to `${INSTALL_DIR}/data/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
-        
-        The installation script will generate a launcher script for controlling the application. The script
-        location will be printed out when running the install script. This script should now be used as the
-        main entrypoint to all appcli functions for managing your application.
-        
-        ## Usage
-        
-        This section details what commands and options are available.
-        
-        ### Top-level Commands
-        
-        To be used in conjunction with your application `./myapp <command>` e.g. `./myapp configure init`
-        
-        | Command      | Description                                                       |
-        | ------------ | ----------------------------------------------------------------- |
-        | backup       | Create a backup of application data and configuration.            |
-        | configure    | Configures the application.                                       |
-        | encrypt      | Encrypts the specified string.                                    |
-        | init         | Initialises the application.                                      |
-        | launcher     | Outputs an appropriate launcher bash script.                      |
-        | migrate      | Migrates the configuration of the application to a newer version. |
-        | orchestrator | Perform docker orchestration                                      |
-        | restore      | Restore a backup of application data and configuration.           |
-        | service      | Lifecycle management commands for application services.           |
-        | task         | Commands for application tasks.                                   |
-        | version      | Fetches the version of the app being managed with appcli.         |
-        | view-backups | View a list of locally-available backups.                         |
-        
-        ### Options
-        
-        | Option                             | Description                                                                                                         |
-        | ---------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
-        | --debug                            | Enables debug level logging.                                                                                        |
-        | -c, --configuration-dir PATH       | Directory containing configuration files. [This is required unless subcommand is one of: `install`.                 |
-        | -d, --data-dir PATH                | Directory containing data produced/consumed by the system. This is required unless subcommand is one of: `install`. |
-        | -t, --environment TEXT             | Deployment environment the system is running in. Defaults to `production`.                                          |
-        | -p, --docker-credentials-file PATH | Path to the Docker credentials file (config.json) on the host for connecting to private Docker registries.          |
-        | -a, --additional-data-dir TEXT     | Additional data directory to expose to launcher container. Can be specified multiple times.                         |
-        | -e, --additional-env-var TEXT      | Additional environment variables to expose to launcher container. Can be specified multiple times.                  |
-        | --help                             | Show the help message and exit.                                                                                     |
-        
-        #### Command: `backup`
-        
-        Creates a backup `.tgz` file in the backup directory that contains files from the configuration and data directory, as
-        configured in `stack-settings.yml`. After the backup is taken, remote backup strategies will be executed (if applicable).
-        
-        usage: `./myapp backup [OPTIONS] [ARGS]`
-        
-        | Option                                         | Description                                        |
-        | ---------------------------------------------- | -------------------------------------------------- |
-        | --pre-stop-services/--no-pre-stop-services     | Whether to stop services before performing backup. |
-        | --post-start-services/--no-post-start-services | Whether to start services after performing backup. |
-        | --help                                         | Show the help message and exit.                    |
-        
-        The `backup` command optionally takes an argument corresponding to the `name` of the backup to run. If no `name` is
-        provided, all backups will attempt to run.
-        #### Command Group: `configure`
-        
-        Configures the application.
-        
-        usage: `./myapp configure [OPTIONS] COMMAND [ARGS]`
-        
-        | Command  | Description                                                                                                               |
-        | -------- | ------------------------------------------------------------------------------------------------------------------------- |
-        | apply    | Applies the settings from the configuration.                                                                              |
-        | diff     | Get the differences between current and default configuration settings.                                                   |
-        | get      | Reads a setting from the configuration.                                                                                   |
-        | init     | Initialises the configuration directory.                                                                                  |
-        | set      | Saves a setting to the configuration. Allows setting the type of value with option `--type`, and defaults to string type. |
-        | template | Configures the baseline templates.                                                                                        |
-        | edit     | Open the settings file for editing with vim-tiny.                                                                         |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `encrypt`
-        
-        Encrypts the specified string.
-        
-        usage: `./myapp encrypt [OPTIONS] TEXT`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `init`
-        
-        Initialises the application.
-        
-        usage: `./myapp init [OPTIONS] COMMAND [ARGS]`
-        
-        | Command  | Description                                                              |
-        | -------- | ------------------------------------------------------------------------ |
-        | keycloak | Initialises a Keycloak instance with BSL-specific initial configuration. |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `launcher`
-        
-        Outputs an appropriate launcher bash script to stdout.
-        
-        usage: `./myapp launcher [OPTIONS]`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `migrate`
-        
-        Migrates the application configuration to work with the current application version.
-        
-        usage: `./myapp migrate [OPTIONS]`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `orchestrator`
-        
-        Perform tasks defined by the orchestrator.
-        
-        usage: `./myapp orchestrator [OPTIONS] COMMAND [ARGS]`
-        
-        All commands are defined within the orchestrators themselves. Run `./myapp orchestrator` to list available commands.
-        
-        | Option | Description                    |
-        | ------ | ------------------------------ |
-        | --help | Show the help message and exit |
-        
-        #### Command: `restore`
-        
-        Restores a specified backup `.tgz` file from the configured backup folder.
-        
-        usage: `./myapp restore BACKUP_FILE`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `service`
-        
-        Runs application services. These are the long-running services which should only exit on command.
-        
-        usage: `./myapp service [OPTIONS] COMMAND [ARGS]`
-        
-        | Command  | Description                                                                                                                                                                                                             |
-        | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | logs     | Prints logs from all services.                                                                                                                                                                                          |
-        | shutdown | Shuts down the system. If one or more service names are provided, shuts down the specified service(s) only.                                                                                                             |
-        | start    | Starts the system. If one or more service names are provided, starts the specified service(s) only.                                                                                                                     |
-        | restart  | Restarts service(s) (`shutdown` followed by `start`). Optionally run a `configure apply` during the restart with the `--apply` flag. If one or more service names are provided, restarts the specified service(s) only. |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `task`
-        
-        Runs application tasks. These are short-lived services which should exit when the task is complete.
-        
-        usage: `./myapp task [OPTIONS] COMMAND [ARGS]`
-        
-        | Command | Description                                                                                  |
-        | ------- | -------------------------------------------------------------------------------------------- |
-        | run     | Runs a specified application task. Optionally run in the background with `-d/--detach` flag. |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `version`
-        
-        Fetches the version of the app being managed with appcli.
-        
-        usage: `./myapp version`
-        
-        #### Command: `view-backups`
-        
-        View a list of all backups in the configured backup folder.
-        
-        usage: `./myapp view-backups`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        ### Usage within scripts and cron
-        
-        By default, the generated `appcli` launcher script will run the CLI container with a virtual terminal session (tty).
-        This may interfere with crontab entries or scripts that use the appcli launcher.
-        
-        To disable tty when running the launcher script, set `NO_TTY` environment variable to `true`.
-        
-            NO_TTY=true ./myapp [...]
-        
-        or
-        
-            export NO_TTY=true
-            ./myapp [...]
-        
-        If required, you can also disable interactive mode with the `NO_INTERACTIVE` environment variable.
-        
-            NO_INTERACTIVE=true ./myapp [...]
-        
-        or
-        
-            export NO_INTERACTIVE=true
-            ./myapp [...]
-        
-        ## Development
-        
-        This section details how to build/test/run/debug the system in a development environment.
-        
-        ### Prerequisites
-        
-        The following must be installed and in the `PATH`:
-        
-        - make
-        - python 3.7+
-        - virtualenv
-        - git
-        
-        ### Build
-        
-            make all
-        
-        ### Install
-        
-            pip install -e .
-        
-        ### Running unit tests
-        
-            make test
-        
-        ## Usage while developing your CLI application
-        
-        While developing, it may be preferable to run your python script directly rather than having to
-        rebuild a container each time you update it.
-        
-        - Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
-        - Set the environment variables which the CLI usually sets for you:
-        
-                export MYAPP_CONFIG_DIR=/tmp/myapp/config \
-                       MYAPP_DATA_DIR=/tmp/myapp/data
-        
-        - Run your CLI application:
-        
-                ./myapp \
-                  --debug \
-                  --configuration-dir "${MYAPP_CONFIG_DIR}" \
-                  --data-dir "${MYAPP_DATA_DIR}"
-        
-        ## Contributing
-        
-        When committing code, call `make all` to automatically run code formatting/ linting/testing.
-        
-        Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
-        settings. This ensures that PR diffs are minimal and focussed on the code change rather than
-        stylistic coding decisions.
-        
-        Install with `pip install black`. This can be run through VSCode or via the CLI. See the `black`
-        documentation for details.
-        
-        ## Licenses
-        
-        Refer to the `LICENSE` file for details.
-        
-        This project makes use of several libraries and frameworks. Refer to the `LICENSES` folder for
-        details.
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+# BSL Application CLI Library
+
+![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
+
+A library for adding CLI interfaces to applications in the brightSPARK Labs style.
+
+## Overview
+
+This library can be leveraged to add a standardised CLI capability to applications to:
+
+- Handle system lifecycle events for services (`service [start|shutdown]`).
+- Allow running arbitrary short-lived tasks (`task run`).
+- Manage configuration (`configure`).
+- Upgrade to a newer version of the application (`upgrade|migrate`).
+- And more.
+
+The CLI is designed to run within a Docker container and launch other Docker containers (i.e.
+Docker-in-Docker). This is generally managed via a `docker-compose.yml` file.
+
+The library exposes the following environment variables to the `docker-compose.yml` file:
+
+- `APP_VERSION` - the version of containers to launch.
+- `<APP_NAME>_CONFIG_DIR` - the directory containing configuration files.
+- `<APP_NAME>_DATA_DIR` - the directory containing data produced/consumed by the system.
+- `<APP_NAME>_GENERATED_CONFIG_DIR` - the directory containing configuration files generated from
+  the templates in `<APP_NAME>_CONFIG_DIR`.
+- `<APP_NAME>_BACKUP_DIR` - the directory to use for system backups.
+- `<APP_NAME>_ENVIRONMENT` - the deployment environment the system is running in. For example
+  `production` or `staging`. This allows multiple instances of the application to run on the same
+  Docker daemon. Defaults to `production`.
+
+NOTE:
+The `APP_NAME` variable is derived from the `app_name` passed in to the `Configuration` object in
+the main python entrypoint to the application. In order for the application to work, the `app_name`
+is forced to conform with the shell variable name standard: `[a-zA-Z_][a-zA-Z_0-9]*`. Any characters
+that do not fit this regex will be replaced with `_`. See
+[here](https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable)
+or [here](https://linuxhint.com/bash-variable-name-rules-legal-illegal/) for details.
+
+The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
+variables within the `settings.yml` file as described in the Installation section.
+
+Stack variables can be set within the `stack-settings.yml` file as described in the
+`Build configuration template directories` section.
+
+## Quick Start
+
+Refer to the [quick start guide](quickstart.md) to get a basic application running.
+
+Otherwise refer to the Installation section below to see all options.
+
+## Installation
+
+### Add the library to your python CLI application
+
+    pip install git+https://github.com/brightsparklabs/appcli.git@<VERSION>
+
+### Define the CLI for your application `myapp`
+
+_Note for appcli version 1.1.3 and below_: Import paths to access to appcli
+internal classes and methods is now by a full path, rather than being exposed
+at the root. This was done to allow access to all methods and classes using
+python3 implicit namespaced packages.
+
+```python
+    # filename: myapp.py
+
+    #!/usr/bin/env python3
+    # # -*- coding: utf-8 -*-
+
+    # standard libraries
+    from pathlib import Path
+
+    # vendor libraries
+    from appcli.cli_builder import create_cli
+    from appcli.models.configuration import Configuration
+    from appcli.orchestrators import DockerComposeOrchestrator
+
+    # ------------------------------------------------------------------------------
+    # CONSTANTS
+    # ------------------------------------------------------------------------------
+
+    # directory containing this script
+    BASE_DIR = Path(__file__).parent
+
+    # ------------------------------------------------------------------------------
+    # PRIVATE METHODS
+    # ------------------------------------------------------------------------------
+
+    def main():
+        configuration = Configuration(
+            app_name='myapp',
+            docker_image='brightsparklabs/myapp',
+            seed_app_configuration_file=BASE_DIR / 'resources/settings.yml',
+            application_context_files_dir=BASE_DIR / 'resources/templates/appcli/context',
+            stack_configuration_file=BASE_DIR / 'resources/stack-settings.yml',
+            baseline_templates_dir=BASE_DIR / 'resources/templates/baseline',
+            configurable_templates_dir=BASE_DIR / 'resources/templates/configurable',
+            orchestrator=DockerComposeOrchestrator(
+                # NOTE: These paths are relative to 'resources/templates/baseline'.
+                docker_compose_file = Path('docker-compose.yml'),
+                docker_compose_override_directory = Path('docker-compose.override.d/'),
+                docker_compose_task_file = Path('docker-compose.tasks.yml'),
+                docker_compose_task_override_directory = Path( 'docker-compose.tasks.override.d/'),
+            ),
+            mandatory_additional_data_dirs=['EXTRA_DATA',],
+            mandatory_additional_env_variables=['ENV_VAR_2',],
+        )
+        cli = create_cli(configuration)
+        cli()
+
+    # ------------------------------------------------------------------------------
+    # ENTRYPOINT
+    # ------------------------------------------------------------------------------
+
+    if __name__ == '__main__':
+        main()
+```
+
+A lot of the fields in the appcli constructor can be defaulted, resulting in less code.
+
+```python
+configuration = Configuration(
+    app_name='myapp',
+    docker_image='brightsparklabs/myapp',
+)
+cli = create_cli(configuration)
+cli()
+```
+
+#### Custom Commands
+
+You can specify some custom top-level commands by adding click commands or command groups to the
+configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
+which you wish to exec against, we can create three custom commands in the following example:
+
+- `myapp ls-root` which lists the contents of the root directory within the `web` service container
+  and prints it out.
+- `myapp ls-root-to-file` which lists the contents of the root directory within the `web` service
+  container and dumps to file within the container.
+- `myapp tee-file` which takes some text and `tee`s it into another file the `web` service
+  container.
+
+```python
+
+def get_ls_root_command(orchestrator: DockerComposeOrchestrator):
+    @click.command(
+        help="List files in the root directory",
+    )
+    @click.pass_context
+    def ls_root(ctx: click.Context):
+
+        # Equivalent command within the container:
+        # `ls -alh`
+        cli_context: CliContext = ctx.obj
+        output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
+        print(output.stdout.decode())
+
+    return ls_root
+
+def get_tee_file_command(orchestrator: DockerComposeOrchestrator):
+    @click.command(
+        help="Tee some text into a file",
+    )
+    @click.pass_context
+    def tee_file(ctx: click.Context):
+
+        # Equivalent command within the container:
+        # `echo "Some data to tee into the custom file" | tee /ls-root.txt`
+        cli_context: CliContext = ctx.obj
+        output: CompletedProcess = orchestrator.exec(cli_context, "web", ["tee", "/my_custom_file.txt"], stdin_input="Some data to tee into the custom file")
+
+    return tee_file
+
+def get_ls_root_to_file_command(orchestrator: DockerComposeOrchestrator):
+    @click.command(
+        help="List files in the root directory and tee to file",
+    )
+    @click.pass_context
+    def ls_root_to_file(ctx: click.Context):
+
+        # Equivalent command within the container:
+        # `ls -alh | tee /ls-root.txt`
+        cli_context: CliContext = ctx.obj
+        output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
+        data = output.stdout.decode()
+        orchestrator.exec(cli_context, "web", ["tee", "/ls-root.txt"], stdin_input=data)
+
+    return ls_root_to_file
+
+def main():
+    orchestrator = DockerComposeOrchestrator(Path("docker-compose.yml"))
+    configuration = Configuration(
+        app_name="appcli_nginx",
+        docker_image="thomas-anderson-bsl/appcli-nginx",
+        seed_app_configuration_file=Path(BASE_DIR, "resources/settings.yml"),
+        stack_configuration_file=Path(BASE_DIR, "resources/stack-settings.yml"),
+        baseline_templates_dir=Path(BASE_DIR, "resources/templates/baseline"),
+        configurable_templates_dir=Path(BASE_DIR, "resources/templates/configurable"),
+        orchestrator=orchestrator,
+        custom_commands={get_tee_file_command(orchestrator),get_ls_root_command(orchestrator),get_ls_root_to_file_command(orchestrator)}
+    )
+    cli = create_cli(configuration)
+    cli()
+
+```
+
+### Build configuration template directories
+
+- Store any Jinja2 variable definitions you wish to use in your configuration
+  template files in `resources/settings.yml`.
+- Store any application context files in `resources/templates/appcli/context/`
+- Store any appcli stack specific keys in `resources/stack-settings.yml`.
+- Store your `docker-compose.yml`/`docker-compose.yml.j2` file in `resources/templates/baseline/`.
+- Configuration files (Jinja2 compatible templates or otherwise) can be stored in one
+  of two locations:
+  - `resources/templates/baseline` - for templates which the end user **is not** expected to modify.
+  - `resources/templates/configurable` - for templates which the end user is expected to modify.
+
+#### Application context files
+
+Template files are templated with Jinja2. The 'data' passed into the templating engine
+is a combination of the `settings.yml` and all application context files
+(stored in `resources/templates/appcli/context`, and referenced in the `Configuration`
+object as `application_context_files_dir`). Application context files that have the
+extension `.j2` are templated using the settings from `settings.yml`.
+
+These are combined to make the data for templating as follows:
+
+```json
+{
+  "settings": {
+    ... all settings from `settings.yml`
+  },
+  "application": {
+    <app_context_file_1>: {
+      ... settings from `app_context_file_1.yml`, optionally jinja2 templated using settings from `settings.yml`
+    },
+    ... additional app_context_files
+  }
+}
+```
+
+As a minimal example with the following YAML files:
+
+```yaml
+# ./settings.yml
+main_settings:
+  abc: 123
+
+# ./resources/templates/appcli/context/app_constants.yml
+other_settings:
+  hello: world
+
+# ./resources/templates/appcli/context/app_variables.yml.j2
+variables:
+  main_abc_setting: {{ settings.main_settings.abc }}
+```
+
+The data for Jinja2 templating engine will be:
+
+```json
+{
+  "settings": {
+    "main_settings": {
+      "abc": 123
+    }
+  },
+  "application": {
+    "app_constants": {
+      "other_settings": {
+        "hello": "world"
+      }
+    },
+    "app_variables": {
+      "variables": {
+        "main_abc_setting": 123
+      }
+    }
+  }
+}
+```
+
+### Configure application backup
+
+Appcli's `backup` command creates backups of configuration and data of an application, stored
+locally in the backup directory. The settings for backups are configured through entries in a
+`backups` block in `stack-settings.yml`.
+
+The available keys for entries in the `backups` block are:
+
+| key            | Description                                                                                                       |
+| -------------- | ----------------------------------------------------------------------------------------------------------------- |
+| name           | The name of the backup. Must be unique between backup definitions and use `kebab-case`.                           |
+| backup_limit   | The number of local backups to keep. Set to `0` to disable rolling deletion.                                      |
+| file_filter    | The file_filter contains lists of glob patterns used to specify what files to include or exclude from the backup. |
+| frequency      | The cron-like frequency at which backups will execute.                                                            |
+| remote_backups | The list of remote backup strategies.                                                                             |
+
+    # filename: stack-settings.yml
+
+    backups:
+      - name: "full"
+        backup_limit: 0
+        file_filter:
+          data_dir:
+            include_list:
+            exclude_list:
+          conf_dir:
+            include_list:
+            exclude_list:
+        frequency: "* * *"
+        remote_backups:
+
+#### Backup name
+
+The backup `name` is a short descriptive name for the backup definition.
+To avoid problems, we _highly_ recommend `name` be:
+
+- unique between items in the `backups` list
+- use `kebab-case`
+
+Examples of good names:
+
+- `full`
+- `conf-only`
+- `audit-logs`
+
+Without a unique `name`, backups from different items in `backups` will
+overwrite each other without warning.
+
+Using `kebab-case` is necessary to avoid some issues with `click` and filesystem
+naming issues.
+
+When using the `backup` command, you are able to supply the name
+of the backup to run. If you have a backup `name` with a space in it, the `click`
+library cannot interpret the name as a whole string (even with quotes), so you
+will be unable to run the backup individually.
+
+If the backup `name` doesn't use `kebab-case`, it may use some characters that
+are incompatible with file and directory naming conventions. Appcli will
+automatically slugify the name to something compatible, but this may cause
+collisions in the folder names of backups to be taken which will lead to backups
+being overwritten. e.g. `s3#1` and `s3&1` will both translate internally to
+`s3-1`.
+
+#### Backup limit
+
+A rolling deletion strategy is used to remove local backups, in order to keep `backup_limit` number
+of backups.
+
+If more than `backup_limit` number of backups exist in the backup directory, the oldest backups will
+be deleted.
+
+Set this value to `0` to keep all backups.
+
+#### File filter
+
+The `file_filter` block enables filtering of files to backup from `conf` and `data` directories. For
+more details including examples, see [here](/README_BACKUP_FILE_FILTER.md).
+
+    # filename: stack-settings.yml
+    # Includes all log files from data dir only
+
+    backups:
+      - name: "full"
+        backup_limit: 0
+        file_filter:
+          data_dir:
+            include_list:
+              - "**/*.log"
+            exclude_list:
+            conf_dir:
+              include_list:
+              exclude_list:
+                - "**/*"
+        frequency: "* * *"
+        remote_backups:
+
+#### Freqency
+
+Appcli supports limiting individual backups to run on only specific days using a cron-like frequency
+filter.
+
+When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
+today's date. Only strategies whose `frequency` pattern match today's date will execute.
+
+The input pattern `pattern` is prefixed with `"* * "` and is used as a standard cron expression to
+check for a match. i.e. `"* * $pattern"`.
+
+Examples:
+
+- `"* * *"` (cron equivalent `"* * * * *"`) will always run.
+- `"* * 0"` (cron equivalent `"* * * * 0"`) will only run on Sunday.
+- `"1 */3 *"` (cron equivalent `"* * 1 */3 *"`) will only run on the first day-of-month of every 3rd
+  month.
+
+#### Remote backup
+
+Appcli supports pushing local backups to remote storage. The list of strategies for pushing to
+remote storage are defined within the `remote_backups` block.
+
+The available keys for every remote backup strategy are:
+
+| key           | Description                                                                                                 |
+| ------------- | ----------------------------------------------------------------------------------------------------------- |
+| name          | A short name or description used to describe this backup.                                                   |
+| strategy_type | The type of this backup, must match an implemented remote backup strategy.                                  |
+| frequency     | The cron-like frequency at which remote backups will execute. Behaves the same as local backup `frequency`. |
+| configuration | Custom configuration block that is specific to each remote backup strategy.                                 |
+
+N.B. remote backups will only run for a local backup that has run. Therefore the `frequency` of the
+local backup will apply first, followed by the `frequency` of the remote backup. This means that
+it's possible to write a remote backup frequency that will never execute. e.g. Local `* * 0` and
+remote `* * 1`.
+
+##### Strategies
+
+###### AWS S3 remote strategy
+
+To use S3 remote backup, set `strategy_type` to `S3`.
+The available configuration keys for an S3 backup are:
+
+| key         | Description                                                                                                                 |
+| ----------- | --------------------------------------------------------------------------------------------------------------------------- |
+| bucket_name | The name of the bucket to upload to.                                                                                        |
+| access_key  | The AWS Access key ID for the account to upload with.                                                                       |
+| secret_key  | The AWS Secret access key for the account to upload with. The value _must_ be encrypted using the appcli `encrypt` command. |
+| bucket_path | The path in the S3 bucket to upload to. Set this to an empty string to upload to the root of the bucket.                    |
+| tags        | Key value pairs of tags to set on the backup object.                                                                        |
+
+    # filename: stack-settings.yml
+
+    backups:
+      - name: "full_backup"
+        backup_limit: 0
+        remote_backups:
+        - name: "weekly_S3"
+          strategy_type: "S3"
+          frequency: "* * 0"
+          configuration:
+            bucket_name: "aws.s3.bucket"
+            access_key: "aws_access_key"
+            secret_key: "enc:id=1:encrypted_text:end"
+            bucket_path: "bucket/path"
+            tags:
+              frequency: "weekly"
+              type: "data"
+
+### Restoring a remote backup
+
+To restore from a remote backup:
+
+1. Acquire the remote backup (`.tgz` file) that you wish to restore. For S3 this can be done by
+   downloading the backup from the specified bucket.
+2. Place the backup `myapp_date.tgz` file in the backup directory. By default this will be
+   `/opt/brightsparklabs/${APP_NAME}/production/backup/`
+3. Confirm that appcli can access the backup by running the `view-backups` command
+4. Run the restore command `./myapp restore BACKUP_FILE.tgz` e.g.
+   `./myapp restore APP_2021-02-02T10:55:48+00:00.tgz`. The restore process will trigger a backup.
+
+### Define a container for your CLI application
+
+    # filename: Dockerfile
+
+    FROM brightsparklabs/appcli
+
+    ENTRYPOINT ["./myapp.py"]
+    WORKDIR /app
+
+    # install compose if using it as the orchestrator
+    RUN pip install docker-compose
+
+    COPY requirements.txt .
+    RUN pip install --requirement requirements.txt
+    COPY src .
+
+    ARG APP_VERSION=latest
+    ENV APP_VERSION=${APP_VERSION}
+
+### Build the container
+
+    # sh
+    docker build -t brightsparklabs/myapp --build-arg APP_VERSION=latest .
+
+### (Optional) Login to private Docker registries and pass through credentials
+
+It is possible to login to private Docker registries on the host, and pass through credentials to
+the CLI container run by the launcher script. This enables pulling and running Docker images from
+private Docker registries.
+
+Login using:
+
+    docker login ${REGISTRY_URL}
+
+The credentials file path can be passed as an option via `--docker-credentials-file` or `-p` to the
+`myapp` container.
+
+### View the installer script
+
+    # sh
+    docker run --rm brightsparklabs/myapp:<version> install
+
+    # or if using a private registry for images
+    docker run --rm brightsparklabs/myapp:<version> \
+      --docker-credentials-file ~/.docker/config.json \
+      install
+
+While it is not mandatory to view the script before running, it is highly recommended.
+
+### Run the installer script
+
+    # sh
+    docker run --rm brightsparklabs/myapp:<version> install | sudo bash
+
+The above will use the following defaults:
+
+- `environment` => `production`.
+- `install-dir` => `/opt/brightsparklabs/${APP_NAME}/production/`.
+- `configuration-dir` => `/opt/brightsparklabs/${APP_NAME}/production/conf/`.
+- `data-dir` => `/opt/brightsparklabs/${APP_NAME}/production/data/`.
+- `backup-dir` => `/opt/brightsparklabs/${APP_NAME}/production/backup/`.
+
+You can modify any of the above if desired. E.g.
+
+    # sh
+    docker run --rm brightsparklabs/myapp:<version> \
+        --environment "uat" \
+        --configuration-dir /etc/myapp \
+        --data-dir /mnt/data/myapp \
+        install --install-dir ${HOME}/apps/myapp \
+    | sudo bash
+
+Where:
+
+- `--environment` defines the environment name for the deployment. This allows multiple instances of
+  the application to be present on the same host.
+  Defaults to `production`.
+- `--install-dir` defines the base path for launcher and the default locations for the configuration
+  and data directories if they are not overrideen (see below).
+  Defaults to `/opt/brightsparklabs/${APP_NAME}/${ENVIRONMENT}/` (where `${ENVIRONMENT}` is defined
+  by `--environment` above).
+- `--configuration-dir` defines the path to the configuration directory.
+  Defaults to `${INSTALL_DIR}/conf/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
+- `--data-dir` defines the path to the data directory.
+  Defaults to `${INSTALL_DIR}/data/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
+
+The installation script will generate a launcher script for controlling the application. The script
+location will be printed out when running the install script. This script should now be used as the
+main entrypoint to all appcli functions for managing your application.
+
+## Migration from appcli version <=1.3.6 to version >1.3.6
+
+As a result of supporting application context files, all references to
+settings in template files have moved.
+
+All settings in `settings.yml` used in templating are now namespaced under
+`settings`. All templates will need to change their references to use this new
+namespacing scheme. For example, in templates that refer to settings, change the
+references like so:
+
+- `my_app.server.hostname` -> `settings.my_app.server.hostname`
+- `my_app.server.http.port` -> `settings.my_app.server.http.port`
+
+## Usage
+
+This section details what commands and options are available.
+
+### Top-level Commands
+
+To be used in conjunction with your application `./myapp <command>` e.g. `./myapp configure init`
+
+| Command      | Description                                                       |
+| ------------ | ----------------------------------------------------------------- |
+| backup       | Create a backup of application data and configuration.            |
+| configure    | Configures the application.                                       |
+| encrypt      | Encrypts the specified string.                                    |
+| init         | Initialises the application.                                      |
+| launcher     | Outputs an appropriate launcher bash script.                      |
+| migrate      | Migrates the configuration of the application to a newer version. |
+| orchestrator | Perform docker orchestration                                      |
+| restore      | Restore a backup of application data and configuration.           |
+| service      | Lifecycle management commands for application services.           |
+| task         | Commands for application tasks.                                   |
+| version      | Fetches the version of the app being managed with appcli.         |
+| view-backups | View a list of locally-available backups.                         |
+
+### Options
+
+| Option                             | Description                                                                                                         |
+| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
+| --debug                            | Enables debug level logging.                                                                                        |
+| -c, --configuration-dir PATH       | Directory containing configuration files. [This is required unless subcommand is one of: `install`.                 |
+| -d, --data-dir PATH                | Directory containing data produced/consumed by the system. This is required unless subcommand is one of: `install`. |
+| -t, --environment TEXT             | Deployment environment the system is running in. Defaults to `production`.                                          |
+| -p, --docker-credentials-file PATH | Path to the Docker credentials file (config.json) on the host for connecting to private Docker registries.          |
+| -a, --additional-data-dir TEXT     | Additional data directory to expose to launcher container. Can be specified multiple times.                         |
+| -e, --additional-env-var TEXT      | Additional environment variables to expose to launcher container. Can be specified multiple times.                  |
+| --help                             | Show the help message and exit.                                                                                     |
+
+#### Command: `backup`
+
+Creates a backup `.tgz` file in the backup directory that contains files from the configuration and
+data directory, as configured in `stack-settings.yml`. After the backup is taken, remote backup
+strategies will be executed (if applicable).
+
+usage: `./myapp backup [OPTIONS] [ARGS]`
+
+| Option                                         | Description                                        |
+| ---------------------------------------------- | -------------------------------------------------- |
+| --pre-stop-services/--no-pre-stop-services     | Whether to stop services before performing backup. |
+| --post-start-services/--no-post-start-services | Whether to start services after performing backup. |
+| --help                                         | Show the help message and exit.                    |
+
+The `backup` command optionally takes an argument corresponding to the `name` of the backup to run.
+If no `name` is provided, all backups will attempt to run.
+
+#### Command Group: `configure`
+
+Configures the application.
+
+usage: `./myapp configure [OPTIONS] COMMAND [ARGS]`
+
+| Command    | Description                                                                                                               |
+| ---------- | ------------------------------------------------------------------------------------------------------------------------- |
+| apply      | Applies the settings from the configuration.                                                                              |
+| diff       | Get the differences between current and default configuration settings.                                                   |
+| get        | Reads a setting from the configuration.                                                                                   |
+| get-secure | Reads a setting from the configuration, decrypting if it is encrypted. This will prompt for the setting key.              |
+| init       | Initialises the configuration directory.                                                                                  |
+| set        | Saves a setting to the configuration. Allows setting the type of value with option `--type`, and defaults to string type. |
+| template   | Configures the baseline templates.                                                                                        |
+| edit       | Open the settings file for editing with vim-tiny.                                                                         |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `encrypt`
+
+Encrypts the specified string.
+
+usage: `./myapp encrypt [OPTIONS] TEXT`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `init`
+
+Initialises the application.
+
+usage: `./myapp init [OPTIONS] COMMAND [ARGS]`
+
+| Command  | Description                                                              |
+| -------- | ------------------------------------------------------------------------ |
+| keycloak | Initialises a Keycloak instance with BSL-specific initial configuration. |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `launcher`
+
+Outputs an appropriate launcher bash script to stdout.
+
+usage: `./myapp launcher [OPTIONS]`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `migrate`
+
+Migrates the application configuration to work with the current application version.
+
+usage: `./myapp migrate [OPTIONS]`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `orchestrator`
+
+Perform tasks defined by the orchestrator.
+
+usage: `./myapp orchestrator [OPTIONS] COMMAND [ARGS]`
+
+All commands are defined within the orchestrators themselves. Run `./myapp orchestrator` to list
+available commands.
+
+For example, the following commands are available to docker-compose:
+
+| Command | Description                                                                                                        |
+| ------- | ------------------------------------------------------------------------------------------------------------------ |
+| ps      | List containers for the appcli project, with current status and exposed ports.                                     |
+| compose | Run a docker compose command. See [docker compose](https://docs.docker.com/engine/reference/commandline/compose/). |
+
+| Option | Description                    |
+| ------ | ------------------------------ |
+| --help | Show the help message and exit |
+
+#### Command: `restore`
+
+Restores a specified backup `.tgz` file from the configured backup folder.
+
+usage: `./myapp restore BACKUP_FILE`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `service`
+
+Runs application services. These are the long-running services which should only exit on command.
+
+usage: `./myapp service [OPTIONS] COMMAND [ARGS]`
+
+| Command  | Description                                                                                                                                                                                                             |
+| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| logs     | Prints logs from all services.                                                                                                                                                                                          |
+| shutdown | Shuts down the system. If one or more service names are provided, shuts down the specified service(s) only.                                                                                                             |
+| start    | Starts the system. If one or more service names are provided, starts the specified service(s) only.                                                                                                                     |
+| restart  | Restarts service(s) (`shutdown` followed by `start`). Optionally run a `configure apply` during the restart with the `--apply` flag. If one or more service names are provided, restarts the specified service(s) only. |
+| status   | Lists all containers for the appcli project, with current status and exposed ports. If one or more service names are provided, lists the status and 
+ exposed ports of the specified service(s) only. |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `task`
+
+Runs application tasks. These are short-lived services which should exit when the task is complete.
+
+usage: `./myapp task [OPTIONS] COMMAND [ARGS]`
+
+| Command | Description                                                                                  |
+| ------- | -------------------------------------------------------------------------------------------- |
+| run     | Runs a specified application task. Optionally run in the background with `-d/--detach` flag. |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `version`
+
+Fetches the version of the app being managed with appcli.
+
+usage: `./myapp version`
+
+#### Command: `view-backups`
+
+View a list of all backups in the configured backup folder.
+
+usage: `./myapp view-backups`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+### Usage within scripts and cron
+
+By default, the generated `appcli` launcher script will run the CLI container with a virtual
+terminal session (tty).  This may interfere with crontab entries or scripts that use the appcli
+launcher.
+
+To disable tty when running the launcher script, set `NO_TTY` environment variable to `true`.
+
+    NO_TTY=true ./myapp [...]
+
+or
+
+    export NO_TTY=true
+    ./myapp [...]
+
+If required, you can also disable interactive mode with the `NO_INTERACTIVE` environment variable.
+
+    NO_INTERACTIVE=true ./myapp [...]
+
+or
+
+    export NO_INTERACTIVE=true
+    ./myapp [...]
+
+## Development
+
+This section details how to build/test/run/debug the system in a development environment.
+
+### Prerequisites
+
+The following must be installed and in the `PATH`:
+
+- make
+- python 3.7+
+- virtualenv
+- git
+
+### Build
+
+    make all
+
+### Install
+
+    pip install -e .
+
+### Running unit tests
+
+    make test
+
+## Usage while developing your CLI application
+
+While developing, it may be preferable to run your python script directly rather than having to
+rebuild a container each time you update it.
+
+- Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
+- Set the environment variables which the CLI usually sets for you:
+
+        export \
+            MYAPP_DATA_DIR=/tmp/myapp/data \
+            MYAPP_CONFIG_DIR=/tmp/myapp/config \
+            MYAPP_GENERATED_CONFIG_DIR=/tmp/myapp/config/.generated \
+            MYAPP_BACKUP_DIR=/tmp/myapp/backup \
+            MYAPP_ENVIRONMENT=dev
+- Run your CLI application:
+
+        ./src/myapp.py \
+              --debug \
+              --configuration-dir "${MYAPP_CONFIG_DIR}" \
+              --data-dir "${MYAPP_DATA_DIR}" \
+              --backup-dir "${MYAPP_BACKUP_DIR}" \
+              --environment "${MYAPP_ENVIRONMENT}
+
+## Contributing
+
+When committing code, call `make all` to automatically run code formatting/ linting/testing.
+
+Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
+settings. This ensures that PR diffs are minimal and focussed on the code change rather than
+stylistic coding decisions.
+
+Install with `pip install black`. This can be run through VSCode or via the CLI. See the `black`
+documentation for details.
+
+## Licenses
+
+Refer to the `LICENSE` file for details.
+
+This project makes use of several libraries and frameworks. Refer to the `LICENSES` folder for
+details.
```

### Comparing `bsl-appcli-1.3.6/README.md` & `bsl-appcli-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: bsl-appcli
+Version: 1.4.0
+Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
+Home-page: https://www.brightsparklabs.com
+Author: brightSPARK Labs
+Author-email: enquire@brightsparklabs.com
+License: MIT License
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # BSL Application CLI Library
 
 ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
 
 A library for adding CLI interfaces to applications in the brightSPARK Labs style.
 
 ## Overview
@@ -20,108 +32,130 @@
 The library exposes the following environment variables to the `docker-compose.yml` file:
 
 - `APP_VERSION` - the version of containers to launch.
 - `<APP_NAME>_CONFIG_DIR` - the directory containing configuration files.
 - `<APP_NAME>_DATA_DIR` - the directory containing data produced/consumed by the system.
 - `<APP_NAME>_GENERATED_CONFIG_DIR` - the directory containing configuration files generated from
   the templates in `<APP_NAME>_CONFIG_DIR`.
+- `<APP_NAME>_BACKUP_DIR` - the directory to use for system backups.
 - `<APP_NAME>_ENVIRONMENT` - the deployment environment the system is running in. For example
   `production` or `staging`. This allows multiple instances of the application to run on the same
   Docker daemon. Defaults to `production`.
 
-Note: the `APP_NAME` variable is derived from the `app_name` passed in to the `Configuration` object in the
-main python entrypoint to the application. In order for the application to work, the `app_name` is forced to conform
-with the shell variable name standard: `[a-zA-Z_][a-zA-Z_0-9]*`. Any characters that do not fit this regex will be
-replaced with `_`. See:
-(https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable)
-(https://linuxhint.com/bash-variable-name-rules-legal-illegal/)
+NOTE:
+The `APP_NAME` variable is derived from the `app_name` passed in to the `Configuration` object in
+the main python entrypoint to the application. In order for the application to work, the `app_name`
+is forced to conform with the shell variable name standard: `[a-zA-Z_][a-zA-Z_0-9]*`. Any characters
+that do not fit this regex will be replaced with `_`. See
+[here](https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable)
+or [here](https://linuxhint.com/bash-variable-name-rules-legal-illegal/) for details.
 
 The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
 variables within the `settings.yml` file as described in the Installation section.
 
 Stack variables can be set within the `stack-settings.yml` file as described in the
 `Build configuration template directories` section.
 
+## Quick Start
+
+Refer to the [quick start guide](quickstart.md) to get a basic application running.
+
+Otherwise refer to the Installation section below to see all options.
+
 ## Installation
 
 ### Add the library to your python CLI application
 
     pip install git+https://github.com/brightsparklabs/appcli.git@<VERSION>
 
 ### Define the CLI for your application `myapp`
 
 _Note for appcli version 1.1.3 and below_: Import paths to access to appcli
 internal classes and methods is now by a full path, rather than being exposed
 at the root. This was done to allow access to all methods and classes using
 python3 implicit namespaced packages.
 
+```python
     # filename: myapp.py
 
     #!/usr/bin/env python3
     # # -*- coding: utf-8 -*-
 
     # standard libraries
-    import os
-    import sys
     from pathlib import Path
 
     # vendor libraries
     from appcli.cli_builder import create_cli
     from appcli.models.configuration import Configuration
     from appcli.orchestrators import DockerComposeOrchestrator
 
     # ------------------------------------------------------------------------------
     # CONSTANTS
     # ------------------------------------------------------------------------------
 
     # directory containing this script
-    BASE_DIR = os.path.dirname(os.path.realpath(__file__))
+    BASE_DIR = Path(__file__).parent
 
     # ------------------------------------------------------------------------------
     # PRIVATE METHODS
     # ------------------------------------------------------------------------------
 
     def main():
         configuration = Configuration(
             app_name='myapp',
             docker_image='brightsparklabs/myapp',
-            seed_app_configuration_file=Path(BASE_DIR, 'resources/settings.yml'),
-            stack_configuration_file=Path(BASE_DIR, 'resources/stack-settings.yml'),
-            baseline_templates_dir=Path(BASE_DIR, 'resources/templates/baseline'),
-            configurable_templates_dir=Path(BASE_DIR, 'resources/templates/configurable'),
+            seed_app_configuration_file=BASE_DIR / 'resources/settings.yml',
+            application_context_files_dir=BASE_DIR / 'resources/templates/appcli/context',
+            stack_configuration_file=BASE_DIR / 'resources/stack-settings.yml',
+            baseline_templates_dir=BASE_DIR / 'resources/templates/baseline',
+            configurable_templates_dir=BASE_DIR / 'resources/templates/configurable',
             orchestrator=DockerComposeOrchestrator(
+                # NOTE: These paths are relative to 'resources/templates/baseline'.
                 docker_compose_file = Path('docker-compose.yml'),
                 docker_compose_override_directory = Path('docker-compose.override.d/'),
                 docker_compose_task_file = Path('docker-compose.tasks.yml'),
-                docker_compose_task_override_directory = Path(
-                    'docker-compose.tasks.override.d/'
-                ),
+                docker_compose_task_override_directory = Path( 'docker-compose.tasks.override.d/'),
             ),
             mandatory_additional_data_dirs=['EXTRA_DATA',],
             mandatory_additional_env_variables=['ENV_VAR_2',],
         )
         cli = create_cli(configuration)
         cli()
 
     # ------------------------------------------------------------------------------
     # ENTRYPOINT
     # ------------------------------------------------------------------------------
 
     if __name__ == '__main__':
         main()
+```
+
+A lot of the fields in the appcli constructor can be defaulted, resulting in less code.
+
+```python
+configuration = Configuration(
+    app_name='myapp',
+    docker_image='brightsparklabs/myapp',
+)
+cli = create_cli(configuration)
+cli()
+```
 
 #### Custom Commands
 
-You can specify some custom top-level commands by adding click commands or command groups to the configuration object.
-Assuming 'web' is the name of the service in the docker-compose.yml file which you wish to exec against, we can create
-three custom commands in the following example:
-
-- `myapp ls-root` which lists the contents of the root directory within the `web` service container and prints it out.
-- `myapp ls-root-to-file` which lists the contents of the root directory within the `web` service container and dumps to file within the container.
-- `myapp tee-file` which takes some text and `tee`s it into another file the `web` service container.
+You can specify some custom top-level commands by adding click commands or command groups to the
+configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
+which you wish to exec against, we can create three custom commands in the following example:
+
+- `myapp ls-root` which lists the contents of the root directory within the `web` service container
+  and prints it out.
+- `myapp ls-root-to-file` which lists the contents of the root directory within the `web` service
+  container and dumps to file within the container.
+- `myapp tee-file` which takes some text and `tee`s it into another file the `web` service
+  container.
 
 ```python
 
 def get_ls_root_command(orchestrator: DockerComposeOrchestrator):
     @click.command(
         help="List files in the root directory",
     )
@@ -183,25 +217,91 @@
 
 ```
 
 ### Build configuration template directories
 
 - Store any Jinja2 variable definitions you wish to use in your configuration
   template files in `resources/settings.yml`.
+- Store any application context files in `resources/templates/appcli/context/`
 - Store any appcli stack specific keys in `resources/stack-settings.yml`.
 - Store your `docker-compose.yml`/`docker-compose.yml.j2` file in `resources/templates/baseline/`.
 - Configuration files (Jinja2 compatible templates or otherwise) can be stored in one
   of two locations:
   - `resources/templates/baseline` - for templates which the end user **is not** expected to modify.
   - `resources/templates/configurable` - for templates which the end user is expected to modify.
 
+#### Application context files
+
+Template files are templated with Jinja2. The 'data' passed into the templating engine
+is a combination of the `settings.yml` and all application context files
+(stored in `resources/templates/appcli/context`, and referenced in the `Configuration`
+object as `application_context_files_dir`). Application context files that have the
+extension `.j2` are templated using the settings from `settings.yml`.
+
+These are combined to make the data for templating as follows:
+
+```json
+{
+  "settings": {
+    ... all settings from `settings.yml`
+  },
+  "application": {
+    <app_context_file_1>: {
+      ... settings from `app_context_file_1.yml`, optionally jinja2 templated using settings from `settings.yml`
+    },
+    ... additional app_context_files
+  }
+}
+```
+
+As a minimal example with the following YAML files:
+
+```yaml
+# ./settings.yml
+main_settings:
+  abc: 123
+
+# ./resources/templates/appcli/context/app_constants.yml
+other_settings:
+  hello: world
+
+# ./resources/templates/appcli/context/app_variables.yml.j2
+variables:
+  main_abc_setting: {{ settings.main_settings.abc }}
+```
+
+The data for Jinja2 templating engine will be:
+
+```json
+{
+  "settings": {
+    "main_settings": {
+      "abc": 123
+    }
+  },
+  "application": {
+    "app_constants": {
+      "other_settings": {
+        "hello": "world"
+      }
+    },
+    "app_variables": {
+      "variables": {
+        "main_abc_setting": 123
+      }
+    }
+  }
+}
+```
+
 ### Configure application backup
 
-Appcli's `backup` command creates backups of configuration and data of an application, stored locally in the
-backup directory. The settings for backups are configured through entries in a `backups` block in `stack-settings.yml`.
+Appcli's `backup` command creates backups of configuration and data of an application, stored
+locally in the backup directory. The settings for backups are configured through entries in a
+`backups` block in `stack-settings.yml`.
 
 The available keys for entries in the `backups` block are:
 
 | key            | Description                                                                                                       |
 | -------------- | ----------------------------------------------------------------------------------------------------------------- |
 | name           | The name of the backup. Must be unique between backup definitions and use `kebab-case`.                           |
 | backup_limit   | The number of local backups to keep. Set to `0` to disable rolling deletion.                                      |
@@ -254,24 +354,26 @@
 automatically slugify the name to something compatible, but this may cause
 collisions in the folder names of backups to be taken which will lead to backups
 being overwritten. e.g. `s3#1` and `s3&1` will both translate internally to
 `s3-1`.
 
 #### Backup limit
 
-A rolling deletion strategy is used to remove local backups, in order to keep `backup_limit` number of backups.
+A rolling deletion strategy is used to remove local backups, in order to keep `backup_limit` number
+of backups.
 
-If more than `backup_limit` number of backups exist in the backup directory, the oldest backups will be deleted.
+If more than `backup_limit` number of backups exist in the backup directory, the oldest backups will
+be deleted.
 
 Set this value to `0` to keep all backups.
 
 #### File filter
 
-The `file_filter` block enables filtering of files to backup from `conf` and `data` directories. For more details
-including examples, see [here](/README_BACKUP_FILE_FILTER.md).
+The `file_filter` block enables filtering of files to backup from `conf` and `data` directories. For
+more details including examples, see [here](/README_BACKUP_FILE_FILTER.md).
 
     # filename: stack-settings.yml
     # Includes all log files from data dir only
 
     backups:
       - name: "full"
         backup_limit: 0
@@ -285,45 +387,48 @@
               exclude_list:
                 - "**/*"
         frequency: "* * *"
         remote_backups:
 
 #### Freqency
 
-Appcli supports limiting individual backups to run on only specific days using a cron-like frequency filter.
+Appcli supports limiting individual backups to run on only specific days using a cron-like frequency
+filter.
 
 When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
 today's date. Only strategies whose `frequency` pattern match today's date will execute.
 
 The input pattern `pattern` is prefixed with `"* * "` and is used as a standard cron expression to
 check for a match. i.e. `"* * $pattern"`.
 
 Examples:
 
 - `"* * *"` (cron equivalent `"* * * * *"`) will always run.
 - `"* * 0"` (cron equivalent `"* * * * 0"`) will only run on Sunday.
-- `"1 */3 *"` (cron equivalent `"* * 1 */3 *"`) will only run on the first day-of-month of every 3rd month.
+- `"1 */3 *"` (cron equivalent `"* * 1 */3 *"`) will only run on the first day-of-month of every 3rd
+  month.
 
 #### Remote backup
 
-Appcli supports pushing local backups to remote storage. The list of strategies for pushing to remote storage are
-defined within the `remote_backups` block.
+Appcli supports pushing local backups to remote storage. The list of strategies for pushing to
+remote storage are defined within the `remote_backups` block.
 
 The available keys for every remote backup strategy are:
 
 | key           | Description                                                                                                 |
 | ------------- | ----------------------------------------------------------------------------------------------------------- |
 | name          | A short name or description used to describe this backup.                                                   |
 | strategy_type | The type of this backup, must match an implemented remote backup strategy.                                  |
 | frequency     | The cron-like frequency at which remote backups will execute. Behaves the same as local backup `frequency`. |
 | configuration | Custom configuration block that is specific to each remote backup strategy.                                 |
 
-N.B. remote backups will only run for a local backup that has run. Therefore the `frequency` of the local backup
-will apply first, followed by the `frequency` of the remote backup. This means that it's possible to write a remote
-backup frequency that will never execute. e.g. Local `* * 0` and remote `* * 1`.
+N.B. remote backups will only run for a local backup that has run. Therefore the `frequency` of the
+local backup will apply first, followed by the `frequency` of the remote backup. This means that
+it's possible to write a remote backup frequency that will never execute. e.g. Local `* * 0` and
+remote `* * 1`.
 
 ##### Strategies
 
 ###### AWS S3 remote strategy
 
 To use S3 remote backup, set `strategy_type` to `S3`.
 The available configuration keys for an S3 backup are:
@@ -354,18 +459,21 @@
               frequency: "weekly"
               type: "data"
 
 ### Restoring a remote backup
 
 To restore from a remote backup:
 
-1. Acquire the remote backup (`.tgz` file) that you wish to restore. For S3 this can be done by downloading the backup from the specified bucket.
-2. Place the backup `myapp_date.tgz` file in the backup directory. By default this will be `/opt/brightsparklabs/${APP_NAME}/production/backup/`
+1. Acquire the remote backup (`.tgz` file) that you wish to restore. For S3 this can be done by
+   downloading the backup from the specified bucket.
+2. Place the backup `myapp_date.tgz` file in the backup directory. By default this will be
+   `/opt/brightsparklabs/${APP_NAME}/production/backup/`
 3. Confirm that appcli can access the backup by running the `view-backups` command
-4. Run the restore command `./myapp restore BACKUP_FILE.tgz` e.g. `./myapp restore APP_2021-02-02T10:55:48+00:00.tgz`. The restore process will trigger a backup.
+4. Run the restore command `./myapp restore BACKUP_FILE.tgz` e.g.
+   `./myapp restore APP_2021-02-02T10:55:48+00:00.tgz`. The restore process will trigger a backup.
 
 ### Define a container for your CLI application
 
     # filename: Dockerfile
 
     FROM brightsparklabs/appcli
 
@@ -402,15 +510,17 @@
 
 ### View the installer script
 
     # sh
     docker run --rm brightsparklabs/myapp:<version> install
 
     # or if using a private registry for images
-    docker run --rm brightsparklabs/myapp:<version> --docker-credentials-file ~/.docker/config.json install
+    docker run --rm brightsparklabs/myapp:<version> \
+      --docker-credentials-file ~/.docker/config.json \
+      install
 
 While it is not mandatory to view the script before running, it is highly recommended.
 
 ### Run the installer script
 
     # sh
     docker run --rm brightsparklabs/myapp:<version> install | sudo bash
@@ -447,14 +557,27 @@
 - `--data-dir` defines the path to the data directory.
   Defaults to `${INSTALL_DIR}/data/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
 
 The installation script will generate a launcher script for controlling the application. The script
 location will be printed out when running the install script. This script should now be used as the
 main entrypoint to all appcli functions for managing your application.
 
+## Migration from appcli version <=1.3.6 to version >1.3.6
+
+As a result of supporting application context files, all references to
+settings in template files have moved.
+
+All settings in `settings.yml` used in templating are now namespaced under
+`settings`. All templates will need to change their references to use this new
+namespacing scheme. For example, in templates that refer to settings, change the
+references like so:
+
+- `my_app.server.hostname` -> `settings.my_app.server.hostname`
+- `my_app.server.http.port` -> `settings.my_app.server.http.port`
+
 ## Usage
 
 This section details what commands and options are available.
 
 ### Top-level Commands
 
 To be used in conjunction with your application `./myapp <command>` e.g. `./myapp configure init`
@@ -485,42 +608,45 @@
 | -p, --docker-credentials-file PATH | Path to the Docker credentials file (config.json) on the host for connecting to private Docker registries.          |
 | -a, --additional-data-dir TEXT     | Additional data directory to expose to launcher container. Can be specified multiple times.                         |
 | -e, --additional-env-var TEXT      | Additional environment variables to expose to launcher container. Can be specified multiple times.                  |
 | --help                             | Show the help message and exit.                                                                                     |
 
 #### Command: `backup`
 
-Creates a backup `.tgz` file in the backup directory that contains files from the configuration and data directory, as
-configured in `stack-settings.yml`. After the backup is taken, remote backup strategies will be executed (if applicable).
+Creates a backup `.tgz` file in the backup directory that contains files from the configuration and
+data directory, as configured in `stack-settings.yml`. After the backup is taken, remote backup
+strategies will be executed (if applicable).
 
 usage: `./myapp backup [OPTIONS] [ARGS]`
 
 | Option                                         | Description                                        |
 | ---------------------------------------------- | -------------------------------------------------- |
 | --pre-stop-services/--no-pre-stop-services     | Whether to stop services before performing backup. |
 | --post-start-services/--no-post-start-services | Whether to start services after performing backup. |
 | --help                                         | Show the help message and exit.                    |
 
-The `backup` command optionally takes an argument corresponding to the `name` of the backup to run. If no `name` is
-provided, all backups will attempt to run.
+The `backup` command optionally takes an argument corresponding to the `name` of the backup to run.
+If no `name` is provided, all backups will attempt to run.
+
 #### Command Group: `configure`
 
 Configures the application.
 
 usage: `./myapp configure [OPTIONS] COMMAND [ARGS]`
 
-| Command  | Description                                                                                                               |
-| -------- | ------------------------------------------------------------------------------------------------------------------------- |
-| apply    | Applies the settings from the configuration.                                                                              |
-| diff     | Get the differences between current and default configuration settings.                                                   |
-| get      | Reads a setting from the configuration.                                                                                   |
-| init     | Initialises the configuration directory.                                                                                  |
-| set      | Saves a setting to the configuration. Allows setting the type of value with option `--type`, and defaults to string type. |
-| template | Configures the baseline templates.                                                                                        |
-| edit     | Open the settings file for editing with vim-tiny.                                                                         |
+| Command    | Description                                                                                                               |
+| ---------- | ------------------------------------------------------------------------------------------------------------------------- |
+| apply      | Applies the settings from the configuration.                                                                              |
+| diff       | Get the differences between current and default configuration settings.                                                   |
+| get        | Reads a setting from the configuration.                                                                                   |
+| get-secure | Reads a setting from the configuration, decrypting if it is encrypted. This will prompt for the setting key.              |
+| init       | Initialises the configuration directory.                                                                                  |
+| set        | Saves a setting to the configuration. Allows setting the type of value with option `--type`, and defaults to string type. |
+| template   | Configures the baseline templates.                                                                                        |
+| edit       | Open the settings file for editing with vim-tiny.                                                                         |
 
 | Option | Description                     |
 | ------ | ------------------------------- |
 | --help | Show the help message and exit. |
 
 #### Command: `encrypt`
 
@@ -568,15 +694,23 @@
 
 #### Command Group: `orchestrator`
 
 Perform tasks defined by the orchestrator.
 
 usage: `./myapp orchestrator [OPTIONS] COMMAND [ARGS]`
 
-All commands are defined within the orchestrators themselves. Run `./myapp orchestrator` to list available commands.
+All commands are defined within the orchestrators themselves. Run `./myapp orchestrator` to list
+available commands.
+
+For example, the following commands are available to docker-compose:
+
+| Command | Description                                                                                                        |
+| ------- | ------------------------------------------------------------------------------------------------------------------ |
+| ps      | List containers for the appcli project, with current status and exposed ports.                                     |
+| compose | Run a docker compose command. See [docker compose](https://docs.docker.com/engine/reference/commandline/compose/). |
 
 | Option | Description                    |
 | ------ | ------------------------------ |
 | --help | Show the help message and exit |
 
 #### Command: `restore`
 
@@ -596,14 +730,16 @@
 
 | Command  | Description                                                                                                                                                                                                             |
 | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | logs     | Prints logs from all services.                                                                                                                                                                                          |
 | shutdown | Shuts down the system. If one or more service names are provided, shuts down the specified service(s) only.                                                                                                             |
 | start    | Starts the system. If one or more service names are provided, starts the specified service(s) only.                                                                                                                     |
 | restart  | Restarts service(s) (`shutdown` followed by `start`). Optionally run a `configure apply` during the restart with the `--apply` flag. If one or more service names are provided, restarts the specified service(s) only. |
+| status   | Lists all containers for the appcli project, with current status and exposed ports. If one or more service names are provided, lists the status and 
+ exposed ports of the specified service(s) only. |
 
 | Option | Description                     |
 | ------ | ------------------------------- |
 | --help | Show the help message and exit. |
 
 #### Command Group: `task`
 
@@ -633,16 +769,17 @@
 
 | Option | Description                     |
 | ------ | ------------------------------- |
 | --help | Show the help message and exit. |
 
 ### Usage within scripts and cron
 
-By default, the generated `appcli` launcher script will run the CLI container with a virtual terminal session (tty).
-This may interfere with crontab entries or scripts that use the appcli launcher.
+By default, the generated `appcli` launcher script will run the CLI container with a virtual
+terminal session (tty).  This may interfere with crontab entries or scripts that use the appcli
+launcher.
 
 To disable tty when running the launcher script, set `NO_TTY` environment variable to `true`.
 
     NO_TTY=true ./myapp [...]
 
 or
 
@@ -687,23 +824,28 @@
 
 While developing, it may be preferable to run your python script directly rather than having to
 rebuild a container each time you update it.
 
 - Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
 - Set the environment variables which the CLI usually sets for you:
 
-        export MYAPP_CONFIG_DIR=/tmp/myapp/config \
-               MYAPP_DATA_DIR=/tmp/myapp/data
-
+        export \
+            MYAPP_DATA_DIR=/tmp/myapp/data \
+            MYAPP_CONFIG_DIR=/tmp/myapp/config \
+            MYAPP_GENERATED_CONFIG_DIR=/tmp/myapp/config/.generated \
+            MYAPP_BACKUP_DIR=/tmp/myapp/backup \
+            MYAPP_ENVIRONMENT=dev
 - Run your CLI application:
 
-        ./myapp \
-          --debug \
-          --configuration-dir "${MYAPP_CONFIG_DIR}" \
-          --data-dir "${MYAPP_DATA_DIR}"
+        ./src/myapp.py \
+              --debug \
+              --configuration-dir "${MYAPP_CONFIG_DIR}" \
+              --data-dir "${MYAPP_DATA_DIR}" \
+              --backup-dir "${MYAPP_BACKUP_DIR}" \
+              --environment "${MYAPP_ENVIRONMENT}
 
 ## Contributing
 
 When committing code, call `make all` to automatically run code formatting/ linting/testing.
 
 Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
 settings. This ensures that PR diffs are minimal and focussed on the code change rather than
```

### Comparing `bsl-appcli-1.3.6/appcli/backup_manager/backup_manager.py` & `bsl-appcli-1.4.0/appcli/backup_manager/backup_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         if not sub_backup_dir.exists():
             sub_backup_dir.mkdir(parents=True, exist_ok=True)
 
         # Get the backup name to use when creating the tar.
         backup_name: Path = os.path.join(
             sub_backup_dir,
             self.__create_backup_filename(
-                cli_context.app_name, self.get_filesystem_safe_name()
+                cli_context.app_name_slug, self.get_filesystem_safe_name()
             ),
         )
 
         data_dir: Path = cli_context.data_dir
         conf_dir: Path = cli_context.configuration_dir
 
         # Determine the list of conf files to add to the tar.
@@ -264,33 +264,32 @@
         Returns:
             List[RemoteBackup]: A list of configured remote backups.
         """
 
         backup_strategies: List[RemoteBackup] = []
 
         for remote_configuration in self.remote_backups:
-
             try:
                 remote_backup: RemoteBackup = RemoteBackup.from_dict(
                     remote_configuration
                 )
 
                 backup_strategies.append(remote_backup)
 
             except TypeError as e:
                 logger.error(f"Failed to create remote strategy - {e}")
 
         return backup_strategies
 
-    def __create_backup_filename(self, app_name: str, backup_name: str) -> str:
+    def __create_backup_filename(self, app_name_slug: str, backup_name: str) -> str:
         """Generate the filename of the backup .tgz file.
-            Format is "<APP_NAME>_<BACKUP_NAME>_<datetime.now>.tgz".
+            Format is "<APP_NAME_SLUG>_<BACKUP_NAME>_<datetime.now>.tgz".
 
         Args:
-            app_name: (str). The application name to be used in the naming of the tgz file.
+            app_name_slug: (str). The application name to be used in the naming of the tgz file.
             backup_name: (str). The name of the backup being taken.
         Returns:
             The formatted .tgz filename.
         """
         # datetime's ISO format includes the ':' separator for the `hours:minutes:seconds`.
         # Since we're using this format in the filename of the backup, the backup filename
         # will include the ':' character.
@@ -298,15 +297,15 @@
         # resouces. To avoid this issue, we remove all ':'.
         now: str = (
             datetime.datetime.now(datetime.timezone.utc)
             .replace(microsecond=0)
             .isoformat()
             .replace(":", "")
         )
-        return f"{app_name.upper()}_{backup_name.upper()}_{now}.tgz"
+        return f"{app_name_slug.upper()}_{backup_name.upper()}_{now}.tgz"
 
     def __rolling_backup_deletion(self, backup_dir: Path):
         """Delete old backups, will only keep the most recent backups.
         The number of backups to keep is specified in the stack settings configuration file.
         Note that the age of the backup is derived from the alphanumerical order of the backup filename.
         This means that any supplementary files in the backup directory could have unintended consequences during
         rolling deletion.
@@ -467,21 +466,42 @@
         logger.debug(f"Backup(s) complete. Generated backups: [{restore_backup_name}]")
 
         # Extract conf and data directories from the tar.
         # This will overwrite the contents of each directory, anything not in the backup (such as files matching the exclude glob patterns) will be left alone.
         try:
             with tarfile.open(backup_name) as tar:
                 conf_dir: Path = cli_context.configuration_dir
-                tar.extractall(
-                    conf_dir, members=self.__members(tar, os.path.basename(conf_dir))
+                data_dir: Path = cli_context.data_dir
+
+                def is_within_directory(directory, target):
+                    abs_directory = os.path.abspath(directory)
+                    abs_target = os.path.abspath(target)
+
+                    prefix = os.path.commonprefix([abs_directory, abs_target])
+
+                    return prefix == abs_directory
+
+                def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+                    for member in tar.getmembers():
+                        member_path = os.path.join(path, member.name)
+                        if not is_within_directory(path, member_path):
+                            raise Exception("Attempted Path Traversal in Tar File")
+
+                    tar.extractall(path, members, numeric_owner=numeric_owner)
+
+                safe_extract(
+                    tar=tar,
+                    path=conf_dir,
+                    members=self.__members(tar, os.path.basename(conf_dir)),
                 )
 
-                data_dir: Path = cli_context.data_dir
-                tar.extractall(
-                    data_dir, members=self.__members(tar, os.path.basename(data_dir))
+                safe_extract(
+                    tar=tar,
+                    path=data_dir,
+                    members=self.__members(tar, os.path.basename(data_dir)),
                 )
 
         except Exception as e:
             logger.error(f"Failed to extract backup. Reason: {e}")
 
         logger.info("Restore complete.")
```

### Comparing `bsl-appcli-1.3.6/appcli/backup_manager/remote_strategy.py` & `bsl-appcli-1.4.0/appcli/backup_manager/remote_strategy.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.3.6/appcli/cli_builder.py` & `bsl-appcli-1.4.0/appcli/cli_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
 def create_cli(configuration: Configuration, desired_environment: Dict[str, str] = {}):
     """Build the CLI to be run
 
     Args:
         configuration (Configuration): the application's configuration settings
     """
-    APP_NAME = configuration.app_name.upper()
+    APP_NAME = configuration.app_name
+    APP_NAME_SLUG = configuration.app_name_slug
     APP_VERSION = os.environ.get("APP_VERSION", "latest")
 
     # --------------------------------------------------------------------------
     # CREATE_CLI: LOGIC
     # --------------------------------------------------------------------------
 
     default_commands = {}
@@ -156,21 +157,22 @@
         if debug:
             logger.info("Enabling debug logging")
             enable_debug_logging()
 
         ctx.obj = CliContext(
             configuration_dir=configuration_dir,
             data_dir=data_dir,
+            application_context_files_dir=configuration.application_context_files_dir,
             additional_data_dirs=additional_data_dir,
             additional_env_variables=additional_env_var,
             environment=environment,
             docker_credentials_file=docker_credentials_file,
             subcommand_args=ctx.obj,
             debug=debug,
-            app_name=APP_NAME,
+            app_name_slug=APP_NAME_SLUG,
             app_version=APP_VERSION,
             commands=default_commands,
             backup_dir=backup_dir,
         )
 
         if ctx.invoked_subcommand is None:
             click.echo(ctx.get_help())
@@ -235,31 +237,33 @@
                     colalign=("right",),
                 ),
             )
 
     def run():
         """Run the entry-point click CLI command"""
         cli(  # pylint: disable=no-value-for-parameter,unexpected-keyword-arg
-            prog_name=configuration.app_name
+            prog_name=configuration.app_name_slug
         )
 
     def check_docker_socket():
         """Check that the docker socket exists, and exit if it does not"""
         if not os.path.exists("/var/run/docker.sock"):
             error_msg = """Docker socket not present. Please launch with a mounted /var/run/docker.sock"""
             error_and_exit(error_msg)
 
     def check_environment():
         """Confirm that mandatory environment variables and additional data directories are defined."""
 
-        ENV_VAR_CONFIG_DIR = f"{APP_NAME}_CONFIG_DIR"
-        ENV_VAR_GENERATED_CONFIG_DIR = f"{APP_NAME}_GENERATED_CONFIG_DIR"
-        ENV_VAR_DATA_DIR = f"{APP_NAME}_DATA_DIR"
-        ENV_VAR_BACKUP_DIR = f"{APP_NAME}_BACKUP_DIR"
-        ENV_VAR_ENVIRONMENT = f"{APP_NAME}_ENVIRONMENT"
+        app_name_slug_upper = APP_NAME_SLUG.upper()
+
+        ENV_VAR_CONFIG_DIR = f"{app_name_slug_upper}_CONFIG_DIR"
+        ENV_VAR_GENERATED_CONFIG_DIR = f"{app_name_slug_upper}_GENERATED_CONFIG_DIR"
+        ENV_VAR_DATA_DIR = f"{app_name_slug_upper}_DATA_DIR"
+        ENV_VAR_BACKUP_DIR = f"{app_name_slug_upper}_BACKUP_DIR"
+        ENV_VAR_ENVIRONMENT = f"{app_name_slug_upper}_ENVIRONMENT"
         launcher_set_mandatory_env_vars = [
             ENV_VAR_CONFIG_DIR,
             ENV_VAR_GENERATED_CONFIG_DIR,
             ENV_VAR_DATA_DIR,
             ENV_VAR_BACKUP_DIR,
             ENV_VAR_ENVIRONMENT,
         ]
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/appcli_command.py` & `bsl-appcli-1.4.0/appcli/commands/appcli_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     LAUNCHER = auto()
 
     MIGRATE = auto()
 
     SERVICE_START = auto()
     SERVICE_SHUTDOWN = auto()
     SERVICE_LOGS = auto()
+    SERVICE_STATUS = auto()
 
     TASK_RUN = auto()
 
     ORCHESTRATOR = auto()
 
     BACKUP = auto()
     RESTORE = auto()
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/backup_manager_cli.py` & `bsl-appcli-1.4.0/appcli/commands/backup_manager_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,21 +36,19 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class BackupManagerCli:
-
     # --------------------------------------------------------------------------
     # CONSTRUCTOR
     # --------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
-
         self.cli_configuration: Configuration = configuration
 
         # ------------------------------------------------------------------------------
         # PUBLIC METHODS
         # ------------------------------------------------------------------------------
 
         @click.command(
@@ -168,15 +166,14 @@
         @click.option(
             "--force",
             is_flag=True,
             help="Force viewing backups even if validation checks fail.",
         )
         @click.pass_context
         def view_backups(ctx, force):
-
             cli_context: CliContext = ctx.obj
             cli_context.get_configuration_dir_state().verify_command_allowed(
                 AppcliCommand.VIEW_BACKUPS, force
             )
 
             backup_manager: BackupManager = self.__create_backup_manager(cli_context)
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/configure_cli.py` & `bsl-appcli-1.4.0/appcli/commands/configure_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,34 @@
                 AppcliCommand.CONFIGURE_GET
             )
 
             # Get settings value and print
             configuration = ConfigurationManager(cli_context, self.cli_configuration)
             print(configuration.get_variable(setting))
 
+        @configure.command(
+            help="Reads a setting from the configuration and decrypts if necessary.",
+            hidden=True,
+        )
+        @click.pass_context
+        def get_secure(ctx):
+            cli_context: CliContext = ctx.obj
+            cli_context.get_configuration_dir_state().verify_command_allowed(
+                AppcliCommand.CONFIGURE_GET
+            )
+
+            # We prompt for the key value so that the key doesn't show up in terminal history
+            # Without this, `history | grep password` might lead a potential attacker to easily find relevant
+            # credentials in the settings files. This just adds another layer of obfuscation.
+            setting = click.prompt("Please enter the key to the setting", type=str)
+
+            # Get settings value and print
+            configuration = ConfigurationManager(cli_context, self.cli_configuration)
+            print(configuration.get_variable(setting, decrypt=True))
+
         @configure.command(help="Saves a setting to the configuration.")
         @click.option(
             "-t",
             "--type",
             type=click.Choice(StringTransformer.get_types()),
             default=StringTransformer.get_string_transformer_type(),
         )
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/configure_template_cli.py` & `bsl-appcli-1.4.0/appcli/commands/configure_template_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 # ------------------------------------------------------------------------------
 
 
 class ConfigureTemplateCli:
     def __init__(self, configuration: Configuration):
         self.cli_configuration: Configuration = configuration
 
-        self.app_name = self.cli_configuration.app_name
-
         # ------------------------------------------------------------------------------
         # CLI METHODS
         # ------------------------------------------------------------------------------
 
         @click.group(
             invoke_without_command=True, help="Configures the baseline templates."
         )
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/debug_cli.py` & `bsl-appcli-1.4.0/appcli/commands/debug_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,16 +50,15 @@
         )
         @click.pass_context
         def info(ctx):
             cli_context: CliContext = ctx.obj
             cli_context.get_configuration_dir_state().verify_command_allowed(
                 AppcliCommand.DEBUG_INFO
             )
-            app_config_file = cli_context.get_app_configuration_file()
-            variables_manager = VariablesManager(app_config_file)
+            variables_manager: VariablesManager = cli_context.get_variables_manager()
 
             print()
             print("=== CLI CONTEXT ===")
             pprint(cli_context)
 
             print()
             print("=== CONFIGURATION ===")
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/encrypt_cli.py` & `bsl-appcli-1.4.0/appcli/commands/encrypt_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,19 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class EncryptCli:
-
     # --------------------------------------------------------------------------
     # CONSTRUCTOR
     # --------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
-
         self.configuration: Configuration = configuration
 
         @click.command(help="Encrypts the specified string.")
         @click.argument("text", required=False)
         @click.pass_context
         def encrypt(ctx: Context, text: str = None):
             """Encrypt a string using the application keyfile.
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/init_cli.py` & `bsl-appcli-1.4.0/appcli/commands/init_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class InitCli:
     def __init__(self, configuration: Configuration):
-        self.app_name = configuration.app_name
+        self.app_name_slug = configuration.app_name_slug
 
         # ------------------------------------------------------------------------------
         # CLI METHODS
         # ------------------------------------------------------------------------------
 
         @click.group(invoke_without_command=True, help="Initialises the application.")
         @click.pass_context
@@ -56,14 +56,14 @@
             "-k",
             is_flag=True,
             help="If supplied, allows insecure and unverified SSL connections to Keycloak.",
         )
         @click.pass_context
         def keycloak(ctx, url, username, password, insecure):
             keycloak = KeycloakManager(url, username, password, insecure=insecure)
-            keycloak.configure_default(self.app_name)
+            keycloak.configure_default(self.app_name_slug)
 
         self.commands = {"init": init}
 
     # ------------------------------------------------------------------------------
     # PRIVATE METHODS
     # ------------------------------------------------------------------------------
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/install_cli.py` & `bsl-appcli-1.4.0/appcli/commands/install_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,23 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class InstallCli:
-
     # ------------------------------------------------------------------------------
     # CONSTRUCTOR
     # ------------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
         self.configuration: Configuration = configuration
-        default_install_dir = f"/opt/brightsparklabs/{configuration.app_name.lower()}"
+        default_install_dir = (
+            f"/opt/brightsparklabs/{configuration.app_name_slug.lower()}"
+        )
 
         @click.command(
             hidden=True, help="Outputs an appropriate installer bash script to stdout."
         )
         @click.option(
             "--install-dir",
             "-i",
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/launcher_cli.py` & `bsl-appcli-1.4.0/appcli/commands/launcher_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,19 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class LauncherCli:
-
     # ------------------------------------------------------------------------------
     # CONSTRUCTOR
     # ------------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
-
         self.configuration: Configuration = configuration
 
         @click.command(help="Outputs an appropriate launcher bash script to stdout.")
         @click.pass_context
         def launcher(ctx):
             cli_context: CliContext = ctx.obj
             cli_context.get_configuration_dir_state().verify_command_allowed(
@@ -64,15 +62,16 @@
             launcher_template = pkg_resources.read_text(
                 templates, LAUNCHER_TEMPLATE_FILENAME
             )
             logger.debug(f"Read template file [{LAUNCHER_TEMPLATE_FILENAME}]")
 
             render_variables = {
                 "app_version": os.environ.get("APP_VERSION", "latest"),
-                "app_name": configuration.app_name.upper(),
+                "app_name": configuration.app_name,
+                "app_name_slug": configuration.app_name_slug,
                 "cli_context": ctx.obj,
                 "configuration": self.configuration,
                 "current_datetime": f"{datetime.datetime.utcnow().isoformat()}+00:00",  # Since we're using utcnow(), we specify the offset manually
             }
 
             logger.debug(
                 f"Rendering template with render variables: [{render_variables}]"
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/migrate_cli.py` & `bsl-appcli-1.4.0/appcli/commands/migrate_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class MigrateCli:
-
     # ------------------------------------------------------------------------------
     # CONSTRUCTOR
     # ------------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
         self.cli_configuration: Configuration = configuration
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/service_cli.py` & `bsl-appcli-1.4.0/appcli/commands/service_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,22 +35,23 @@
 class ServiceAction(enum.Enum):
     """
     Enum representing avaliable actions to apply to an appcli service or group of services.
 
     Options:
         START: Start service(s)
         SHUTDOWN: Shutdown service(s)
+        STATUS: Get status of service(s)
     """
 
     START = enum.auto()
     SHUTDOWN = enum.auto()
+    STATUS = enum.auto()
 
 
 class ServiceCli:
-
     # --------------------------------------------------------------------------
     # CONSTRUCTOR
     # --------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
         self.cli_configuration: Configuration = configuration
         self.orchestrator = configuration.orchestrator
@@ -172,14 +173,30 @@
         def stop(ctx: Context, service_names: tuple[str, ...]):
             cli_context: CliContext = ctx.obj
             cli_context.get_configuration_dir_state().verify_command_allowed(
                 AppcliCommand.SERVICE_SHUTDOWN
             )
             self._action_orchestrator(ctx, ServiceAction.SHUTDOWN, service_names)
 
+        @service.command(help="Gets the status of services.")
+        @click.argument(
+            "service_names",
+            required=False,
+            type=click.STRING,
+            nargs=-1,
+            callback=self._validate_service_names,
+        )
+        @click.pass_context
+        def status(ctx: Context, service_names: tuple[str, ...]):
+            cli_context: CliContext = ctx.obj
+            cli_context.get_configuration_dir_state().verify_command_allowed(
+                AppcliCommand.SERVICE_STATUS
+            )
+            self._action_orchestrator(ctx, ServiceAction.STATUS, service_names)
+
         # Add the 'logs' subcommand
         service.add_command(self.orchestrator.get_logs_command())
 
         # expose the CLI commands
         self.commands = {
             "service": service,
         }
@@ -235,32 +252,40 @@
             post_hook = hooks.post_start
 
         elif action == ServiceAction.SHUTDOWN:
             action_run_function = self.orchestrator.shutdown
             pre_hook = hooks.pre_shutdown
             post_hook = hooks.post_shutdown
 
+        elif action == ServiceAction.STATUS:
+            action_run_function = self.orchestrator.status
+            pre_hook = None
+            post_hook = None
+
         else:
             error_and_exit(f"Unhandled action called: [{action.name}]")
 
         pre_run_log_message = (
             f"{action.name} "
             + (
                 ", ".join(service_names)
                 if service_names is not None and len(service_names) > 0
                 else self.cli_configuration.app_name
             )
             + " ..."
         )
         post_run_log_message = f"{action.name} command finished with code [%i]"
 
-        logger.debug(f"Running pre-{action.name} hook")
-        pre_hook(ctx)
+        if pre_hook is not None:
+            logger.debug(f"Running pre-{action.name} hook")
+            pre_hook(ctx)
 
         logger.info(pre_run_log_message)
         result = action_run_function(ctx.obj, service_names)
 
-        logger.debug(f"Running post-{action.name} hook")
-        post_hook(ctx, result)
+        if post_hook is not None:
+            logger.debug(f"Running post-{action.name} hook")
+            post_hook(ctx, result)
 
+        click.echo(result.stdout)
         logger.info(post_run_log_message, result.returncode)
         sys.exit(result.returncode)
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/task_cli.py` & `bsl-appcli-1.4.0/appcli/commands/task_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class TaskCli:
-
     # --------------------------------------------------------------------------
     # CONSTRUCTOR
     # --------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
         self.cli_configuration: Configuration = configuration
         self.orchestrator = configuration.orchestrator
```

### Comparing `bsl-appcli-1.3.6/appcli/commands/version_cli.py` & `bsl-appcli-1.4.0/appcli/commands/version_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,19 @@
 
 # ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class VersionCli:
-
     # --------------------------------------------------------------------------
     # CONSTRUCTOR
     # --------------------------------------------------------------------------
 
     def __init__(self, configuration: Configuration):
-
         self.configuration: Configuration = configuration
 
         @click.command(help="Fetches app version")
         @click.pass_context
         def version(ctx):
             """Fetches the version of the app being managed with appcli"""
             cli_context: CliContext = ctx.obj
```

### Comparing `bsl-appcli-1.3.6/appcli/common/data_class_extensions.py` & `bsl-appcli-1.4.0/appcli/common/data_class_extensions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.3.6/appcli/configuration/configuration_dir_state.py` & `bsl-appcli-1.4.0/appcli/configuration/configuration_dir_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
             return False
 
 
 class NoDirectoryProvidedConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where appcli doesn't know the path to configuration dir."""
 
     def __init__(self) -> None:
-
         default_error_message = (
             "No configuration directory provided to appcli. Run 'install'."
         )
 
         disallowed_command = get_disallowed_command_from_allowed_commands(
             [AppcliCommand.INSTALL],
             default_error_message,
@@ -139,44 +138,41 @@
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class NoDirectoryProvidedBackupDirState(ConfigurationDirState):
     """Represents the backup dir state where appcli doesn't know the path to backup dir."""
 
     def __init__(self) -> None:
-
         disallowed_command = {
             AppcliCommand.BACKUP: "Cannot backup due to missing backup directory. Run 'install'.",
             AppcliCommand.RESTORE: "Cannot restore due to missing backup directory. Run 'install'.",
             AppcliCommand.VIEW_BACKUPS: "Cannot view backups due to missing backup directory. Run 'install'.",
         }
         disallowed_command_unless_forced = {}
 
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class BackupDirectoryDoesNotExist(ConfigurationDirState):
     """Represents the backup dir state where the backup directory does not exist."""
 
     def __init__(self) -> None:
-
         disallowed_command = {
             AppcliCommand.RESTORE: "Cannot restore due to missing backup directory. Run 'backup'.",
             AppcliCommand.VIEW_BACKUPS: "Cannot view backups due to missing backup directory. Run 'backup'.",
         }
         disallowed_command_unless_forced = {}
 
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class UninitialisedConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where config directory hasn't been initialised."""
 
     def __init__(self) -> None:
-
         default_error_message = "Cannot run command against uninitialised application. Run 'configure init'."
 
         disallowed_command = get_disallowed_command_from_allowed_commands(
             [
                 AppcliCommand.CONFIGURE_INIT,
                 AppcliCommand.LAUNCHER,
                 AppcliCommand.BACKUP,
@@ -191,20 +187,20 @@
 
 
 class UnappliedConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where configuration hasn't been applied yet, i.e. the generated
     configuration doesn't exist."""
 
     def __init__(self) -> None:
-
         disallowed_command = {
             AppcliCommand.CONFIGURE_INIT: "Cannot initialise an existing configuration.",
             AppcliCommand.SERVICE_START: "Cannot start services due to missing generated configuration. Run 'configure apply'.",
             AppcliCommand.SERVICE_SHUTDOWN: "Cannot stop services due to missing generated configuration. Run 'configure apply'.",
             AppcliCommand.SERVICE_LOGS: "Cannot get service logs due to missing generated configuration. Run 'configure apply'.",
+            AppcliCommand.SERVICE_STATUS: "Cannot get the status of services due to missing generated configuration. Run 'configure apply'.",
             AppcliCommand.TASK_RUN: "Cannot run tasks due to missing generated configuration. Run 'configure apply'.",
             AppcliCommand.ORCHESTRATOR: "Cannot run orchestrator commands due to missing generated configuration. Run 'configure apply'.",
         }
         disallowed_command_unless_forced = {}
 
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
@@ -222,15 +218,14 @@
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class DirtyConfConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where config directory is dirty."""
 
     def __init__(self) -> None:
-
         disallowed_command = {
             AppcliCommand.CONFIGURE_INIT: "Cannot initialise an existing configuration.",
             AppcliCommand.MIGRATE: "Cannot migrate with a dirty configuration. Run 'configure apply'.",
         }
         disallowed_command_unless_forced = {
             AppcliCommand.SERVICE_START: "Cannot start with dirty configuration. Run 'configure apply'.",
             AppcliCommand.TASK_RUN: "Cannot run task with dirty configuration. Run 'configure apply'.",
@@ -240,15 +235,14 @@
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class DirtyGenConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where generated directory is dirty."""
 
     def __init__(self) -> None:
-
         disallowed_command = {
             AppcliCommand.CONFIGURE_INIT: "Cannot initialise an existing configuration.",
             AppcliCommand.MIGRATE: "Cannot migrate with a dirty generated configuration. Run 'configure apply'.",
         }
         disallowed_command_unless_forced = {
             AppcliCommand.CONFIGURE_APPLY: "Cannot 'configure apply' over a dirty generated directory as it will overwrite existing modifications.",
             AppcliCommand.SERVICE_START: "Cannot start service with dirty generated configuration. Run 'configure apply'.",
@@ -259,15 +253,14 @@
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class DirtyConfAndGenConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where both the conf and generated directory are dirty."""
 
     def __init__(self) -> None:
-
         disallowed_command = {
             AppcliCommand.CONFIGURE_INIT: "Cannot initialise an existing configuration.",
             AppcliCommand.MIGRATE: "Cannot migrate with a dirty generated configuration. Run 'configure apply'.",
         }
         disallowed_command_unless_forced = {
             AppcliCommand.CONFIGURE_APPLY: "Cannot 'configure apply' over a dirty generated directory as it will overwrite existing modifications.",
             AppcliCommand.SERVICE_START: "Cannot start service with dirty generated configuration. Run 'configure apply'.",
@@ -278,28 +271,26 @@
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class RequiresMigrationConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where configuration and application versions are misaligned."""
 
     def __init__(self, error: str) -> None:
-
         disallowed_command = get_disallowed_command_from_allowed_commands(
             [AppcliCommand.MIGRATE], error
         )
         disallowed_command_unless_forced = {}
 
         super().__init__(disallowed_command, disallowed_command_unless_forced)
 
 
 class InvalidConfigurationDirState(ConfigurationDirState):
     """Represents the configuration dir state where configuration is invalid and incompatible with appcli."""
 
     def __init__(self, error: str) -> None:
-
         default_error_message = f"Invalid configuration state, this error must be rectified before continuing. {error}"
 
         # Remove the 'VIEW_BACKUPS' and 'RESTORE' commands from the set of 'disallowed' commands so that we can add them
         # as 'disallowed unless forced' commands
         disallowed_command = get_disallowed_command_from_allowed_commands(
             [AppcliCommand.VIEW_BACKUPS, AppcliCommand.RESTORE], default_error_message
         )
```

### Comparing `bsl-appcli-1.3.6/appcli/configuration_manager.py` & `bsl-appcli-1.4.0/appcli/configuration_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # standard library
 import json
 import os
 import shutil
 import tarfile
 import tempfile
 from datetime import datetime, timezone
-from distutils.dir_util import copy_tree
 from pathlib import Path
 from typing import Iterable
 
 # vendor libraries
 from jinja2 import StrictUndefined, Template
 
 from appcli.crypto import crypto
@@ -54,14 +53,15 @@
 
     def __init__(self, cli_context: CliContext, configuration: Configuration):
         self.cli_context = cli_context
         self.config_repo: ConfigurationGitRepository = ConfigurationGitRepository(
             cli_context.configuration_dir
         )
         self.cli_configuration: Configuration = configuration
+        self.variables_manager: VariablesManager = cli_context.get_variables_manager()
 
     def initialise_configuration(self):
         """Initialises the configuration repository"""
 
         if not self.config_repo.is_repo_on_master_branch():
             error_and_exit(
                 "Cannot initialise configuration, repo is not on master branch."
@@ -124,19 +124,20 @@
         current_stack_settings_variables = (
             stack_config_file.read_text()
             if stack_settings_exists_pre_migration
             else None
         )
 
         # Migrate the current configuration variables
-        current_variables = self.__get_variables_manager().get_all_variables()
+        current_variables = self.variables_manager.get_all_variables()
 
         # Compare migrated config to the 'clean config' of the new version, and make sure all variables have been set and are the same type.
+        key_file = self.cli_context.get_key_file()
         clean_new_version_variables = VariablesManager(
-            self.cli_configuration.seed_app_configuration_file
+            self.cli_configuration.seed_app_configuration_file, key_file=key_file
         ).get_all_variables()
 
         migrated_variables = self.cli_configuration.hooks.migrate_variables(
             self.cli_context,
             current_variables,
             config_version,
             clean_new_version_variables,
@@ -178,49 +179,38 @@
         )
         if self.__directory_is_not_empty(configurable_templates_dir):
             logger.warning(
                 f"Configurable templates directory [{configurable_templates_dir}] is non-empty, please check for compatibility"
             )
 
         # Write out 'migrated' variables file
-        self.__get_variables_manager().set_all_variables(migrated_variables)
+        self.variables_manager.set_all_variables(migrated_variables)
 
         # If stack settings existed pre-migration, then replace the default with the existing settings
         if stack_settings_exists_pre_migration:
             logger.warning(
                 "Stack settings file was copied directly from previous version, please check for compatibility"
             )
             stack_config_file.write_text(current_stack_settings_variables)
 
         # Commit the new variables file
         self.config_repo.commit_changes(
             f"Migrated variables file from version [{config_version}] to version [{app_version}]"
         )
 
-    def get_variable(self, variable: str):
-        return self.__get_variables_manager().get_variable(variable)
+    def get_variable(self, variable: str, decrypt: bool = False):
+        return self.variables_manager.get_variable(variable, decrypt=decrypt)
 
     def set_variable(self, variable: str, value: any):
-        return self.__get_variables_manager().set_variable(variable, value)
-
-    def __get_variables_manager(self):
-        """Get the variables manager for the current configuration"""
-        return VariablesManager(self.cli_context.get_app_configuration_file())
+        return self.variables_manager.set_variable(variable, value)
 
     def get_stack_variable(self, variable: str):
-        return self.__get_stack_variables_manager().get_variable(variable)
-
-    def set_stack_variable(self, variable: str, value: any):
-        return self.__get_stack_variables_manager().set_variable(variable, value)
-
-    def __get_stack_variables_manager(self):
-        return VariablesManager(self.cli_context.get_stack_configuration_file())
+        return self.variables_manager.get_stack_variable(variable)
 
     def __create_new_configuration_branch_and_files(self):
-
         app_version: str = self.cli_context.app_version
         app_version_branch: str = self.config_repo.generate_branch_name(app_version)
 
         # Try to get an existing key
         path_to_key_file = self.cli_context.get_key_file()
         key_file_contents = None
         if path_to_key_file.exists():
@@ -358,14 +348,15 @@
     ):
         """Applies templates from a source directory to the generated directory
 
         Args:
             template_path (Path): directory to the templates
             generated_configuration_dir (Path): directory to output generated files
         """
+        template_data = self.variables_manager.get_templating_configuration()
         for template_file in template_path.glob("**/*"):
             relative_file = template_file.relative_to(template_path)
             target_file = generated_configuration_dir.joinpath(relative_file)
 
             if template_file.is_dir():
                 logger.debug("Creating directory [%s] ...", target_file)
                 target_file.mkdir(parents=True, exist_ok=True)
@@ -374,15 +365,15 @@
             if template_file.suffix == ".j2":
                 # parse jinja2 templates against configuration
                 target_file = target_file.with_suffix("")
                 logger.debug("Generating configuration file [%s] ...", target_file)
                 self.__generate_from_template(
                     template_file,
                     target_file,
-                    self.__get_variables_manager().get_all_variables(),
+                    template_data,
                 )
             else:
                 logger.debug("Copying configuration file to [%s] ...", target_file)
                 shutil.copy2(template_file, target_file)
 
     def __directory_is_not_empty(self, directory: Path) -> bool:
         """Checks if a directory is not empty.
@@ -410,15 +401,15 @@
             return None
 
         temp_dir = Path(tempfile.mkdtemp())
 
         # Due to a limitation with 'copytree', it fails to copy if the root directory exists
         # before copying. So we delete the temp dir prior to copying.
         os.rmdir(temp_dir)
-        copy_tree(str(directory_to_backup), str(temp_dir))
+        shutil.copytree(str(directory_to_backup), str(temp_dir), dirs_exist_ok=True)
 
         return temp_dir
 
     def __overwrite_directory(self, source_dir: Path, target_dir: Path):
         """Copies the contents of one directory to another, overwriting any existing contents.
         If the source directory doesn't exist, the target directory will not either.
 
@@ -436,15 +427,15 @@
 
         # If the source directory doesn't exist, or isn't a directory, then do not create the
         # target directory
         if source_dir is None or not source_dir.exists() or not source_dir.is_dir():
             return
 
         os.mkdir(target_dir)
-        copy_tree(str(source_dir), str(target_dir))
+        shutil.copytree(str(source_dir), str(target_dir), dirs_exist_ok=True)
 
     def __backup_and_create_new_generated_config_dir(
         self, current_config_version
     ) -> Path:
         """Backup the generated configuration dir, and delete all its contents
 
         Returns:
@@ -565,19 +556,23 @@
             # creation of the tar file to fail
             clean_additional_filename_descriptor = (
                 additional_filename_descriptor.replace("/", "-")
             )
             basename = os.path.basename(source_dir)
             output_filename = os.path.join(
                 os.path.dirname(source_dir),
+                Path(".generated-archive/"),
                 f"{basename}_{clean_additional_filename_descriptor}_{current_datetime}.tgz",
             )
 
             # Create the backup
             logger.debug(f"Backing up directory [{source_dir}] to [{output_filename}]")
+            output_dir = os.path.dirname(output_filename)
+            if not os.path.exists(output_dir):
+                os.makedirs(output_dir)
             with tarfile.open(output_filename, "w:gz") as tar:
                 tar.add(source_dir, arcname=os.path.basename(source_dir))
 
             # Ensure the backup has been successfully created before deleting the existing generated configuration directory
             if not os.path.exists(output_filename):
                 error_and_exit(
                     f"Current generated configuration directory backup failed. Could not write out file [{output_filename}]."
```

### Comparing `bsl-appcli-1.3.6/appcli/crypto/cipher.py` & `bsl-appcli-1.4.0/appcli/crypto/cipher.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.3.6/appcli/crypto/crypto.py` & `bsl-appcli-1.4.0/appcli/crypto/crypto.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,7 +55,25 @@
                 replaced_line = replaced_line.replace(
                     encrypted_string, decrypted_string
                 )
 
             replaced_lines.append(replaced_line)
 
     decrypted_file.write_text("".join(replaced_lines))
+
+
+def decrypt_value(encrypted_value: str, key_file: Path):
+    """Decrypts a given input value. If the value is unencrypted, will return
+    it verbatim.
+    """
+
+    if not isinstance(encrypted_value, str):
+        logger.debug(f"Did not decrypt non-string value [{encrypted_value}].")
+        return encrypted_value
+
+    regex = "^enc:[^:]+:[^:]+:end$"
+    if re.match(regex, encrypted_value) is None:
+        logger.debug(f"Did not decrypt unencrypted value [{encrypted_value}].")
+        return encrypted_value
+
+    cipher = Cipher(key_file)
+    return cipher.decrypt(encrypted_value)
```

### Comparing `bsl-appcli-1.3.6/appcli/functions.py` & `bsl-appcli-1.4.0/appcli/functions.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.3.6/appcli/git_repositories/git_repositories.py` & `bsl-appcli-1.4.0/appcli/git_repositories/git_repositories.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.3.6/appcli/keycloak_manager.py` & `bsl-appcli-1.4.0/appcli/keycloak_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,56 +194,56 @@
 
         kc = self.__get_keycloak_admin(realm_name)
         user_id = kc.get_user_id(username)
         all_realm_roles = kc.get_realm_roles()
         roles = [role for role in all_realm_roles if role["name"] == role_name]
         kc.assign_realm_roles(user_id, None, roles)
 
-    def configure_default(self, app_name):
+    def configure_default(self, app_name_slug):
         """Applies the default opinionated configuration to Keycloak
 
         This does the following:
-         - Creates a realm named '<app_name>'
-         - For realm '<app_name>', creates a client with the name '<app_name>', which has an audience mapper to itself,
+         - Creates a realm named '<app_name_slug>'
+         - For realm '<app_name_slug>', creates a client with the name '<app_name_slug>', which has an audience mapper to itself,
            and redirect URIs of ["*"]
-         - For realm '<app_name>', creates a realm role '<app_name>-admin'
-         - For realm '<app_name>', creates a user 'test.user' with password 'password', and assigns the realm role
-           '<app_name>-admin'
+         - For realm '<app_name_slug>', creates a realm role '<app_name_slug>-admin'
+         - For realm '<app_name_slug>', creates a user 'test.user' with password 'password', and assigns the realm role
+           '<app_name_slug>-admin'
 
         """
-        self.create_realm(app_name)
-        logger.debug(f"Created realm [{app_name}]")
+        self.create_realm(app_name_slug)
+        logger.debug(f"Created realm [{app_name_slug}]")
 
         client_payload = {
             "redirectUris": ["*"],
             "protocolMappers": [
                 {
-                    "name": f"{app_name}-audience",
+                    "name": f"{app_name_slug}-audience",
                     "protocol": "openid-connect",
                     "protocolMapper": "oidc-audience-mapper",
                     "consentRequired": "false",
                     "config": {
-                        "included.client.audience": app_name,
+                        "included.client.audience": app_name_slug,
                         "id.token.claim": "false",
                         "access.token.claim": "true",
                     },
                 }
             ],
         }
-        self.create_client(app_name, app_name, client_payload)
-        secret = self.get_client_secret(app_name, app_name)
-        logger.debug(f"Created client [{app_name}] with secret [{secret}]")
+        self.create_client(app_name_slug, app_name_slug, client_payload)
+        secret = self.get_client_secret(app_name_slug, app_name_slug)
+        logger.debug(f"Created client [{app_name_slug}] with secret [{secret}]")
 
-        realm_role = f"{app_name}-admin"
-        self.create_realm_role(app_name, realm_role)
+        realm_role = f"{app_name_slug}-admin"
+        self.create_realm_role(app_name_slug, realm_role)
         logger.debug(f"Created realm role [{realm_role}]")
 
         username = "test.user"
         self.create_user(
-            app_name, username, "password", "Test", "User", "test.user@email.test"
+            app_name_slug, username, "password", "Test", "User", "test.user@email.test"
         )
         logger.debug(
-            f"Created user [test.user] with password [password] in realm [{app_name}]"
+            f"Created user [test.user] with password [password] in realm [{app_name_slug}]"
         )
 
-        self.assign_realm_role(app_name, username, realm_role)
+        self.assign_realm_role(app_name_slug, username, realm_role)
         logger.debug(f"Assigned realm role [{realm_role}] to user [test.user]")
```

### Comparing `bsl-appcli-1.3.6/appcli/logger.py` & `bsl-appcli-1.4.0/appcli/logger.py`

 * *Files identical despite different names*

### Comparing `bsl-appcli-1.3.6/appcli/models/cli_context.py` & `bsl-appcli-1.4.0/appcli/models/cli_context.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # local libraries
 from appcli.configuration.configuration_dir_state import (
     ConfigurationDirState,
     ConfigurationDirStateFactory,
 )
 from appcli.logger import logger
+from appcli.variables_manager import VariablesManager
 
 
 class CliContext(NamedTuple):
     """Shared context from a run of the CLI."""
 
     # ---------------------------------
     # data passed in when CLI invoked on the command line
@@ -25,14 +26,17 @@
 
     data_dir: Path
     """ Directory to use for persistent data storage. """
 
     backup_dir: Path
     """ Directory to store backups in. """
 
+    application_context_files_dir: Path
+    """ Directory containing application context files. """
+
     additional_data_dirs: Iterable[Tuple[str, Path]]
     """ Additional directories to use for persistent data storage. """
 
     additional_env_variables: Iterable[Tuple[str, str]]
     """ Additional environment variables to define in CLI container. """
 
     environment: str
@@ -47,15 +51,15 @@
     debug: bool
     """ Whether to print debug logs. """
 
     # ---------------------------------
     # CLI build data
     # ---------------------------------
 
-    app_name: str
+    app_name_slug: str
     """ The application's name """
 
     app_version: str
     """ The application's version """
 
     commands: Dict
     """ Internal commands. """
@@ -150,8 +154,22 @@
 
     def get_project_name(self) -> str:
         """Get a unique name for the application and environment
 
         Returns:
             str: the project name
         """
-        return f"{self.app_name}_{self.environment}"
+        # NOTE: Must be lowercase, see https://github.com/brightsparklabs/appcli/issues/301
+        return f"{self.app_name_slug}_{self.environment}".lower()
+
+    def get_variables_manager(self) -> VariablesManager:
+        """Get the Variables Manager for the current cli context.
+
+        Returns:
+            VariablesManager: the variables manager for the current cli context.
+        """
+        return VariablesManager(
+            configuration_file=self.get_app_configuration_file(),
+            stack_configuration_file=self.get_stack_configuration_file(),
+            key_file=self.get_key_file(),
+            application_context_files_dir=self.application_context_files_dir,
+        )
```

### Comparing `bsl-appcli-1.3.6/appcli/models/configuration.py` & `bsl-appcli-1.4.0/appcli/models/configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
 # # -*- coding: utf-8 -*-
 
 # standard libraries
+import inspect
+import os
 import re
 from pathlib import Path
 from subprocess import CompletedProcess
 from typing import Callable, Dict, FrozenSet, Iterable, NamedTuple
 
 # vendor libraries
 import click
-from pydantic import BaseModel, validator
+from pydantic import BaseModel
 
 # local libraries
-from appcli.orchestrators import Orchestrator
+from appcli.orchestrators import DockerComposeOrchestrator, Orchestrator
 
 
 class Hooks(NamedTuple):
     """Hooks to run before/after stages"""
 
     migrate_variables: Callable[
         [click.Context, Dict, str, Dict], Dict
@@ -55,37 +57,68 @@
 
     app_name: str
     """ Name of the application (do not use spaces). """
 
     docker_image: str
     """ The docker image used to run the CLI. """
 
-    seed_app_configuration_file: Path
+    seed_app_configuration_file: Path = Path(
+        os.path.dirname(
+            inspect.stack()[-1].filename
+        ),  # Filename at the top of the call-stack.
+        "resources/settings.yml",
+    )
     """
     Path to a seed YAML file containing variables which are applied to the
     templates to generate the final configuration files.
     """
 
-    stack_configuration_file: Path
+    stack_configuration_file: Path = Path(
+        os.path.dirname(
+            inspect.stack()[-1].filename
+        ),  # Filename at the top of the call-stack.
+        "resources/stack-settings.yml",
+    )
     """
     Path to the stack configuration file which contains variables which are used to
     configure the stack.
     """
 
-    baseline_templates_dir: Path
+    baseline_templates_dir: Path = Path(
+        os.path.dirname(
+            inspect.stack()[-1].filename
+        ),  # Filename at the top of the call-stack.
+        "resources/templates/baseline",
+    )
     """
     Directory containing the baseline set of jinja2 templates used to generate the final
     configuration files. These template files are expected to remain static and should
     only be overridden as a hotfix.
     """
 
-    orchestrator: Orchestrator
+    orchestrator: Orchestrator = DockerComposeOrchestrator(
+        docker_compose_file=Path("docker-compose.yml"),
+        docker_compose_task_file=Path("docker-compose.tasks.yml"),
+    )
     """ Orchestrator to use to launch Docker containers. """
 
-    configurable_templates_dir: Path = None
+    application_context_files_dir: Path = None
+    """
+    Optional. Path to directory containing YAML files which are applied to
+    templates to generate the final configuration files. These application
+    context files can be templates themselves, which are rendered by the
+    main app configuration file.
+    """
+
+    configurable_templates_dir: Path = Path(
+        os.path.dirname(
+            inspect.stack()[-1].filename
+        ),  # Filename at the top of the call-stack.
+        "resources/templates/configurable",
+    )
     """
     Optional. Directory containing a default initial set of configurable jinja2 templates
     used to generate the final configuration files. These template files are expected to be
     modified as required on a per-deployment basis.
     """
 
     hooks: Hooks = Hooks()
@@ -110,27 +143,39 @@
     """
     Optional. Generated files which should be forcibly decrypted. It is
     generally bad practice to do this unless a post hook re-encrypts the
     generated files. Paths are relative and will be resolved against the
     generated configuration directory.
     """
 
-    @validator("app_name")
-    def app_name_must_be_shell_safe(cls, value):
-        # Use a validator to create a shell-safe version of the application name.
-        # This transforms the app_name variable by replacing any unsafe shell
-        # characters with '_', and returning the new string.
-        # Safe characters are: [a-z],[A-Z],[0-9] or '_'.
-        # First character cannot be [0-9].
-        # https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable
-        # https://linuxhint.com/bash-variable-name-rules-legal-illegal/
+    auto_configure_on_install: bool = True
+    """
+    Optional. Whether to run the corresponding install and configure
+    commands on the application. Equivalent to:
+        docker run --rm brightsparklabs/myapp:<version> install | sudo bash
+        /opt/brightsparklabs/myapp/production/myapp configure init
+        /opt/brightsparklabs/myapp/production/myapp configure apply
+    """
+
+    @property
+    def app_name_slug(self) -> str:
+        """
+        Returns a slug version of the application name which is shell safe.
+
+        This transforms the app_name variable by replacing any unsafe shell
+        characters with '_', and returning the new string.
+        Safe characters are: [a-z],[A-Z],[0-9] or '_'.
+        First character cannot be [0-9].
+        https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable
+        https://linuxhint.com/bash-variable-name-rules-legal-illegal/
+        """
         return "".join(
             [
-                re.sub(r"[^a-zA-Z_]", "_", value[0]),  # First character.
-                re.sub(r"[^a-zA-Z0-9_]", "_", value[1:]),
+                re.sub(r"[^a-zA-Z_]", "_", self.app_name[0]),  # First character.
+                re.sub(r"[^a-zA-Z0-9_]", "_", self.app_name[1:]),
             ]
         )
 
     class Config:
         # This is a requirement for pydantic to disable type checking for arbitrary user types for fields.
         # This is necessary as one or more of the fields are custom classes (e.g. Orchestrator)
         arbitrary_types_allowed = True
```

### Comparing `bsl-appcli-1.3.6/appcli/orchestrators.py` & `bsl-appcli-1.4.0/appcli/orchestrators.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # standard libraries
 from __future__ import annotations
 
 import os
 import subprocess
 import sys
+import textwrap
 from pathlib import Path
 from subprocess import CompletedProcess
 from tempfile import NamedTemporaryFile
 from typing import Iterable, List
 
 # vendor libraries
 import click
@@ -68,14 +69,29 @@
             service_names (tuple[str,...], optional): Names of the services to shutdown. If not provided, shuts down all services.
 
         Returns:
             CompletedProcess: Result of the orchestrator command.
         """
         raise NotImplementedError
 
+    def status(
+        self, cli_context: CliContext, service_name: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        """
+        Gets the status of Docker containers (services). Optionally accepts a tuple of service names to get the status of.
+
+        Args:
+            cli_context (CliContext): The current CLI context.
+            service_names (tuple[str,...], optional): Names of the services to get the status of. If not provided, gets the status of all services.
+
+        Returns:
+            CompletedProcess: Result of the orchestrator command.
+        """
+        raise NotImplementedError
+
     def task(
         self,
         cli_context: CliContext,
         service_name: str,
         extra_args: Iterable[str],
         detached: bool = False,
     ) -> CompletedProcess:
@@ -212,14 +228,22 @@
             # We cannot use the 'down' command as it removes more than just the specified service (by design).
             # https://github.com/docker/compose/issues/5420
             # `-fsv` flags mean forcibly stop the container before removing, and delete attached anonymous volumes
             command = ("rm", "-fsv") + service_names
             return self.__compose_service(cli_context, command)
         return self.__compose_service(cli_context, ("down",))
 
+    def status(
+        self, cli_context: CliContext, service_names: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        command = ("ps", "-a")
+        if service_names is not None and len(service_names) > 0:
+            command += service_names
+        return self.__compose_service(cli_context, command)
+
     def task(
         self,
         cli_context: CliContext,
         service_name: str,
         extra_args: Iterable[str],
         detached: bool = False,
     ) -> CompletedProcess:
@@ -419,14 +443,26 @@
                 "Docker Swarm orchestrator cannot stop individual services. Attempted to shutdown [%s].",
                 service_names,
             )
             return CompletedProcess(args=None, returncode=1)
 
         return self.__docker_stack(cli_context, ("rm",))
 
+    def status(
+        self, cli_context: CliContext, service_names: tuple[str, ...] = None
+    ) -> CompletedProcess:
+        if service_names is not None and len(service_names) > 0:
+            logger.error(
+                "Docker Swarm orchestrator cannot check the status of individual services. Attempted to get the status of [%s].",
+                service_names,
+            )
+            return CompletedProcess(args=None, returncode=1)
+
+        return self.__docker_stack(cli_context, ("ps",))
+
     def task(
         self,
         cli_context: CliContext,
         service_name: str,
         extra_args: Iterable[str],
         detached: bool = False,
     ) -> CompletedProcess:
@@ -441,15 +477,14 @@
     def exec(
         self,
         cli_context: CliContext,
         service_name: str,
         command: Iterable[str],
         stdin_input: str = None,
     ) -> CompletedProcess:
-
         # Running 'docker exec' on containers in a docker swarm is non-trivial
         # due to the distributed nature of docker swarm, and the fact there could
         # be replicas of a single service.
         raise NotImplementedError
 
     def verify_service_names(
         self, cli_context: CliContext, service_names: tuple[str, ...]
@@ -692,12 +727,33 @@
 
     if command is not None:
         docker_compose_command.extend(command)
 
     logger.debug(docker_compose_command)
     logger.debug("Running [%s]", " ".join(docker_compose_command))
     encoded_input = stdin_input.encode("utf-8") if stdin_input is not None else None
-    logger.debug(f"Encoded input: [{encoded_input}]")
+    logger.debug("Encoded input: [%s]", encoded_input)
     result = subprocess.run(
-        docker_compose_command, capture_output=True, input=encoded_input
+        docker_compose_command,
+        capture_output=True,
+        input=encoded_input,
     )
+    # For failures, error log both stdout/stderr if present.
+    if result.returncode != 0:
+        if result.stdout:
+            logger.error(
+                "Command failed - stdout:\n%s",
+                textwrap.indent(result.stdout.decode("utf-8"), "    "),
+            )
+        if result.stderr:
+            logger.error(
+                "Command failed - stderr:\n%s",
+                textwrap.indent(result.stdout.decode("utf-8"), "    "),
+            )
+    # For normal exits, just debug log the stdout if present.
+    elif result.stdout:
+        logger.debug(
+            "Command output:\n%s",
+            textwrap.indent(result.stdout.decode("utf-8"), "    "),
+        )
+
     return result
```

### Comparing `bsl-appcli-1.3.6/appcli/string_transformer.py` & `bsl-appcli-1.4.0/appcli/string_transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,24 +6,47 @@
 ________________________________________________________________________________
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
 # standard library
-from distutils.util import strtobool
 from typing import List
 
 # ------------------------------------------------------------------------------
+# FUNCTIONS
+# ------------------------------------------------------------------------------
+
+
+# NOTE: This is a copy of the `distutils.util.strtobool` function.
+# `distutils` is depricated and removed in python-3.12.
+# See https://docs.python.org/3/whatsnew/3.10.html#distutils-deprecated
+# And https://github.com/python/cpython/blob/3.10/Lib/distutils/util.py#L308
+# And https://stackoverflow.com/questions/42248342/yes-no-prompt-in-python3-using-strtobool
+def strtobool(val):
+    """Convert a string representation of truth to true (1) or false (0).
+    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+    'val' is anything else.
+    """
+    val = val.lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    elif val in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    else:
+        raise ValueError("invalid truth value %r" % (val,))
+
+
+# ------------------------------------------------------------------------------
 # CLASSES
 # ------------------------------------------------------------------------------
 
 
 class StringTransformer:
-
     # The 'type' string for string to string transformation (i.e. identity function)
     STRING_TRANSFORMER_TYPE = "str"
 
     # The supported transformation functions
     TRANSFORMATION_FUNCTIONS = {
         STRING_TRANSFORMER_TYPE: lambda s: (str(s)),
         "bool": lambda s: (bool(strtobool(s))),
```

### Comparing `bsl-appcli-1.3.6/appcli/templates/launcher.j2` & `bsl-appcli-1.4.0/appcli/templates/launcher.j2`

 * *Files 18% similar despite different names*

```diff
@@ -9,30 +9,32 @@
  # Generated at {{ current_datetime }}
  ##
 
 # ------------------------------------------------------------------------------
 # VARIABLES
 # ------------------------------------------------------------------------------
 
+{% set app_name_slug_upper = app_name_slug|upper %}
+
 # Variables are defaulted so that they can be overridden at runtime if desired
-MOUNTED_CONFIG_DIR="{{ '${' }}{{ app_name }}_CONFIG_DIR:-{{ cli_context.configuration_dir }}{{ '}' }}"
-MOUNTED_GENERATED_CONFIG_DIR="{{ '${' }}{{ app_name }}_GENERATED_CONFIG_DIR:-{{ cli_context.get_generated_configuration_dir() }}{{ '}' }}"
-MOUNTED_DATA_DIR="{{ '${' }}{{ app_name }}_DATA_DIR:-{{ cli_context.data_dir }}{{ '}' }}"
-MOUNTED_BACKUP_DIR="{{ '${' }}{{ app_name }}_BACKUP_DIR:-{{ cli_context.backup_dir }}{{ '}' }}"
-ENVIRONMENT="{{ '${' }}{{ app_name }}_ENVIRONMENT:-{{ cli_context.environment }}{{ '}' }}"
+MOUNTED_CONFIG_DIR="{{ '${' }}{{ app_name_slug_upper }}_CONFIG_DIR:-{{ cli_context.configuration_dir }}{{ '}' }}"
+MOUNTED_GENERATED_CONFIG_DIR="{{ '${' }}{{ app_name_slug_upper }}_GENERATED_CONFIG_DIR:-{{ cli_context.get_generated_configuration_dir() }}{{ '}' }}"
+MOUNTED_DATA_DIR="{{ '${' }}{{ app_name_slug_upper }}_DATA_DIR:-{{ cli_context.data_dir }}{{ '}' }}"
+MOUNTED_BACKUP_DIR="{{ '${' }}{{ app_name_slug_upper }}_BACKUP_DIR:-{{ cli_context.backup_dir }}{{ '}' }}"
+ENVIRONMENT="{{ '${' }}{{ app_name_slug_upper }}_ENVIRONMENT:-{{ cli_context.environment }}{{ '}' }}"
 
 # ------------------------------------------------------------------------------
 # LOGIC
 # ------------------------------------------------------------------------------
 
 function main()
 {
 
     docker run \
-        --name {{ app_name }}_{{ cli_context.environment }}_launcher_$(date +%s) \
+        --name {{ app_name_slug }}_{{ cli_context.environment }}_launcher_$(date +%s) \
         --rm \
         $( [[ "${NO_INTERACTIVE}" != "true" ]] && echo "--interactive") \
         $( [[ "${NO_TTY}" != "true" ]] && echo "--tty") \
 {% if cli_context.docker_credentials_file %}
         --volume "{{ cli_context.docker_credentials_file }}:/root/.docker/config.json" \
 {% endif %}
 {% for name, value in cli_context.additional_env_variables %}
@@ -40,23 +42,23 @@
 {% endfor %}
 {% for name, path in cli_context.additional_data_dirs %}
         --env {{ name }}="{{ path }}" \
         --volume "{{ path }}:{{ path }}" \
 {% endfor %}
         --volume /var/run/docker.sock:/var/run/docker.sock \
         --env APP_NAME="{{ app_name }}" \
-        --env {{ app_name }}_CONFIG_DIR="${MOUNTED_CONFIG_DIR}" \
+        --env {{ app_name_slug_upper }}_CONFIG_DIR="${MOUNTED_CONFIG_DIR}" \
         --volume "${MOUNTED_CONFIG_DIR}:${MOUNTED_CONFIG_DIR}" \
-        --env {{ app_name }}_GENERATED_CONFIG_DIR="${MOUNTED_GENERATED_CONFIG_DIR}" \
+        --env {{ app_name_slug_upper }}_GENERATED_CONFIG_DIR="${MOUNTED_GENERATED_CONFIG_DIR}" \
         --volume "${MOUNTED_GENERATED_CONFIG_DIR}:${MOUNTED_GENERATED_CONFIG_DIR}" \
-        --env {{ app_name }}_DATA_DIR="${MOUNTED_DATA_DIR}" \
+        --env {{ app_name_slug_upper }}_DATA_DIR="${MOUNTED_DATA_DIR}" \
         --volume "${MOUNTED_DATA_DIR}:${MOUNTED_DATA_DIR}" \
-        --env {{ app_name }}_BACKUP_DIR="${MOUNTED_BACKUP_DIR}" \
+        --env {{ app_name_slug_upper }}_BACKUP_DIR="${MOUNTED_BACKUP_DIR}" \
         --volume "${MOUNTED_BACKUP_DIR}:${MOUNTED_BACKUP_DIR}" \
-        --env {{ app_name }}_ENVIRONMENT="${ENVIRONMENT}" \
+        --env {{ app_name_slug_upper }}_ENVIRONMENT="${ENVIRONMENT}" \
         --network host \
         {{ configuration.docker_image }}:{{ app_version }} \
             --configuration-dir "${MOUNTED_CONFIG_DIR}" \
             --data-dir "${MOUNTED_DATA_DIR}" \
             --backup-dir "${MOUNTED_BACKUP_DIR}" \
             --environment "${ENVIRONMENT}" \
 {% for name, path in cli_context.additional_data_dirs %}
```

### Comparing `bsl-appcli-1.3.6/bsl_appcli.egg-info/PKG-INFO` & `bsl-appcli-1.4.0/bsl_appcli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,732 +1,862 @@
 Metadata-Version: 2.1
 Name: bsl-appcli
-Version: 1.3.6
+Version: 1.4.0
 Summary: A library for adding CLI interfaces to applications in the brightSPARK Labs style
 Home-page: https://www.brightsparklabs.com
 Author: brightSPARK Labs
 Author-email: enquire@brightsparklabs.com
 License: MIT License
-Description: # BSL Application CLI Library
-        
-        ![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
-        
-        A library for adding CLI interfaces to applications in the brightSPARK Labs style.
-        
-        ## Overview
-        
-        This library can be leveraged to add a standardised CLI capability to applications to:
-        
-        - Handle system lifecycle events for services (`service [start|shutdown]`).
-        - Allow running arbitrary short-lived tasks (`task run`).
-        - Manage configuration (`configure`).
-        - Upgrade to a newer version of the application (`upgrade|migrate`).
-        - And more.
-        
-        The CLI is designed to run within a Docker container and launch other Docker containers (i.e.
-        Docker-in-Docker). This is generally managed via a `docker-compose.yml` file.
-        
-        The library exposes the following environment variables to the `docker-compose.yml` file:
-        
-        - `APP_VERSION` - the version of containers to launch.
-        - `<APP_NAME>_CONFIG_DIR` - the directory containing configuration files.
-        - `<APP_NAME>_DATA_DIR` - the directory containing data produced/consumed by the system.
-        - `<APP_NAME>_GENERATED_CONFIG_DIR` - the directory containing configuration files generated from
-          the templates in `<APP_NAME>_CONFIG_DIR`.
-        - `<APP_NAME>_ENVIRONMENT` - the deployment environment the system is running in. For example
-          `production` or `staging`. This allows multiple instances of the application to run on the same
-          Docker daemon. Defaults to `production`.
-        
-        Note: the `APP_NAME` variable is derived from the `app_name` passed in to the `Configuration` object in the
-        main python entrypoint to the application. In order for the application to work, the `app_name` is forced to conform
-        with the shell variable name standard: `[a-zA-Z_][a-zA-Z_0-9]*`. Any characters that do not fit this regex will be
-        replaced with `_`. See:
-        (https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable)
-        (https://linuxhint.com/bash-variable-name-rules-legal-illegal/)
-        
-        The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
-        variables within the `settings.yml` file as described in the Installation section.
-        
-        Stack variables can be set within the `stack-settings.yml` file as described in the
-        `Build configuration template directories` section.
-        
-        ## Installation
-        
-        ### Add the library to your python CLI application
-        
-            pip install git+https://github.com/brightsparklabs/appcli.git@<VERSION>
-        
-        ### Define the CLI for your application `myapp`
-        
-        _Note for appcli version 1.1.3 and below_: Import paths to access to appcli
-        internal classes and methods is now by a full path, rather than being exposed
-        at the root. This was done to allow access to all methods and classes using
-        python3 implicit namespaced packages.
-        
-            # filename: myapp.py
-        
-            #!/usr/bin/env python3
-            # # -*- coding: utf-8 -*-
-        
-            # standard libraries
-            import os
-            import sys
-            from pathlib import Path
-        
-            # vendor libraries
-            from appcli.cli_builder import create_cli
-            from appcli.models.configuration import Configuration
-            from appcli.orchestrators import DockerComposeOrchestrator
-        
-            # ------------------------------------------------------------------------------
-            # CONSTANTS
-            # ------------------------------------------------------------------------------
-        
-            # directory containing this script
-            BASE_DIR = os.path.dirname(os.path.realpath(__file__))
-        
-            # ------------------------------------------------------------------------------
-            # PRIVATE METHODS
-            # ------------------------------------------------------------------------------
-        
-            def main():
-                configuration = Configuration(
-                    app_name='myapp',
-                    docker_image='brightsparklabs/myapp',
-                    seed_app_configuration_file=Path(BASE_DIR, 'resources/settings.yml'),
-                    stack_configuration_file=Path(BASE_DIR, 'resources/stack-settings.yml'),
-                    baseline_templates_dir=Path(BASE_DIR, 'resources/templates/baseline'),
-                    configurable_templates_dir=Path(BASE_DIR, 'resources/templates/configurable'),
-                    orchestrator=DockerComposeOrchestrator(
-                        docker_compose_file = Path('docker-compose.yml'),
-                        docker_compose_override_directory = Path('docker-compose.override.d/'),
-                        docker_compose_task_file = Path('docker-compose.tasks.yml'),
-                        docker_compose_task_override_directory = Path(
-                            'docker-compose.tasks.override.d/'
-                        ),
-                    ),
-                    mandatory_additional_data_dirs=['EXTRA_DATA',],
-                    mandatory_additional_env_variables=['ENV_VAR_2',],
-                )
-                cli = create_cli(configuration)
-                cli()
-        
-            # ------------------------------------------------------------------------------
-            # ENTRYPOINT
-            # ------------------------------------------------------------------------------
-        
-            if __name__ == '__main__':
-                main()
-        
-        #### Custom Commands
-        
-        You can specify some custom top-level commands by adding click commands or command groups to the configuration object.
-        Assuming 'web' is the name of the service in the docker-compose.yml file which you wish to exec against, we can create
-        three custom commands in the following example:
-        
-        - `myapp ls-root` which lists the contents of the root directory within the `web` service container and prints it out.
-        - `myapp ls-root-to-file` which lists the contents of the root directory within the `web` service container and dumps to file within the container.
-        - `myapp tee-file` which takes some text and `tee`s it into another file the `web` service container.
-        
-        ```python
-        
-        def get_ls_root_command(orchestrator: DockerComposeOrchestrator):
-            @click.command(
-                help="List files in the root directory",
-            )
-            @click.pass_context
-            def ls_root(ctx: click.Context):
-        
-                # Equivalent command within the container:
-                # `ls -alh`
-                cli_context: CliContext = ctx.obj
-                output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
-                print(output.stdout.decode())
-        
-            return ls_root
-        
-        def get_tee_file_command(orchestrator: DockerComposeOrchestrator):
-            @click.command(
-                help="Tee some text into a file",
-            )
-            @click.pass_context
-            def tee_file(ctx: click.Context):
-        
-                # Equivalent command within the container:
-                # `echo "Some data to tee into the custom file" | tee /ls-root.txt`
-                cli_context: CliContext = ctx.obj
-                output: CompletedProcess = orchestrator.exec(cli_context, "web", ["tee", "/my_custom_file.txt"], stdin_input="Some data to tee into the custom file")
-        
-            return tee_file
-        
-        def get_ls_root_to_file_command(orchestrator: DockerComposeOrchestrator):
-            @click.command(
-                help="List files in the root directory and tee to file",
-            )
-            @click.pass_context
-            def ls_root_to_file(ctx: click.Context):
-        
-                # Equivalent command within the container:
-                # `ls -alh | tee /ls-root.txt`
-                cli_context: CliContext = ctx.obj
-                output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
-                data = output.stdout.decode()
-                orchestrator.exec(cli_context, "web", ["tee", "/ls-root.txt"], stdin_input=data)
-        
-            return ls_root_to_file
-        
-        def main():
-            orchestrator = DockerComposeOrchestrator(Path("docker-compose.yml"))
-            configuration = Configuration(
-                app_name="appcli_nginx",
-                docker_image="thomas-anderson-bsl/appcli-nginx",
-                seed_app_configuration_file=Path(BASE_DIR, "resources/settings.yml"),
-                stack_configuration_file=Path(BASE_DIR, "resources/stack-settings.yml"),
-                baseline_templates_dir=Path(BASE_DIR, "resources/templates/baseline"),
-                configurable_templates_dir=Path(BASE_DIR, "resources/templates/configurable"),
-                orchestrator=orchestrator,
-                custom_commands={get_tee_file_command(orchestrator),get_ls_root_command(orchestrator),get_ls_root_to_file_command(orchestrator)}
-            )
-            cli = create_cli(configuration)
-            cli()
-        
-        ```
-        
-        ### Build configuration template directories
-        
-        - Store any Jinja2 variable definitions you wish to use in your configuration
-          template files in `resources/settings.yml`.
-        - Store any appcli stack specific keys in `resources/stack-settings.yml`.
-        - Store your `docker-compose.yml`/`docker-compose.yml.j2` file in `resources/templates/baseline/`.
-        - Configuration files (Jinja2 compatible templates or otherwise) can be stored in one
-          of two locations:
-          - `resources/templates/baseline` - for templates which the end user **is not** expected to modify.
-          - `resources/templates/configurable` - for templates which the end user is expected to modify.
-        
-        ### Configure application backup
-        
-        Appcli's `backup` command creates backups of configuration and data of an application, stored locally in the
-        backup directory. The settings for backups are configured through entries in a `backups` block in `stack-settings.yml`.
-        
-        The available keys for entries in the `backups` block are:
-        
-        | key            | Description                                                                                                       |
-        | -------------- | ----------------------------------------------------------------------------------------------------------------- |
-        | name           | The name of the backup. Must be unique between backup definitions and use `kebab-case`.                           |
-        | backup_limit   | The number of local backups to keep. Set to `0` to disable rolling deletion.                                      |
-        | file_filter    | The file_filter contains lists of glob patterns used to specify what files to include or exclude from the backup. |
-        | frequency      | The cron-like frequency at which backups will execute.                                                            |
-        | remote_backups | The list of remote backup strategies.                                                                             |
-        
-            # filename: stack-settings.yml
-        
-            backups:
-              - name: "full"
-                backup_limit: 0
-                file_filter:
-                  data_dir:
-                    include_list:
-                    exclude_list:
-                  conf_dir:
-                    include_list:
-                    exclude_list:
-                frequency: "* * *"
-                remote_backups:
-        
-        #### Backup name
-        
-        The backup `name` is a short descriptive name for the backup definition.
-        To avoid problems, we _highly_ recommend `name` be:
-        
-        - unique between items in the `backups` list
-        - use `kebab-case`
-        
-        Examples of good names:
-        
-        - `full`
-        - `conf-only`
-        - `audit-logs`
-        
-        Without a unique `name`, backups from different items in `backups` will
-        overwrite each other without warning.
-        
-        Using `kebab-case` is necessary to avoid some issues with `click` and filesystem
-        naming issues.
-        
-        When using the `backup` command, you are able to supply the name
-        of the backup to run. If you have a backup `name` with a space in it, the `click`
-        library cannot interpret the name as a whole string (even with quotes), so you
-        will be unable to run the backup individually.
-        
-        If the backup `name` doesn't use `kebab-case`, it may use some characters that
-        are incompatible with file and directory naming conventions. Appcli will
-        automatically slugify the name to something compatible, but this may cause
-        collisions in the folder names of backups to be taken which will lead to backups
-        being overwritten. e.g. `s3#1` and `s3&1` will both translate internally to
-        `s3-1`.
-        
-        #### Backup limit
-        
-        A rolling deletion strategy is used to remove local backups, in order to keep `backup_limit` number of backups.
-        
-        If more than `backup_limit` number of backups exist in the backup directory, the oldest backups will be deleted.
-        
-        Set this value to `0` to keep all backups.
-        
-        #### File filter
-        
-        The `file_filter` block enables filtering of files to backup from `conf` and `data` directories. For more details
-        including examples, see [here](/README_BACKUP_FILE_FILTER.md).
-        
-            # filename: stack-settings.yml
-            # Includes all log files from data dir only
-        
-            backups:
-              - name: "full"
-                backup_limit: 0
-                file_filter:
-                  data_dir:
-                    include_list:
-                      - "**/*.log"
-                    exclude_list:
-                    conf_dir:
-                      include_list:
-                      exclude_list:
-                        - "**/*"
-                frequency: "* * *"
-                remote_backups:
-        
-        #### Freqency
-        
-        Appcli supports limiting individual backups to run on only specific days using a cron-like frequency filter.
-        
-        When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
-        today's date. Only strategies whose `frequency` pattern match today's date will execute.
-        
-        The input pattern `pattern` is prefixed with `"* * "` and is used as a standard cron expression to
-        check for a match. i.e. `"* * $pattern"`.
-        
-        Examples:
-        
-        - `"* * *"` (cron equivalent `"* * * * *"`) will always run.
-        - `"* * 0"` (cron equivalent `"* * * * 0"`) will only run on Sunday.
-        - `"1 */3 *"` (cron equivalent `"* * 1 */3 *"`) will only run on the first day-of-month of every 3rd month.
-        
-        #### Remote backup
-        
-        Appcli supports pushing local backups to remote storage. The list of strategies for pushing to remote storage are
-        defined within the `remote_backups` block.
-        
-        The available keys for every remote backup strategy are:
-        
-        | key           | Description                                                                                                 |
-        | ------------- | ----------------------------------------------------------------------------------------------------------- |
-        | name          | A short name or description used to describe this backup.                                                   |
-        | strategy_type | The type of this backup, must match an implemented remote backup strategy.                                  |
-        | frequency     | The cron-like frequency at which remote backups will execute. Behaves the same as local backup `frequency`. |
-        | configuration | Custom configuration block that is specific to each remote backup strategy.                                 |
-        
-        N.B. remote backups will only run for a local backup that has run. Therefore the `frequency` of the local backup
-        will apply first, followed by the `frequency` of the remote backup. This means that it's possible to write a remote
-        backup frequency that will never execute. e.g. Local `* * 0` and remote `* * 1`.
-        
-        ##### Strategies
-        
-        ###### AWS S3 remote strategy
-        
-        To use S3 remote backup, set `strategy_type` to `S3`.
-        The available configuration keys for an S3 backup are:
-        
-        | key         | Description                                                                                                                 |
-        | ----------- | --------------------------------------------------------------------------------------------------------------------------- |
-        | bucket_name | The name of the bucket to upload to.                                                                                        |
-        | access_key  | The AWS Access key ID for the account to upload with.                                                                       |
-        | secret_key  | The AWS Secret access key for the account to upload with. The value _must_ be encrypted using the appcli `encrypt` command. |
-        | bucket_path | The path in the S3 bucket to upload to. Set this to an empty string to upload to the root of the bucket.                    |
-        | tags        | Key value pairs of tags to set on the backup object.                                                                        |
-        
-            # filename: stack-settings.yml
-        
-            backups:
-              - name: "full_backup"
-                backup_limit: 0
-                remote_backups:
-                - name: "weekly_S3"
-                  strategy_type: "S3"
-                  frequency: "* * 0"
-                  configuration:
-                    bucket_name: "aws.s3.bucket"
-                    access_key: "aws_access_key"
-                    secret_key: "enc:id=1:encrypted_text:end"
-                    bucket_path: "bucket/path"
-                    tags:
-                      frequency: "weekly"
-                      type: "data"
-        
-        ### Restoring a remote backup
-        
-        To restore from a remote backup:
-        
-        1. Acquire the remote backup (`.tgz` file) that you wish to restore. For S3 this can be done by downloading the backup from the specified bucket.
-        2. Place the backup `myapp_date.tgz` file in the backup directory. By default this will be `/opt/brightsparklabs/${APP_NAME}/production/backup/`
-        3. Confirm that appcli can access the backup by running the `view-backups` command
-        4. Run the restore command `./myapp restore BACKUP_FILE.tgz` e.g. `./myapp restore APP_2021-02-02T10:55:48+00:00.tgz`. The restore process will trigger a backup.
-        
-        ### Define a container for your CLI application
-        
-            # filename: Dockerfile
-        
-            FROM brightsparklabs/appcli
-        
-            ENTRYPOINT ["./myapp.py"]
-            WORKDIR /app
-        
-            # install compose if using it as the orchestrator
-            RUN pip install docker-compose
-        
-            COPY requirements.txt .
-            RUN pip install --requirement requirements.txt
-            COPY src .
-        
-            ARG APP_VERSION=latest
-            ENV APP_VERSION=${APP_VERSION}
-        
-        ### Build the container
-        
-            # sh
-            docker build -t brightsparklabs/myapp --build-arg APP_VERSION=latest .
-        
-        ### (Optional) Login to private Docker registries and pass through credentials
-        
-        It is possible to login to private Docker registries on the host, and pass through credentials to
-        the CLI container run by the launcher script. This enables pulling and running Docker images from
-        private Docker registries.
-        
-        Login using:
-        
-            docker login ${REGISTRY_URL}
-        
-        The credentials file path can be passed as an option via `--docker-credentials-file` or `-p` to the
-        `myapp` container.
-        
-        ### View the installer script
-        
-            # sh
-            docker run --rm brightsparklabs/myapp:<version> install
-        
-            # or if using a private registry for images
-            docker run --rm brightsparklabs/myapp:<version> --docker-credentials-file ~/.docker/config.json install
-        
-        While it is not mandatory to view the script before running, it is highly recommended.
-        
-        ### Run the installer script
-        
-            # sh
-            docker run --rm brightsparklabs/myapp:<version> install | sudo bash
-        
-        The above will use the following defaults:
-        
-        - `environment` => `production`.
-        - `install-dir` => `/opt/brightsparklabs/${APP_NAME}/production/`.
-        - `configuration-dir` => `/opt/brightsparklabs/${APP_NAME}/production/conf/`.
-        - `data-dir` => `/opt/brightsparklabs/${APP_NAME}/production/data/`.
-        - `backup-dir` => `/opt/brightsparklabs/${APP_NAME}/production/backup/`.
-        
-        You can modify any of the above if desired. E.g.
-        
-            # sh
-            docker run --rm brightsparklabs/myapp:<version> \
-                --environment "uat" \
-                --configuration-dir /etc/myapp \
-                --data-dir /mnt/data/myapp \
-                install --install-dir ${HOME}/apps/myapp \
-            | sudo bash
-        
-        Where:
-        
-        - `--environment` defines the environment name for the deployment. This allows multiple instances of
-          the application to be present on the same host.
-          Defaults to `production`.
-        - `--install-dir` defines the base path for launcher and the default locations for the configuration
-          and data directories if they are not overrideen (see below).
-          Defaults to `/opt/brightsparklabs/${APP_NAME}/${ENVIRONMENT}/` (where `${ENVIRONMENT}` is defined
-          by `--environment` above).
-        - `--configuration-dir` defines the path to the configuration directory.
-          Defaults to `${INSTALL_DIR}/conf/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
-        - `--data-dir` defines the path to the data directory.
-          Defaults to `${INSTALL_DIR}/data/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
-        
-        The installation script will generate a launcher script for controlling the application. The script
-        location will be printed out when running the install script. This script should now be used as the
-        main entrypoint to all appcli functions for managing your application.
-        
-        ## Usage
-        
-        This section details what commands and options are available.
-        
-        ### Top-level Commands
-        
-        To be used in conjunction with your application `./myapp <command>` e.g. `./myapp configure init`
-        
-        | Command      | Description                                                       |
-        | ------------ | ----------------------------------------------------------------- |
-        | backup       | Create a backup of application data and configuration.            |
-        | configure    | Configures the application.                                       |
-        | encrypt      | Encrypts the specified string.                                    |
-        | init         | Initialises the application.                                      |
-        | launcher     | Outputs an appropriate launcher bash script.                      |
-        | migrate      | Migrates the configuration of the application to a newer version. |
-        | orchestrator | Perform docker orchestration                                      |
-        | restore      | Restore a backup of application data and configuration.           |
-        | service      | Lifecycle management commands for application services.           |
-        | task         | Commands for application tasks.                                   |
-        | version      | Fetches the version of the app being managed with appcli.         |
-        | view-backups | View a list of locally-available backups.                         |
-        
-        ### Options
-        
-        | Option                             | Description                                                                                                         |
-        | ---------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
-        | --debug                            | Enables debug level logging.                                                                                        |
-        | -c, --configuration-dir PATH       | Directory containing configuration files. [This is required unless subcommand is one of: `install`.                 |
-        | -d, --data-dir PATH                | Directory containing data produced/consumed by the system. This is required unless subcommand is one of: `install`. |
-        | -t, --environment TEXT             | Deployment environment the system is running in. Defaults to `production`.                                          |
-        | -p, --docker-credentials-file PATH | Path to the Docker credentials file (config.json) on the host for connecting to private Docker registries.          |
-        | -a, --additional-data-dir TEXT     | Additional data directory to expose to launcher container. Can be specified multiple times.                         |
-        | -e, --additional-env-var TEXT      | Additional environment variables to expose to launcher container. Can be specified multiple times.                  |
-        | --help                             | Show the help message and exit.                                                                                     |
-        
-        #### Command: `backup`
-        
-        Creates a backup `.tgz` file in the backup directory that contains files from the configuration and data directory, as
-        configured in `stack-settings.yml`. After the backup is taken, remote backup strategies will be executed (if applicable).
-        
-        usage: `./myapp backup [OPTIONS] [ARGS]`
-        
-        | Option                                         | Description                                        |
-        | ---------------------------------------------- | -------------------------------------------------- |
-        | --pre-stop-services/--no-pre-stop-services     | Whether to stop services before performing backup. |
-        | --post-start-services/--no-post-start-services | Whether to start services after performing backup. |
-        | --help                                         | Show the help message and exit.                    |
-        
-        The `backup` command optionally takes an argument corresponding to the `name` of the backup to run. If no `name` is
-        provided, all backups will attempt to run.
-        #### Command Group: `configure`
-        
-        Configures the application.
-        
-        usage: `./myapp configure [OPTIONS] COMMAND [ARGS]`
-        
-        | Command  | Description                                                                                                               |
-        | -------- | ------------------------------------------------------------------------------------------------------------------------- |
-        | apply    | Applies the settings from the configuration.                                                                              |
-        | diff     | Get the differences between current and default configuration settings.                                                   |
-        | get      | Reads a setting from the configuration.                                                                                   |
-        | init     | Initialises the configuration directory.                                                                                  |
-        | set      | Saves a setting to the configuration. Allows setting the type of value with option `--type`, and defaults to string type. |
-        | template | Configures the baseline templates.                                                                                        |
-        | edit     | Open the settings file for editing with vim-tiny.                                                                         |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `encrypt`
-        
-        Encrypts the specified string.
-        
-        usage: `./myapp encrypt [OPTIONS] TEXT`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `init`
-        
-        Initialises the application.
-        
-        usage: `./myapp init [OPTIONS] COMMAND [ARGS]`
-        
-        | Command  | Description                                                              |
-        | -------- | ------------------------------------------------------------------------ |
-        | keycloak | Initialises a Keycloak instance with BSL-specific initial configuration. |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `launcher`
-        
-        Outputs an appropriate launcher bash script to stdout.
-        
-        usage: `./myapp launcher [OPTIONS]`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `migrate`
-        
-        Migrates the application configuration to work with the current application version.
-        
-        usage: `./myapp migrate [OPTIONS]`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `orchestrator`
-        
-        Perform tasks defined by the orchestrator.
-        
-        usage: `./myapp orchestrator [OPTIONS] COMMAND [ARGS]`
-        
-        All commands are defined within the orchestrators themselves. Run `./myapp orchestrator` to list available commands.
-        
-        | Option | Description                    |
-        | ------ | ------------------------------ |
-        | --help | Show the help message and exit |
-        
-        #### Command: `restore`
-        
-        Restores a specified backup `.tgz` file from the configured backup folder.
-        
-        usage: `./myapp restore BACKUP_FILE`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `service`
-        
-        Runs application services. These are the long-running services which should only exit on command.
-        
-        usage: `./myapp service [OPTIONS] COMMAND [ARGS]`
-        
-        | Command  | Description                                                                                                                                                                                                             |
-        | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | logs     | Prints logs from all services.                                                                                                                                                                                          |
-        | shutdown | Shuts down the system. If one or more service names are provided, shuts down the specified service(s) only.                                                                                                             |
-        | start    | Starts the system. If one or more service names are provided, starts the specified service(s) only.                                                                                                                     |
-        | restart  | Restarts service(s) (`shutdown` followed by `start`). Optionally run a `configure apply` during the restart with the `--apply` flag. If one or more service names are provided, restarts the specified service(s) only. |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command Group: `task`
-        
-        Runs application tasks. These are short-lived services which should exit when the task is complete.
-        
-        usage: `./myapp task [OPTIONS] COMMAND [ARGS]`
-        
-        | Command | Description                                                                                  |
-        | ------- | -------------------------------------------------------------------------------------------- |
-        | run     | Runs a specified application task. Optionally run in the background with `-d/--detach` flag. |
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        #### Command: `version`
-        
-        Fetches the version of the app being managed with appcli.
-        
-        usage: `./myapp version`
-        
-        #### Command: `view-backups`
-        
-        View a list of all backups in the configured backup folder.
-        
-        usage: `./myapp view-backups`
-        
-        | Option | Description                     |
-        | ------ | ------------------------------- |
-        | --help | Show the help message and exit. |
-        
-        ### Usage within scripts and cron
-        
-        By default, the generated `appcli` launcher script will run the CLI container with a virtual terminal session (tty).
-        This may interfere with crontab entries or scripts that use the appcli launcher.
-        
-        To disable tty when running the launcher script, set `NO_TTY` environment variable to `true`.
-        
-            NO_TTY=true ./myapp [...]
-        
-        or
-        
-            export NO_TTY=true
-            ./myapp [...]
-        
-        If required, you can also disable interactive mode with the `NO_INTERACTIVE` environment variable.
-        
-            NO_INTERACTIVE=true ./myapp [...]
-        
-        or
-        
-            export NO_INTERACTIVE=true
-            ./myapp [...]
-        
-        ## Development
-        
-        This section details how to build/test/run/debug the system in a development environment.
-        
-        ### Prerequisites
-        
-        The following must be installed and in the `PATH`:
-        
-        - make
-        - python 3.7+
-        - virtualenv
-        - git
-        
-        ### Build
-        
-            make all
-        
-        ### Install
-        
-            pip install -e .
-        
-        ### Running unit tests
-        
-            make test
-        
-        ## Usage while developing your CLI application
-        
-        While developing, it may be preferable to run your python script directly rather than having to
-        rebuild a container each time you update it.
-        
-        - Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
-        - Set the environment variables which the CLI usually sets for you:
-        
-                export MYAPP_CONFIG_DIR=/tmp/myapp/config \
-                       MYAPP_DATA_DIR=/tmp/myapp/data
-        
-        - Run your CLI application:
-        
-                ./myapp \
-                  --debug \
-                  --configuration-dir "${MYAPP_CONFIG_DIR}" \
-                  --data-dir "${MYAPP_DATA_DIR}"
-        
-        ## Contributing
-        
-        When committing code, call `make all` to automatically run code formatting/ linting/testing.
-        
-        Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
-        settings. This ensures that PR diffs are minimal and focussed on the code change rather than
-        stylistic coding decisions.
-        
-        Install with `pip install black`. This can be run through VSCode or via the CLI. See the `black`
-        documentation for details.
-        
-        ## Licenses
-        
-        Refer to the `LICENSE` file for details.
-        
-        This project makes use of several libraries and frameworks. Refer to the `LICENSES` folder for
-        details.
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# BSL Application CLI Library
+
+![Test Python](https://github.com/brightsparklabs/appcli/actions/workflows/build_python.yml/badge.svg)
+
+A library for adding CLI interfaces to applications in the brightSPARK Labs style.
+
+## Overview
+
+This library can be leveraged to add a standardised CLI capability to applications to:
+
+- Handle system lifecycle events for services (`service [start|shutdown]`).
+- Allow running arbitrary short-lived tasks (`task run`).
+- Manage configuration (`configure`).
+- Upgrade to a newer version of the application (`upgrade|migrate`).
+- And more.
+
+The CLI is designed to run within a Docker container and launch other Docker containers (i.e.
+Docker-in-Docker). This is generally managed via a `docker-compose.yml` file.
+
+The library exposes the following environment variables to the `docker-compose.yml` file:
+
+- `APP_VERSION` - the version of containers to launch.
+- `<APP_NAME>_CONFIG_DIR` - the directory containing configuration files.
+- `<APP_NAME>_DATA_DIR` - the directory containing data produced/consumed by the system.
+- `<APP_NAME>_GENERATED_CONFIG_DIR` - the directory containing configuration files generated from
+  the templates in `<APP_NAME>_CONFIG_DIR`.
+- `<APP_NAME>_BACKUP_DIR` - the directory to use for system backups.
+- `<APP_NAME>_ENVIRONMENT` - the deployment environment the system is running in. For example
+  `production` or `staging`. This allows multiple instances of the application to run on the same
+  Docker daemon. Defaults to `production`.
+
+NOTE:
+The `APP_NAME` variable is derived from the `app_name` passed in to the `Configuration` object in
+the main python entrypoint to the application. In order for the application to work, the `app_name`
+is forced to conform with the shell variable name standard: `[a-zA-Z_][a-zA-Z_0-9]*`. Any characters
+that do not fit this regex will be replaced with `_`. See
+[here](https://unix.stackexchange.com/questions/428880/list-of-acceptable-initial-characters-for-a-bash-variable)
+or [here](https://linuxhint.com/bash-variable-name-rules-legal-illegal/) for details.
+
+The `docker-compose.yml` can be templated by renaming to `docker-compose.yml.j2`, and setting
+variables within the `settings.yml` file as described in the Installation section.
+
+Stack variables can be set within the `stack-settings.yml` file as described in the
+`Build configuration template directories` section.
+
+## Quick Start
+
+Refer to the [quick start guide](quickstart.md) to get a basic application running.
+
+Otherwise refer to the Installation section below to see all options.
+
+## Installation
+
+### Add the library to your python CLI application
+
+    pip install git+https://github.com/brightsparklabs/appcli.git@<VERSION>
+
+### Define the CLI for your application `myapp`
+
+_Note for appcli version 1.1.3 and below_: Import paths to access to appcli
+internal classes and methods is now by a full path, rather than being exposed
+at the root. This was done to allow access to all methods and classes using
+python3 implicit namespaced packages.
+
+```python
+    # filename: myapp.py
+
+    #!/usr/bin/env python3
+    # # -*- coding: utf-8 -*-
+
+    # standard libraries
+    from pathlib import Path
+
+    # vendor libraries
+    from appcli.cli_builder import create_cli
+    from appcli.models.configuration import Configuration
+    from appcli.orchestrators import DockerComposeOrchestrator
+
+    # ------------------------------------------------------------------------------
+    # CONSTANTS
+    # ------------------------------------------------------------------------------
+
+    # directory containing this script
+    BASE_DIR = Path(__file__).parent
+
+    # ------------------------------------------------------------------------------
+    # PRIVATE METHODS
+    # ------------------------------------------------------------------------------
+
+    def main():
+        configuration = Configuration(
+            app_name='myapp',
+            docker_image='brightsparklabs/myapp',
+            seed_app_configuration_file=BASE_DIR / 'resources/settings.yml',
+            application_context_files_dir=BASE_DIR / 'resources/templates/appcli/context',
+            stack_configuration_file=BASE_DIR / 'resources/stack-settings.yml',
+            baseline_templates_dir=BASE_DIR / 'resources/templates/baseline',
+            configurable_templates_dir=BASE_DIR / 'resources/templates/configurable',
+            orchestrator=DockerComposeOrchestrator(
+                # NOTE: These paths are relative to 'resources/templates/baseline'.
+                docker_compose_file = Path('docker-compose.yml'),
+                docker_compose_override_directory = Path('docker-compose.override.d/'),
+                docker_compose_task_file = Path('docker-compose.tasks.yml'),
+                docker_compose_task_override_directory = Path( 'docker-compose.tasks.override.d/'),
+            ),
+            mandatory_additional_data_dirs=['EXTRA_DATA',],
+            mandatory_additional_env_variables=['ENV_VAR_2',],
+        )
+        cli = create_cli(configuration)
+        cli()
+
+    # ------------------------------------------------------------------------------
+    # ENTRYPOINT
+    # ------------------------------------------------------------------------------
+
+    if __name__ == '__main__':
+        main()
+```
+
+A lot of the fields in the appcli constructor can be defaulted, resulting in less code.
+
+```python
+configuration = Configuration(
+    app_name='myapp',
+    docker_image='brightsparklabs/myapp',
+)
+cli = create_cli(configuration)
+cli()
+```
+
+#### Custom Commands
+
+You can specify some custom top-level commands by adding click commands or command groups to the
+configuration object.  Assuming 'web' is the name of the service in the docker-compose.yml file
+which you wish to exec against, we can create three custom commands in the following example:
+
+- `myapp ls-root` which lists the contents of the root directory within the `web` service container
+  and prints it out.
+- `myapp ls-root-to-file` which lists the contents of the root directory within the `web` service
+  container and dumps to file within the container.
+- `myapp tee-file` which takes some text and `tee`s it into another file the `web` service
+  container.
+
+```python
+
+def get_ls_root_command(orchestrator: DockerComposeOrchestrator):
+    @click.command(
+        help="List files in the root directory",
+    )
+    @click.pass_context
+    def ls_root(ctx: click.Context):
+
+        # Equivalent command within the container:
+        # `ls -alh`
+        cli_context: CliContext = ctx.obj
+        output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
+        print(output.stdout.decode())
+
+    return ls_root
+
+def get_tee_file_command(orchestrator: DockerComposeOrchestrator):
+    @click.command(
+        help="Tee some text into a file",
+    )
+    @click.pass_context
+    def tee_file(ctx: click.Context):
+
+        # Equivalent command within the container:
+        # `echo "Some data to tee into the custom file" | tee /ls-root.txt`
+        cli_context: CliContext = ctx.obj
+        output: CompletedProcess = orchestrator.exec(cli_context, "web", ["tee", "/my_custom_file.txt"], stdin_input="Some data to tee into the custom file")
+
+    return tee_file
+
+def get_ls_root_to_file_command(orchestrator: DockerComposeOrchestrator):
+    @click.command(
+        help="List files in the root directory and tee to file",
+    )
+    @click.pass_context
+    def ls_root_to_file(ctx: click.Context):
+
+        # Equivalent command within the container:
+        # `ls -alh | tee /ls-root.txt`
+        cli_context: CliContext = ctx.obj
+        output: CompletedProcess = orchestrator.exec(cli_context, "web", ["ls", "-alh", "/"])
+        data = output.stdout.decode()
+        orchestrator.exec(cli_context, "web", ["tee", "/ls-root.txt"], stdin_input=data)
+
+    return ls_root_to_file
+
+def main():
+    orchestrator = DockerComposeOrchestrator(Path("docker-compose.yml"))
+    configuration = Configuration(
+        app_name="appcli_nginx",
+        docker_image="thomas-anderson-bsl/appcli-nginx",
+        seed_app_configuration_file=Path(BASE_DIR, "resources/settings.yml"),
+        stack_configuration_file=Path(BASE_DIR, "resources/stack-settings.yml"),
+        baseline_templates_dir=Path(BASE_DIR, "resources/templates/baseline"),
+        configurable_templates_dir=Path(BASE_DIR, "resources/templates/configurable"),
+        orchestrator=orchestrator,
+        custom_commands={get_tee_file_command(orchestrator),get_ls_root_command(orchestrator),get_ls_root_to_file_command(orchestrator)}
+    )
+    cli = create_cli(configuration)
+    cli()
+
+```
+
+### Build configuration template directories
+
+- Store any Jinja2 variable definitions you wish to use in your configuration
+  template files in `resources/settings.yml`.
+- Store any application context files in `resources/templates/appcli/context/`
+- Store any appcli stack specific keys in `resources/stack-settings.yml`.
+- Store your `docker-compose.yml`/`docker-compose.yml.j2` file in `resources/templates/baseline/`.
+- Configuration files (Jinja2 compatible templates or otherwise) can be stored in one
+  of two locations:
+  - `resources/templates/baseline` - for templates which the end user **is not** expected to modify.
+  - `resources/templates/configurable` - for templates which the end user is expected to modify.
+
+#### Application context files
+
+Template files are templated with Jinja2. The 'data' passed into the templating engine
+is a combination of the `settings.yml` and all application context files
+(stored in `resources/templates/appcli/context`, and referenced in the `Configuration`
+object as `application_context_files_dir`). Application context files that have the
+extension `.j2` are templated using the settings from `settings.yml`.
+
+These are combined to make the data for templating as follows:
+
+```json
+{
+  "settings": {
+    ... all settings from `settings.yml`
+  },
+  "application": {
+    <app_context_file_1>: {
+      ... settings from `app_context_file_1.yml`, optionally jinja2 templated using settings from `settings.yml`
+    },
+    ... additional app_context_files
+  }
+}
+```
+
+As a minimal example with the following YAML files:
+
+```yaml
+# ./settings.yml
+main_settings:
+  abc: 123
+
+# ./resources/templates/appcli/context/app_constants.yml
+other_settings:
+  hello: world
+
+# ./resources/templates/appcli/context/app_variables.yml.j2
+variables:
+  main_abc_setting: {{ settings.main_settings.abc }}
+```
+
+The data for Jinja2 templating engine will be:
+
+```json
+{
+  "settings": {
+    "main_settings": {
+      "abc": 123
+    }
+  },
+  "application": {
+    "app_constants": {
+      "other_settings": {
+        "hello": "world"
+      }
+    },
+    "app_variables": {
+      "variables": {
+        "main_abc_setting": 123
+      }
+    }
+  }
+}
+```
+
+### Configure application backup
+
+Appcli's `backup` command creates backups of configuration and data of an application, stored
+locally in the backup directory. The settings for backups are configured through entries in a
+`backups` block in `stack-settings.yml`.
+
+The available keys for entries in the `backups` block are:
+
+| key            | Description                                                                                                       |
+| -------------- | ----------------------------------------------------------------------------------------------------------------- |
+| name           | The name of the backup. Must be unique between backup definitions and use `kebab-case`.                           |
+| backup_limit   | The number of local backups to keep. Set to `0` to disable rolling deletion.                                      |
+| file_filter    | The file_filter contains lists of glob patterns used to specify what files to include or exclude from the backup. |
+| frequency      | The cron-like frequency at which backups will execute.                                                            |
+| remote_backups | The list of remote backup strategies.                                                                             |
+
+    # filename: stack-settings.yml
+
+    backups:
+      - name: "full"
+        backup_limit: 0
+        file_filter:
+          data_dir:
+            include_list:
+            exclude_list:
+          conf_dir:
+            include_list:
+            exclude_list:
+        frequency: "* * *"
+        remote_backups:
+
+#### Backup name
+
+The backup `name` is a short descriptive name for the backup definition.
+To avoid problems, we _highly_ recommend `name` be:
+
+- unique between items in the `backups` list
+- use `kebab-case`
+
+Examples of good names:
+
+- `full`
+- `conf-only`
+- `audit-logs`
+
+Without a unique `name`, backups from different items in `backups` will
+overwrite each other without warning.
+
+Using `kebab-case` is necessary to avoid some issues with `click` and filesystem
+naming issues.
+
+When using the `backup` command, you are able to supply the name
+of the backup to run. If you have a backup `name` with a space in it, the `click`
+library cannot interpret the name as a whole string (even with quotes), so you
+will be unable to run the backup individually.
+
+If the backup `name` doesn't use `kebab-case`, it may use some characters that
+are incompatible with file and directory naming conventions. Appcli will
+automatically slugify the name to something compatible, but this may cause
+collisions in the folder names of backups to be taken which will lead to backups
+being overwritten. e.g. `s3#1` and `s3&1` will both translate internally to
+`s3-1`.
+
+#### Backup limit
+
+A rolling deletion strategy is used to remove local backups, in order to keep `backup_limit` number
+of backups.
+
+If more than `backup_limit` number of backups exist in the backup directory, the oldest backups will
+be deleted.
+
+Set this value to `0` to keep all backups.
+
+#### File filter
+
+The `file_filter` block enables filtering of files to backup from `conf` and `data` directories. For
+more details including examples, see [here](/README_BACKUP_FILE_FILTER.md).
+
+    # filename: stack-settings.yml
+    # Includes all log files from data dir only
+
+    backups:
+      - name: "full"
+        backup_limit: 0
+        file_filter:
+          data_dir:
+            include_list:
+              - "**/*.log"
+            exclude_list:
+            conf_dir:
+              include_list:
+              exclude_list:
+                - "**/*"
+        frequency: "* * *"
+        remote_backups:
+
+#### Freqency
+
+Appcli supports limiting individual backups to run on only specific days using a cron-like frequency
+filter.
+
+When the `backup` command is run, each backup strategy will check if the `frequency` pattern matches
+today's date. Only strategies whose `frequency` pattern match today's date will execute.
+
+The input pattern `pattern` is prefixed with `"* * "` and is used as a standard cron expression to
+check for a match. i.e. `"* * $pattern"`.
+
+Examples:
+
+- `"* * *"` (cron equivalent `"* * * * *"`) will always run.
+- `"* * 0"` (cron equivalent `"* * * * 0"`) will only run on Sunday.
+- `"1 */3 *"` (cron equivalent `"* * 1 */3 *"`) will only run on the first day-of-month of every 3rd
+  month.
+
+#### Remote backup
+
+Appcli supports pushing local backups to remote storage. The list of strategies for pushing to
+remote storage are defined within the `remote_backups` block.
+
+The available keys for every remote backup strategy are:
+
+| key           | Description                                                                                                 |
+| ------------- | ----------------------------------------------------------------------------------------------------------- |
+| name          | A short name or description used to describe this backup.                                                   |
+| strategy_type | The type of this backup, must match an implemented remote backup strategy.                                  |
+| frequency     | The cron-like frequency at which remote backups will execute. Behaves the same as local backup `frequency`. |
+| configuration | Custom configuration block that is specific to each remote backup strategy.                                 |
+
+N.B. remote backups will only run for a local backup that has run. Therefore the `frequency` of the
+local backup will apply first, followed by the `frequency` of the remote backup. This means that
+it's possible to write a remote backup frequency that will never execute. e.g. Local `* * 0` and
+remote `* * 1`.
+
+##### Strategies
+
+###### AWS S3 remote strategy
+
+To use S3 remote backup, set `strategy_type` to `S3`.
+The available configuration keys for an S3 backup are:
+
+| key         | Description                                                                                                                 |
+| ----------- | --------------------------------------------------------------------------------------------------------------------------- |
+| bucket_name | The name of the bucket to upload to.                                                                                        |
+| access_key  | The AWS Access key ID for the account to upload with.                                                                       |
+| secret_key  | The AWS Secret access key for the account to upload with. The value _must_ be encrypted using the appcli `encrypt` command. |
+| bucket_path | The path in the S3 bucket to upload to. Set this to an empty string to upload to the root of the bucket.                    |
+| tags        | Key value pairs of tags to set on the backup object.                                                                        |
+
+    # filename: stack-settings.yml
+
+    backups:
+      - name: "full_backup"
+        backup_limit: 0
+        remote_backups:
+        - name: "weekly_S3"
+          strategy_type: "S3"
+          frequency: "* * 0"
+          configuration:
+            bucket_name: "aws.s3.bucket"
+            access_key: "aws_access_key"
+            secret_key: "enc:id=1:encrypted_text:end"
+            bucket_path: "bucket/path"
+            tags:
+              frequency: "weekly"
+              type: "data"
+
+### Restoring a remote backup
+
+To restore from a remote backup:
+
+1. Acquire the remote backup (`.tgz` file) that you wish to restore. For S3 this can be done by
+   downloading the backup from the specified bucket.
+2. Place the backup `myapp_date.tgz` file in the backup directory. By default this will be
+   `/opt/brightsparklabs/${APP_NAME}/production/backup/`
+3. Confirm that appcli can access the backup by running the `view-backups` command
+4. Run the restore command `./myapp restore BACKUP_FILE.tgz` e.g.
+   `./myapp restore APP_2021-02-02T10:55:48+00:00.tgz`. The restore process will trigger a backup.
+
+### Define a container for your CLI application
+
+    # filename: Dockerfile
+
+    FROM brightsparklabs/appcli
+
+    ENTRYPOINT ["./myapp.py"]
+    WORKDIR /app
+
+    # install compose if using it as the orchestrator
+    RUN pip install docker-compose
+
+    COPY requirements.txt .
+    RUN pip install --requirement requirements.txt
+    COPY src .
+
+    ARG APP_VERSION=latest
+    ENV APP_VERSION=${APP_VERSION}
+
+### Build the container
+
+    # sh
+    docker build -t brightsparklabs/myapp --build-arg APP_VERSION=latest .
+
+### (Optional) Login to private Docker registries and pass through credentials
+
+It is possible to login to private Docker registries on the host, and pass through credentials to
+the CLI container run by the launcher script. This enables pulling and running Docker images from
+private Docker registries.
+
+Login using:
+
+    docker login ${REGISTRY_URL}
+
+The credentials file path can be passed as an option via `--docker-credentials-file` or `-p` to the
+`myapp` container.
+
+### View the installer script
+
+    # sh
+    docker run --rm brightsparklabs/myapp:<version> install
+
+    # or if using a private registry for images
+    docker run --rm brightsparklabs/myapp:<version> \
+      --docker-credentials-file ~/.docker/config.json \
+      install
+
+While it is not mandatory to view the script before running, it is highly recommended.
+
+### Run the installer script
+
+    # sh
+    docker run --rm brightsparklabs/myapp:<version> install | sudo bash
+
+The above will use the following defaults:
+
+- `environment` => `production`.
+- `install-dir` => `/opt/brightsparklabs/${APP_NAME}/production/`.
+- `configuration-dir` => `/opt/brightsparklabs/${APP_NAME}/production/conf/`.
+- `data-dir` => `/opt/brightsparklabs/${APP_NAME}/production/data/`.
+- `backup-dir` => `/opt/brightsparklabs/${APP_NAME}/production/backup/`.
+
+You can modify any of the above if desired. E.g.
+
+    # sh
+    docker run --rm brightsparklabs/myapp:<version> \
+        --environment "uat" \
+        --configuration-dir /etc/myapp \
+        --data-dir /mnt/data/myapp \
+        install --install-dir ${HOME}/apps/myapp \
+    | sudo bash
+
+Where:
+
+- `--environment` defines the environment name for the deployment. This allows multiple instances of
+  the application to be present on the same host.
+  Defaults to `production`.
+- `--install-dir` defines the base path for launcher and the default locations for the configuration
+  and data directories if they are not overrideen (see below).
+  Defaults to `/opt/brightsparklabs/${APP_NAME}/${ENVIRONMENT}/` (where `${ENVIRONMENT}` is defined
+  by `--environment` above).
+- `--configuration-dir` defines the path to the configuration directory.
+  Defaults to `${INSTALL_DIR}/conf/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
+- `--data-dir` defines the path to the data directory.
+  Defaults to `${INSTALL_DIR}/data/` (`${INSTALL_DIR}` is defined by `--install-dir` above).
+
+The installation script will generate a launcher script for controlling the application. The script
+location will be printed out when running the install script. This script should now be used as the
+main entrypoint to all appcli functions for managing your application.
+
+## Migration from appcli version <=1.3.6 to version >1.3.6
+
+As a result of supporting application context files, all references to
+settings in template files have moved.
+
+All settings in `settings.yml` used in templating are now namespaced under
+`settings`. All templates will need to change their references to use this new
+namespacing scheme. For example, in templates that refer to settings, change the
+references like so:
+
+- `my_app.server.hostname` -> `settings.my_app.server.hostname`
+- `my_app.server.http.port` -> `settings.my_app.server.http.port`
+
+## Usage
+
+This section details what commands and options are available.
+
+### Top-level Commands
+
+To be used in conjunction with your application `./myapp <command>` e.g. `./myapp configure init`
+
+| Command      | Description                                                       |
+| ------------ | ----------------------------------------------------------------- |
+| backup       | Create a backup of application data and configuration.            |
+| configure    | Configures the application.                                       |
+| encrypt      | Encrypts the specified string.                                    |
+| init         | Initialises the application.                                      |
+| launcher     | Outputs an appropriate launcher bash script.                      |
+| migrate      | Migrates the configuration of the application to a newer version. |
+| orchestrator | Perform docker orchestration                                      |
+| restore      | Restore a backup of application data and configuration.           |
+| service      | Lifecycle management commands for application services.           |
+| task         | Commands for application tasks.                                   |
+| version      | Fetches the version of the app being managed with appcli.         |
+| view-backups | View a list of locally-available backups.                         |
+
+### Options
+
+| Option                             | Description                                                                                                         |
+| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
+| --debug                            | Enables debug level logging.                                                                                        |
+| -c, --configuration-dir PATH       | Directory containing configuration files. [This is required unless subcommand is one of: `install`.                 |
+| -d, --data-dir PATH                | Directory containing data produced/consumed by the system. This is required unless subcommand is one of: `install`. |
+| -t, --environment TEXT             | Deployment environment the system is running in. Defaults to `production`.                                          |
+| -p, --docker-credentials-file PATH | Path to the Docker credentials file (config.json) on the host for connecting to private Docker registries.          |
+| -a, --additional-data-dir TEXT     | Additional data directory to expose to launcher container. Can be specified multiple times.                         |
+| -e, --additional-env-var TEXT      | Additional environment variables to expose to launcher container. Can be specified multiple times.                  |
+| --help                             | Show the help message and exit.                                                                                     |
+
+#### Command: `backup`
+
+Creates a backup `.tgz` file in the backup directory that contains files from the configuration and
+data directory, as configured in `stack-settings.yml`. After the backup is taken, remote backup
+strategies will be executed (if applicable).
+
+usage: `./myapp backup [OPTIONS] [ARGS]`
+
+| Option                                         | Description                                        |
+| ---------------------------------------------- | -------------------------------------------------- |
+| --pre-stop-services/--no-pre-stop-services     | Whether to stop services before performing backup. |
+| --post-start-services/--no-post-start-services | Whether to start services after performing backup. |
+| --help                                         | Show the help message and exit.                    |
+
+The `backup` command optionally takes an argument corresponding to the `name` of the backup to run.
+If no `name` is provided, all backups will attempt to run.
+
+#### Command Group: `configure`
+
+Configures the application.
+
+usage: `./myapp configure [OPTIONS] COMMAND [ARGS]`
+
+| Command    | Description                                                                                                               |
+| ---------- | ------------------------------------------------------------------------------------------------------------------------- |
+| apply      | Applies the settings from the configuration.                                                                              |
+| diff       | Get the differences between current and default configuration settings.                                                   |
+| get        | Reads a setting from the configuration.                                                                                   |
+| get-secure | Reads a setting from the configuration, decrypting if it is encrypted. This will prompt for the setting key.              |
+| init       | Initialises the configuration directory.                                                                                  |
+| set        | Saves a setting to the configuration. Allows setting the type of value with option `--type`, and defaults to string type. |
+| template   | Configures the baseline templates.                                                                                        |
+| edit       | Open the settings file for editing with vim-tiny.                                                                         |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `encrypt`
+
+Encrypts the specified string.
+
+usage: `./myapp encrypt [OPTIONS] TEXT`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `init`
+
+Initialises the application.
+
+usage: `./myapp init [OPTIONS] COMMAND [ARGS]`
+
+| Command  | Description                                                              |
+| -------- | ------------------------------------------------------------------------ |
+| keycloak | Initialises a Keycloak instance with BSL-specific initial configuration. |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `launcher`
+
+Outputs an appropriate launcher bash script to stdout.
+
+usage: `./myapp launcher [OPTIONS]`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `migrate`
+
+Migrates the application configuration to work with the current application version.
+
+usage: `./myapp migrate [OPTIONS]`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `orchestrator`
+
+Perform tasks defined by the orchestrator.
+
+usage: `./myapp orchestrator [OPTIONS] COMMAND [ARGS]`
+
+All commands are defined within the orchestrators themselves. Run `./myapp orchestrator` to list
+available commands.
+
+For example, the following commands are available to docker-compose:
+
+| Command | Description                                                                                                        |
+| ------- | ------------------------------------------------------------------------------------------------------------------ |
+| ps      | List containers for the appcli project, with current status and exposed ports.                                     |
+| compose | Run a docker compose command. See [docker compose](https://docs.docker.com/engine/reference/commandline/compose/). |
+
+| Option | Description                    |
+| ------ | ------------------------------ |
+| --help | Show the help message and exit |
+
+#### Command: `restore`
+
+Restores a specified backup `.tgz` file from the configured backup folder.
+
+usage: `./myapp restore BACKUP_FILE`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `service`
+
+Runs application services. These are the long-running services which should only exit on command.
+
+usage: `./myapp service [OPTIONS] COMMAND [ARGS]`
+
+| Command  | Description                                                                                                                                                                                                             |
+| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| logs     | Prints logs from all services.                                                                                                                                                                                          |
+| shutdown | Shuts down the system. If one or more service names are provided, shuts down the specified service(s) only.                                                                                                             |
+| start    | Starts the system. If one or more service names are provided, starts the specified service(s) only.                                                                                                                     |
+| restart  | Restarts service(s) (`shutdown` followed by `start`). Optionally run a `configure apply` during the restart with the `--apply` flag. If one or more service names are provided, restarts the specified service(s) only. |
+| status   | Lists all containers for the appcli project, with current status and exposed ports. If one or more service names are provided, lists the status and 
+ exposed ports of the specified service(s) only. |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command Group: `task`
+
+Runs application tasks. These are short-lived services which should exit when the task is complete.
+
+usage: `./myapp task [OPTIONS] COMMAND [ARGS]`
+
+| Command | Description                                                                                  |
+| ------- | -------------------------------------------------------------------------------------------- |
+| run     | Runs a specified application task. Optionally run in the background with `-d/--detach` flag. |
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+#### Command: `version`
+
+Fetches the version of the app being managed with appcli.
+
+usage: `./myapp version`
+
+#### Command: `view-backups`
+
+View a list of all backups in the configured backup folder.
+
+usage: `./myapp view-backups`
+
+| Option | Description                     |
+| ------ | ------------------------------- |
+| --help | Show the help message and exit. |
+
+### Usage within scripts and cron
+
+By default, the generated `appcli` launcher script will run the CLI container with a virtual
+terminal session (tty).  This may interfere with crontab entries or scripts that use the appcli
+launcher.
+
+To disable tty when running the launcher script, set `NO_TTY` environment variable to `true`.
+
+    NO_TTY=true ./myapp [...]
+
+or
+
+    export NO_TTY=true
+    ./myapp [...]
+
+If required, you can also disable interactive mode with the `NO_INTERACTIVE` environment variable.
+
+    NO_INTERACTIVE=true ./myapp [...]
+
+or
+
+    export NO_INTERACTIVE=true
+    ./myapp [...]
+
+## Development
+
+This section details how to build/test/run/debug the system in a development environment.
+
+### Prerequisites
+
+The following must be installed and in the `PATH`:
+
+- make
+- python 3.7+
+- virtualenv
+- git
+
+### Build
+
+    make all
+
+### Install
+
+    pip install -e .
+
+### Running unit tests
+
+    make test
+
+## Usage while developing your CLI application
+
+While developing, it may be preferable to run your python script directly rather than having to
+rebuild a container each time you update it.
+
+- Ensure docker is installed (more specifically a docker socket at `/var/run/docker.sock`).
+- Set the environment variables which the CLI usually sets for you:
+
+        export \
+            MYAPP_DATA_DIR=/tmp/myapp/data \
+            MYAPP_CONFIG_DIR=/tmp/myapp/config \
+            MYAPP_GENERATED_CONFIG_DIR=/tmp/myapp/config/.generated \
+            MYAPP_BACKUP_DIR=/tmp/myapp/backup \
+            MYAPP_ENVIRONMENT=dev
+- Run your CLI application:
+
+        ./src/myapp.py \
+              --debug \
+              --configuration-dir "${MYAPP_CONFIG_DIR}" \
+              --data-dir "${MYAPP_DATA_DIR}" \
+              --backup-dir "${MYAPP_BACKUP_DIR}" \
+              --environment "${MYAPP_ENVIRONMENT}
+
+## Contributing
+
+When committing code, call `make all` to automatically run code formatting/ linting/testing.
+
+Appcli uses the python code formatter [black](https://pypi.org/project/black/) with default
+settings. This ensures that PR diffs are minimal and focussed on the code change rather than
+stylistic coding decisions.
+
+Install with `pip install black`. This can be run through VSCode or via the CLI. See the `black`
+documentation for details.
+
+## Licenses
+
+Refer to the `LICENSE` file for details.
+
+This project makes use of several libraries and frameworks. Refer to the `LICENSES` folder for
+details.
```

### Comparing `bsl-appcli-1.3.6/setup.py` & `bsl-appcli-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 Python Package File
 ________________________________________________________________________________
 
 Created by brightSPARK Labs
 www.brightsparklabs.com
 """
 
+import re
+
 # to use a consistent encoding
 from codecs import open
 from os import path
 from subprocess import PIPE, run
 
 # always prefer setuptools over distutils
 from setuptools import find_namespace_packages, setup
@@ -22,15 +24,17 @@
 # ------------------------------------------------------------------------------
 
 
 def get_version():
     try:
         process = run(["git", "describe", "--dirty", "--always"], stdout=PIPE)
         line = process.stdout.strip().decode("utf-8")
-        return line
+        # Needs to be PEP 440 compliant.
+        compliant_version = re.sub("-.*", "", line)
+        return compliant_version
     except Exception:
         return "UNKNOWN"
 
 
 # ------------------------------------------------------------------------------
 # SETUP DEFINITION
 # ------------------------------------------------------------------------------
@@ -49,25 +53,26 @@
     license="MIT License",
     author="brightSPARK Labs",
     author_email="enquire@brightsparklabs.com",
     url="https://www.brightsparklabs.com",
     packages=find_namespace_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
-        "boto3==1.20.40",
-        "click==8.0.3",
+        "boto3==1.26.104",
+        "click==8.1.3",
         "coloredlogs==15.0.1",
         "cronex==0.1.3.1",
-        "dataclasses-json==0.5.6",
-        "deepdiff==5.7.0",
-        "GitPython==3.1.26",
-        "jinja2==3.0.3",
-        "pycryptodome==3.12.0",
-        "pydantic==1.9.0",
+        "dataclasses-json==0.5.7",
+        "deepdiff==6.3.0",
+        "GitPython==3.1.31",
+        "jinja2==3.1.2",
+        "pre-commit==3.2.1",
+        "pycryptodome==3.17",
+        "pydantic==1.10.7",
         "python-keycloak==0.22.0",
-        "python-slugify==5.0.2",
-        "ruamel-yaml==0.17.20",
-        "tabulate==0.8.9",
-        "wheel==0.37.1",
+        "python-slugify==8.0.1",
+        "ruamel-yaml==0.17.21",
+        "tabulate==0.9.0",
+        "wheel==0.40.0",
     ],
     extras_require={"dev": ["black", "flake8", "isort", "pytest"]},
 )
```


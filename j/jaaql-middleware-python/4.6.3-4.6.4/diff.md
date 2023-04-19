# Comparing `tmp/jaaql-middleware-python-4.6.3.tar.gz` & `tmp/jaaql-middleware-python-4.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.6.3.tar", last modified: Mon Apr 17 22:20:49 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.6.4.tar", last modified: Wed Apr 19 14:05:16 2023, max compression
```

## Comparing `jaaql-middleware-python-4.6.3.tar` & `jaaql-middleware-python-4.6.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.633696 jaaql-middleware-python-4.6.3/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-04-17 22:20:49.633696 jaaql-middleware-python-4.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.569696 jaaql-middleware-python-4.6.3/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.573695 jaaql-middleware-python-4.6.3/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4835 2023-04-17 22:14:35.000000 jaaql-middleware-python-4.6.3/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.577696 jaaql-middleware-python-4.6.3/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.3/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/db/db_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.581695 jaaql-middleware-python-4.6.3/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6320 2023-04-06 12:25:17.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.586696 jaaql-middleware-python-4.6.3/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.3/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.590696 jaaql-middleware-python-4.6.3/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.592695 jaaql-middleware-python-4.6.3/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.596696 jaaql-middleware-python-4.6.3/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.3/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.607695 jaaql-middleware-python-4.6.3/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    31004 2023-04-17 22:16:44.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3727 2023-04-17 22:18:42.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    41782 2023-04-17 22:17:20.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.608696 jaaql-middleware-python-4.6.3/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.3/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.616695 jaaql-middleware-python-4.6.3/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.620695 jaaql-middleware-python-4.6.3/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.3/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.3/jaaql/services/patch_script_install.py
--rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/services/script_install.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.627696 jaaql-middleware-python-4.6.3/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.632696 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 22:20:49.633696 jaaql-middleware-python-4.6.3/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.676764 jaaql-middleware-python-4.6.4/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-04-19 14:05:16.676764 jaaql-middleware-python-4.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.611798 jaaql-middleware-python-4.6.4/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.614800 jaaql-middleware-python-4.6.4/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4835 2023-04-19 14:05:12.000000 jaaql-middleware-python-4.6.4/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.617796 jaaql-middleware-python-4.6.4/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.4/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/db/db_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.623765 jaaql-middleware-python-4.6.4/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6320 2023-04-06 12:25:17.000000 jaaql-middleware-python-4.6.4/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.4/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.629802 jaaql-middleware-python-4.6.4/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.4/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.632788 jaaql-middleware-python-4.6.4/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.4/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.4/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.634764 jaaql-middleware-python-4.6.4/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.639762 jaaql-middleware-python-4.6.4/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.4/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.651765 jaaql-middleware-python-4.6.4/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    31004 2023-04-17 22:16:44.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3727 2023-04-17 22:18:42.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    41782 2023-04-17 22:17:20.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.653767 jaaql-middleware-python-4.6.4/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.4/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.661790 jaaql-middleware-python-4.6.4/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.4/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.664762 jaaql-middleware-python-4.6.4/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.4/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.4/jaaql/services/patch_script_install.py
+-rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/services/script_install.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.670771 jaaql-middleware-python-4.6.4/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.4/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.4/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:16.675765 jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-04-19 14:05:16.000000 jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2023-04-19 14:05:16.000000 jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:05:16.000000 jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-04-19 14:05:16.000000 jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 14:05:16.000000 jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:05:16.676764 jaaql-middleware-python-4.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.4/setup.py
```

### Comparing `jaaql-middleware-python-4.6.3/LICENSE.txt` & `jaaql-middleware-python-4.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/PKG-INFO` & `jaaql-middleware-python-4.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.3
+Version: 4.6.4
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.3/jaaql/constants.py` & `jaaql-middleware-python-4.6.4/jaaql/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,9 +143,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.6.3"
+VERSION = "4.6.4"
```

### Comparing `jaaql-middleware-python-4.6.3/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.6.4/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.6.4/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.6.4/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.6.4/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.6.4/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.6.4/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.6.4/jaaql/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.6.4/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.6.4/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.6.4/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/jaaql.py` & `jaaql-middleware-python-4.6.4/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.6.4/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.6.4/jaaql/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.6.4/jaaql/mvc/base_controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.6.4/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.6.4/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.6.4/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.6.4/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/mvc/model.py` & `jaaql-middleware-python-4.6.4/jaaql/mvc/model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.6.4/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.6.4/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.6.4/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.6.4/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.6.4/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.6.4/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.6.4/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.6.4/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/services/script_install.py` & `jaaql-middleware-python-4.6.4/jaaql/services/script_install.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.6.4/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/utilities/options.py` & `jaaql-middleware-python-4.6.4/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.6.4/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.6.4/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.6.4/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.3
+Version: 4.6.4
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.6.4/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.3/setup.py` & `jaaql-middleware-python-4.6.4/setup.py`

 * *Files identical despite different names*


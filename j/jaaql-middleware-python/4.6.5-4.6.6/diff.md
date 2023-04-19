# Comparing `tmp/jaaql-middleware-python-4.6.5.tar.gz` & `tmp/jaaql-middleware-python-4.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.6.5.tar", last modified: Wed Apr 19 14:38:22 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.6.6.tar", last modified: Wed Apr 19 14:39:38 2023, max compression
```

## Comparing `jaaql-middleware-python-4.6.5.tar` & `jaaql-middleware-python-4.6.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.727970 jaaql-middleware-python-4.6.5/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-04-19 14:38:22.727970 jaaql-middleware-python-4.6.5/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.635506 jaaql-middleware-python-4.6.5/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.641502 jaaql-middleware-python-4.6.5/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4835 2023-04-19 14:38:08.000000 jaaql-middleware-python-4.6.5/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.647508 jaaql-middleware-python-4.6.5/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.5/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/db/db_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.654502 jaaql-middleware-python-4.6.5/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6320 2023-04-06 12:25:17.000000 jaaql-middleware-python-4.6.5/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.5/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.660503 jaaql-middleware-python-4.6.5/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.5/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.667540 jaaql-middleware-python-4.6.5/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.5/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.5/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.669504 jaaql-middleware-python-4.6.5/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.674507 jaaql-middleware-python-4.6.5/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.5/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.692092 jaaql-middleware-python-4.6.5/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    31004 2023-04-17 22:16:44.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3727 2023-04-17 22:18:42.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    41782 2023-04-17 22:17:20.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.694093 jaaql-middleware-python-4.6.5/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.5/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.705970 jaaql-middleware-python-4.6.5/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.5/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.710967 jaaql-middleware-python-4.6.5/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.5/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.5/jaaql/services/patch_script_install.py
--rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/services/script_install.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.719968 jaaql-middleware-python-4.6.5/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.5/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.5/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:38:22.725967 jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-04-19 14:38:22.000000 jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2023-04-19 14:38:22.000000 jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:38:22.000000 jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-04-19 14:38:22.000000 jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 14:38:22.000000 jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 14:38:22.727970 jaaql-middleware-python-4.6.5/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.137682 jaaql-middleware-python-4.6.6/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-04-19 14:39:38.136682 jaaql-middleware-python-4.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.073112 jaaql-middleware-python-4.6.6/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.077109 jaaql-middleware-python-4.6.6/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4835 2023-04-19 14:39:36.000000 jaaql-middleware-python-4.6.6/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.081109 jaaql-middleware-python-4.6.6/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.6/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/db/db_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.085110 jaaql-middleware-python-4.6.6/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6320 2023-04-06 12:25:17.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.089113 jaaql-middleware-python-4.6.6/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.6/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.093109 jaaql-middleware-python-4.6.6/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.095145 jaaql-middleware-python-4.6.6/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.098109 jaaql-middleware-python-4.6.6/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.6/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.110109 jaaql-middleware-python-4.6.6/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    31004 2023-04-17 22:16:44.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3727 2023-04-17 22:18:42.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    41782 2023-04-17 22:17:20.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.112110 jaaql-middleware-python-4.6.6/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.6/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.119684 jaaql-middleware-python-4.6.6/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.6/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.123683 jaaql-middleware-python-4.6.6/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.6/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.6/jaaql/services/patch_script_install.py
+-rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/services/script_install.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.128682 jaaql-middleware-python-4.6.6/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.6/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:39:38.135683 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-04-19 14:39:37.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2023-04-19 14:39:38.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:39:37.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-04-19 14:39:38.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 14:39:38.000000 jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:39:38.137682 jaaql-middleware-python-4.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.6/setup.py
```

### Comparing `jaaql-middleware-python-4.6.5/LICENSE.txt` & `jaaql-middleware-python-4.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/PKG-INFO` & `jaaql-middleware-python-4.6.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.5
+Version: 4.6.6
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.5/jaaql/constants.py` & `jaaql-middleware-python-4.6.6/jaaql/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,9 +143,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.6.5"
+VERSION = "4.6.6"
```

### Comparing `jaaql-middleware-python-4.6.5/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.6.6/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.6.6/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.6.6/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_internal.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.6.6/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.6.6/jaaql/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.6.6/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.6.6/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.6.6/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/jaaql.py` & `jaaql-middleware-python-4.6.6/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.6.6/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.6.6/jaaql/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.6.6/jaaql/mvc/base_controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.6.6/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.6.6/jaaql/mvc/controller.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.6.6/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.6.6/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/mvc/model.py` & `jaaql-middleware-python-4.6.6/jaaql/mvc/model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.6.6/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.6.6/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.6.6/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.6.6/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.6.6/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.6.6/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.6.6/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.6.6/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/services/script_install.py` & `jaaql-middleware-python-4.6.6/jaaql/services/script_install.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.6.6/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/utilities/options.py` & `jaaql-middleware-python-4.6.6/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.6.6/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.6.6/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.6.6/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.5
+Version: 4.6.6
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.5/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.6.6/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.5/setup.py` & `jaaql-middleware-python-4.6.6/setup.py`

 * *Files identical despite different names*


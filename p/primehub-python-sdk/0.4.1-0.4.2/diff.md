# Comparing `tmp/primehub-python-sdk-0.4.1.tar.gz` & `tmp/primehub-python-sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primehub-python-sdk-0.4.1.tar", last modified: Tue Apr 18 08:56:10 2023, max compression
+gzip compressed data, was "primehub-python-sdk-0.4.2.tar", last modified: Wed Apr 19 02:55:11 2023, max compression
```

## Comparing `primehub-python-sdk-0.4.1.tar` & `primehub-python-sdk-0.4.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.754494 primehub-python-sdk-0.4.1/primehub/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 08:55:58.000000 primehub-python-sdk-0.4.1/primehub/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33979 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_instancetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/apptemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/deployments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.754494 primehub-python-sdk-0.4.1/primehub/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/devlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/doc_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/instancetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/me.py
--rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/recurring_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/resource_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/primehub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/primehub/utils/argparser/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/argparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/optionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/graphql_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_instancetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_cmd_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_cmd_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_graphql_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_group_resource_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_http_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_implementation_in_source_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_output_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_recurring_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_sdk_to_admin_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_sdk_to_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_sdk_to_cli_module_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_validator_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.801779 primehub-python-sdk-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-19 02:55:11.801779 primehub-python-sdk-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.797779 primehub-python-sdk-0.4.2/primehub/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 02:54:58.000000 primehub-python-sdk-0.4.2/primehub/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33960 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_instancetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/admin_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/apptemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/deployments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.797779 primehub-python-sdk-0.4.2/primehub/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/extras/devlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/extras/doc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/extras/e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/instancetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/me.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/recurring_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/resource_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.797779 primehub-python-sdk-0.4.2/primehub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.797779 primehub-python-sdk-0.4.2/primehub/utils/argparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/argparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/optionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/utils/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/primehub/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.797779 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-19 02:55:11.000000 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-19 02:55:11.000000 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 02:55:11.000000 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-19 02:55:11.000000 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 02:55:11.000000 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 02:55:11.000000 primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 02:55:11.801779 primehub-python-sdk-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 02:55:11.801779 primehub-python-sdk-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/graphql_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_admin_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_admin_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_admin_instancetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_cmd_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_cmd_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_graphql_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_group_resource_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_implementation_in_source_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_recurring_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_sdk_to_admin_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_sdk_to_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_sdk_to_cli_module_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_validator_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-19 02:54:22.000000 primehub-python-sdk-0.4.2/tests/test_volumes.py
```

### Comparing `primehub-python-sdk-0.4.1/LICENSE` & `primehub-python-sdk-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/PKG-INFO` & `primehub-python-sdk-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primehub-python-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: PrimeHub Python SDK
 Home-page: https://github.com/InfuseAI/primehub-python-sdk
 Author: qrtt1
 Author-email: qrtt1@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/primehub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `primehub-python-sdk-0.4.1/README.md` & `primehub-python-sdk-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/__init__.py` & `primehub-python-sdk-0.4.2/primehub/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_groups.py` & `primehub-python-sdk-0.4.2/primehub/admin_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -864,15 +864,15 @@
           quotaGpu
           quotaMemory
           projectQuotaCpu
           projectQuotaGpu
           projectQuotaMemory
           sharedVolumeCapacity
         }
-        """ + group_basic_info
+        """
 
         apply_auto_fill(config)
 
         # cannot specify admins when creating
         if config.get('admins'):
             config['admins'] = ''
```

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_images.py` & `primehub-python-sdk-0.4.2/primehub/admin_images.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_instancetypes.py` & `primehub-python-sdk-0.4.2/primehub/admin_instancetypes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_reports.py` & `primehub-python-sdk-0.4.2/primehub/admin_reports.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_secrets.py` & `primehub-python-sdk-0.4.2/primehub/admin_secrets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_users.py` & `primehub-python-sdk-0.4.2/primehub/admin_users.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/admin_volumes.py` & `primehub-python-sdk-0.4.2/primehub/admin_volumes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/apps.py` & `primehub-python-sdk-0.4.2/primehub/apps.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/apptemplates.py` & `primehub-python-sdk-0.4.2/primehub/apptemplates.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/cli.py` & `primehub-python-sdk-0.4.2/primehub/cli.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/config.py` & `primehub-python-sdk-0.4.2/primehub/config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/datasets.py` & `primehub-python-sdk-0.4.2/primehub/datasets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/deployments.py` & `primehub-python-sdk-0.4.2/primehub/deployments.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/extras/devlab.py` & `primehub-python-sdk-0.4.2/primehub/extras/devlab.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/extras/doc_generator.py` & `primehub-python-sdk-0.4.2/primehub/extras/doc_generator.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/extras/e2e.py` & `primehub-python-sdk-0.4.2/primehub/extras/e2e.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/files.py` & `primehub-python-sdk-0.4.2/primehub/files.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/groups.py` & `primehub-python-sdk-0.4.2/primehub/groups.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/images.py` & `primehub-python-sdk-0.4.2/primehub/images.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/info.py` & `primehub-python-sdk-0.4.2/primehub/info.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/instancetypes.py` & `primehub-python-sdk-0.4.2/primehub/instancetypes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/jobs.py` & `primehub-python-sdk-0.4.2/primehub/jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/me.py` & `primehub-python-sdk-0.4.2/primehub/me.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/models.py` & `primehub-python-sdk-0.4.2/primehub/models.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/notebooks.py` & `primehub-python-sdk-0.4.2/primehub/notebooks.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/recurring_jobs.py` & `primehub-python-sdk-0.4.2/primehub/recurring_jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/resource_operations.py` & `primehub-python-sdk-0.4.2/primehub/resource_operations.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/secrets.py` & `primehub-python-sdk-0.4.2/primehub/secrets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/__init__.py` & `primehub-python-sdk-0.4.2/primehub/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/argparser/__init__.py` & `primehub-python-sdk-0.4.2/primehub/utils/argparser/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/completion.py` & `primehub-python-sdk-0.4.2/primehub/utils/completion.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/core.py` & `primehub-python-sdk-0.4.2/primehub/utils/core.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/decorators.py` & `primehub-python-sdk-0.4.2/primehub/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/display.py` & `primehub-python-sdk-0.4.2/primehub/utils/display.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/http_client.py` & `primehub-python-sdk-0.4.2/primehub/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/permission.py` & `primehub-python-sdk-0.4.2/primehub/utils/permission.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/utils/validator.py` & `primehub-python-sdk-0.4.2/primehub/utils/validator.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub/volumes.py` & `primehub-python-sdk-0.4.2/primehub/volumes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/PKG-INFO` & `primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primehub-python-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: PrimeHub Python SDK
 Home-page: https://github.com/InfuseAI/primehub-python-sdk
 Author: qrtt1
 Author-email: qrtt1@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/primehub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/SOURCES.txt` & `primehub-python-sdk-0.4.2/primehub_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/setup.py` & `primehub-python-sdk-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/__init__.py` & `primehub-python-sdk-0.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/graphql_formatter.py` & `primehub-python-sdk-0.4.2/tests/graphql_formatter.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_admin_groups.py` & `primehub-python-sdk-0.4.2/tests/test_admin_groups.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_admin_images.py` & `primehub-python-sdk-0.4.2/tests/test_admin_images.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_admin_instancetypes.py` & `primehub-python-sdk-0.4.2/tests/test_admin_instancetypes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_admin_users.py` & `primehub-python-sdk-0.4.2/tests/test_admin_users.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_cli_config.py` & `primehub-python-sdk-0.4.2/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_cmd_config.py` & `primehub-python-sdk-0.4.2/tests/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_cmd_me.py` & `primehub-python-sdk-0.4.2/tests/test_cmd_me.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_config.py` & `primehub-python-sdk-0.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_datasets.py` & `primehub-python-sdk-0.4.2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_files.py` & `primehub-python-sdk-0.4.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_graphql_lint.py` & `primehub-python-sdk-0.4.2/tests/test_graphql_lint.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_group_resource_operation.py` & `primehub-python-sdk-0.4.2/tests/test_group_resource_operation.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_http_utils.py` & `primehub-python-sdk-0.4.2/tests/test_http_utils.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_implementation_in_source_level.py` & `primehub-python-sdk-0.4.2/tests/test_implementation_in_source_level.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_jobs.py` & `primehub-python-sdk-0.4.2/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_print.py` & `primehub-python-sdk-0.4.2/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_recurring_jobs.py` & `primehub-python-sdk-0.4.2/tests/test_recurring_jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_sdk_to_admin_cli.py` & `primehub-python-sdk-0.4.2/tests/test_sdk_to_admin_cli.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_sdk_to_cli.py` & `primehub-python-sdk-0.4.2/tests/test_sdk_to_cli.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_sdk_to_cli_module_alias.py` & `primehub-python-sdk-0.4.2/tests/test_sdk_to_cli_module_alias.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_test_utils.py` & `primehub-python-sdk-0.4.2/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_validator_tools.py` & `primehub-python-sdk-0.4.2/tests/test_validator_tools.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.1/tests/test_volumes.py` & `primehub-python-sdk-0.4.2/tests/test_volumes.py`

 * *Files identical despite different names*


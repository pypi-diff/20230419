# Comparing `tmp/vertica-python-1.3.1.tar.gz` & `tmp/vertica-python-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertica-python-1.3.1.tar", last modified: Mon Mar  6 13:50:39 2023, max compression
+gzip compressed data, was "vertica-python-1.3.2.tar", last modified: Wed Apr 19 08:47:54 2023, max compression
```

## Comparing `vertica-python-1.3.1.tar` & `vertica-python-1.3.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.732676 vertica-python-1.3.1/
--rw-rw-r--   0 sren      (1000) sren      (1000)    11357 2023-03-06 13:50:39.000000 vertica-python-1.3.1/LICENSE
--rw-rw-r--   0 sren      (1000) sren      (1000)      136 2023-03-06 13:50:39.000000 vertica-python-1.3.1/MANIFEST.in
--rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-03-06 13:50:39.732676 vertica-python-1.3.1/PKG-INFO
--rw-rw-r--   0 sren      (1000) sren      (1000)    43416 2023-03-06 13:50:39.000000 vertica-python-1.3.1/README.md
--rw-rw-r--   0 sren      (1000) sren      (1000)       38 2023-03-06 13:50:39.732676 vertica-python-1.3.1/setup.cfg
--rw-rw-r--   0 sren      (1000) sren      (1000)     3689 2023-03-06 13:50:39.000000 vertica-python-1.3.1/setup.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/
--rw-rw-r--   0 sren      (1000) sren      (1000)     3252 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4974 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/compat.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    21667 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/datatypes.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5662 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2281 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/os_utils.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1761 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/__init__.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/tests/common/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1761 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/common/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6437 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/common/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      848 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/conftest.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/tests/integration_tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1761 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7590 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5798 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_authentication.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4296 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_cancel.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4670 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_column.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4748 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_connection.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    61012 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_cursor.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    41695 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_datatypes.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     7551 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_dates.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2886 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    13226 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_loadbalance.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3870 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_timezones.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5438 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_transfer_format.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4510 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/integration_tests/test_unicode.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/tests/unit_tests/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1761 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2388 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/base.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1994 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/test_errors.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1731 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/test_logging.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3260 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/test_notice.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4623 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/test_parsedsn.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3542 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/test_sql_literal.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4661 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/tests/unit_tests/test_timestamps.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/vertica/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1762 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4888 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/column.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    37653 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/connection.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    44802 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/cursor.py
--rw-rw-r--   0 sren      (1000) sren      (1000)    25087 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/deserializer.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2602 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/log.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python/vertica/messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     2061 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/__init__.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.732676 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     3410 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3294 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/authentication.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2270 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/backend_key_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2035 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/bind_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2037 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/close_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2447 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/command_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3006 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/command_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      891 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/copy_done_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2209 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/copy_in_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2390 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/data_row.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2047 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/empty_query_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)      895 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2164 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/error_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2428 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/load_balance_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1106 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/load_file.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2023 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/no_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3896 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/notice_response.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3569 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/parameter_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3051 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/parameter_status.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2037 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/parse_complete.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2696 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/portal_suspended.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2557 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/ready_for_query.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     6543 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/row_description.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2247 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/unknown.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2107 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/verify_files.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2288 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/write_file.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.732676 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/
--rw-rw-r--   0 sren      (1000) sren      (1000)     2780 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4894 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/bind.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2895 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/cancel_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2917 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/close.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2341 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_data.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1932 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_done.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1638 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_error.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2478 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_fail.py
--rwxrwxr-x   0 sren      (1000) sren      (1000)    10291 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/crypt_windows.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3423 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/describe.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1000 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2842 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/execute.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2301 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/flush.py
--rwxrwxr-x   0 sren      (1000) sren      (1000)     2105 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/load_balance_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3010 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/parse.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4301 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/password.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2548 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/query.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     2081 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/ssl_request.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     4477 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/startup.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1928 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/sync.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1933 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/terminate.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     1344 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/verified_files.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     5210 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/messages/message.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.732676 vertica-python-1.3.1/vertica_python/vertica/mixins/
--rw-rw-r--   0 sren      (1000) sren      (1000)      675 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/mixins/__init__.py
--rw-rw-r--   0 sren      (1000) sren      (1000)     3551 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python/vertica/mixins/notice_response_attr.py
-drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-03-06 13:50:39.728676 vertica-python-1.3.1/vertica_python.egg-info/
--rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python.egg-info/PKG-INFO
--rw-rw-r--   0 sren      (1000) sren      (1000)     5192 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python.egg-info/SOURCES.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)        1 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python.egg-info/dependency_links.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)       33 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python.egg-info/requires.txt
--rw-rw-r--   0 sren      (1000) sren      (1000)       15 2023-03-06 13:50:39.000000 vertica-python-1.3.1/vertica_python.egg-info/top_level.txt
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.499573 vertica-python-1.3.2/
+-rw-rw-r--   0 sren      (1000) sren      (1000)    11357 2023-04-19 08:47:53.000000 vertica-python-1.3.2/LICENSE
+-rw-rw-r--   0 sren      (1000) sren      (1000)      136 2023-04-19 08:47:53.000000 vertica-python-1.3.2/MANIFEST.in
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-04-19 08:47:54.499573 vertica-python-1.3.2/PKG-INFO
+-rw-rw-r--   0 sren      (1000) sren      (1000)    43416 2023-04-19 08:47:53.000000 vertica-python-1.3.2/README.md
+-rw-rw-r--   0 sren      (1000) sren      (1000)       38 2023-04-19 08:47:54.499573 vertica-python-1.3.2/setup.cfg
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3662 2023-04-19 08:47:53.000000 vertica-python-1.3.2/setup.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3198 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4947 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/compat.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    21640 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/datatypes.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5635 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2254 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/os_utils.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/__init__.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/common/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/common/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6410 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/common/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      821 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/conftest.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/integration_tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7563 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5771 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_authentication.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4269 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cancel.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4643 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_column.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4721 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_connection.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    60985 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cursor.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    41668 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_datatypes.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     7524 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_dates.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2859 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    13199 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_loadbalance.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3843 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_timezones.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5411 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_transfer_format.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4483 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/integration_tests/test_unicode.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python/tests/unit_tests/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1734 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2361 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/base.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1967 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_errors.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1704 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_logging.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3233 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_notice.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4596 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_parsedsn.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3515 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_sql_literal.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4634 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/tests/unit_tests/test_timestamps.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1735 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4861 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/column.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    37620 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/connection.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    44858 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/cursor.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)    25060 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/deserializer.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2575 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/log.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2034 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/__init__.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3383 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3267 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/authentication.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2243 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/backend_key_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2008 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/bind_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/close_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3540 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2979 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      864 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_done_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2182 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_in_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2363 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/data_row.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2020 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/empty_query_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      868 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2137 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/error_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2401 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_balance_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1079 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_file.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1996 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/no_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3878 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/notice_response.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3542 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3024 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_status.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2010 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parse_complete.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2669 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/portal_suspended.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2530 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/ready_for_query.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     6516 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/row_description.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2220 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/unknown.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2080 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/verify_files.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2261 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/write_file.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.495573 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2753 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4867 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/bind.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2868 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/cancel_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2890 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/close.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2314 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_data.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1905 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_done.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1611 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_error.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2451 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_fail.py
+-rwxrwxr-x   0 sren      (1000) sren      (1000)    10264 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/crypt_windows.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3396 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/describe.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)      973 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2815 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/execute.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2274 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/flush.py
+-rwxrwxr-x   0 sren      (1000) sren      (1000)     2078 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/load_balance_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2983 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/parse.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4274 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/password.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2521 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/query.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     2054 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/ssl_request.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     4743 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/startup.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1901 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/sync.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1906 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/terminate.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1317 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/verified_files.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5183 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/messages/message.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.499573 vertica-python-1.3.2/vertica_python/vertica/mixins/
+-rw-rw-r--   0 sren      (1000) sren      (1000)      648 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/mixins/__init__.py
+-rw-rw-r--   0 sren      (1000) sren      (1000)     3524 2023-04-19 08:47:53.000000 vertica-python-1.3.2/vertica_python/vertica/mixins/notice_response_attr.py
+drwxrwxr-x   0 sren      (1000) sren      (1000)        0 2023-04-19 08:47:54.491573 vertica-python-1.3.2/vertica_python.egg-info/
+-rw-rw-r--   0 sren      (1000) sren      (1000)     1393 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/PKG-INFO
+-rw-rw-r--   0 sren      (1000) sren      (1000)     5192 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)        1 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)       33 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/requires.txt
+-rw-rw-r--   0 sren      (1000) sren      (1000)       15 2023-04-19 08:47:54.000000 vertica-python-1.3.2/vertica_python.egg-info/top_level.txt
```

### Comparing `vertica-python-1.3.1/LICENSE` & `vertica-python-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vertica-python-1.3.1/PKG-INFO` & `vertica-python-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-python
-Version: 1.3.1
+Version: 1.3.2
 Summary: Official native Python client for the Vertica database.
 Home-page: https://github.com/vertica/vertica-python
 Author: Justin Berka, Alex Kim, Siting Ren
 Author-email: justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com
 License: Apache License 2.0
 Description: vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.
 Keywords: database vertica
```

### Comparing `vertica-python-1.3.1/README.md` & `vertica-python-1.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 *vertica-python* is a native Python client for the Vertica (http://www.vertica.com) database. *vertica-python* is the replacement of the deprecated Python client *vertica_db_client*, which was removed since Vertica server version 9.3.
 
 :loudspeaker: 08/14/2018: *vertica-python* becomes Vertica’s first officially supported open source database client, see the blog [here](https://my.vertica.com/blog/vertica-python-becomes-verticas-first-officially-supported-open-source-database-client/).
 
 Please check out [release notes](https://github.com/vertica/vertica-python/releases) to learn about the latest improvements.
 
-vertica-python has been tested with Vertica 12.0.3 and Python 3.7/3.8/3.9/3.10/3.11. Feel free to submit issues and/or pull requests (Read up on our [contributing guidelines](#contributing-guidelines)).
+vertica-python has been tested with Vertica 12.0.4 and Python 3.7/3.8/3.9/3.10/3.11. Feel free to submit issues and/or pull requests (Read up on our [contributing guidelines](#contributing-guidelines)).
 
 
 ## Installation
 
 To install vertica-python with pip:
 ```bash
 # Latest release version
```

### Comparing `vertica-python-1.3.1/setup.py` & `vertica-python-1.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -41,15 +41,15 @@
 ReqOpts = collections.namedtuple('ReqOpts', ['skip_requirements_regex', 'default_vcs'])
 
 opts = ReqOpts(None, 'git')
 
 # version should use the format 'x.x.x' (instead of 'vx.x.x')
 setup(
     name='vertica-python',
-    version='1.3.1',
+    version='1.3.2',
     description='Official native Python client for the Vertica database.',
     long_description="vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.",
     long_description_content_type='text/markdown',
     author='Justin Berka, Alex Kim, Siting Ren',
     author_email='justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com',
     url='https://github.com/vertica/vertica-python',
     keywords="database vertica",
```

### Comparing `vertica-python-1.3.1/vertica_python/__init__.py` & `vertica-python-1.3.2/vertica_python/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -43,28 +43,28 @@
 from . import errors
 from .errors import (
     Error, Warning, DataError, DatabaseError, IntegrityError, InterfaceError,
     InternalError, NotSupportedError, OperationalError, ProgrammingError)
 
 # Main module for this library.
 __author__ = 'Vertica'
-__copyright__ = 'Copyright (c) 2018-2023 Micro Focus or one of its affiliates.'
+__copyright__ = 'Copyright (c) 2018-2023 Open Text.'
 __license__ = 'Apache 2.0'
 
 __all__ = ['Connection', 'PROTOCOL_VERSION', 'version_info', 'apilevel', 'threadsafety',
            'paramstyle', 'connect', 'parse_dsn', 'Error', 'Warning', 'DataError', 'DatabaseError',
            'IntegrityError', 'InterfaceError', 'InternalError', 'NotSupportedError',
            'OperationalError', 'ProgrammingError']
 
 # The version number of this library.
-version_info = (1, 3, 1)
+version_info = (1, 3, 2)
 __version__ = '.'.join(map(str, version_info))
 
-# The protocol version (3.12) implemented in this library.
-PROTOCOL_VERSION = 3 << 16 | 12
+# The protocol version (3.14) implemented in this library.
+PROTOCOL_VERSION = 3 << 16 | 14
 
 apilevel = 2.0
 threadsafety = 1  # Threads may share the module, but not connections!
 
 # Accepted paramstyles are
 #   'qmark' = Question mark style, e.g. '...WHERE name=?'
 #   'named' = Named style, e.g. '...WHERE name=:name'
```

### Comparing `vertica-python-1.3.1/vertica_python/compat.py` & `vertica-python-1.3.2/vertica_python/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/datatypes.py` & `vertica-python-1.3.2/vertica_python/datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/errors.py` & `vertica-python-1.3.2/vertica_python/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/os_utils.py` & `vertica-python-1.3.2/vertica_python/os_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/__init__.py` & `vertica-python-1.3.2/vertica_python/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/common/__init__.py` & `vertica-python-1.3.2/vertica_python/tests/common/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/common/base.py` & `vertica-python-1.3.2/vertica_python/tests/common/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/conftest.py` & `vertica-python-1.3.2/vertica_python/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2019-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/__init__.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/base.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_authentication.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_cancel.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cancel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2019-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_column.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_connection.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_cursor.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_datatypes.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_dates.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_errors.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_loadbalance.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_loadbalance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_timezones.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_timezones.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_transfer_format.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_transfer_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2022-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/integration_tests/test_unicode.py` & `vertica-python-1.3.2/vertica_python/tests/integration_tests/test_unicode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/__init__.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/base.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/test_errors.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/test_logging.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2019-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/test_notice.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_notice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2019-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/test_parsedsn.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_parsedsn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/test_sql_literal.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_sql_literal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/tests/unit_tests/test_timestamps.py` & `vertica-python-1.3.2/vertica_python/tests/unit_tests/test_timestamps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/__init__.py` & `vertica-python-1.3.2/vertica_python/vertica/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/column.py` & `vertica-python-1.3.2/vertica_python/vertica/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/connection.py` & `vertica-python-1.3.2/vertica_python/vertica/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -73,15 +73,15 @@
 DEFAULT_LOG_PATH = 'vertica_python.log'
 DEFAULT_BINARY_TRANSFER = False
 DEFAULT_REQUEST_COMPLEX_TYPES = True
 try:
     DEFAULT_USER = getpass.getuser()
 except Exception as e:
     DEFAULT_USER = None
-    print("WARN: Cannot get the login user name: {}".format(str(e)))
+    warnings.warn(f"Cannot get the login user name: {str(e)}")
 
 
 def connect(**kwargs):
     # type: (Any) -> Connection
     """Opens a new connection to a Vertica database."""
     return Connection(kwargs)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/cursor.py` & `vertica-python-1.3.2/vertica_python/vertica/cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -35,14 +35,15 @@
 
 
 from __future__ import print_function, division, absolute_import
 
 import datetime
 import glob
 import inspect
+import os
 import re
 import sys
 import traceback
 from decimal import Decimal
 from io import IOBase, BytesIO, StringIO
 from math import isnan
 from tempfile import NamedTemporaryFile, SpooledTemporaryFile, TemporaryFile
@@ -649,15 +650,15 @@
                        "Cursor.register_sql_literal_adapter() function."
                        .format(type(py_obj)))
                 raise TypeError(msg)
 
     # noinspection PyArgumentList
     def format_operation_with_parameters(self, operation, parameters, is_copy_data=False):
         if isinstance(parameters, dict):
-            if parameters and ':' not in operation:
+            if parameters and ':' not in operation and os.environ.get('VERTICA_PYTHON_IGNORE_NAMED_PARAMETER_CHECK') != '1':
                 raise ValueError(f'Invalid SQL: {operation}'
                     "\nHINT: When argument 'parameters' is a dict, variables in SQL should be specified with named (:name) placeholders."
                     " If you use a dict to represent the value of a ROW type column, enclose the dict with brackets('[]') to construct a list.")
             for key, param in parameters.items():
                 if not isinstance(key, str):
                     key = str(key)
                 key = as_text(key)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/deserializer.py` & `vertica-python-1.3.2/vertica_python/vertica/deserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2022-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/log.py` & `vertica-python-1.3.2/vertica_python/vertica/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/__init__.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/__init__.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/authentication.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/backend_key_data.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/backend_key_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/bind_complete.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/terminate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -31,18 +31,12 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
-from ..message import BackendMessage
+from ..message import BulkFrontendMessage
 
 
-class BindComplete(BackendMessage):
-    message_id = b'2'
-
-    def __init__(self, data):
-        BackendMessage.__init__(self)
-
-
-BackendMessage.register(BindComplete)
+class Terminate(BulkFrontendMessage):
+    message_id = b'X'
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/close_complete.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/no_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -34,15 +34,15 @@
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
 from ..message import BackendMessage
 
 
-class CloseComplete(BackendMessage):
-    message_id = b'3'
+class NoData(BackendMessage):
+    message_id = b'n'
 
     def __init__(self, data):
         BackendMessage.__init__(self)
 
 
-BackendMessage.register(CloseComplete)
+BackendMessage.register(NoData)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/command_complete.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/bind_complete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -29,36 +29,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-"""
-CommandComplete message
-
-The server prompt that indicates a command has completed. The command tag
-string is the name of the command that was run.
-"""
-
 from __future__ import print_function, division, absolute_import
 
-import re
-
-from struct import unpack
-
 from ..message import BackendMessage
 
 
-class CommandComplete(BackendMessage):
-    message_id = b'C'
+class BindComplete(BackendMessage):
+    message_id = b'2'
 
     def __init__(self, data):
         BackendMessage.__init__(self)
-        data = unpack('{0}sx'.format(len(data) - 1), data)[0]
-        self.command_tag = data.decode('utf-8')
-
-    def __str__(self):
-        return 'CommandComplete: command_tag = "{}"'.format(self.command_tag)
 
 
-BackendMessage.register(CommandComplete)
+BackendMessage.register(BindComplete)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/command_description.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/command_description.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/copy_done_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_done_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/copy_in_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_balance_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -31,23 +31,31 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
-from struct import unpack
-
 from ..message import BackendMessage
+from struct import unpack
 
 
-class CopyInResponse(BackendMessage):
-    message_id = b'G'
+class LoadBalanceResponse(BackendMessage):
+    message_id = b'Y'
 
     def __init__(self, data):
         BackendMessage.__init__(self)
-        values = unpack('!B{0}H'.format((len(data) - 1) // 2), data)
-        self.format = values[0]
-        self.column_formats = values[2::]
+        unpacked = unpack('!I{0}sx'.format(len(data) - 5), data)
+        self.port = unpacked[0]
+        self.host = unpacked[1].decode('utf-8')
+
+    def get_port(self):
+        return self.port
+
+    def get_host(self):
+        return self.host
+
+    def __str__(self):
+        return "LoadBalanceResponse: host={}, port={}".format(self.host, self.port)
 
 
-BackendMessage.register(CopyInResponse)
+BackendMessage.register(LoadBalanceResponse)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/data_row.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/data_row.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/empty_query_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parse_complete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -34,15 +34,15 @@
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
 from ..message import BackendMessage
 
 
-class EmptyQueryResponse(BackendMessage):
-    message_id = b'I'
+class ParseComplete(BackendMessage):
+    message_id = b'1'
 
     def __init__(self, data):
         BackendMessage.__init__(self)
 
 
-BackendMessage.register(EmptyQueryResponse)
+BackendMessage.register(ParseComplete)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/end_of_batch_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/error_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/error_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/load_balance_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -29,33 +29,46 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
+"""
+ParameterStatus message
+
+A ParameterStatus message will be generated whenever the backend believes the
+frontend should know about a setting parameter value. For example, when you do
+SET SESSION AUTOCOMMIT ON | OFF, you get back a parameter status telling you the
+new value of autocommit.
+
+At present Vertica supports a handful of parameters, they are:
+  standard_conforming_strings, server_version, client_locale, client_label,
+  long_string_types, protocol_version, auto_commit, MARS
+
+More parameters would be added in the future. Accordingly, a frontend should
+simply ignore ParameterStatus for parameters that it does not understand or care
+about.
+"""
+
 from __future__ import print_function, division, absolute_import
 
-from ..message import BackendMessage
 from struct import unpack
 
+from ..message import BackendMessage
 
-class LoadBalanceResponse(BackendMessage):
-    message_id = b'Y'
+
+class ParameterStatus(BackendMessage):
+    message_id = b'S'
 
     def __init__(self, data):
         BackendMessage.__init__(self)
-        unpacked = unpack('!I{0}sx'.format(len(data) - 5), data)
-        self.port = unpacked[0]
-        self.host = unpacked[1].decode('utf-8')
-
-    def get_port(self):
-        return self.port
-
-    def get_host(self):
-        return self.host
+        null_byte = data.find(b'\x00')
+        unpacked = unpack('{0}sx{1}sx'.format(null_byte, len(data) - null_byte - 2), data)
+        self.name = unpacked[0].decode('utf-8')
+        self.value = unpacked[1].decode('utf-8')
 
     def __str__(self):
-        return "LoadBalanceResponse: host={}, port={}".format(self.host, self.port)
+        return "ParameterStatus: {} = {}".format(self.name, self.value)
 
 
-BackendMessage.register(LoadBalanceResponse)
+BackendMessage.register(ParameterStatus)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/load_file.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/load_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/no_data.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/close_complete.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -34,15 +34,15 @@
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
 from ..message import BackendMessage
 
 
-class NoData(BackendMessage):
-    message_id = b'n'
+class CloseComplete(BackendMessage):
+    message_id = b'3'
 
     def __init__(self, data):
         BackendMessage.__init__(self)
 
 
-BackendMessage.register(NoData)
+BackendMessage.register(CloseComplete)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/notice_response.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/notice_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -95,14 +95,14 @@
         pos = 0
         while pos < len(data) - 1:
             null_byte = data.find(b'\x00', pos)
 
             unpacked = unpack_from('c{0}sx'.format(null_byte - 1 - pos), data, pos)
             key = unpacked[0]
             value = unpacked[1]
-            data_mapping[key] = value.decode('utf-8', 'replace')
+            data_mapping[key] = value.decode('utf-8', 'backslashreplace')
 
             pos += (len(value) + 2)
 
         return data_mapping
 
 BackendMessage.register(NoticeResponse)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/parameter_description.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/parameter_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/parameter_status.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/ssl_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -29,46 +29,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-"""
-ParameterStatus message
-
-A ParameterStatus message will be generated whenever the backend believes the
-frontend should know about a setting parameter value. For example, when you do
-SET SESSION AUTOCOMMIT ON | OFF, you get back a parameter status telling you the
-new value of autocommit.
-
-At present Vertica supports a handful of parameters, they are:
-  standard_conforming_strings, server_version, client_locale, client_label,
-  long_string_types, protocol_version, auto_commit, MARS
-
-More parameters would be added in the future. Accordingly, a frontend should
-simply ignore ParameterStatus for parameters that it does not understand or care
-about.
-"""
-
 from __future__ import print_function, division, absolute_import
 
-from struct import unpack
-
-from ..message import BackendMessage
-
-
-class ParameterStatus(BackendMessage):
-    message_id = b'S'
+from struct import pack
 
-    def __init__(self, data):
-        BackendMessage.__init__(self)
-        null_byte = data.find(b'\x00')
-        unpacked = unpack('{0}sx{1}sx'.format(null_byte, len(data) - null_byte - 2), data)
-        self.name = unpacked[0].decode('utf-8')
-        self.value = unpacked[1].decode('utf-8')
+from ..message import BulkFrontendMessage
 
-    def __str__(self):
-        return "ParameterStatus: {} = {}".format(self.name, self.value)
 
+class SslRequest(BulkFrontendMessage):
+    message_id = None
+    SSL_REQUEST = 80877103
 
-BackendMessage.register(ParameterStatus)
+    def read_bytes(self):
+        bytes_ = pack('!I', self.SSL_REQUEST)
+        return bytes_
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/parse_complete.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -31,18 +31,12 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
-from ..message import BackendMessage
+from ..message import BulkFrontendMessage
 
 
-class ParseComplete(BackendMessage):
-    message_id = b'1'
-
-    def __init__(self, data):
-        BackendMessage.__init__(self)
-
-
-BackendMessage.register(ParseComplete)
+class Sync(BulkFrontendMessage):
+    message_id = b'S'
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/portal_suspended.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/portal_suspended.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/ready_for_query.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/ready_for_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/row_description.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/row_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/unknown.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/unknown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/verify_files.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/verify_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/backend_messages/write_file.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/write_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/__init__.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/bind.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/bind.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/cancel_request.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/cancel_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/close.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/close.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_data.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_done.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_done.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_error.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/copy_fail.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/copy_fail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/crypt_windows.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/crypt_windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/describe.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/describe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/end_of_batch_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/execute.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/flush.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/flush.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/load_balance_request.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/load_balance_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/parse.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/password.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/query.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/startup.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/startup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -40,14 +40,16 @@
 Startup message.
 """
 
 from __future__ import print_function, division, absolute_import
 
 import platform
 import os
+import socket
+import warnings
 from struct import pack
 
 # noinspection PyUnresolvedReferences,PyCompatibility
 
 import vertica_python
 from ..message import BulkFrontendMessage
 
@@ -59,36 +61,44 @@
                  binary_transfer, request_complex_types):
         BulkFrontendMessage.__init__(self)
 
         try:
             os_platform = platform.platform()
         except Exception as e:
             os_platform = ''
-            print("WARN: Cannot get the OS info: {}".format(str(e)))
+            warnings.warn(f"Cannot get the OS info: {str(e)}")
 
         try:
             pid = str(os.getpid())
         except Exception as e:
             pid = '0'
-            print("WARN: Cannot get the process ID: {}".format(str(e)))
+            warnings.warn(f"Cannot get the process ID: {str(e)}")
+
+        try:
+            os_hostname = socket.gethostname()
+        except Exception as e:
+            os_hostname = ''
+            warnings.warn(f"Cannot get the OS hostname: {str(e)}")
 
         request_complex_types = 'true' if request_complex_types else 'false'
 
         self.parameters = {
             b'user': user,
             b'database': database,
             b'client_label': session_label,
             b'client_type': 'vertica-python',
             b'client_version': vertica_python.__version__,
             b'client_os': os_platform,
             b'client_os_user_name': os_user_name,
+            b'client_os_hostname': os_hostname,
             b'client_pid': pid,
             b'autocommit': 'on' if autocommit else 'off',
             b'binary_data_protocol': '1' if binary_transfer else '0', # Defaults to text format '0'
             b'protocol_features': '{"request_complex_types":' + request_complex_types + '}',
+            b'protocol_compat': 'VER',
         }
 
     def read_bytes(self):
         # The fixed protocol version is followed by pairs of parameter name and value strings.
         # A zero byte is required as a terminator after the last name/value pair.
         # Parameters can appear in any order.
         fixed_protocol_version = 3 << 16 | 5
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/terminate.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/backend_messages/copy_in_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
@@ -31,12 +31,23 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 from __future__ import print_function, division, absolute_import
 
-from ..message import BulkFrontendMessage
+from struct import unpack
 
+from ..message import BackendMessage
 
-class Terminate(BulkFrontendMessage):
-    message_id = b'X'
+
+class CopyInResponse(BackendMessage):
+    message_id = b'G'
+
+    def __init__(self, data):
+        BackendMessage.__init__(self)
+        values = unpack('!B{0}H'.format((len(data) - 1) // 2), data)
+        self.format = values[0]
+        self.column_formats = values[2::]
+
+
+BackendMessage.register(CopyInResponse)
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/frontend_messages/verified_files.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/frontend_messages/verified_files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2020-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/messages/message.py` & `vertica-python-1.3.2/vertica_python/vertica/messages/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2018-2023 Open Text.
 # Copyright (c) 2018 Uber Technologies, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/mixins/__init__.py` & `vertica-python-1.3.2/vertica_python/vertica/mixins/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2019-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python/vertica/mixins/notice_response_attr.py` & `vertica-python-1.3.2/vertica_python/vertica/mixins/notice_response_attr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Micro Focus or one of its affiliates.
+# Copyright (c) 2019-2023 Open Text.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `vertica-python-1.3.1/vertica_python.egg-info/PKG-INFO` & `vertica-python-1.3.2/vertica_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertica-python
-Version: 1.3.1
+Version: 1.3.2
 Summary: Official native Python client for the Vertica database.
 Home-page: https://github.com/vertica/vertica-python
 Author: Justin Berka, Alex Kim, Siting Ren
 Author-email: justin.berka@gmail.com, alex.kim@uber.com, sitingren@hotmail.com
 License: Apache License 2.0
 Description: vertica-python is the official Vertica database client for the Python programming language. Please check the [project homepage](https://github.com/vertica/vertica-python) for the details.
 Keywords: database vertica
```

### Comparing `vertica-python-1.3.1/vertica_python.egg-info/SOURCES.txt` & `vertica-python-1.3.2/vertica_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*


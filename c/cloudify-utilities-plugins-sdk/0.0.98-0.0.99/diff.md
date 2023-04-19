# Comparing `tmp/cloudify-utilities-plugins-sdk-0.0.98.tar.gz` & `tmp/cloudify-utilities-plugins-sdk-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-utilities-plugins-sdk-0.0.98.tar", last modified: Mon Jan  9 14:03:58 2023, max compression
+gzip compressed data, was "cloudify-utilities-plugins-sdk-0.0.99.tar", last modified: Wed Jan 11 21:12:18 2023, max compression
```

## Comparing `cloudify-utilities-plugins-sdk-0.0.98.tar` & `cloudify-utilities-plugins-sdk-0.0.99.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.278503 cloudify-utilities-plugins-sdk-0.0.98/
--rw-r--r--   0 root         (0) root         (0)    10174 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/LICENSE
--rw-r--r--   0 root         (0) root         (0)      658 2023-01-09 14:03:58.278503 cloudify-utilities-plugins-sdk-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6968 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.270503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/
--rw-r--r--   0 root         (0) root         (0)      617 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1066 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/_compat.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/clean_json.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/cli_tool_base.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/constants.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12345 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/filters.py
--rw-r--r--   0 root         (0) root         (0)     3061 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/ftp.py
--rw-r--r--   0 root         (0) root         (0)     2191 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/hcl.py
--rw-r--r--   0 root         (0) root         (0)     6774 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/importer.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/iso9660.py
--rw-r--r--   0 root         (0) root         (0)     9750 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/ovf.py
--rw-r--r--   0 root         (0) root         (0)    13520 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/processes.py
--rw-r--r--   0 root         (0) root         (0)     7142 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/resource_downloader.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/secure_property_management.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/
--rw-r--r--   0 root         (0) root         (0)      617 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8534 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_cli_tool_base.py
--rw-r--r--   0 root         (0) root         (0)    18144 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_filters.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_ftp.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_hcl.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_iso9660.py
--rw-r--r--   0 root         (0) root         (0)    19810 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_ovf.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_processess.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_resource_downloader.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_secure_property_management.py
--rw-r--r--   0 root         (0) root         (0)    19776 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)    60279 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/
--rw-r--r--   0 root         (0) root         (0)      620 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/client_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/authentication.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/decorators.py
--rw-r--r--   0 root         (0) root         (0)     5772 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/utils.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/state/
--rw-r--r--   0 root         (0) root         (0)      684 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/state/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/state/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5676 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/tests/test_client_resolver.py
--rw-r--r--   0 root         (0) root         (0)     6438 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/tests/test_connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/
--rw-r--r--   0 root         (0) root         (0)      653 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/tests/
--rw-r--r--   0 root         (0) root         (0)      627 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42994 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/tests/test_sdk.py
--rw-r--r--   0 root         (0) root         (0)    14163 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.274503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/
--rw-r--r--   0 root         (0) root         (0)      617 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4354 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/base_connection.py
--rw-r--r--   0 root         (0) root         (0)     4444 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/netconf_connection.py
--rw-r--r--   0 root         (0) root         (0)    13820 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/terminal_connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.278503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/
--rw-r--r--   0 root         (0) root         (0)      617 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5115 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/fake_server.py
--rw-r--r--   0 root         (0) root         (0)     6733 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/test_base_connection.py
--rw-r--r--   0 root         (0) root         (0)     8440 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/test_netconf_connection.py
--rw-r--r--   0 root         (0) root         (0)    17340 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/test_terminal_connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-09 14:03:58.278503 cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      658 2023-01-09 14:03:58.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2443 2023-01-09 14:03:58.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-09 14:03:58.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      187 2023-01-09 14:03:58.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-01-09 14:03:58.000000 cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-09 14:03:58.278503 cloudify-utilities-plugins-sdk-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1898 2023-01-09 14:03:37.000000 cloudify-utilities-plugins-sdk-0.0.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)    10174 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      658 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/clean_json.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/cli_tool_base.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/filters.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/hcl.py
+-rw-r--r--   0 root         (0) root         (0)     6774 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/importer.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/iso9660.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/ovf.py
+-rw-r--r--   0 root         (0) root         (0)    13520 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/processes.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/resource_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/secure_property_management.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8534 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_cli_tool_base.py
+-rw-r--r--   0 root         (0) root         (0)    18144 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_filters.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_hcl.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_iso9660.py
+-rw-r--r--   0 root         (0) root         (0)    19810 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_ovf.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_processess.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_resource_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_secure_property_management.py
+-rw-r--r--   0 root         (0) root         (0)    19776 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)    60279 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/client_resolver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/authentication.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/utils.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/state/
+-rw-r--r--   0 root         (0) root         (0)      684 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/state/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/state/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5676 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/tests/test_client_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     6438 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/tests/test_connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/
+-rw-r--r--   0 root         (0) root         (0)      653 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/tests/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42994 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/tests/test_sdk.py
+-rw-r--r--   0 root         (0) root         (0)    14163 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/base_connection.py
+-rw-r--r--   0 root         (0) root         (0)     4444 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/netconf_connection.py
+-rw-r--r--   0 root         (0) root         (0)    13820 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/terminal_connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5115 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/fake_server.py
+-rw-r--r--   0 root         (0) root         (0)     6733 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/test_base_connection.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/test_netconf_connection.py
+-rw-r--r--   0 root         (0) root         (0)    17340 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/test_terminal_connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      658 2023-01-11 21:12:18.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-01-11 21:12:18.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 21:12:18.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      187 2023-01-11 21:12:18.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-01-11 21:12:18.000000 cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-11 21:12:18.590378 cloudify-utilities-plugins-sdk-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-01-11 21:12:03.000000 cloudify-utilities-plugins-sdk-0.0.99/setup.py
```

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/LICENSE` & `cloudify-utilities-plugins-sdk-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/PKG-INFO` & `cloudify-utilities-plugins-sdk-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudify-utilities-plugins-sdk
-Version: 0.0.98
+Version: 0.0.99
 Summary: Utilities SDK for extending Cloudify
 Home-page: https://github.com/cloudify-incubator/cloudify-utilities-plugins-sdk
 Author: Cloudify Platform Ltd.
 Author-email: hello@cloudify.co
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/README.md` & `cloudify-utilities-plugins-sdk-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/_compat.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/clean_json.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/clean_json.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/cli_tool_base.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/cli_tool_base.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/exceptions.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/filters.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/filters.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/ftp.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/ftp.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/hcl.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/hcl.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/importer.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/importer.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/iso9660.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/iso9660.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/ovf.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/ovf.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/processes.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/processes.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/resource_downloader.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/resource_downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,46 +75,50 @@
     schema = split[0]
     kwargs = {}
     try:
         import git
         if tag_name:
             kwargs["branch"] = tag_name
         if username:
-            auth_url_part = ''
-            if username:
-                auth_url_part = '{}:{}@'.format(username, password)
+            auth_url_part = '{}:{}@'.format(username, password)
             updated_url = '{}://{}{}'.format(
                 schema, auth_url_part, split[1])
             source_path = updated_url
-        repo = git.Repo.clone_from(source_path, tmp_path, **kwargs)
-        for submodule in repo.submodules:
-            submodule.update(init=True)
+        git_clone(git, source_path, tmp_path, kwargs)
     except git.exc.GitCommandError as e:
         if "Permission denied" in str(e):
             raise NonRecoverableError(
                 "User cfyuser might not have read permissions to "
                 "the private key or the key is not allowed to the repo"
             )
         elif 'Host key verification failed' in str(e):
             host_beginning = source_path.index('@') + 1
             host_end = source_path.index(':')
             host = source_path[host_beginning: host_end]
             os.system("ssh-keyscan -t rsa {} >> ~/.ssh/known_hosts"
                       .format(host))
-            git.Repo.clone_from(source_path, tmp_path, **kwargs)
+            git_clone(git, source_path, tmp_path, kwargs)
         else:
             raise NonRecoverableError(e)
     except ImportError:
         raise NonRecoverableError(
             "Clone git repo is only supported if git is installed "
             "on your manager and accessible in the management "
             "user's path.")
     return tmp_path
 
 
+def git_clone(git, source_path, tmp_path, kwargs):
+    repo = git.Repo.clone_from(source_path, tmp_path, **kwargs)
+    for submodule in repo.submodules:
+        # force needed in case there are folders already in the repo otherwise
+        # it initiates the submodule but says that all files were deleted
+        submodule.update(init=True, recursive=True, force=True)
+
+
 def get_http_https_resource(source_path,
                             file_type,
                             dir=None,
                             username=None,
                             password=None):
     if not file_type:
         # try and figure-out the type from headers
```

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/secure_property_management.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/secure_property_management.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_cli_tool_base.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_cli_tool_base.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_filters.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_ftp.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_ftp.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_hcl.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_hcl.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_iso9660.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_iso9660.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_ovf.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_ovf.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_processess.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_processess.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_resource_downloader.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_resource_downloader.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_secure_property_management.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_secure_property_management.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/tests/test_utils.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_common_sdk/utils.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_common_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/client_resolver.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/client_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/authentication.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/authentication.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/configuration.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/configuration.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/decorators.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/decorators.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/connection/utils.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/connection/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/exceptions.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/state/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/state/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/state/resources.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/state/resources.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/tests/test_client_resolver.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/tests/test_client_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_kubernetes_sdk/tests/test_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_kubernetes_sdk/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/tests/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/tests/test_sdk.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_rest_sdk/utility.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_rest_sdk/utility.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/base_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/base_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/netconf_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/netconf_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/terminal_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/terminal_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/__init__.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/fake_server.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/fake_server.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/test_base_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/test_base_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/test_netconf_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/test_netconf_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_terminal_sdk/tests/test_terminal_connection.py` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_terminal_sdk/tests/test_terminal_connection.py`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/PKG-INFO` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudify-utilities-plugins-sdk
-Version: 0.0.98
+Version: 0.0.99
 Summary: Utilities SDK for extending Cloudify
 Home-page: https://github.com/cloudify-incubator/cloudify-utilities-plugins-sdk
 Author: Cloudify Platform Ltd.
 Author-email: hello@cloudify.co
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/cloudify_utilities_plugins_sdk.egg-info/SOURCES.txt` & `cloudify-utilities-plugins-sdk-0.0.99/cloudify_utilities_plugins_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudify-utilities-plugins-sdk-0.0.98/setup.py` & `cloudify-utilities-plugins-sdk-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import setuptools
 
 
 setuptools.setup(
     name='cloudify-utilities-plugins-sdk',
-    version='0.0.98',
+    version='0.0.99',
     author='Cloudify Platform Ltd.',
     author_email='hello@cloudify.co',
     description='Utilities SDK for extending Cloudify',
     long_description="""
         # Cloudify Utilities SDK
 
         Utilities SDK for extending Cloudify features.
```


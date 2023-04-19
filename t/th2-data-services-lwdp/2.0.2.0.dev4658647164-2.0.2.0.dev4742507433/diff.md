# Comparing `tmp/th2_data_services_lwdp-2.0.2.0.dev4658647164.tar.gz` & `tmp/th2_data_services_lwdp-2.0.2.0.dev4742507433.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4658647164.tar", last modified: Mon Apr 10 15:16:13 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.0.2.0.dev4742507433.tar", last modified: Wed Apr 19 11:01:48 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164.tar` & `th2_data_services_lwdp-2.0.2.0.dev4742507433.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-10 15:15:57.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1636 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    38684 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11129 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-04-10 15:12:04.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-10 15:16:13.000000 th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-19 11:01:32.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38764 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-19 10:59:08.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/response_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-19 11:01:48.000000 th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.0.2.0.dev4658647164
+Version: 2.0.2.0.dev4742507433
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/README.md` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/setup.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     long_description_content_type="text/markdown",
     author="TH2-devs",
     author_email="th2-devs@exactprosystems.com",
     url="https://github.com/th2-net/th2-ds-source-lwdp",
     license="Apache License 2.0",
     python_requires=">=3.7",
     install_requires=requirements,
-    packages=find_namespace_packages(include=["th2_data_services.*"]),
+    packages=find_namespace_packages(include=["th2_data_services", "th2_data_services.*"]),
     include_package_data=True,
-)
+)
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     DEFAULT_BUFFER_LIMIT,
 )
 from th2_data_services.utils.decode_error_handler import UNICODE_REPLACE_HANDLER
 from th2_data_services.data_source.lwdp.filters.event_filters import LwDPEventFilter
 from th2_data_services.data_source.lwdp.utils import (
     _check_datetime,
     _check_list_or_tuple,
+    _check_response_formats,
 )
 from th2_data_services.data_source.lwdp.utils.json import BufferedJSONProcessor
 from th2_data_services.data_source.lwdp.page import PageNotFound
 
 Event = dict
 
 # LOG import logging
@@ -634,42 +635,41 @@
     def __init__(self, id: str, use_stub=False, response_formats: List[str] = None):
         """GetMessageById constructor.
 
         Args:
             id: Message id.
             use_stub: If True the command returns stub instead of exception.
             response_formats: Allowed values: ["BASE_64","JSON_PARSED"] and ["BASE_64"]
+
         """
         super().__init__()
         self._id = id
         self._stub_status = use_stub
         self._response_formats = response_formats
 
     def handle(self, data_source: HTTPDataSource) -> dict:  # noqa: D102
         api: HTTPAPI = data_source.source_api
-        if not isinstance(self._response_formats,list) and self._response_formats is not None:
-            raise Exception("response_formats argument should be a list")
-        if self._response_formats in [None,["JSON_PARSED","BASE_64"],["BASE_64","JSON_PARSED"]]:
+        if self._response_formats in [['JSON_PARSED','BASE_64'],['BASE_64','JSON_PARSED'],None]:
             only_raw = False
-        elif self._response_formats in [["BASE_64"]]:
+        elif self._response_formats == ['BASE_64']:
             only_raw = True
         else:
-            raise Exception('response_formats takes only values ["BASE_64","JSON_PARSED"] or ["BASE_64"]')
-        url = api.get_url_find_message_by_id(self._id,only_raw=only_raw)
+            raise Exception("response_formats should be either ['BASE_64'] or ['JSON_PARSED','BASE_64']")
 
+        url = api.get_url_find_message_by_id(self._id, only_raw)
         # LOG         logger.info(url)
         response = api.execute_request(url)
         if response.status_code in (404, 408) and self._stub_status:
             stub = data_source.message_stub_builder.build(
                 {data_source.message_struct.MESSAGE_ID: self._id}
             )
             return stub
         elif response.status_code in (404, 408):
             # LOG             logger.error(f"Unable to find the message. Id: {self._id}")
-            raise MessageNotFound(self._id)
+            raise MessageNotFound(self._id,"Unable to find the message")
         else:
             return response.json()
 
 
 class GetMessagesById(IHTTPCommand):
     """A Class-Command for request to lw-data-provider.
 
@@ -685,14 +685,15 @@
     def __init__(self, ids: List[str], use_stub=False, response_formats: List[str] = None):
         """GetMessagesById constructor.
 
         Args:
             ids: Message id list.
             use_stub: If True the command returns stub instead of exception.
             response_formats: Allowed values: ["BASE_64","JSON_PARSED"] and ["BASE_64"]
+
         """
         super().__init__()
         self._ids: ids = ids
         self._stub_status = use_stub
         self._response_formats = response_formats
 
     def handle(self, data_source: HTTPDataSource) -> List[dict]:  # noqa: D102
@@ -757,14 +758,15 @@
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         if response_formats is None:
             response_formats = [ResponseFormat.JSON_PARSED]
         _check_datetime(start_timestamp)
         if end_timestamp:
             _check_datetime(end_timestamp)
+        _check_response_formats(response_formats)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
 
@@ -864,14 +866,15 @@
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
         if response_formats is None:
             response_formats = [ResponseFormat.JSON_PARSED]
         _check_datetime(start_timestamp)
         _check_datetime(end_timestamp)
+        _check_response_formats(response_formats)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
 
@@ -933,14 +936,15 @@
             keep_open: If true, keeps pulling for new message until don't have one outside the requested range.
             max_url_length: API request url max length.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
+        _check_response_formats(response_formats)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
         if response_formats is None:
@@ -1017,14 +1021,15 @@
             keep_open: If true, keeps pulling for new message until don't have one outside the requested range.
             char_enc: Encoding for the byte stream.
             decode_error_handler: Registered decode error handler.
             cache: If True, all requested data from lw-data-provider will be saved to cache.
             max_url_length: API request url max length.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
+        _check_response_formats(response_formats)
         super().__init__(
             cache=cache,
             buffer_limit=buffer_limit,
             char_enc=char_enc,
             decode_error_handler=decode_error_handler,
         )
         if response_formats is None:
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,18 @@
         """REST-API `book/{bookID}/message/groups` call returns a list of message groups in book named bookID."""
         return self.__encode_url(f"{self._url}/book/{book_id}/message/groups")
 
     def get_url_find_event_by_id(self, event_id: str) -> str:
         """REST-API `event` call returns a single event with the specified id."""
         return self.__encode_url(f"{self._url}/event/{event_id}")
 
-    def get_url_find_message_by_id(self, message_id: str, only_raw: bool = False) -> str:
-        """REST-API `message` call returns a single message with the specified id."""
+    def get_url_find_message_by_id(
+        self, message_id: str, only_raw: bool = False
+    ) -> str:
+        """REST-API `message` call returns a single      message with the specified id."""
         return self.__encode_url(f"{self._url}/message/{message_id}?onlyRaw={only_raw}")
 
     def get_url_get_pages_info_all(self, book_id: str):
         """REST-API `search/see/page-infos/{$BOOK_ID}/all` call returns page information with the specified timeframe."""
         url = f"{self._url}/search/sse/page-infos/{book_id}/all"
         return self.__encode_url(url)
 
@@ -154,15 +156,15 @@
         kwargs = {
             "startTimestamp": start_timestamp,
             "messageId": message_ids,
             "stream": stream,
             "searchDirection": search_direction,
             "resultCountLimit": result_count_limit,
             "endTimestamp": end_timestamp,
-            "responseFormats": response_formats,
+            "responseFormat": response_formats,
             "keepOpen": keep_open,
             "bookId": book_id,
         }
         if stream:
             kwargs["stream"] = None
             optional = [f"&stream={x}" for x in stream]
         else:
@@ -170,15 +172,15 @@
             optional = [f"&messageId={x}" for x in message_ids]
 
         query = ""
         url = f"{self._url}/search/sse/messages?"
         for k, v in kwargs.items():
             if v is None:
                 continue
-            if k in ["stream", "responseFormats", "messageId"]:
+            if k in ["stream", "responseFormat", "messageId"]:
                 for item in v:
                     query += f"&{k}={item}"
             else:
                 query += f"&{k}={v}"
         url = f"{url}{query[1:]}"
         urls = self.__split_requests(url, optional, max_url_length)
         return [self.__encode_url(url) for url in urls]
@@ -214,25 +216,25 @@
             Iterable object which return messages as parts of streaming response or message stream pointers.
         """
         kwargs = {
             "startTimestamp": start_timestamp,
             "endTimestamp": end_timestamp,
             "bookId": book_id,
             "sort": sort,
-            "responseFormats": response_formats,
+            "responseFormat": response_formats,
             "keepOpen": keep_open,
         }
         groups = [f"&group={x}" for x in groups]  # "&group=".join(groups)  #
         options = []
         url = f"{self._url}/search/sse/messages/group?"
 
         for k, v in kwargs.items():
             if v is None:
                 continue
-            if k in ["responseFormats"]:
+            if k in ["responseFormat"]:
                 for item in v:
                     options.append(self._option(k, item))
             else:
                 options.append(self._option(k, v))
 
         options_url = "&".join(options)
         url = f"{url}{options_url}"
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .misc import _check_list_or_tuple, _check_datetime
+from .misc import _check_list_or_tuple, _check_datetime, _check_response_formats
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,24 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from datetime import datetime
-
+from typing import List
+from th2_data_services.data_source.lwdp.utils.response_formats import ResponseFormats
 
 def _check_list_or_tuple(variable, var_name):  # noqa
     if not (isinstance(variable, tuple) or isinstance(variable, list)):
         raise TypeError(f"{var_name} argument has to be list or tuple type. Got {type(variable)}")
 
 
 def _check_datetime(dt: datetime):
     if not isinstance(dt, datetime):
         raise TypeError("Provided timestamp should be `datetime` object")
+
+
+def _check_response_formats(formats: List[str]):
+    rf = ResponseFormats()
+    if not rf.is_valid_response_format(formats):
+        raise Exception("Invalid response format")
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.0.2.0.dev4658647164
+Version: 2.0.2.0.dev4742507433
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.2.0.dev4658647164/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.0.2.0.dev4742507433/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,12 +33,13 @@
 th2_data_services/data_source/lwdp/interfaces/source_api.py
 th2_data_services/data_source/lwdp/source_api/__init__.py
 th2_data_services/data_source/lwdp/source_api/grpc.py
 th2_data_services/data_source/lwdp/source_api/http.py
 th2_data_services/data_source/lwdp/utils/__init__.py
 th2_data_services/data_source/lwdp/utils/json.py
 th2_data_services/data_source/lwdp/utils/misc.py
+th2_data_services/data_source/lwdp/utils/response_formats.py
 th2_data_services_lwdp.egg-info/PKG-INFO
 th2_data_services_lwdp.egg-info/SOURCES.txt
 th2_data_services_lwdp.egg-info/dependency_links.txt
 th2_data_services_lwdp.egg-info/requires.txt
 th2_data_services_lwdp.egg-info/top_level.txt
```


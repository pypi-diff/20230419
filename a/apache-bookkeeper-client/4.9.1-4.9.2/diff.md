# Comparing `tmp/apache-bookkeeper-client-4.9.1.tar.gz` & `tmp/apache-bookkeeper-client-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-bookkeeper-client-4.9.1.tar", last modified: Sun Apr  7 20:19:49 2019, max compression
+gzip compressed data, was "dist/apache-bookkeeper-client-4.9.2.tar", last modified: Thu May 16 18:23:06 2019, max compression
```

## Comparing `apache-bookkeeper-client-4.9.1.tar` & `apache-bookkeeper-client-4.9.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1115 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/PKG-INFO
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     2730 2019-03-21 20:53:00.000000 apache-bookkeeper-client-4.9.1/setup.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)       67 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/setup.cfg
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)        1 2019-04-07 20:19:14.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/not-zip-safe
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1115 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/PKG-INFO
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)       11 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/namespace_packages.txt
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)       11 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/top_level.txt
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1606 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/SOURCES.txt
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)        1 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/dependency_links.txt
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      147 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/requires.txt
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      190 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/README.rst
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/admin/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     3620 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/admin/namespaces.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      664 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/admin/exceptions.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     4079 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/admin/namespace.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     2588 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/admin/client.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      657 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/admin/__init__.py
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    53179 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_rpc_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     2493 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/common_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    53441 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/stream_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     7396 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     4969 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_rpc_pb2_grpc.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     7141 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/cluster_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    51558 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/storage_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     8462 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/storage_pb2_grpc.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    11814 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_store_pb2.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      571 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/proto/__init__.py
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    10198 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/exceptions.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     7665 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/datetime_helpers.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     8445 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/method.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1293 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/service_uri.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    11260 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/retry.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     7369 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/timeout.py
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/router/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      822 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/router/router.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      643 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/router/__init__.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1081 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/general_helpers.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    11612 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/protobuf_helpers.py
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/future/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1217 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/future/_helpers.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1752 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/future/base.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      680 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/future/__init__.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     5939 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/future/polling.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     1090 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/util.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)    10755 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/grpc_helpers.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      571 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/__init__.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     2622 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/common/constants.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     2126 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/types.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      742 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/__init__.py
-drwxrwxr-x   0 eolivelli  (1000) eolivelli  (1000)        0 2019-04-07 20:19:49.000000 apache-bookkeeper-client-4.9.1/bookkeeper/kv/
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      664 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/kv/exceptions.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     6354 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/kv/futures.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     5125 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/kv/table.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)     2734 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/kv/client.py
--rw-rw-r--   0 eolivelli  (1000) eolivelli  (1000)      654 2018-12-20 22:53:05.000000 apache-bookkeeper-client-4.9.1/bookkeeper/kv/__init__.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/
+-rw-r--r--   0 mmerli     (501) staff       (20)     1115 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/PKG-INFO
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/kv/
+-rw-r--r--   0 mmerli     (501) staff       (20)     2734 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/kv/client.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      654 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/kv/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     6354 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/kv/futures.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      664 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/kv/exceptions.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     5125 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/kv/table.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/
+-rw-r--r--   0 mmerli     (501) staff       (20)     2493 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/common_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      571 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     8462 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/storage_pb2_grpc.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     7396 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    53179 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_rpc_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     7141 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/cluster_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    53441 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/stream_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    11814 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_store_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    51558 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/storage_pb2.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     4969 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_rpc_pb2_grpc.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/admin/
+-rw-r--r--   0 mmerli     (501) staff       (20)     2588 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/admin/client.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      657 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/admin/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      664 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/admin/exceptions.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     4079 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/admin/namespace.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     3620 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/admin/namespaces.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      742 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     2126 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/types.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/
+-rw-r--r--   0 mmerli     (501) staff       (20)     7665 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/datetime_helpers.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     1293 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/service_uri.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     1090 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/util.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     2622 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/constants.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     7369 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/timeout.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      571 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    10755 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/grpc_helpers.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    11260 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/retry.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    11612 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/protobuf_helpers.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     8445 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/method.py
+-rw-r--r--   0 mmerli     (501) staff       (20)    10198 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/exceptions.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/future/
+-rw-r--r--   0 mmerli     (501) staff       (20)      680 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/future/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     5939 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/future/polling.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     1752 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/future/base.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     1217 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/future/_helpers.py
+-rw-r--r--   0 mmerli     (501) staff       (20)     1081 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/general_helpers.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/router/
+-rw-r--r--   0 mmerli     (501) staff       (20)      643 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/router/__init__.py
+-rw-r--r--   0 mmerli     (501) staff       (20)      957 2019-05-07 21:45:52.000000 apache-bookkeeper-client-4.9.2/bookkeeper/common/router/router.py
+drwxr-xr-x   0 mmerli     (501) staff       (20)        0 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/
+-rw-r--r--   0 mmerli     (501) staff       (20)     1115 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/PKG-INFO
+-rw-r--r--   0 mmerli     (501) staff       (20)        1 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/not-zip-safe
+-rw-r--r--   0 mmerli     (501) staff       (20)       11 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 mmerli     (501) staff       (20)     1606 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mmerli     (501) staff       (20)      149 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/requires.txt
+-rw-r--r--   0 mmerli     (501) staff       (20)       11 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/top_level.txt
+-rw-r--r--   0 mmerli     (501) staff       (20)        1 2019-05-16 18:23:05.000000 apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mmerli     (501) staff       (20)     2732 2019-05-16 18:22:33.000000 apache-bookkeeper-client-4.9.2/setup.py
+-rw-r--r--   0 mmerli     (501) staff       (20)       67 2019-05-16 18:23:06.000000 apache-bookkeeper-client-4.9.2/setup.cfg
+-rw-r--r--   0 mmerli     (501) staff       (20)      190 2019-04-15 21:57:20.000000 apache-bookkeeper-client-4.9.2/README.rst
```

### Comparing `apache-bookkeeper-client-4.9.1/PKG-INFO` & `apache-bookkeeper-client-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: apache-bookkeeper-client
-Version: 4.9.1
+Version: 4.9.2
 Summary: Apache BookKeeper client library
 Home-page: https://github.com/apache/bookkeeper/tree/master/stream/clients/python
 Author: Apache BookKeeper
 Author-email: dev@bookkeeper.apache.org
 License: Apache 2.0
 Description: Python Client for Apache BookKeeper
         ===================================
```

### Comparing `apache-bookkeeper-client-4.9.1/setup.py` & `apache-bookkeeper-client-4.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 import setuptools
 
 # Package metadata.
 
 name = 'apache-bookkeeper-client'
 description = 'Apache BookKeeper client library'
-version = '4.9.1'
+version = '4.9.2'
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = 'Development Status :: 3 - Alpha'
 dependencies = [
     'protobuf>=3.0.0',
     'requests<3.0.0dev,>=2.18.0',
     'setuptools>=34.0.0',
     'six>=1.10.0',
     'pytz',
     'futures>=3.2.0;python_version<"3.2"',
     'grpcio>=1.8.2',
-    'mmh3>=2.5.1'
+    'pymmh3>=0.0.3'
 ]
 extras = {
 }
 
 # Setup boilerplate below this line.
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/PKG-INFO` & `apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: apache-bookkeeper-client
-Version: 4.9.1
+Version: 4.9.2
 Summary: Apache BookKeeper client library
 Home-page: https://github.com/apache/bookkeeper/tree/master/stream/clients/python
 Author: Apache BookKeeper
 Author-email: dev@bookkeeper.apache.org
 License: Apache 2.0
 Description: Python Client for Apache BookKeeper
         ===================================
```

### Comparing `apache-bookkeeper-client-4.9.1/apache_bookkeeper_client.egg-info/SOURCES.txt` & `apache-bookkeeper-client-4.9.2/apache_bookkeeper_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/admin/namespaces.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/admin/namespaces.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/admin/exceptions.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/kv/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/admin/namespace.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/admin/namespace.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/admin/client.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/admin/client.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/admin/__init__.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_rpc_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/common_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/stream_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_rpc_pb2_grpc.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/cluster_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/storage_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/storage_pb2_grpc.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/storage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/kv_store_pb2.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/kv_store_pb2.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/proto/__init__.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/exceptions.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/datetime_helpers.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/method.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/method.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/service_uri.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/service_uri.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/retry.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/retry.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/timeout.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/timeout.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/router/router.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/router/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import mmh3
+from bookkeeper.common.router.router import BytesHashRouter
 
-__SEED__ = 383242705
-
-
-class BytesHashRouter(object):
-    """A router that computes hash values for keys using MurmurHash3"""
-
-    def __init__(self):
-        return
-
-    def getRoutingKey(self, key):
-        return mmh3.hash64(key, seed=__SEED__, signed=True)[0]
+__all__ = [
+    'BytesHashRouter',
+]
```

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/router/__init__.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/future/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,12 +6,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from bookkeeper.common.router.router import BytesHashRouter
+"""Futures for dealing with asynchronous operations."""
+
+from bookkeeper.common.future.base import Future
 
 __all__ = [
-    'BytesHashRouter',
+    'Future',
 ]
```

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/general_helpers.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/general_helpers.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/protobuf_helpers.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/protobuf_helpers.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/future/_helpers.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/future/_helpers.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/future/base.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/future/base.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/future/polling.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/future/polling.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/util.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/util.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/grpc_helpers.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/grpc_helpers.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/__init__.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/common/constants.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/common/constants.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/types.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/types.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/__init__.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/kv/exceptions.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/admin/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/kv/futures.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/kv/futures.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/kv/table.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/kv/table.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/kv/client.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/kv/client.py`

 * *Files identical despite different names*

### Comparing `apache-bookkeeper-client-4.9.1/bookkeeper/kv/__init__.py` & `apache-bookkeeper-client-4.9.2/bookkeeper/kv/__init__.py`

 * *Files identical despite different names*


# Comparing `tmp/blissdata-0.3.2.tar.gz` & `tmp/blissdata-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blissdata-0.3.2.tar", last modified: Mon Jan 23 08:48:13 2023, max compression
+gzip compressed data, was "blissdata-0.3.3.tar", last modified: Wed Apr 19 11:54:37 2023, max compression
```

## Comparing `blissdata-0.3.2.tar` & `blissdata-0.3.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.522478 blissdata-0.3.2/
--rw-r--r--   0 root         (0) root         (0)     7651 2023-01-23 08:48:08.000000 blissdata-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1592 2023-01-23 08:48:13.522478 blissdata-0.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-23 08:48:08.000000 blissdata-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.510478 blissdata-0.3.2/blissdata/
--rw-r--r--   0 root         (0) root         (0)      288 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.510478 blissdata-0.3.2/blissdata/beacon/
--rw-r--r--   0 root         (0) root         (0)       27 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/beacon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3414 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/beacon/_base.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/beacon/config.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/beacon/data.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/beacon/files.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.510478 blissdata-0.3.2/blissdata/common/
--rw-r--r--   0 root         (0) root         (0)      262 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.510478 blissdata-0.3.2/blissdata/data/
--rwxr-xr-x   0 root         (0) root         (0)      262 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.514478 blissdata-0.3.2/blissdata/data/events/
--rw-r--r--   0 root         (0) root         (0)      584 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/events/channel.py
--rw-r--r--   0 root         (0) root         (0)    17760 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/events/lima.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/events/node.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/events/scan.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/events/walk.py
--rw-r--r--   0 root         (0) root         (0)     1187 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/expiration.py
--rw-r--r--   0 root         (0) root         (0)    13578 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/lima_image.py
--rw-r--r--   0 root         (0) root         (0)    57212 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.514478 blissdata-0.3.2/blissdata/data/nodes/
--rw-r--r--   0 root         (0) root         (0)      261 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13600 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/channel.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/dataset.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/dataset_collection.py
--rwxr-xr-x   0 root         (0) root         (0)    14590 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/lima.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/node_ref_channel.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/proposal.py
--rwxr-xr-x   0 root         (0) root         (0)     6855 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/scan.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/nodes/scan_group.py
--rw-r--r--   0 root         (0) root         (0)     7796 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/remote_node.py
--rwxr-xr-x   0 root         (0) root         (0)    23623 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/data/scan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.518478 blissdata-0.3.2/blissdata/h5api/
--rw-r--r--   0 root         (0) root         (0)       68 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/abstract.py
--rw-r--r--   0 root         (0) root         (0)     4363 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/dynamic_hdf5.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/file_arguments.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/static_hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.518478 blissdata-0.3.2/blissdata/h5api/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/utils/bliss.py
--rw-r--r--   0 root         (0) root         (0)     7399 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/utils/hdf5.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/utils/hdf5_retry.py
--rw-r--r--   0 root         (0) root         (0)     8634 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/utils/lima.py
--rw-r--r--   0 root         (0) root         (0)      423 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/h5api/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.518478 blissdata-0.3.2/blissdata/redis/
--rw-r--r--   0 root         (0) root         (0)      524 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13124 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/redis/caching.py
--rw-r--r--   0 root         (0) root         (0)     6194 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/redis/connection.py
--rw-r--r--   0 root         (0) root         (0)     5777 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/redis/manager.py
--rw-r--r--   0 root         (0) root         (0)    32367 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/redis/proxy.py
--rw-r--r--   0 root         (0) root         (0)      819 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/redis/scripting.py
--rw-r--r--   0 root         (0) root         (0)    32749 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/settings.py
--rw-r--r--   0 root         (0) root         (0)    29284 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/streaming.py
--rw-r--r--   0 root         (0) root         (0)     9214 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/streaming_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.518478 blissdata-0.3.2/blissdata/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.518478 blissdata-0.3.2/blissdata/tests/beacon/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/beacon/__init__.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/beacon/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/beacon/test_data.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/beacon/test_files.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.522478 blissdata-0.3.2/blissdata/tests/h5api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/h5api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12924 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/h5api/scanner.py
--rw-r--r--   0 root         (0) root         (0)    10776 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/h5api/test_dynamic_files.py
--rw-r--r--   0 root         (0) root         (0)     6032 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/h5api/test_static_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.522478 blissdata-0.3.2/blissdata/tests/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-01-23 08:48:08.000000 blissdata-0.3.2/blissdata/tests/redis/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-23 08:48:13.510478 blissdata-0.3.2/blissdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1592 2023-01-23 08:48:13.000000 blissdata-0.3.2/blissdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2109 2023-01-23 08:48:13.000000 blissdata-0.3.2/blissdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-23 08:48:13.000000 blissdata-0.3.2/blissdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-01-23 08:48:13.000000 blissdata-0.3.2/blissdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-01-23 08:48:13.000000 blissdata-0.3.2/blissdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-01-23 08:48:08.000000 blissdata-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      890 2023-01-23 08:48:13.522478 blissdata-0.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       69 2023-01-23 08:48:08.000000 blissdata-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.175657 blissdata-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)     7651 2023-04-19 11:54:32.000000 blissdata-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-04-19 11:54:37.175657 blissdata-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-19 11:54:32.000000 blissdata-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.163657 blissdata-0.3.3/blissdata/
+-rw-r--r--   0 root         (0) root         (0)      288 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.167657 blissdata-0.3.3/blissdata/beacon/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/beacon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/beacon/_base.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/beacon/config.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/beacon/data.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/beacon/files.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.167657 blissdata-0.3.3/blissdata/common/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.167657 blissdata-0.3.3/blissdata/data/
+-rwxr-xr-x   0 root         (0) root         (0)      262 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.167657 blissdata-0.3.3/blissdata/data/events/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/events/channel.py
+-rw-r--r--   0 root         (0) root         (0)    17760 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/events/lima.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/events/node.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/events/scan.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/events/walk.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/expiration.py
+-rw-r--r--   0 root         (0) root         (0)    13578 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/lima_image.py
+-rw-r--r--   0 root         (0) root         (0)    57212 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.171656 blissdata-0.3.3/blissdata/data/nodes/
+-rw-r--r--   0 root         (0) root         (0)      261 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13651 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/channel.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/dataset_collection.py
+-rwxr-xr-x   0 root         (0) root         (0)    14590 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/lima.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/node_ref_channel.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/proposal.py
+-rwxr-xr-x   0 root         (0) root         (0)     7177 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/scan.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/nodes/scan_group.py
+-rw-r--r--   0 root         (0) root         (0)     7796 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/remote_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    23843 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/data/scan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.171656 blissdata-0.3.3/blissdata/h5api/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/abstract.py
+-rw-r--r--   0 root         (0) root         (0)     4363 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/dynamic_hdf5.py
+-rw-r--r--   0 root         (0) root         (0)      757 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/file_arguments.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/static_hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.171656 blissdata-0.3.3/blissdata/h5api/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/utils/bliss.py
+-rw-r--r--   0 root         (0) root         (0)     7399 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/utils/hdf5.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/utils/hdf5_retry.py
+-rw-r--r--   0 root         (0) root         (0)     8634 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/utils/lima.py
+-rw-r--r--   0 root         (0) root         (0)      423 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/h5api/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.175657 blissdata-0.3.3/blissdata/redis/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13145 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/redis/caching.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/redis/connection.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/redis/manager.py
+-rw-r--r--   0 root         (0) root         (0)    32406 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/redis/proxy.py
+-rw-r--r--   0 root         (0) root         (0)      819 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/redis/scripting.py
+-rw-r--r--   0 root         (0) root         (0)    33542 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/settings.py
+-rw-r--r--   0 root         (0) root         (0)    29324 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/streaming.py
+-rw-r--r--   0 root         (0) root         (0)     9214 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/streaming_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.175657 blissdata-0.3.3/blissdata/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.175657 blissdata-0.3.3/blissdata/tests/beacon/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/beacon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/beacon/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/beacon/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/beacon/test_files.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.175657 blissdata-0.3.3/blissdata/tests/h5api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/h5api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/h5api/scanner.py
+-rw-r--r--   0 root         (0) root         (0)    10776 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/h5api/test_dynamic_files.py
+-rw-r--r--   0 root         (0) root         (0)     6032 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/h5api/test_static_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.175657 blissdata-0.3.3/blissdata/tests/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-19 11:54:32.000000 blissdata-0.3.3/blissdata/tests/redis/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 11:54:37.163657 blissdata-0.3.3/blissdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-04-19 11:54:37.000000 blissdata-0.3.3/blissdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-04-19 11:54:37.000000 blissdata-0.3.3/blissdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 11:54:37.000000 blissdata-0.3.3/blissdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2023-04-19 11:54:37.000000 blissdata-0.3.3/blissdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 11:54:37.000000 blissdata-0.3.3/blissdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-19 11:54:32.000000 blissdata-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-19 11:54:37.175657 blissdata-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-19 11:54:32.000000 blissdata-0.3.3/setup.py
```

### Comparing `blissdata-0.3.2/LICENSE` & `blissdata-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/PKG-INFO` & `blissdata-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissdata
-Version: 0.3.2
+Version: 0.3.3
 Summary: Bliss data streaming client
 Home-page: https://gitlab.esrf.fr/bliss/bliss/-/tree/master/blissdata
 Author: BCU (ESRF)
 License: LGPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blissdata-0.3.2/README.md` & `blissdata-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/beacon/_base.py` & `blissdata-0.3.3/blissdata/beacon/_base.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/beacon/config.py` & `blissdata-0.3.3/blissdata/beacon/config.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/beacon/data.py` & `blissdata-0.3.3/blissdata/beacon/data.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/beacon/files.py` & `blissdata-0.3.3/blissdata/beacon/files.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/client.py` & `blissdata-0.3.3/blissdata/client.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/common/utils.py` & `blissdata-0.3.3/blissdata/common/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This file is part of the bliss project
 #
 # Copyright (c) 2015-2023 Beamline Control Unit, ESRF
 # Distributed under the GNU LGPLv3. See LICENSE for more info.
 
 import fnmatch
+import re
 from collections.abc import Mapping
 
 
 class UndefinedType:
     __slots__ = []
 
 
@@ -137,7 +138,22 @@
 
             if matching_names:
                 break
 
         matches[pat] = matching_names
 
     return matches
+
+
+def natural_sort(words):
+    def convert(text):
+        return int(text) if text.isdigit() else text.lower()
+
+    def alphanum_key(key):
+        return [
+            convert(c)
+            for c in re.split(
+                "([0-9]+)", key.decode() if isinstance(key, bytes) else key
+            )
+        ]
+
+    return sorted(words, key=alphanum_key)
```

### Comparing `blissdata-0.3.2/blissdata/data/events/__init__.py` & `blissdata-0.3.3/blissdata/data/events/__init__.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/events/channel.py` & `blissdata-0.3.3/blissdata/data/events/channel.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/events/lima.py` & `blissdata-0.3.3/blissdata/data/events/lima.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/events/node.py` & `blissdata-0.3.3/blissdata/data/events/node.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/events/scan.py` & `blissdata-0.3.3/blissdata/data/events/scan.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/events/walk.py` & `blissdata-0.3.3/blissdata/data/events/walk.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/expiration.py` & `blissdata-0.3.3/blissdata/data/expiration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 from blissdata.client import get_redis_proxy
 
-_DATA_EXPIRATION_TIME = 600  # 5 minutes
+_DATA_EXPIRATION_TIME = 600  # 10 minutes
 _PARENT_EXPIRATION_TIME = 24 * 3600  # 1 day
 
 
 def set_default_expiration_time(seconds: int, data: Optional[bool] = False):
     if data:
         global _DATA_EXPIRATION_TIME
         _DATA_EXPIRATION_TIME = seconds
```

### Comparing `blissdata-0.3.2/blissdata/data/lima_image.py` & `blissdata-0.3.3/blissdata/data/lima_image.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/node.py` & `blissdata-0.3.3/blissdata/data/node.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/nodes/channel.py` & `blissdata-0.3.3/blissdata/data/nodes/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from blissdata.data.events import EventData, ChannelDataEvent
 
 
 # Default length of published channels
 CHANNEL_MAX_LEN = 2048
 
 
+class RedisDataExpiredError(Exception):
+    pass
+
+
 class _ChannelDataNodeBase(DataNode):
     _NODE_TYPE = NotImplemented
 
     def __init__(self, name, **kwargs):
         super().__init__(self._NODE_TYPE, name, **kwargs)
         self._queue = self._create_stream("data", maxlen=CHANNEL_MAX_LEN)
         self._register_stream_priority(f"{self.db_name}_data", 2)
```

### Comparing `blissdata-0.3.2/blissdata/data/nodes/dataset.py` & `blissdata-0.3.3/blissdata/data/nodes/dataset.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/nodes/lima.py` & `blissdata-0.3.3/blissdata/data/nodes/lima.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/nodes/node_ref_channel.py` & `blissdata-0.3.3/blissdata/data/nodes/node_ref_channel.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/nodes/scan.py` & `blissdata-0.3.3/blissdata/data/nodes/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # This file is part of the bliss project
 #
 # Copyright (c) 2015-2023 Beamline Control Unit, ESRF
 # Distributed under the GNU LGPLv3. See LICENSE for more info.
 
 from blissdata.data.node import DataNodeContainer
-from blissdata.data.nodes.channel import ChannelDataNode
+from blissdata.data.nodes.channel import ChannelDataNode, RedisDataExpiredError
 from blissdata.data.nodes.lima import LimaImageChannelDataNode
 from blissdata.streaming_events import StreamEvent
 from blissdata.data.events import (
     Event,
     EventType,
     EventData,
     EndScanEvent,
@@ -175,10 +175,18 @@
                 chan.db_connection = saved_db_connection
 
     result = pipeline.execute()
 
     for i, (channel_name, get_data_func) in enumerate(
         scan_channel_get_data_func.items()
     ):
+        if not result[i]:
+            raise RedisDataExpiredError("Redis data channel expired.")
+
+        if result[i][0][0] != b"1-0":  # first event is 1-0, not 0-0
+            raise RedisDataExpiredError(
+                f"Redis data channel {channel_name} have been trimmed out."
+            )
+
         yield channel_name, get_data_func(result[i])
     for channel_name, view in scan_image_get_view.items():
         yield channel_name, view
```

### Comparing `blissdata-0.3.2/blissdata/data/remote_node.py` & `blissdata-0.3.3/blissdata/data/remote_node.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/data/scan.py` & `blissdata-0.3.3/blissdata/data/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,34 @@
 # Copyright (c) 2015-2023 Beamline Control Unit, ESRF
 # Distributed under the GNU LGPLv3. See LICENSE for more info.
 
 
 import sys
 import numpy
 import gevent
+import gevent.event
 import typing
 import warnings
 import contextlib
 
 from typing import Dict
 
 from blissdata.data.nodes.channel import ChannelDataNode
 from blissdata.data.node import get_or_create_node
 from blissdata.data.events import Event
 from blissdata.data.events import EventType
 from blissdata.streaming import DataStreamReaderStopHandler
 
 
+def get_data(scan):
+    # keep get_data() wrapper for scripts backward compatibility until the
+    # new data API provide the same functionality (expected for Bliss 1.12)
+    return scan.get_data()
+
+
 def get_counter_names(scan):
     """
     Return a list of counter names
     """
     return [
         node.name for node in scan.nodes.values() if isinstance(node, ChannelDataNode)
     ]
```

### Comparing `blissdata-0.3.2/blissdata/h5api/abstract.py` & `blissdata-0.3.3/blissdata/h5api/abstract.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/h5api/dynamic_hdf5.py` & `blissdata-0.3.3/blissdata/h5api/dynamic_hdf5.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/h5api/file_arguments.py` & `blissdata-0.3.3/blissdata/h5api/file_arguments.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/h5api/static_hdf5.py` & `blissdata-0.3.3/blissdata/h5api/static_hdf5.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/h5api/utils/bliss.py` & `blissdata-0.3.3/blissdata/h5api/utils/bliss.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/h5api/utils/hdf5.py` & `blissdata-0.3.3/blissdata/h5api/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/h5api/utils/hdf5_retry.py` & `blissdata-0.3.3/blissdata/h5api/utils/hdf5_retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def ignore_retry_timeout(method: Callable) -> Callable:
     if inspect.isgeneratorfunction(method):
 
         @wraps(method)
         def wrapper(self, *args, **kw):
             try:
-                yield from method(self, *args, *kw)
+                yield from method(self, *args, **kw)
             except RetryTimeoutError:
                 pass
 
     else:
 
         @wraps(method)
         def wrapper(self, *args, **kw):
```

### Comparing `blissdata-0.3.2/blissdata/h5api/utils/lima.py` & `blissdata-0.3.3/blissdata/h5api/utils/lima.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/redis/__init__.py` & `blissdata-0.3.3/blissdata/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/redis/caching.py` & `blissdata-0.3.3/blissdata/redis/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Client-side Redis cache with an invalidation connection.
 """
 
 import os
 import gevent
 import gevent.event
+import gevent.select
 from functools import wraps
 from contextlib import ExitStack, contextmanager
 from collections.abc import MutableMapping
 import redis.exceptions
 
 
 class RedisCacheError(RuntimeError):
```

### Comparing `blissdata-0.3.2/blissdata/redis/connection.py` & `blissdata-0.3.3/blissdata/redis/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     proxy = pool.create_proxy()
 
 These proxies are also greenlet-safe. You will have one cache per pool.
 """
 
 import os
 import gevent
+import gevent.lock
 import socket
 import redis
 
 from blissdata.redis import proxy as redis_proxy
 
 
 class RedisDbConnectionPool(redis.ConnectionPool):
```

### Comparing `blissdata-0.3.2/blissdata/redis/manager.py` & `blissdata-0.3.3/blissdata/redis/manager.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/redis/proxy.py` & `blissdata-0.3.3/blissdata/redis/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import fnmatch
 import time
 from functools import wraps
 from collections.abc import MutableMapping
 from collections import Counter
 from contextlib import contextmanager
 import gevent
+import gevent.event
+import gevent.lock
 import redis
 import redis.client
 
 from blissdata.redis.caching import RedisCacheError
 from blissdata.redis.caching import RedisCache
 from blissdata.common.utils import grouped
```

### Comparing `blissdata-0.3.2/blissdata/redis/scripting.py` & `blissdata-0.3.3/blissdata/redis/scripting.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/settings.py` & `blissdata-0.3.3/blissdata/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from functools import wraps
 import weakref
 import pickle
 import logging
 import numpy
 from blissdata.client import get_redis_proxy
 from blissdata.redis.scripting import register_script, evaluate_script
-from blissdata.common.utils import Undefined
+from blissdata.common.utils import Undefined, natural_sort
 
 logger = logging.getLogger(__name__)
 
 
 def auto_coerce(s):
     """Convert variable to a new type from the str representation"""
     if s is None:
@@ -756,14 +756,28 @@
         super().__init__(*args, **kw)
         register_script(
             self.connection,
             "orderedhashsetting_helper_script",
             orderedhashsetting_helper_script,
         )
 
+        # check if this ordered hash is built from an existing hash setting
+        if self.connection.exists(self.name) and not self.connection.exists(
+            self._name_order
+        ):
+            if self.connection.type(self.name) == b"hash":
+                # we can provide a default order (alphabetical), to ensure an ordered hash
+                # can be built on top of an existing hash ; this is to preserve
+                # settings coherency in case of type "upgrade" (like when Lima ROIs
+                # have been ordered from "normal" hashes)
+                sorted_keys = natural_sort(self.connection.hkeys(self.name))
+                self.connection.zadd(
+                    self._name_order, {v: k for k, v in enumerate(sorted_keys)}
+                )
+
     @property
     def _name_order(self):
         return self._name + ":creation_order"
 
     def ttl(self, value=-1):
         hash_ttl = super().ttl(value)
         ttl_func(self.connection, self._name_order, value)
```

### Comparing `blissdata-0.3.2/blissdata/streaming.py` & `blissdata-0.3.3/blissdata/streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # This file is part of the bliss project
 #
 # Copyright (c) 2015-2023 Beamline Control Unit, ESRF
 # Distributed under the GNU LGPLv3. See LICENSE for more info.
 
 import sys
 import gevent
+import gevent.event
+import gevent.queue
 import uuid
 import enum
 import fnmatch
 import time
 import logging
 from contextlib import contextmanager
 from blissdata.settings import BaseSetting, pipeline
```

### Comparing `blissdata-0.3.2/blissdata/streaming_events.py` & `blissdata-0.3.3/blissdata/streaming_events.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/beacon/test_config.py` & `blissdata-0.3.3/blissdata/tests/beacon/test_config.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/beacon/test_data.py` & `blissdata-0.3.3/blissdata/tests/beacon/test_data.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/beacon/test_files.py` & `blissdata-0.3.3/blissdata/tests/beacon/test_files.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/h5api/scanner.py` & `blissdata-0.3.3/blissdata/tests/h5api/scanner.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/h5api/test_dynamic_files.py` & `blissdata-0.3.3/blissdata/tests/h5api/test_dynamic_files.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/h5api/test_static_files.py` & `blissdata-0.3.3/blissdata/tests/h5api/test_static_files.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata/tests/redis/manager.py` & `blissdata-0.3.3/blissdata/tests/redis/manager.py`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/blissdata.egg-info/PKG-INFO` & `blissdata-0.3.3/blissdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissdata
-Version: 0.3.2
+Version: 0.3.3
 Summary: Bliss data streaming client
 Home-page: https://gitlab.esrf.fr/bliss/bliss/-/tree/master/blissdata
 Author: BCU (ESRF)
 License: LGPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blissdata-0.3.2/blissdata.egg-info/SOURCES.txt` & `blissdata-0.3.3/blissdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blissdata-0.3.2/setup.cfg` & `blissdata-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 tango = 
 	pytango >=9.3.1
 test = 
 	pytest >=7
 	pytest-mock
 dev = 
 	%(test)s
-	black >=22
+	black ==22.3
 	flake8 >=4
 beacon = 
 	ruamel.yaml
 
 [flake8]
 ignore = E501, E203, W503
 max-line-length = 88
```


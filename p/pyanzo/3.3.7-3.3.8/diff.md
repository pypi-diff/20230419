# Comparing `tmp/pyanzo-3.3.7.tar.gz` & `tmp/pyanzo-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyanzo-3.3.7.tar", last modified: Tue Jan 31 22:14:13 2023, max compression
+gzip compressed data, was "pyanzo-3.3.8.tar", last modified: Wed Apr 19 19:02:24 2023, max compression
```

## Comparing `pyanzo-3.3.7.tar` & `pyanzo-3.3.8.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/
--rw-r--r--   0 silverfang   (501) staff       (20)      812 2023-01-31 22:14:13.000000 pyanzo-3.3.7/PKG-INFO
--rw-r--r--   0 silverfang   (501) staff       (20)      135 2022-08-19 01:48:08.000000 pyanzo-3.3.7/LICENSE
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/
--rw-r--r--   0 silverfang   (501) staff       (20)      812 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/PKG-INFO
--rw-r--r--   0 silverfang   (501) staff       (20)        1 2020-06-30 21:36:32.000000 pyanzo-3.3.7/pyanzo.egg-info/not-zip-safe
--rw-r--r--   0 silverfang   (501) staff       (20)     2715 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/SOURCES.txt
--rw-r--r--   0 silverfang   (501) staff       (20)       20 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/entry_points.txt
--rw-r--r--   0 silverfang   (501) staff       (20)       48 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/requires.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        7 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/top_level.txt
--rw-r--r--   0 silverfang   (501) staff       (20)        1 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo.egg-info/dependency_links.txt
--rw-r--r--   0 silverfang   (501) staff       (20)      897 2021-01-06 22:11:36.000000 pyanzo-3.3.7/HISTORY.md
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/pyanzo/
--rw-r--r--   0 silverfang   (501) staff       (20)     6434 2022-08-19 01:48:08.000000 pyanzo-3.3.7/pyanzo/query_result.py
--rw-r--r--   0 silverfang   (501) staff       (20)    16652 2022-08-19 01:48:08.000000 pyanzo-3.3.7/pyanzo/anzo_request.py
--rw-r--r--   0 silverfang   (501) staff       (20)    19078 2022-10-18 03:46:43.000000 pyanzo-3.3.7/pyanzo/anzo_client.py
--rw-r--r--   0 silverfang   (501) staff       (20)    21258 2022-10-18 03:11:43.000000 pyanzo-3.3.7/pyanzo/graphmart_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)     1061 2022-08-19 01:48:08.000000 pyanzo-3.3.7/pyanzo/__init__.py
--rw-r--r--   0 silverfang   (501) staff       (20)    15951 2023-01-31 22:06:39.000000 pyanzo-3.3.7/pyanzo/orchestration_wrapper.py
--rw-r--r--   0 silverfang   (501) staff       (20)     8960 2022-08-19 01:48:08.000000 pyanzo-3.3.7/pyanzo/lds_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)    18589 2023-01-31 22:13:54.000000 pyanzo-3.3.7/pyanzo/quad_store.py
--rw-r--r--   0 silverfang   (501) staff       (20)     1998 2022-08-19 01:48:08.000000 pyanzo-3.3.7/pyanzo/uris.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/
--rw-r--r--   0 silverfang   (501) staff       (20)    16440 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_quad_store.py
--rw-r--r--   0 silverfang   (501) staff       (20)    17326 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_basic.py
--rw-r--r--   0 silverfang   (501) staff       (20)      930 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_common.py
--rw-r--r--   0 silverfang   (501) staff       (20)     3499 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_auth.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6676 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_advanced.py
--rw-r--r--   0 silverfang   (501) staff       (20)     2869 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_execute_semantic_service.py
--rw-r--r--   0 silverfang   (501) staff       (20)     4695 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_orchestration_wrapper.py
--rw-r--r--   0 silverfang   (501) staff       (20)        0 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/__init__.py
--rw-r--r--   0 silverfang   (501) staff       (20)     9066 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_query_graphmart.py
--rw-r--r--   0 silverfang   (501) staff       (20)     2066 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_query_system_tables.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6484 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_lds_manager.py
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/
--rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.7/tests/test_assets/sample.n3
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/trig/
--rwxr-xr-x   0 silverfang   (501) staff       (20)    23062 2022-02-14 16:18:37.000000 pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)     3221 2022-02-14 16:18:37.000000 pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig
--rw-r--r--   0 silverfang   (501) staff       (20)     3452 2022-02-14 16:18:37.000000 pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_AZG.trig
--rwxr-xr-x   0 silverfang   (501) staff       (20)      855 2020-11-07 03:54:19.000000 pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_Graphmart_export.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/
--rw-r--r--   0 silverfang   (501) staff       (20)     3483 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/flds.trig
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/
--rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.part-00000.gz.ttl.gz.crc
--rw-r--r--   0 silverfang   (501) staff       (20)      339 2020-11-07 03:54:19.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/part-00000.gz.ttl.gz
--rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..lsdir.crc
--rw-r--r--   0 silverfang   (501) staff       (20)       39 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.lsdir
--rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..jobMetadata.crc
--rw-r--r--   0 silverfang   (501) staff       (20)      154 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.jobMetadata
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/onts/
--rw-r--r--   0 silverfang   (501) staff       (20)     3237 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
--rw-r--r--   0 silverfang   (501) staff       (20)       50 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/onts/.ontsdir
--rw-r--r--   0 silverfang   (501) staff       (20)      102 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/.lsdir
--rw-r--r--   0 silverfang   (501) staff       (20)      240 2021-04-21 23:24:42.000000 pyanzo-3.3.7/tests/test_assets/sample.trig
--rw-r--r--   0 silverfang   (501) staff       (20)      493 2021-04-21 23:24:42.000000 pyanzo-3.3.7/tests/test_assets/trig_with_bnodes.trig
--rw-r--r--   0 silverfang   (501) staff       (20)      266 2020-11-07 03:54:19.000000 pyanzo-3.3.7/tests/test_assets/simple_journal_query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)      227 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/malformed_journal_query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)      254 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/malformed_graphmart_query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)      755 2021-04-21 23:24:42.000000 pyanzo-3.3.7/tests/test_assets/sample.json
--rw-r--r--   0 silverfang   (501) staff       (20)      255 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/simple_graphmart_query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)     1094 2021-04-21 23:24:42.000000 pyanzo-3.3.7/tests/test_assets/sample.trix
--rw-r--r--   0 silverfang   (501) staff       (20)    15330 2020-11-07 03:54:19.000000 pyanzo-3.3.7/tests/test_assets/gmart.trig
--rw-r--r--   0 silverfang   (501) staff       (20)      292 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/test_assets/query_test_graphmart.sh
--rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.7/tests/test_assets/sample.ttl
--rw-r--r--   0 silverfang   (501) staff       (20)     2002 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_get.py
--rw-r--r--   0 silverfang   (501) staff       (20)     8032 2022-09-06 00:47:10.000000 pyanzo-3.3.7/tests/test_query_journal.py
--rw-r--r--   0 silverfang   (501) staff       (20)       40 2020-06-30 21:09:10.000000 pyanzo-3.3.7/tests/query.rq
--rw-r--r--   0 silverfang   (501) staff       (20)     8746 2022-10-13 17:19:17.000000 pyanzo-3.3.7/tests/test_graphmart_manager.py
--rw-r--r--   0 silverfang   (501) staff       (20)     4618 2021-01-06 22:11:36.000000 pyanzo-3.3.7/tests/test_update_journal.py
--rw-r--r--   0 silverfang   (501) staff       (20)     5736 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_query_lds.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6146 2022-08-19 01:48:08.000000 pyanzo-3.3.7/tests/test_add_and_remove.py
--rw-r--r--   0 silverfang   (501) staff       (20)      251 2022-10-11 15:10:33.000000 pyanzo-3.3.7/MANIFEST.in
-drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-01-31 22:14:13.000000 pyanzo-3.3.7/docs/
--rw-r--r--   0 silverfang   (501) staff       (20)      304 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/index.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       33 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/contributing.rst
--rw-r--r--   0 silverfang   (501) staff       (20)      607 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/Makefile
--rwxr-xr-x   0 silverfang   (501) staff       (20)     4854 2022-08-17 19:11:17.000000 pyanzo-3.3.7/docs/conf.py
--rw-r--r--   0 silverfang   (501) staff       (20)       55 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/modules.rst
--rw-r--r--   0 silverfang   (501) staff       (20)     1099 2020-11-07 03:54:19.000000 pyanzo-3.3.7/docs/usage.rst
--rw-r--r--   0 silverfang   (501) staff       (20)      768 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/make.bat
--rw-r--r--   0 silverfang   (501) staff       (20)       28 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/history.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       74 2020-11-07 03:54:19.000000 pyanzo-3.3.7/docs/installation.rst
--rw-r--r--   0 silverfang   (501) staff       (20)     1355 2020-06-30 21:09:10.000000 pyanzo-3.3.7/docs/pyanzo.rst
--rw-r--r--   0 silverfang   (501) staff       (20)       26 2021-01-06 22:11:36.000000 pyanzo-3.3.7/docs/readme.rst
--rw-r--r--   0 silverfang   (501) staff       (20)     3145 2022-08-19 01:48:08.000000 pyanzo-3.3.7/README.md
--rw-r--r--   0 silverfang   (501) staff       (20)     1792 2023-01-31 22:14:03.000000 pyanzo-3.3.7/setup.py
--rw-r--r--   0 silverfang   (501) staff       (20)     6548 2022-02-14 16:18:37.000000 pyanzo-3.3.7/CONTRIBUTING.md
--rw-r--r--   0 silverfang   (501) staff       (20)      417 2023-01-31 22:14:13.000000 pyanzo-3.3.7/setup.cfg
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:24.000040 pyanzo-3.3.8/
+-rw-r--r--   0 silverfang   (501) staff       (20)     6548 2022-02-14 16:18:37.000000 pyanzo-3.3.8/CONTRIBUTING.md
+-rw-r--r--   0 silverfang   (501) staff       (20)      897 2021-01-06 22:11:36.000000 pyanzo-3.3.8/HISTORY.md
+-rw-r--r--   0 silverfang   (501) staff       (20)      135 2022-08-19 01:48:08.000000 pyanzo-3.3.8/LICENSE
+-rw-r--r--   0 silverfang   (501) staff       (20)      251 2022-10-11 15:10:33.000000 pyanzo-3.3.8/MANIFEST.in
+-rw-r--r--   0 silverfang   (501) staff       (20)      771 2023-04-19 19:02:24.000347 pyanzo-3.3.8/PKG-INFO
+-rw-r--r--   0 silverfang   (501) staff       (20)     3145 2022-08-19 01:48:08.000000 pyanzo-3.3.8/README.md
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.921843 pyanzo-3.3.8/docs/
+-rw-r--r--   0 silverfang   (501) staff       (20)      607 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/Makefile
+-rwxr-xr-x   0 silverfang   (501) staff       (20)     4854 2022-08-17 19:11:17.000000 pyanzo-3.3.8/docs/conf.py
+-rw-r--r--   0 silverfang   (501) staff       (20)       33 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/contributing.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       28 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/history.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      304 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/index.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       74 2020-11-07 03:54:19.000000 pyanzo-3.3.8/docs/installation.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)      768 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/make.bat
+-rw-r--r--   0 silverfang   (501) staff       (20)       55 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/modules.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)     1355 2020-06-30 21:09:10.000000 pyanzo-3.3.8/docs/pyanzo.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)       26 2021-01-06 22:11:36.000000 pyanzo-3.3.8/docs/readme.rst
+-rw-r--r--   0 silverfang   (501) staff       (20)     1099 2020-11-07 03:54:19.000000 pyanzo-3.3.8/docs/usage.rst
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.931159 pyanzo-3.3.8/pyanzo/
+-rw-r--r--   0 silverfang   (501) staff       (20)     1061 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/__init__.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    19006 2023-04-19 16:08:21.000000 pyanzo-3.3.8/pyanzo/anzo_client.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    17025 2023-04-19 19:01:50.000000 pyanzo-3.3.8/pyanzo/anzo_request.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     1048 2023-03-16 20:38:35.000000 pyanzo-3.3.8/pyanzo/api_properties.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    11493 2023-03-16 18:26:47.000000 pyanzo-3.3.8/pyanzo/api_request.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    21258 2022-10-18 03:11:43.000000 pyanzo-3.3.8/pyanzo/graphmart_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     8960 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/lds_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    15951 2023-01-31 22:06:39.000000 pyanzo-3.3.8/pyanzo/orchestration_wrapper.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    18589 2023-01-31 22:13:54.000000 pyanzo-3.3.8/pyanzo/quad_store.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     6434 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/query_result.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     1998 2022-08-19 01:48:08.000000 pyanzo-3.3.8/pyanzo/uris.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.934708 pyanzo-3.3.8/pyanzo.egg-info/
+-rw-r--r--   0 silverfang   (501) staff       (20)      771 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/PKG-INFO
+-rw-r--r--   0 silverfang   (501) staff       (20)     2729 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/SOURCES.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        1 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/dependency_links.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        1 2020-06-30 21:36:32.000000 pyanzo-3.3.8/pyanzo.egg-info/not-zip-safe
+-rw-r--r--   0 silverfang   (501) staff       (20)       48 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/requires.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)        7 2023-04-19 19:02:23.000000 pyanzo-3.3.8/pyanzo.egg-info/top_level.txt
+-rw-r--r--   0 silverfang   (501) staff       (20)      417 2023-04-19 19:02:24.001570 pyanzo-3.3.8/setup.cfg
+-rw-r--r--   0 silverfang   (501) staff       (20)     1792 2023-04-19 18:55:10.000000 pyanzo-3.3.8/setup.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.962310 pyanzo-3.3.8/tests/
+-rw-r--r--   0 silverfang   (501) staff       (20)        0 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/__init__.py
+-rw-r--r--   0 silverfang   (501) staff       (20)       40 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/query.rq
+-rw-r--r--   0 silverfang   (501) staff       (20)     6146 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_add_and_remove.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     6676 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_advanced.py
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.972317 pyanzo-3.3.8/tests/test_assets/
+-rw-r--r--   0 silverfang   (501) staff       (20)    15330 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/gmart.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)      254 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/malformed_graphmart_query.rq
+-rw-r--r--   0 silverfang   (501) staff       (20)      227 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/malformed_journal_query.rq
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.974183 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/
+-rw-r--r--   0 silverfang   (501) staff       (20)      102 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/.lsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3483 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/flds.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.975820 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/
+-rw-r--r--   0 silverfang   (501) staff       (20)       50 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/.ontsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)     3237 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.911036 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.911136 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.992402 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/
+-rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..jobMetadata.crc
+-rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/..lsdir.crc
+-rw-r--r--   0 silverfang   (501) staff       (20)      154 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.jobMetadata
+-rw-r--r--   0 silverfang   (501) staff       (20)       39 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.lsdir
+-rw-r--r--   0 silverfang   (501) staff       (20)       12 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/.part-00000.gz.ttl.gz.crc
+-rw-r--r--   0 silverfang   (501) staff       (20)      339 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/rdf.ttl.gz/Loaddata_Person_734ff.ttl.gz/20200502131201.ttl.gz/part-00000.gz.ttl.gz
+-rw-r--r--   0 silverfang   (501) staff       (20)      292 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/query_test_graphmart.sh
+-rw-r--r--   0 silverfang   (501) staff       (20)      755 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.json
+-rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.n3
+-rw-r--r--   0 silverfang   (501) staff       (20)      240 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)     1094 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.trix
+-rw-r--r--   0 silverfang   (501) staff       (20)      194 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/sample.ttl
+-rw-r--r--   0 silverfang   (501) staff       (20)      255 2020-06-30 21:09:10.000000 pyanzo-3.3.8/tests/test_assets/simple_graphmart_query.rq
+-rw-r--r--   0 silverfang   (501) staff       (20)      266 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/simple_journal_query.rq
+drwxr-xr-x   0 silverfang   (501) staff       (20)        0 2023-04-19 19:02:23.999210 pyanzo-3.3.8/tests/test_assets/trig/
+-rw-r--r--   0 silverfang   (501) staff       (20)     3452 2022-02-14 16:18:37.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_AZG.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)      855 2020-11-07 03:54:19.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_export.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)    23062 2022-02-14 16:18:37.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig
+-rwxr-xr-x   0 silverfang   (501) staff       (20)     3221 2022-02-14 16:18:37.000000 pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)      493 2021-04-21 23:24:42.000000 pyanzo-3.3.8/tests/test_assets/trig_with_bnodes.trig
+-rw-r--r--   0 silverfang   (501) staff       (20)     3499 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_auth.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    17326 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_basic.py
+-rw-r--r--   0 silverfang   (501) staff       (20)      930 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_common.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     2869 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_execute_semantic_service.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     2002 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_get.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     8746 2022-10-13 17:19:17.000000 pyanzo-3.3.8/tests/test_graphmart_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     6484 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_lds_manager.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     4695 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_orchestration_wrapper.py
+-rw-r--r--   0 silverfang   (501) staff       (20)    16440 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_quad_store.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     9066 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_query_graphmart.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     8032 2022-09-06 00:47:10.000000 pyanzo-3.3.8/tests/test_query_journal.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     5736 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_query_lds.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     2066 2022-08-19 01:48:08.000000 pyanzo-3.3.8/tests/test_query_system_tables.py
+-rw-r--r--   0 silverfang   (501) staff       (20)     4618 2021-01-06 22:11:36.000000 pyanzo-3.3.8/tests/test_update_journal.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyanzo-3.3.7/PKG-INFO` & `pyanzo-3.3.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyanzo
-Version: 3.3.7
+Version: 3.3.8
 Summary: PyAnzo is a library for interacting with Anzo
-Home-page: UNKNOWN
+Home-page: 
 Author: Tommy Fang, William Ades, Curtis Galione, Andrew Parisi, Alex Ledger
 Author-email: info@cambridgesemantics.com
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: pyanzo
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `pyanzo-3.3.7/pyanzo.egg-info/PKG-INFO` & `pyanzo-3.3.8/pyanzo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyanzo
-Version: 3.3.7
+Version: 3.3.8
 Summary: PyAnzo is a library for interacting with Anzo
-Home-page: UNKNOWN
+Home-page: 
 Author: Tommy Fang, William Ades, Curtis Galione, Andrew Parisi, Alex Ledger
 Author-email: info@cambridgesemantics.com
-License: UNKNOWN
-Description: UNKNOWN
 Keywords: pyanzo
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
```

### Comparing `pyanzo-3.3.7/pyanzo.egg-info/SOURCES.txt` & `pyanzo-3.3.8/pyanzo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 docs/modules.rst
 docs/pyanzo.rst
 docs/readme.rst
 docs/usage.rst
 pyanzo/__init__.py
 pyanzo/anzo_client.py
 pyanzo/anzo_request.py
+pyanzo/api_properties.py
+pyanzo/api_request.py
 pyanzo/graphmart_manager.py
 pyanzo/lds_manager.py
 pyanzo/orchestration_wrapper.py
 pyanzo/quad_store.py
 pyanzo/query_result.py
 pyanzo/uris.py
 pyanzo.egg-info/PKG-INFO
 pyanzo.egg-info/SOURCES.txt
 pyanzo.egg-info/dependency_links.txt
-pyanzo.egg-info/entry_points.txt
 pyanzo.egg-info/not-zip-safe
 pyanzo.egg-info/requires.txt
 pyanzo.egg-info/top_level.txt
 tests/__init__.py
 tests/query.rq
 tests/test_add_and_remove.py
 tests/test_advanced.py
```

### Comparing `pyanzo-3.3.7/HISTORY.md` & `pyanzo-3.3.8/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/query_result.py` & `pyanzo-3.3.8/pyanzo/query_result.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/anzo_request.py` & `pyanzo-3.3.8/pyanzo/anzo_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import os
 import requests
 import json
 
 # /*******************************************************************************
 #  * Copyright (c) 2019 - 2022 Cambridge Semantics Incorporated.
 #  * All rights reserved.
-#  * 
+#  *
 #  * Contributors:
 #  *     Cambridge Semantics Incorporated
 #  *******************************************************************************/
 
+
 class AnzoRequest:
     """Encodes a request against Anzo and supports executing the request.
 
     Instances of AnzoRequest are typically constructed with an
     AnzoRequestBuilder. When a request is executed, a RunTimeError may be
     raised depending on the status code of the HTTP response.
 
@@ -26,20 +27,16 @@
         headers: The HTTP headers included in the request
         data: The body of the HTTP request
         timeout_seconds: Timeout for the request in seconds
     """
 
     COOKIE_KEY = "Cookie"
 
-    def __init__(self, url: str,
-                 username: str,
-                 password: str,
-                 auth_token: str,
-                 headers: Dict[str, Any],
-                 data: Any,
+    def __init__(self, url: str, username: str, password: str, auth_token: str,
+                 headers: Dict[str, Any], data: Any,
                  timeout_seconds: float) -> None:
         self.url = url
         self.username = username
         self.password = password
         self.auth_token = auth_token
         self.headers = headers
         self.data = data
@@ -60,49 +57,47 @@
             if self.username and self.password:
                 authorization = (self.username, self.password)
             else:
                 authorization = ("", "")
 
             if self.auth_token:
                 self.headers[self.COOKIE_KEY] = self.auth_token
-
-            response = requests.post(
-                self.url,
-                headers=self.headers,
-                data=self.data,
-                auth=authorization,
-                verify=False,
-                timeout=self.timeout_seconds
-            )
+            try:
+                verify = self.ssl_verify()
+            except OSError as err:
+                print("Invalid cert path provided, setting verify=False")
+                print(err)
+                verify = False
+
+            response = requests.post(self.url,
+                                     headers=self.headers,
+                                     data=self.data,
+                                     auth=authorization,
+                                     verify=verify,
+                                     timeout=self.timeout_seconds)
 
         except requests.exceptions.ReadTimeout:
-            msg = (
-                f"Request timed out with the timeout set to "
-                f"{self.timeout_seconds} seconds"
-            )
+            msg = (f"Request timed out with the timeout set to "
+                   f"{self.timeout_seconds} seconds")
             raise TimeoutError(msg) from None
         except Exception as e:
             raise RuntimeError from e
 
         if response.status_code > 299:
-            error = (
-                f"Response from {self.url} returned with "
-                f"non-success status code {response.status_code} "
-                f"and response text: {response.text}"
-            )
+            error = (f"Response from {self.url} returned with "
+                     f"non-success status code {response.status_code} "
+                     f"and response text: {response.text}")
 
             raise RuntimeError(error)
         return response.text
 
     def __str__(self) -> str:
-        return (
-            f"<AnzoRequest url='{self.url}, "
-            f"username='{self.username}', "
-            f"password='{self.password}'>"
-        )
+        return (f"<AnzoRequest url='{self.url}, "
+                f"username='{self.username}', "
+                f"password='{self.password}'>")
 
 
 class AnzoRequestBuilder:
     """Builds an AnzoRequest for executing a request against Anzo.
 
     Builds an AnzoRequest step-by-step. Once a request is fully specified,
     build() returns an AnzoRequest object which can be executed.
@@ -257,23 +252,23 @@
             raise RuntimeError("Query Filepaths must end in '.rq'")
 
         with open(query_file, 'r') as query_file_handle:
             query_string = query_file_handle.read()
             self.payload_dict[self.PAYLOAD_UPDATE_KEY] = query_string
         self.payload_dict[self.PAYLOAD_FORMAT_KEY] = self.TEXT_JSON_FORMAT
 
-    def with_graphmart(self, graphmart_uri: str,
+    def with_graphmart(self,
+                       graphmart_uri: str,
                        named_graphs: List[str] = None) -> None:
         """Adds the graphmart postfix and uri to the AnzoRequestBuilder.
         """
 
         encoded_graphmart_uri = quote(graphmart_uri, safe='')
         self.url_postfix = (
-            f"{self.GRAPHMART_QUERY_POSTFIX}/{encoded_graphmart_uri}"
-        )
+            f"{self.GRAPHMART_QUERY_POSTFIX}/{encoded_graphmart_uri}")
 
         if named_graphs:
             self.payload_dict[self.DEFAULT_GRAPH_KEY] = named_graphs
             self.payload_dict[self.NAMED_GRAPH_KEY] = named_graphs
 
     def with_query_journal(self, named_graphs: List[str] = None) -> None:
         """Adds the journal postfix to the AnzoRequestBuilder and sets up
@@ -313,15 +308,16 @@
         # https://stackoverflow.com/questions/23384230/how-to-post-multiple-value-with-same-key-in-python-requests  # noqa
         # for more info.
 
         if named_graphs:
             self.payload_dict[self.USING_GRAPH_KEY] = named_graphs
             self.payload_dict[self.USING_NAMED_GRAPH_KEY] = named_graphs
 
-    def with_lds_cat_entry(self, lds_cat_entry: str,
+    def with_lds_cat_entry(self,
+                           lds_cat_entry: str,
                            named_graphs: List[str] = None) -> None:
         """Adds the lds postfix and uri to the AnzoRequestBuilder.
 
         Raises:
             RuntimeError: If the postfix has already been set.
         """
 
@@ -329,16 +325,15 @@
         encoded_lds_cat_entry = quote(lds_cat_entry, safe='')
         self.url_postfix = f'{self.LDS_QUERY_POSTFIX}/{encoded_lds_cat_entry}'
 
         if named_graphs:
             self.payload_dict[self.DEFAULT_GRAPH_KEY] = named_graphs
             self.payload_dict[self.NAMED_GRAPH_KEY] = named_graphs
 
-    def with_semantic_service(self, service_uri: str,
-                              request: List) -> None:
+    def with_semantic_service(self, service_uri: str, request: List) -> None:
         """Adds the semantic service postfix and payload to the AnzoRequestBuilder.
 
         Raises:
             RuntimeError: If the postfix has already been set.
         """
 
         self._raise_if_url_postfix_is_set()
@@ -391,14 +386,20 @@
         Raises:
             RuntimeError: We currently don't support skipping the cache
                    so if a user tries to do it, an error is raised.
         """
         if skip_cache:
             self.payload_dict[self.SKIP_CACHE] = "true"
 
+    def ssl_verify(self):
+        verify = os.getenv('REQUESTS_CA_BUNDLE', False)
+        if verify and not os.path.isfile(verify):
+            raise IOError("Configured CA Bundle does not exist: " + verify)
+        return verify
+
     def build(self) -> AnzoRequest:
         """
         Combine all of the relevant components to build an AnzoRequest.
 
         Returns:
             A fully developed AnzoRequest object
 
@@ -406,35 +407,28 @@
             ValueError: If any of the relevant components (base_url,
                 url_postfix, username and password or authentication,
                 and payload_dict OR
                 payload_list) of the request are missing.
         """
 
         if not self.base_url:
-            raise ValueError(
-                "Can't build an AnzoRequest because "
-                "self.base_url is missing"
-            )
+            raise ValueError("Can't build an AnzoRequest because "
+                             "self.base_url is missing")
 
         if not self.url_postfix:
-            raise ValueError(
-                "Can't build an AnzoRequest because "
-                "self.url_postfix is missing"
-            )
+            raise ValueError("Can't build an AnzoRequest because "
+                             "self.url_postfix is missing")
 
-        if not((self.username and self.password) or self.auth_token):
+        if not ((self.username and self.password) or self.auth_token):
             raise ValueError(
-                "Can't build AnzoRequest because authorization is missing"
-            )
+                "Can't build AnzoRequest because authorization is missing")
 
         if self.payload_dict and self.payload_list:
-            raise ValueError(
-                "Both self.payload_dict and self.payload_list"
-                "cannot be populated"
-            )
+            raise ValueError("Both self.payload_dict and self.payload_list"
+                             "cannot be populated")
 
         if not self.timeout_seconds:
             raise ValueError("A timeout for the request must be specified")
 
         # Set the data of the request based on the payload.
         # Python-Requests is generous with the type that data can be,
         # so we have two cases:
@@ -446,11 +440,10 @@
         if self.payload_dict:
             data = self.payload_dict
         elif self.payload_list:
             data = json.dumps(self.payload_list)
 
         full_url = f"{self.base_url}/{self.url_postfix}"
 
-        return AnzoRequest(
-            full_url, self.username, self.password, self.auth_token,
-            self.headers, data, self.timeout_seconds
-        )
+        return AnzoRequest(full_url, self.username, self.password,
+                           self.auth_token, self.headers, data,
+                           self.timeout_seconds)
```

### Comparing `pyanzo-3.3.7/pyanzo/anzo_client.py` & `pyanzo-3.3.8/pyanzo/anzo_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional
 from .query_result import QueryResult, QuadStore
 from .anzo_request import AnzoRequestBuilder
 from .uris import ALL_NAMED_GRAPHS_URI
 # /*******************************************************************************
 #  * Copyright (c) 2019 - 2022 Cambridge Semantics Incorporated.
 #  * All rights reserved.
-#  * 
+#  *
 #  * Contributors:
 #  *     Cambridge Semantics Incorporated
 #  *******************************************************************************/
 
 
 class AnzoClient:
     """A class for interacting with an Anzo Server.
@@ -56,15 +56,15 @@
     def __init__(self,
                  server: str,
                  port: str,
                  username: str = "",
                  password: str = "",
                  auth_token: str = "",
                  timeout_seconds: float = 7200.,
-                 ssl_workaround = True) -> None:
+                 ssl_workaround=True) -> None:
         """Constructs an AnzoClient for interacting with an Anzo server.
 
         Args:
             server: The server that Anzo is running on.
             port: The port on which Anzo is listening for HTTPS traffic.
                 Often 443 or 8443.
             username (optional): Username of the user with which
@@ -81,15 +81,15 @@
                 and password or an auth_token, but not both.
         """
 
         self.server = server
         self.port = port
         if ssl_workaround:
             self.__ssl_config()
-        
+
         if username and not password:
             error = "If a username is specified a password also needs to be"
             raise ValueError(error)
 
         if password and not username:
             error = "If password is specified a username also needs to be"
             raise ValueError(error)
@@ -133,22 +133,20 @@
         Returns:
             The result of the query in a QueryResult object.
         """
         # Check if either a query_string or a query_file, but not both.
         if not query_string and not query_file:
             raise ValueError(
                 "Method query_graphmart requires either a query string "
-                "or query file"
-            )
+                "or query file")
 
         if query_string and query_file:
             raise ValueError(
                 "Method query_graphmart received both a query string "
-                "and a query file. Only one should be provided"
-            )
+                "and a query file. Only one should be provided")
 
         if not graphmart:
             raise ValueError("A graphmart is required")
 
         arb = AnzoRequestBuilder()
         arb.with_url(self.server, self.port)
         arb.with_auth(self.username, self.password, self.auth_token)
@@ -162,15 +160,16 @@
 
         arb.with_cache_skipped(skip_cache)
 
         anzo_request = arb.build()
         response_text = anzo_request.execute_request()
         return QueryResult(response_text)
 
-    def query_journal(self, query_string: str = "",
+    def query_journal(self,
+                      query_string: str = "",
                       query_file: str = "",
                       named_graphs: List[str] = None) -> QueryResult:
         """Executes a SPARQL query against the Anzo journal.
 
         Given some query, execute a query against the Anzo journal.
         Either a query_string or query_file must be provided, but not both.
 
@@ -189,22 +188,20 @@
         Returns:
             The result of the query in a QueryResult object.
         """
 
         if not query_string and not query_file:
             raise ValueError(
                 "Method query_journal requires either a query string "
-                "or query file"
-            )
+                "or query file")
 
         if query_string and query_file:
             raise ValueError(
                 "Method query_journal received both a query string "
-                "and a query file. Only one should be provided"
-            )
+                "and a query file. Only one should be provided")
 
         if not named_graphs:
             named_graphs = [ALL_NAMED_GRAPHS_URI]
 
         arb = AnzoRequestBuilder()
         arb.with_url(self.server, self.port)
         arb.with_auth(self.username, self.password, self.auth_token)
@@ -216,15 +213,16 @@
         elif query_file:
             arb.with_query_file(query_file)
 
         anzo_request = arb.build()
         response_text = anzo_request.execute_request()
         return QueryResult(response_text)
 
-    def update_journal(self, query_string: str = "",
+    def update_journal(self,
+                       query_string: str = "",
                        query_file: str = "") -> QueryResult:
         """Executes a SPARQL update query against the Anzo journal.
 
         The query must be conform the UPDATE query spec, as outlined in
         https://www.w3.org/TR/sparql11-update/.
 
         In summary, it's expected the query have one of the following clauses:
@@ -243,22 +241,20 @@
         Returns:
             The result of the query in a QueryResult object.
         """
 
         if not query_string and not query_file:
             raise ValueError(
                 "Method query_journal requires either a query string "
-                "or query file"
-            )
+                "or query file")
 
         if query_string and query_file:
             raise ValueError(
                 "Method query_journal received both a query string "
-                "and a query file. Only one should be provided"
-            )
+                "and a query file. Only one should be provided")
 
         named_graphs = [ALL_NAMED_GRAPHS_URI]
 
         arb = AnzoRequestBuilder()
         arb.with_url(self.server, self.port)
         arb.with_auth(self.username, self.password, self.auth_token)
         arb.with_timeout_seconds(self.timeout_seconds)
@@ -269,18 +265,19 @@
         elif query_file:
             arb.with_update_file(query_file)
 
         anzo_request = arb.build()
         response_text = anzo_request.execute_request()
         return QueryResult(response_text)
 
-    def query_lds(self, lds_cat_entry: str, query_string: str = "",
+    def query_lds(self,
+                  lds_cat_entry: str,
+                  query_string: str = "",
                   query_file: str = "",
-                  named_graphs: Optional[List[str]] = None
-                  ) -> QueryResult:
+                  named_graphs: Optional[List[str]] = None) -> QueryResult:
         """Executes a SPARQL query against an Anzo linked dataset catalog entry
 
         Args:
             lds_cat_entry: URI of the linked dataset catalog entry to query.
                 This URI will encode both the linked dataset and the associated
                 volume datasource.
             query_string: (optional) SPARQL query string to execute against the
@@ -295,18 +292,16 @@
                 ["urn://graph1", "urn://graph2"].
 
         Returns:
             The result of the query in a QueryResult object.
         """
 
         if not query_string and not query_file:
-            raise ValueError(
-                "Method query_lds requires either a query string "
-                "or query file"
-            )
+            raise ValueError("Method query_lds requires either a query string "
+                             "or query file")
 
         arb = AnzoRequestBuilder()
         arb.with_url(self.server, self.port)
         arb.with_auth(self.username, self.password, self.auth_token)
         arb.with_timeout_seconds(self.timeout_seconds)
         arb.with_lds_cat_entry(lds_cat_entry, named_graphs)
 
@@ -315,39 +310,39 @@
         elif query_file:
             arb.with_query_file(query_file)
 
         anzo_request = arb.build()
         response_text = anzo_request.execute_request()
         return QueryResult(response_text)
 
-    def query_system_tables(self,
-                            query_string: str = "",
-                            query_file: str = "",
-                            ) -> QueryResult:
+    def query_system_tables(
+        self,
+        query_string: str = "",
+        query_file: str = "",
+    ) -> QueryResult:
         """Executes a SPARQL query against the anzo system tables
 
         Args:
             query_string: (optional) SPARQL query string to execute against the
                 system tables. Either query_string or query_file must be
                 provided, but not both.
             query_file: (optional) File with SPARQL query to execute against
                 the system tables. Either query_string or query_file must be
                 provided, but not both.
 
         Returns:
             The result of the query in a QueryResult object.
         """
 
-        return self.query_lds(
-            self.SYSTEM_TABLE_LDS_URI, query_string, query_file,
-            named_graphs=[ALL_NAMED_GRAPHS_URI]
-        )
+        return self.query_lds(self.SYSTEM_TABLE_LDS_URI,
+                              query_string,
+                              query_file,
+                              named_graphs=[ALL_NAMED_GRAPHS_URI])
 
-    def execute_semantic_service(self,
-                                 service_uri: str,
+    def execute_semantic_service(self, service_uri: str,
                                  request: QuadStore) -> QuadStore:
         """Executes a Semantic Service on Anzo
 
         Args:
             service_uri: URI of the semantic service
             request: The request payload as a quadstore
 
@@ -360,15 +355,16 @@
         arb.with_auth(self.username, self.password, self.auth_token)
         arb.with_timeout_seconds(self.timeout_seconds)
         arb.with_semantic_service(service_uri, request.as_anzo_json_list())
         anzo_request = arb.build()
         response_json = json.loads(anzo_request.execute_request())
         return QuadStore.from_anzo_json_list(response_json)
 
-    def get(self, named_graph_uri: str,
+    def get(self,
+            named_graph_uri: str,
             include_metadata_graph: bool = False) -> QuadStore:
         """Gets the contents of a named graph and optionally its
         metadata graph
 
         If the graph doesn't exist, then a ValueError is raised.
 
         Args:
@@ -457,15 +453,15 @@
         arb.with_auth(self.username, self.password, self.auth_token)
         arb.with_timeout_seconds(self.timeout_seconds)
         if not quad_store:
             quad_store = QuadStore.from_trig_file(trig_filename)
         arb.with_remove(quad_store.as_anzo_json_list())
         anzo_request = arb.build()
         anzo_request.execute_request()
-        
+
     ## Work around for SSL related DH Key errors
     # ex: [SSL: SSL_NEGATIVE_LENGTH] dh key too small (_ssl.c:600)
     def __ssl_config(self):
         import requests
         try:
             requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += 'HIGH:!DH:!aNULL'
             requests.packages.urllib3.contrib.pyopenssl.DEFAULT_SSL_CIPHER_LIST += 'HIGH:!DH:!aNULL'
```

### Comparing `pyanzo-3.3.7/pyanzo/graphmart_manager.py` & `pyanzo-3.3.8/pyanzo/graphmart_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/__init__.py` & `pyanzo-3.3.8/pyanzo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/orchestration_wrapper.py` & `pyanzo-3.3.8/pyanzo/orchestration_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/lds_manager.py` & `pyanzo-3.3.8/pyanzo/lds_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/quad_store.py` & `pyanzo-3.3.8/pyanzo/quad_store.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/pyanzo/uris.py` & `pyanzo-3.3.8/pyanzo/uris.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_quad_store.py` & `pyanzo-3.3.8/tests/test_quad_store.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_basic.py` & `pyanzo-3.3.8/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_common.py` & `pyanzo-3.3.8/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_auth.py` & `pyanzo-3.3.8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_advanced.py` & `pyanzo-3.3.8/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_execute_semantic_service.py` & `pyanzo-3.3.8/tests/test_execute_semantic_service.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_orchestration_wrapper.py` & `pyanzo-3.3.8/tests/test_orchestration_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_query_graphmart.py` & `pyanzo-3.3.8/tests/test_query_graphmart.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_query_system_tables.py` & `pyanzo-3.3.8/tests/test_query_system_tables.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_lds_manager.py` & `pyanzo-3.3.8/tests/test_lds_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig` & `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_graph.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig` & `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_registry.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_AZG.trig` & `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_AZG.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/trig/PyAnzo_Graphmart_export.trig` & `pyanzo-3.3.8/tests/test_assets/trig/PyAnzo_Graphmart_export.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/flds.trig` & `pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/flds.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig` & `pyanzo-3.3.8/tests/test_assets/pyanzo_test_dataset/onts/PyAnzo_Dictionary_-_PyAnzo_Datasource_-_Auto.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/sample.json` & `pyanzo-3.3.8/tests/test_assets/sample.json`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/sample.trix` & `pyanzo-3.3.8/tests/test_assets/sample.trix`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_assets/gmart.trig` & `pyanzo-3.3.8/tests/test_assets/gmart.trig`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_get.py` & `pyanzo-3.3.8/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_query_journal.py` & `pyanzo-3.3.8/tests/test_query_journal.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_graphmart_manager.py` & `pyanzo-3.3.8/tests/test_graphmart_manager.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_update_journal.py` & `pyanzo-3.3.8/tests/test_update_journal.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_query_lds.py` & `pyanzo-3.3.8/tests/test_query_lds.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/tests/test_add_and_remove.py` & `pyanzo-3.3.8/tests/test_add_and_remove.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/docs/Makefile` & `pyanzo-3.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/docs/conf.py` & `pyanzo-3.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/docs/usage.rst` & `pyanzo-3.3.8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/docs/make.bat` & `pyanzo-3.3.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/docs/pyanzo.rst` & `pyanzo-3.3.8/docs/pyanzo.rst`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/README.md` & `pyanzo-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pyanzo-3.3.7/setup.py` & `pyanzo-3.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     keywords='pyanzo',
     name='pyanzo',
     packages=find_packages(include=['pyanzo', 'pyanzo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='',
-    version='3.3.7',
+    version='3.3.8',
     zip_safe=False,
 )
```

### Comparing `pyanzo-3.3.7/CONTRIBUTING.md` & `pyanzo-3.3.8/CONTRIBUTING.md`

 * *Files identical despite different names*


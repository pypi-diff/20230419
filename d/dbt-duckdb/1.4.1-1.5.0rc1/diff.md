# Comparing `tmp/dbt-duckdb-1.4.1.tar.gz` & `tmp/dbt-duckdb-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-duckdb-1.4.1.tar", last modified: Thu Mar 16 16:10:26 2023, max compression
+gzip compressed data, was "dbt-duckdb-1.5.0rc1.tar", last modified: Wed Apr 19 20:36:09 2023, max compression
```

## Comparing `dbt-duckdb-1.4.1.tar` & `dbt-duckdb-1.5.0rc1.tar`

### file list

```diff
@@ -1,47 +1,57 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.250530 dbt-duckdb-1.4.1/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)    13048 2023-03-16 16:10:26.250351 dbt-duckdb-1.4.1/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)    12744 2023-03-16 16:10:09.000000 dbt-duckdb-1.4.1/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.244083 dbt-duckdb-1.4.1/dbt/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.244489 dbt-duckdb-1.4.1/dbt/adapters/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/adapters/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.245894 dbt-duckdb-1.4.1/dbt/adapters/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)      407 2023-02-04 17:38:18.000000 dbt-duckdb-1.4.1/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       18 2023-03-16 16:10:09.000000 dbt-duckdb-1.4.1/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 jwills     (501) staff       (20)    10207 2023-03-14 04:05:32.000000 dbt-duckdb-1.4.1/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-10 17:41:01.000000 dbt-duckdb-1.4.1/dbt/adapters/duckdb/glue.py
--rw-r--r--   0 jwills     (501) staff       (20)     8219 2023-03-14 04:05:32.000000 dbt-duckdb-1.4.1/dbt/adapters/duckdb/impl.py
--rw-r--r--   0 jwills     (501) staff       (20)     2182 2023-03-10 17:41:01.000000 dbt-duckdb-1.4.1/dbt/adapters/duckdb/relation.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.246142 dbt-duckdb-1.4.1/dbt/include/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.246423 dbt-duckdb-1.4.1/dbt/include/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.247419 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/
--rw-r--r--   0 jwills     (501) staff       (20)     7122 2023-03-14 04:18:59.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 jwills     (501) staff       (20)      950 2023-02-13 18:23:20.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/catalog.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.248076 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 jwills     (501) staff       (20)     3861 2023-03-06 17:20:50.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1394 2023-01-10 04:54:42.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 jwills     (501) staff       (20)      862 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/snapshot_merge.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.249471 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-06 17:20:50.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1711 2023-03-06 17:20:50.000000 dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/upstream.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-03-16 16:10:26.250197 dbt-duckdb-1.4.1/dbt_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)    13048 2023-03-16 16:10:26.000000 dbt-duckdb-1.4.1/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1221 2023-03-16 16:10:26.000000 dbt-duckdb-1.4.1/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-03-16 16:10:26.000000 dbt-duckdb-1.4.1/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       60 2023-03-16 16:10:26.000000 dbt-duckdb-1.4.1/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        4 2023-03-16 16:10:26.000000 dbt-duckdb-1.4.1/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-03-16 16:10:26.250562 dbt-duckdb-1.4.1/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1366 2023-03-10 17:41:01.000000 dbt-duckdb-1.4.1/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.855300 dbt-duckdb-1.5.0rc1/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)    13051 2023-04-19 20:36:09.855118 dbt-duckdb-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)    12744 2023-03-21 22:22:36.000000 dbt-duckdb-1.5.0rc1/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.846926 dbt-duckdb-1.5.0rc1/dbt/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.847184 dbt-duckdb-1.5.0rc1/dbt/adapters/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.849434 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       21 2023-04-19 20:35:31.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/buenavista.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3163 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 jwills     (501) staff       (20)     6057 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/credentials.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7866 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/environments.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-26 18:59:50.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/glue.py
+-rw-r--r--   0 jwills     (501) staff       (20)     6984 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850216 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 jwills     (501) staff       (20)     1291 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)      589 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1669 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1034 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2050 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1141 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850359 dbt-duckdb-1.5.0rc1/dbt/include/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850641 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.851551 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/
+-rw-r--r--   0 jwills     (501) staff       (20)     7122 2023-03-21 22:22:36.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      950 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/catalog.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.852698 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 jwills     (501) staff       (20)     3916 2023-03-30 16:27:45.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1417 2023-04-03 22:00:10.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      862 2023-03-27 04:56:30.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/snapshot_merge.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.854144 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/upstream.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.854936 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)    13051 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1551 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       63 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        4 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-19 20:36:09.855332 dbt-duckdb-1.5.0rc1/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1369 2023-04-19 20:35:31.000000 dbt-duckdb-1.5.0rc1/setup.py
```

### Comparing `dbt-duckdb-1.4.1/LICENSE` & `dbt-duckdb-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/PKG-INFO` & `dbt-duckdb-1.5.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.4.1
+Version: 1.5.0rc1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
```

### Comparing `dbt-duckdb-1.4.1/README.md` & `dbt-duckdb-1.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/adapters/duckdb/glue.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/glue.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/adapters/duckdb/impl.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import importlib.util
 import os
-import tempfile
 from typing import List
 from typing import Optional
 from typing import Sequence
 
 import agate
 import duckdb
 
@@ -82,14 +80,18 @@
         return self.config.credentials.external_root
 
     @available
     def use_database(self) -> bool:
         return duckdb.__version__ >= "0.7.0"
 
     @available
+    def get_binding_char(self):
+        return DuckDBConnectionManager.env().get_binding_char()
+
+    @available
     def external_write_options(self, write_location: str, rendered_options: dict) -> str:
         if "format" not in rendered_options:
             ext = os.path.splitext(write_location)[1].lower()
             if ext:
                 rendered_options["format"] = ext[1:]
             elif "delimiter" in rendered_options:
                 rendered_options["format"] = "csv"
@@ -103,15 +105,20 @@
         if "partition_by" in rendered_options:
             v = rendered_options["partition_by"]
             if "," in v and not v.startswith("("):
                 rendered_options["partition_by"] = f"({v})"
 
         ret = []
         for k, v in rendered_options.items():
-            if k.lower() in {"delimiter", "quote", "escape", "null"} and not v.startswith("'"):
+            if k.lower() in {
+                "delimiter",
+                "quote",
+                "escape",
+                "null",
+            } and not v.startswith("'"):
                 ret.append(f"{k} '{v}'")
             else:
                 ret.append(f"{k} {v}")
         return ", ".join(ret)
 
     @available
     def external_read_location(self, write_location: str, rendered_options: dict) -> str:
@@ -130,55 +137,19 @@
         """This is just a quick-fix. Python models do not execute begin function so the transaction_open is always false."""
         try:
             self.connections.commit_if_has_connection()
         except DbtInternalError:
             pass
 
     def submit_python_job(self, parsed_model: dict, compiled_code: str) -> AdapterResponse:
-
         connection = self.connections.get_if_exists()
         if not connection:
             connection = self.connections.get_thread_connection()
-        con = connection.handle.cursor()
-
-        def load_df_function(table_name: str):
-            """
-            Currently con.table method dos not support fully qualified name - https://github.com/duckdb/duckdb/issues/5038
-
-            Can be replaced by con.table, after it is fixed.
-            """
-            return con.query(f"select * from {table_name}")
-
-        identifier = parsed_model["alias"]
-        mod_file = tempfile.NamedTemporaryFile(suffix=".py", delete=False)
-        mod_file.write(compiled_code.lstrip().encode("utf-8"))
-        mod_file.close()
-        try:
-            spec = importlib.util.spec_from_file_location(identifier, mod_file.name)
-            if not spec:
-                raise DbtRuntimeError(
-                    "Failed to load python model as module: {}".format(identifier)
-                )
-            module = importlib.util.module_from_spec(spec)
-            if spec.loader:
-                spec.loader.exec_module(module)
-            else:
-                raise DbtRuntimeError(
-                    "Python module spec is missing loader: {}".format(identifier)
-                )
-
-            # Do the actual work to run the code here
-            dbt = module.dbtObj(load_df_function)
-            df = module.model(dbt, con)
-            module.materialize(df, con)
-        except Exception as err:
-            raise DbtRuntimeError(f"Python model failed:\n" f"{err}")
-        finally:
-            os.unlink(mod_file.name)
-        return AdapterResponse(_message="OK")
+        env = DuckDBConnectionManager.env()
+        return env.submit_python_job(connection.handle, parsed_model, compiled_code)
 
     def get_rows_different_sql(
         self,
         relation_a: BaseRelation,
         relation_b: BaseRelation,
         column_names: Optional[List[str]] = None,
         except_operator: str = "EXCEPT",
```

### Comparing `dbt-duckdb-1.4.1/dbt/adapters/duckdb/relation.py` & `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/relation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 from dataclasses import dataclass
 from typing import Any
 from typing import Optional
 from typing import Type
 
+from .connections import DuckDBConnectionManager
+from .utils import SourceConfig
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.base.relation import Self
 from dbt.contracts.graph.nodes import SourceDefinition
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DuckDBRelation(BaseRelation):
-    external_location: Optional[str] = None
+    external: Optional[str] = None
 
     @classmethod
     def create_from_source(cls: Type[Self], source: SourceDefinition, **kwargs: Any) -> Self:
-
-        # Some special handling here to allow sources that are external files to be specified
-        # via a `external_location` meta field. If the source's meta field is used, we include
-        # some logic to allow basic templating of the external location based on the individual
-        # name or identifier for the table itself to cut down on boilerplate.
-        ext_location = None
-        if "external_location" in source.meta:
-            ext_location = source.meta["external_location"]
-        elif "external_location" in source.source_meta:
-            # Use str.format here to allow for some basic templating outside of Jinja
-            ext_location = source.source_meta["external_location"]
-
-        if ext_location:
+        source_config = SourceConfig.create(source)
+        # First check to see if a 'plugin' is defined in the meta argument for
+        # the source or its parent configuration, and if it is, use the environment
+        # associated with this run to get the name of the source that we should
+        # reference in the compiled model
+        if "plugin" in source_config.meta:
+            plugin_name = source_config.meta["plugin"]
+            DuckDBConnectionManager.env().load_source(plugin_name, source_config)
+        elif "external_location" in source_config.meta:
             # Call str.format with the schema, name and identifier for the source so that they
             # can be injected into the string; this helps reduce boilerplate when all
             # of the tables in the source have a similar location based on their name
             # and/or identifier.
-            ext_location = ext_location.format(
-                schema=source.schema, name=source.name, identifier=source.identifier
+            ext_location = source_config.meta["external_location"].format(
+                **source_config.as_dict()
             )
             # If it's a function call or already has single quotes, don't add them
             if "(" not in ext_location and not ext_location.startswith("'"):
                 ext_location = f"'{ext_location}'"
-            kwargs["external_location"] = ext_location
+            kwargs["external"] = ext_location
 
         return super().create_from_source(source, **kwargs)  # type: ignore
 
     def render(self) -> str:
-        if self.external_location:
-            return self.external_location
+        if self.external:
+            return self.external
         else:
             return super().render()
```

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/adapters.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/catalog.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/external.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% materialization external, adapter="duckdb", supported_languages=['sql', 'python'] %}
 
   {%- set location = render(config.get('location', default=external_location(this, config))) -%})
   {%- set rendered_options = render_write_options(config) -%}
+  {%- set format = config.get('format', 'parquet') -%}
   {%- set write_options = adapter.external_write_options(location, rendered_options) -%}
   {%- set read_location = adapter.external_read_location(location, rendered_options) -%}
 
   -- set language - python or sql
   {%- set language = model['language'] -%}
 
   {%- set target_relation = this.incorporate(type='view') %}
```

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/materializations/table.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/seed.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/seed.sql`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 {% macro duckdb__get_binding_char() %}
-  {{ return('?') }}
+  {{ return(adapter.get_binding_char()) }}
 {% endmacro %}
 
 {% macro duckdb__get_batch_size() %}
   {{ return(10000) }}
 {% endmacro %}
 
 {% macro duckdb__load_csv_rows(model, agate_table) %}
```

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/snapshot_merge.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/datediff.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.4.1/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
          and upstream.config.materialized=='external'
       %}
         {%- set upstream_rel = api.Relation.create(
           database=upstream['database'],
           schema=upstream['schema'],
           identifier=upstream['alias']
         ) -%}
-        {%- set location = upstream.config.get('location', external_location(upstream, upstream.config)) -%}
-        {%- set rendered_options = render_write_options(config) -%}
+        {%- set location = upstream.config.get('location', external_location(upstream_rel, upstream.config)) -%}
+        {%- set rendered_options = render_write_options(upstream.config) -%}
         {%- set upstream_location = adapter.external_read_location(location, rendered_options) -%}
         {% if upstream_rel.schema not in upstream_schemas %}
           {% call statement('main', language='sql') -%}
             create schema if not exists {{ upstream_rel.schema }}
           {%- endcall %}
           {% do upstream_schemas.update({upstream_rel.schema: None}) %}
         {% endif %}
```

### Comparing `dbt-duckdb-1.4.1/dbt_duckdb.egg-info/PKG-INFO` & `dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.4.1
+Version: 1.5.0rc1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
```

### Comparing `dbt-duckdb-1.4.1/dbt_duckdb.egg-info/SOURCES.txt` & `dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 MANIFEST.in
 README.md
 setup.py
 dbt/__init__.py
 dbt/adapters/__init__.py
 dbt/adapters/duckdb/__init__.py
 dbt/adapters/duckdb/__version__.py
+dbt/adapters/duckdb/buenavista.py
 dbt/adapters/duckdb/connections.py
+dbt/adapters/duckdb/credentials.py
+dbt/adapters/duckdb/environments.py
 dbt/adapters/duckdb/glue.py
 dbt/adapters/duckdb/impl.py
 dbt/adapters/duckdb/relation.py
+dbt/adapters/duckdb/utils.py
+dbt/adapters/duckdb/plugins/__init__.py
+dbt/adapters/duckdb/plugins/excel.py
+dbt/adapters/duckdb/plugins/gsheet.py
+dbt/adapters/duckdb/plugins/iceberg.py
+dbt/adapters/duckdb/plugins/sqlalchemy.py
 dbt/include/__init__.py
 dbt/include/duckdb/__init__.py
 dbt/include/duckdb/dbt_project.yml
 dbt/include/duckdb/macros/adapters.sql
 dbt/include/duckdb/macros/catalog.sql
 dbt/include/duckdb/macros/seed.sql
 dbt/include/duckdb/macros/snapshot_merge.sql
```

### Comparing `dbt-duckdb-1.4.1/setup.py` & `dbt-duckdb-1.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+dbt@gmail.com",
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core~=1.4.0",
+        "dbt-core~=1.5.0rc1",
         "duckdb>=0.5.0",
     ],
     extras_require={
         "glue": ["boto3", "mypy-boto3-glue"],
     },
 )
```


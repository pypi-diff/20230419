# Comparing `tmp/pycentroid-1.0.1.tar.gz` & `tmp/pycentroid-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycentroid-1.0.1.tar", last modified: Wed Apr 19 05:02:37 2023, max compression
+gzip compressed data, was "pycentroid-1.0.2.tar", last modified: Wed Apr 19 05:09:21 2023, max compression
```

## Comparing `pycentroid-1.0.1.tar` & `pycentroid-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.548836 pycentroid-1.0.1/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1517 2023-04-19 04:16:31.000000 pycentroid-1.0.1/LICENSE.txt
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      606 2023-04-19 05:02:37.549121 pycentroid-1.0.1/PKG-INFO
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      120 2023-04-19 04:16:31.000000 pycentroid-1.0.1/README.rst
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      461 2023-04-19 05:02:16.000000 pycentroid-1.0.1/pyproject.toml
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1208 2023-04-19 05:02:37.553615 pycentroid-1.0.1/setup.cfg
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      703 2023-04-19 04:16:31.000000 pycentroid-1.0.1/setup.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.341422 pycentroid-1.0.1/src/
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.356281 pycentroid-1.0.1/src/centroid/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      578 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/__init__.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.373932 pycentroid-1.0.1/src/centroid/client/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)       45 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/client/__init__.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     6226 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/client/client.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     7741 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/client/metadata.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.399785 pycentroid-1.0.1/src/centroid/common/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      501 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/__init__.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1561 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/application.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     2945 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/configuration.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     4797 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/datetime.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     2122 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/events.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      162 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/exceptions.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1642 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/expect.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1514 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/common/objects.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.497031 pycentroid-1.0.1/src/centroid/data/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      169 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/__init__.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      706 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/application.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     2801 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/configuration.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1851 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/context.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     3454 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/loaders.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)       99 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/model.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)       61 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/queryable.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     5317 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/data/types.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.526250 pycentroid-1.0.1/src/centroid/query/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      963 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/__init__.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)    10449 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/closure_parser.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     2367 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/data_objects.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     4202 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/method_parser.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1612 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/object_name_validator.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)    10221 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/open_data_formatter.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)    35735 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/open_data_parser.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1158 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/open_data_query.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      823 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/query_entity.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)    21081 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/query_expression.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     6782 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/query_field.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      127 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/query_value.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      273 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/resolvers.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)    20832 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/sql_formatter.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     5778 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/query/utils.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.533190 pycentroid-1.0.1/src/centroid/sqlite/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      129 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/sqlite/__init__.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)    13211 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/sqlite/adapter.py
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     3439 2023-04-19 04:16:31.000000 pycentroid-1.0.1/src/centroid/sqlite/dialect.py
-drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:02:37.547544 pycentroid-1.0.1/src/pycentroid.egg-info/
--rw-r--r--   0 kbarbounakis   (501) staff       (20)      606 2023-04-19 05:02:37.000000 pycentroid-1.0.1/src/pycentroid.egg-info/PKG-INFO
--rw-r--r--   0 kbarbounakis   (501) staff       (20)     1537 2023-04-19 05:02:37.000000 pycentroid-1.0.1/src/pycentroid.egg-info/SOURCES.txt
--rw-r--r--   0 kbarbounakis   (501) staff       (20)        1 2023-04-19 05:02:37.000000 pycentroid-1.0.1/src/pycentroid.egg-info/dependency_links.txt
--rw-r--r--   0 kbarbounakis   (501) staff       (20)        1 2023-04-19 04:18:30.000000 pycentroid-1.0.1/src/pycentroid.egg-info/not-zip-safe
--rw-r--r--   0 kbarbounakis   (501) staff       (20)       98 2023-04-19 05:02:37.000000 pycentroid-1.0.1/src/pycentroid.egg-info/requires.txt
--rw-r--r--   0 kbarbounakis   (501) staff       (20)        9 2023-04-19 05:02:37.000000 pycentroid-1.0.1/src/pycentroid.egg-info/top_level.txt
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.639853 pycentroid-1.0.2/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1517 2023-04-19 04:16:31.000000 pycentroid-1.0.2/LICENSE.txt
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      615 2023-04-19 05:09:21.640185 pycentroid-1.0.2/PKG-INFO
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      120 2023-04-19 04:16:31.000000 pycentroid-1.0.2/README.rst
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      461 2023-04-19 05:09:00.000000 pycentroid-1.0.2/pyproject.toml
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1217 2023-04-19 05:09:21.641992 pycentroid-1.0.2/setup.cfg
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      703 2023-04-19 04:16:31.000000 pycentroid-1.0.2/setup.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.587521 pycentroid-1.0.2/src/
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.591873 pycentroid-1.0.2/src/centroid/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      578 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/__init__.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.596028 pycentroid-1.0.2/src/centroid/client/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)       45 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/client/__init__.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     6226 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/client/client.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     7741 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/client/metadata.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.602996 pycentroid-1.0.2/src/centroid/common/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      501 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/__init__.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1561 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/application.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     2945 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/configuration.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     4797 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/datetime.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     2122 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/events.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      162 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/exceptions.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1642 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/expect.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1514 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/common/objects.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.611273 pycentroid-1.0.2/src/centroid/data/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      169 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/__init__.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      706 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/application.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     2801 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/configuration.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1851 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/context.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     3454 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/loaders.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)       99 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/model.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)       61 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/queryable.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     5317 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/data/types.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.626327 pycentroid-1.0.2/src/centroid/query/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      963 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/__init__.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)    10449 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/closure_parser.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     2367 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/data_objects.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     4202 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/method_parser.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1612 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/object_name_validator.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)    10221 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/open_data_formatter.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)    35735 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/open_data_parser.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1158 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/open_data_query.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      823 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/query_entity.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)    21081 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/query_expression.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     6782 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/query_field.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      127 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/query_value.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      273 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/resolvers.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)    20832 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/sql_formatter.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     5778 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/query/utils.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.630282 pycentroid-1.0.2/src/centroid/sqlite/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      129 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/sqlite/__init__.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)    13211 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/sqlite/adapter.py
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     3439 2023-04-19 04:16:31.000000 pycentroid-1.0.2/src/centroid/sqlite/dialect.py
+drwxr-xr-x   0 kbarbounakis   (501) staff       (20)        0 2023-04-19 05:09:21.639153 pycentroid-1.0.2/src/pycentroid.egg-info/
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)      615 2023-04-19 05:09:21.000000 pycentroid-1.0.2/src/pycentroid.egg-info/PKG-INFO
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)     1537 2023-04-19 05:09:21.000000 pycentroid-1.0.2/src/pycentroid.egg-info/SOURCES.txt
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)        1 2023-04-19 05:09:21.000000 pycentroid-1.0.2/src/pycentroid.egg-info/dependency_links.txt
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)        1 2023-04-19 04:18:30.000000 pycentroid-1.0.2/src/pycentroid.egg-info/not-zip-safe
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)       98 2023-04-19 05:09:21.000000 pycentroid-1.0.2/src/pycentroid.egg-info/requires.txt
+-rw-r--r--   0 kbarbounakis   (501) staff       (20)        9 2023-04-19 05:09:21.000000 pycentroid-1.0.2/src/pycentroid.egg-info/top_level.txt
```

### Comparing `pycentroid-1.0.1/LICENSE.txt` & `pycentroid-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/PKG-INFO` & `pycentroid-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pycentroid
-Version: 1.0.1
+Version: 1.0.2
 Summary: @themost-framework for python
 Home-page: https://github.com/centroid-py/centroid/
 Author: Kyriakos Barbounakis
 Author-email: Kyriakos Barbounakis <k.barbounakis@gmail.com>
-License: MIT
+License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/centroid-py/centroid
 Project-URL: Bug Tracker, https://github.com/centroid-py/centroid/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pycentroid-1.0.1/setup.cfg` & `pycentroid-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pycentroid
 description = @themost-framework for python
 author = Kyriakos Barbounakis
 author_email = k.barbounakis@gmail.com
-license = MIT
+license = BSD-3-Clause
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/centroid-py/centroid/
 project_urls = 
 	Documentation = https://github.com/centroid-py/centroid/
 platforms = any
```

### Comparing `pycentroid-1.0.1/setup.py` & `pycentroid-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/__init__.py` & `pycentroid-1.0.2/src/centroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/client/client.py` & `pycentroid-1.0.2/src/centroid/client/client.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/client/metadata.py` & `pycentroid-1.0.2/src/centroid/client/metadata.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/common/application.py` & `pycentroid-1.0.2/src/centroid/common/application.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/common/configuration.py` & `pycentroid-1.0.2/src/centroid/common/configuration.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/common/datetime.py` & `pycentroid-1.0.2/src/centroid/common/datetime.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/common/events.py` & `pycentroid-1.0.2/src/centroid/common/events.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/common/expect.py` & `pycentroid-1.0.2/src/centroid/common/expect.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/common/objects.py` & `pycentroid-1.0.2/src/centroid/common/objects.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/data/application.py` & `pycentroid-1.0.2/src/centroid/data/application.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/data/configuration.py` & `pycentroid-1.0.2/src/centroid/data/configuration.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/data/context.py` & `pycentroid-1.0.2/src/centroid/data/context.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/data/loaders.py` & `pycentroid-1.0.2/src/centroid/data/loaders.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/data/types.py` & `pycentroid-1.0.2/src/centroid/data/types.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/__init__.py` & `pycentroid-1.0.2/src/centroid/query/__init__.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/closure_parser.py` & `pycentroid-1.0.2/src/centroid/query/closure_parser.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/data_objects.py` & `pycentroid-1.0.2/src/centroid/query/data_objects.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/method_parser.py` & `pycentroid-1.0.2/src/centroid/query/method_parser.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/object_name_validator.py` & `pycentroid-1.0.2/src/centroid/query/object_name_validator.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/open_data_formatter.py` & `pycentroid-1.0.2/src/centroid/query/open_data_formatter.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/open_data_parser.py` & `pycentroid-1.0.2/src/centroid/query/open_data_parser.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/open_data_query.py` & `pycentroid-1.0.2/src/centroid/query/open_data_query.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/query_entity.py` & `pycentroid-1.0.2/src/centroid/query/query_entity.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/query_expression.py` & `pycentroid-1.0.2/src/centroid/query/query_expression.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/query_field.py` & `pycentroid-1.0.2/src/centroid/query/query_field.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/sql_formatter.py` & `pycentroid-1.0.2/src/centroid/query/sql_formatter.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/query/utils.py` & `pycentroid-1.0.2/src/centroid/query/utils.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/sqlite/adapter.py` & `pycentroid-1.0.2/src/centroid/sqlite/adapter.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/centroid/sqlite/dialect.py` & `pycentroid-1.0.2/src/centroid/sqlite/dialect.py`

 * *Files identical despite different names*

### Comparing `pycentroid-1.0.1/src/pycentroid.egg-info/PKG-INFO` & `pycentroid-1.0.2/src/pycentroid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pycentroid
-Version: 1.0.1
+Version: 1.0.2
 Summary: @themost-framework for python
 Home-page: https://github.com/centroid-py/centroid/
 Author: Kyriakos Barbounakis
 Author-email: Kyriakos Barbounakis <k.barbounakis@gmail.com>
-License: MIT
+License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/centroid-py/centroid
 Project-URL: Bug Tracker, https://github.com/centroid-py/centroid/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pycentroid-1.0.1/src/pycentroid.egg-info/SOURCES.txt` & `pycentroid-1.0.2/src/pycentroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/dagster-duckdb-polars-0.18.7.tar.gz` & `tmp/dagster-duckdb-polars-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-polars-0.18.7.tar", last modified: Thu Apr 13 15:13:57 2023, max compression
+gzip compressed data, was "dagster-duckdb-polars-0.19.0.tar", last modified: Wed Apr 19 19:12:33 2023, max compression
```

## Comparing `dagster-duckdb-polars-0.18.7.tar` & `dagster-duckdb-polars-0.19.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7372 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/duckdb_polars_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 15:13:57.000000 dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-13 15:13:57.533635 dagster-duckdb-polars-0.18.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1386 2023-04-13 15:03:07.000000 dagster-duckdb-polars-0.18.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:12:33.670839 dagster-duckdb-polars-0.19.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-19 19:12:33.670839 dagster-duckdb-polars-0.19.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:12:33.670839 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars/
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars/duckdb_polars_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 19:12:33.670839 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-19 19:12:33.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-19 19:12:33.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:12:33.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 19:12:33.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-19 19:12:33.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 19:12:33.000000 dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-19 19:12:33.670839 dagster-duckdb-polars-0.19.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-04-19 19:01:30.000000 dagster-duckdb-polars-0.19.0/setup.py
```

### Comparing `dagster-duckdb-polars-0.18.7/LICENSE` & `dagster-duckdb-polars-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.18.7/PKG-INFO` & `dagster-duckdb-polars-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.18.7
+Version: 0.19.0
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.18.7/dagster_duckdb_polars/duckdb_polars_type_handler.py` & `dagster-duckdb-polars-0.19.0/dagster_duckdb_polars/duckdb_polars_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-polars-0.18.7/dagster_duckdb_polars.egg-info/PKG-INFO` & `dagster-duckdb-polars-0.19.0/dagster_duckdb_polars.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-polars
-Version: 0.18.7
+Version: 0.19.0
 Summary: Package for storing Polars DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-polars
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-polars-0.18.7/setup.py` & `dagster-duckdb-polars-0.19.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_polars_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.2.7",
-        "dagster-duckdb==0.18.7",
+        "dagster==1.3.0",
+        "dagster-duckdb==0.19.0",
         "polars[pyarrow]",
     ],
     zip_safe=False,
 )
```


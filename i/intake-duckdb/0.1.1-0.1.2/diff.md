# Comparing `tmp/intake-duckdb-0.1.1.tar.gz` & `tmp/intake-duckdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-duckdb-0.1.1.tar", last modified: Mon Apr 10 16:58:26 2023, max compression
+gzip compressed data, was "intake-duckdb-0.1.2.tar", last modified: Wed Apr 19 20:49:31 2023, max compression
```

## Comparing `intake-duckdb-0.1.1.tar` & `intake-duckdb-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:26.852043 intake-duckdb-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-10 16:58:10.000000 intake-duckdb-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-10 16:58:26.848043 intake-duckdb-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-10 16:58:10.000000 intake-duckdb-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:26.848043 intake-duckdb-0.1.1/intake_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-10 16:58:10.000000 intake-duckdb-0.1.1/intake_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-10 16:58:10.000000 intake-duckdb-0.1.1/intake_duckdb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-10 16:58:10.000000 intake-duckdb-0.1.1/intake_duckdb/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:58:26.848043 intake-duckdb-0.1.1/intake_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-10 16:58:26.000000 intake-duckdb-0.1.1/intake_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 16:58:26.000000 intake-duckdb-0.1.1/intake_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:58:26.000000 intake-duckdb-0.1.1/intake_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-10 16:58:26.000000 intake-duckdb-0.1.1/intake_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 16:58:26.000000 intake-duckdb-0.1.1/intake_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 16:58:26.000000 intake-duckdb-0.1.1/intake_duckdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-10 16:58:10.000000 intake-duckdb-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:58:26.852043 intake-duckdb-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:49:31.362708 intake-duckdb-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-19 20:49:31.362708 intake-duckdb-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:49:31.362708 intake-duckdb-0.1.2/intake_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/intake_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/intake_duckdb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/intake_duckdb/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/intake_duckdb/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:49:31.362708 intake-duckdb-0.1.2/intake_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-19 20:49:31.000000 intake-duckdb-0.1.2/intake_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-19 20:49:31.000000 intake-duckdb-0.1.2/intake_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:49:31.000000 intake-duckdb-0.1.2/intake_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 20:49:31.000000 intake-duckdb-0.1.2/intake_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-19 20:49:31.000000 intake-duckdb-0.1.2/intake_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 20:49:31.000000 intake-duckdb-0.1.2/intake_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-19 20:49:15.000000 intake-duckdb-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:49:31.362708 intake-duckdb-0.1.2/setup.cfg
```

### Comparing `intake-duckdb-0.1.1/LICENSE` & `intake-duckdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-duckdb-0.1.1/PKG-INFO` & `intake-duckdb-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-duckdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: DuckDB plugin for Intake
 Author: Blake Rosenthal
 Maintainer-email: Blake Rosenthal <brosenthal@anaconda.com>
 License: Copyright (c) 2023, Anaconda, Inc.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -29,26 +29,35 @@
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Keywords: intake,duckdb,duck
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # Intake-DuckDB
 
+[![Build Status](https://github.com/intake/intake-duckdb//actions/workflows/main.yaml/badge.svg)](https://github.com/intake/intake-duckdb/actions)
+[![Documentation Status](https://readthedocs.org/projects/intake-duckdb/badge/?version=latest)](http://intake-duckdb.readthedocs.io/en/latest/?badge=latest)
+
 DuckDB Plugin for Intake
 
 ## Installation
 
+From PyPI
 ```shell
 pip install intake-duckdb
 ```
 
+Or conda-forge
+```shell
+conda install -c conda-forge intake-duckdb
+```
 ## Usage
 
 Load an entire table into a dataframe
 ```python
 source = intake.open_duckdb("path/to/dbfile", "tablename")
 df = source.read()
 
@@ -74,7 +83,30 @@
 
 # list the sources in 'cat'
 list(cat)
 
 df = cat["tablename"].read()
 df_chunks = [chunk for chunk in cat["tablename"](chunks=10).read_chunked()]
 ```
+
+Run DuckDB queries on other Intake sources (that produce pandas DataFrames) within the same catalog
+```yaml
+# cat.yaml
+sources:
+  csv_source:
+    args:
+      urlpath: https://data.csv
+    description: Remote CSV source
+    driver: csv
+
+  duck_source:
+    args:
+      targets:
+        - csv_source
+      sql_expr: SELECT col FROM csv_source LIMIT 10
+    description: Source referencing other sources in catalog
+    driver: duckdb_transform
+```
+```python
+cat  = intake.open_catalog("cat.yaml")
+duck_source = cat.duck_source.read()
+```
```

### Comparing `intake-duckdb-0.1.1/intake_duckdb/base.py` & `intake-duckdb-0.1.2/intake_duckdb/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
-from intake.source import base
+from intake.source import DataSource
+from intake.source.base import Schema
 
 from . import __version__
 
 
-class DuckDBSource(base.DataSource):
+class DuckDBSource(DataSource):
     """
     DuckDB table to dataframe reader. Can take either a table name or a SQL expression.
     Partitionable.
 
     Caches entire dataframe in memory.
 
     Parameters
@@ -72,29 +73,32 @@
 
         super(DuckDBSource, self).__init__(metadata=metadata)
 
     def _load(self):
         self._load_metadata()
         self._dataframe = self._duckdb.df()
 
-    def _get_schema(self):
+    def _get_schema(self, context=None):
         if self._schema is None:
             import duckdb
 
+            if context is not None:
+                globals().update(context)
+
             self._con = self._con or duckdb.connect(self._uri)
             self._duckdb = self._con.sql(self._sql_expr)
             self._bins = np.linspace(
                 0, self._duckdb.shape[0], self._chunks + 1, dtype=int
             )
 
             shape = self._duckdb.shape
             columns = self._duckdb.columns
             dtypes = self._duckdb.types
 
-            self._schema = base.Schema(
+            self._schema = Schema(
                 datashape=None,
                 dtype=dict(zip(columns, dtypes)),
                 shape=shape,
                 npartitions=self._chunks,
                 extra_metadata={},
             )
```

### Comparing `intake-duckdb-0.1.1/intake_duckdb.egg-info/PKG-INFO` & `intake-duckdb-0.1.2/intake_duckdb.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-duckdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: DuckDB plugin for Intake
 Author: Blake Rosenthal
 Maintainer-email: Blake Rosenthal <brosenthal@anaconda.com>
 License: Copyright (c) 2023, Anaconda, Inc.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -29,26 +29,35 @@
         (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Keywords: intake,duckdb,duck
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # Intake-DuckDB
 
+[![Build Status](https://github.com/intake/intake-duckdb//actions/workflows/main.yaml/badge.svg)](https://github.com/intake/intake-duckdb/actions)
+[![Documentation Status](https://readthedocs.org/projects/intake-duckdb/badge/?version=latest)](http://intake-duckdb.readthedocs.io/en/latest/?badge=latest)
+
 DuckDB Plugin for Intake
 
 ## Installation
 
+From PyPI
 ```shell
 pip install intake-duckdb
 ```
 
+Or conda-forge
+```shell
+conda install -c conda-forge intake-duckdb
+```
 ## Usage
 
 Load an entire table into a dataframe
 ```python
 source = intake.open_duckdb("path/to/dbfile", "tablename")
 df = source.read()
 
@@ -74,7 +83,30 @@
 
 # list the sources in 'cat'
 list(cat)
 
 df = cat["tablename"].read()
 df_chunks = [chunk for chunk in cat["tablename"](chunks=10).read_chunked()]
 ```
+
+Run DuckDB queries on other Intake sources (that produce pandas DataFrames) within the same catalog
+```yaml
+# cat.yaml
+sources:
+  csv_source:
+    args:
+      urlpath: https://data.csv
+    description: Remote CSV source
+    driver: csv
+
+  duck_source:
+    args:
+      targets:
+        - csv_source
+      sql_expr: SELECT col FROM csv_source LIMIT 10
+    description: Source referencing other sources in catalog
+    driver: duckdb_transform
+```
+```python
+cat  = intake.open_catalog("cat.yaml")
+duck_source = cat.duck_source.read()
+```
```

### Comparing `intake-duckdb-0.1.1/pyproject.toml` & `intake-duckdb-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -25,21 +25,29 @@
     "pandas",
     "duckdb",
 ]
 
 [project.entry-points."intake.drivers"]
 duckdb = "intake_duckdb:DuckDBSource"
 duckdb_cat = "intake_duckdb:DuckDBCatalog"
+duckdb_transform = "intake_duckdb:DuckDBTransform"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "intake[server]",
     "python-snappy",
 ]
+docs = [
+    "sphinx",
+    "sphinx_rtd_theme",
+    "numpydoc",
+    "entrypoints",
+    "myst-parser",
+]
 
 [tool.setuptools]
 packages = [
     "intake_duckdb",
 ]
 
 [tool.setuptools-git-versioning]
```

